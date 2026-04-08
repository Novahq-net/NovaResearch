# NovaLogic GLB File Format
Visit [https://novahq.net](https://novahq.net) for more information on NovaLogic file formats and tools to work with these files.

## GLB Information
GLB files are binary files that store server and player listings for NovaLogic games.
The information below is for a **decrypted** GLB. **SEE:** [GLB Decryption](#glb-decryption).

**Games:** `Comanche 4`, `Delta Force: Task Force Dagger`, `Delta Force: Black Hawk Down`, `Delta Force: Black Hawk Down Team Sabre`,
`Joint Operations (Early versions)`

---

## GLB Structure
GLB files follow a sequential structure with tagged blocks. Fields vary by game.

1. Read **GLB** header
2. Jump to **FIEL** using the header's relative offset
3. Read **FIEL** definitions (field names + types)
4. Read one or more **DATA** blocks until **PLYR** or **XXXX**
5. If present, read **PLYR** blocks until **XXXX**
6. Stop when **XXXX** is encountered

---

## "GLB " (Header)
*Marker: `0x47 0x4C 0x42 0x20`*

| Field | Type | Description |
| --- | --- | --- |
| Marker | char[4] | ASCII `"GLB "` (`0x47 0x4C 0x42 0x20`) |
| Length | int32 | Relative offset to `FIEL` |
| **Payload:** | | |
| FileName | cstring | Null-terminated filename |
| Unknown | int32 | Always `0x00000100`? |
| Month | int32 | Timestamp component |
| Day | int32 | Timestamp component |
| Year | int32 | Timestamp component |
| Hour | int32 | Timestamp component |
| Minute | int32 | Timestamp component |
| Second | int32 | Timestamp component |
| Unknown | int32 | Always `0x00000002`? |

---

## "FIEL" (Field Definitions)

| Field | Type | Description |
| --- | --- | --- |
| Marker | char[4] | ASCII `"FIEL"` |
| Length | int32 | Relative offset to first `DATA` |
| **Payload:** | | |
| Count | int32 | Number of field definitions |
| *Repeated Count times:* | | |
| FieldName | cstring | Field name |
| FieldType | int32 | `0` = string, `1` = int32 |

---

## "DATA" (Server Block, repeats until PLYR or XXXX)

| Field | Type | Description |
| --- | --- | --- |
| Marker | char[4] | ASCII `"DATA"` |
| Length | int32 | Length of payload |
| **Payload:** | | |
| FielCount | int32 | Field count for this block |
| ServerCount | int32 | Number of server records |
| LobbyType | int32 | Lobby classification (see below) |
| FielIndex | int32 * FielCount | Sequential from 0 (purpose unknown) |
| *Repeated ServerCount times:* | | |
| RID | int32 | Server record ID |
| IPAddress | byte[4] | IPv4 address bytes |
| AgeMs | int32 | Age in milliseconds |
| Fields | cstring * FielCount | Dynamic, null-terminated (see below) |

**LobbyType values:**

| ID | Meaning |
| --- | --- |
| 0 | Consumer |
| 1 | Tournament |
| 6 | Stats |
| 8 | Affiliate |

### Server Fields (dynamic, null-terminated strings)
The fields are governed by the `FIEL` block definitions and vary by game:

**Shared fields for C4/BHD/TFD:**
`ServerName`, `GameType`, `MissionName`, `Region`, `Players`,
`MaxPlayers`, `Dedicated`, `TimeLeft`, `Password`, `Country`,
`Msg`, `Age`

**BHD remaining fields:**
`TimeOfDay`, `Stat`, `LevelRange`, `Locked`,
`Tracers`, `Skins`, `BBMode`, `Mod`, `PIX`, `BHDEXP1`, `BHDEXP2`

---

## "PLYR" (Player Block, after DATA blocks, repeats until XXXX)

| Field | Type | Description |
| --- | --- | --- |
| Marker | char[4] | ASCII `"PLYR"` |
| Length | int32 | Length of payload |
| **Payload:** | | |
| RID | int32 | Server RID this player list belongs to |
| PlayerCount | int32 | Number of player names |
| *Repeated PlayerCount times:* | | |
| PlayerName | cstring | Player name |

---

## "XXXX" (End of File)
Length: `0` (4 bytes of zeros)

---

# GLB Decryption
This is the decryption routine used to obtain the plaintext GLB stream before parsing the file structure.
See the NovaTools repo for a full decrypt and encrypt implementation.

### Inputs / Constants
- **Key String**: `"NOVAWORLD"`
- **Salt (Multiplier)**: `0x5731`
- **Cipher Seed**: `0xA0C2`
- **Cipher Offsets** (7 bytes): `[112, 222, 76, 186, 40, 150, 4]`
- Each byte advances the LCG: `seed = ((seed * SALT) + 1) & 0xFFFF`
- Indices:
  - `keyIdx` cycles `0..keyLen-1`
  - `patternIdx` cycles `0..6`
  - `baseOffset` starts `0` and increases by `+2` each time `patternIdx` wraps (every 7 bytes)

### Per-byte transform
For each input byte `c = data[i]`:

```
seed = ((seed * SALT) + 1) & 0xFFFF

plainByte =
    ( c
    - keyBytes[keyIdx]
    + CIPHER_OFFSETS[patternIdx]
    + baseOffset
    - seed
    ) & 0xFF
```

### PHP Decrypt Implementation
The following implementation demonstrates the transform logic. See the NovaTools repo for a full decrypt and encrypt implementation.

```php
private const string KEY            = "NOVAWORLD";
private const int    SALT           = 0x5731;
private const int    CIPHER_SEED    = 0xA0C2;
private const array  CIPHER_OFFSETS = [112, 222, 76, 186, 40, 150, 4];

private function transform(string $data, bool $method): string {

    $keyBytes = array_map('ord', str_split(self::KEY));
    $keyLen = count($keyBytes);

    $pattern = self::CIPHER_OFFSETS;
    $patternCount = count($pattern);
    $seed = self::CIPHER_SEED;

    $sign = $method === self::DECRYPT ? -1 : 1;

    $patternIdx = 0;
    $baseOffset = 0;
    $keyIdx = 0;

    $result = [];
    for ($i = 0; $i < strlen($data); $i++) {
        $seed = (($seed * self::SALT) + 1) & 0xFFFF;

        $byte = (ord($data[$i])
            + $sign * $keyBytes[$keyIdx]
            - $sign * $pattern[$patternIdx]
            - $sign * $baseOffset
            + $sign * $seed
        ) & 0xFF;

        $result[] = chr($byte);

        if (++$keyIdx === $keyLen) $keyIdx = 0;
        if (++$patternIdx === $patternCount) {
            $patternIdx = 0;
            $baseOffset += 2;
        }
    }

    return implode('', $result);
}
```