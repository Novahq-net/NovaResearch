# NovaLogic GSB File Format
Visit [https://novahq.net](https://novahq.net) for more information on NovaLogic file formats and tools to work with these files.

## GSB Information
GSB files are binary files that store server and player listings for NovaLogic games.
The information below is for a **decrypted** GSB. **SEE:** [GBS Decryption](#gsb-decryption).

**Games:** `Joint Operations: Combined Arms`, `Delta Force Xtreme` `Delta Force Xtreme 2`.


## GSB Structure
Each block follows the pattern: `[Marker(4)] [Length(int32)] [Payload(Length)]`
Payload is encrypted; markers and lengths are plaintext.

1. Read **GSB** header
2. Jump to **IVAR** using the header's relative offset
3. Read **IVAR** block (Variables/Metadata)
4. Read **FLDS** block (Field definitions)
5. Read one or more **SVRS** blocks
6. Stop when **XXXX** is encountered

---

## "GSB " (Header)
*Marker: `0x47 0x53 0x42 0x20`*

| Field | Type | Description |
| --- | --- | --- |
| Marker | char[4] | ASCII `"GSB "` (`0x47 0x53 0x42 0x20`) |
| Length | int32 | Relative offset to `IVAR` |
| **Payload:** | | |
| Unknown | int32 | Always `0x00010000` (previously documented as `0x00000100` due to endianness misread) |
| Year | int16 | Timestamp component |
| Month | int8 | Timestamp component |
| Day | int8 | Timestamp component |
| Hour | int8 | Timestamp component |
| Minute | int8 | Timestamp component |
| Second | int8 | Timestamp component |
| Unknown | int8 | Unknown |
| Unknown | int16 | Always `0x0400` (previously documented as `0x0002` due to endianness misread) |
| FileName | cstring | Null-terminated filename |

---

## "IVAR" (Variables: TotalServers, TotalPlayers)

| Field | Type | Description |
| --- | --- | --- |
| Marker | char[4] | ASCII `"IVAR"` |
| Length | int32 | Relative offset to `FLDS` |
| **Payload:** | | |
| Count | int16 | Number of variable pairs |
| *Repeated Count times:* | | |
| Name | cstring | Variable name |
| Value | cstring | Variable value |

---

## "FLDS" (Field Definitions)

| Field | Type | Description |
| --- | --- | --- |
| Marker | char[4] | ASCII `"FLDS"` |
| Length | int32 | Relative offset to first `SVRS` |
| **Payload:** | | |
| Count | int16 | Number of field names |
| *Repeated Count times:* | | |
| FieldName | cstring | Field name |

---

## "SVRS" (Server Block, repeats until XXXX)

| Field | Type | Description |
| --- | --- | --- |
| Marker | char[4] | ASCII `"SVRS"` |
| Length | int32 | Length of payload |
| **Payload:** | | |
| ServerCount | int16 | Number of server records |
| *Repeated ServerCount times:* | | |
| RID | int32 | Server record ID |
| IPAddress | byte[4] | IPv4 address bytes |
| Fields | cstring * FLDS Count | Dynamic, null-terminated (see below) |
| PlayerCount | int16 | Number of players in this server |
| *Repeated PlayerCount times:* | | |
| PlayerName | cstring | Player name |

### Server Fields (dynamic, null-terminated strings)
The fields are governed by the `FLDS` block definitions and vary by game:

**Shared fields for JOP/DFX/DFX2:**
`ServerName`, `GameType`, `MissionName`, `Region`, `Players`,
`MaxPlayers`, `Dedicated`, `TimeLeft`, `Password`, `Country`,
`Msg`, `Age`, `TimeOfDay`, `Stat`, `LevelRange`, `Locked`,
`Tracers`, `Skins`, `BBMode`, `Mod`, `PIX`, `PBSERVER`, `VER1`

**JOP remaining fields:**
`Exp`, `Expbits`, `Joicon2`

**DFX/DFX2 remaining fields:**
`JOStats`, `PLoad`, `Exp`, `JOStatRestrictArrayString`,
`Expbits`, `Joicon2`, `DFXCATEGORY2`

---

## "XXXX" (End of File)
Length: `0` (4 bytes of zeros)

---

# GSB Decryption
This is the decryption routine used to obtain the plaintext GSB stream before parsing the file structure.
See the NovaTools repo for a full decrypt and encrypt implementation.
The GSB format utilizes a multi-pass approach involving a stream cipher and a rolling offset.

### Inputs / Constants
- **Key String**: `"3209452104342624532341"`
- **Salt (Multiplier)**: `0x04B05731`
- **Initial Hash**: Derived by summing the (index + byte value squared) for each character in the key, plus the key length and `0x32`.

### Derived Constants
Since the key and salt are fixed, the following values are precomputed constants:
1. **Counter (Rolling Pass Start)**: `0x41` — `((SALT * hash(KEY)) + 1) & 0xFF`
2. **Step (Rolling Pass Increment)**: `0x72` — `((SALT * COUNTER) + 1) & 0xFF`
3. **Seed (Stream Cipher Seed)**: `0xD3D3` — `((SALT * STEP) + 1) & 0xFFFF`
4. **Reverse**: `true` — `SEED & 1`

---

### Decryption Routine
The GSB format is chunk-based. For each chunk (Header + Payload), the following steps are performed in order:

1.  **Stream Cipher Pass**: Bytes are transformed using an LCG-based PRNG seeded by the derived `Seed`.
2.  **Rolling Offset Pass**: Each byte is modified by an offset: $(counter + index) \pmod{256}$. The counter starts at `COUNTER` and increases by `STEP` after every byte.
3.  **Conditional Reverse**: If `REVERSE` is true (LSB of `SEED` is set), the entire byte buffer for that chunk is reversed.
4.  **Key Repeat Pass**: A simple repeating XOR/substitution pass using the key string bytes as offsets.

> **Note**: The encryption routine for GSB is simply the reverse of this process (Key Repeat -> Reverse -> Rolling Offset -> Stream Cipher).

---

### PHP Decrypt Implementation
The following implementation demonstrates the multi-pass transformation logic. See the NovaTools repo for a full decrypt and encrypt implementation.

```php
private const string KEY            = "3209452104342624532341";
private const int    SALT           = 0x04B05731;
private const int    CIPHER_COUNTER = 0x41;   // ((SALT * hash(KEY)) + 1) & 0xFF
private const int    CIPHER_STEP    = 0x72;   // ((SALT * CIPHER_COUNTER) + 1) & 0xFF
private const int    CIPHER_SEED    = 0xD3D3; // ((SALT * CIPHER_STEP) + 1) & 0xFFFF
private const bool   CIPHER_REVERSE = true;   // CIPHER_SEED & 1

private function transform(string &$buffer, bool $method): void {

    $this->streamCipherPass($buffer, self::CIPHER_SEED, self::DECRYPT);
    $this->rollingOffsetPass($buffer, self::CIPHER_COUNTER, self::CIPHER_STEP, self::DECRYPT);

    if (self::CIPHER_REVERSE)
        $buffer = strrev($buffer);

    $this->keyRepeatPass($buffer, self::KEY, self::DECRYPT);
}
```