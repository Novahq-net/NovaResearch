# NovaLogic CBIN File Format
Visit [https://novahq.net](https://novahq.net) for more information on NovaLogic file formats and tools to work with these files.  

## CBIN Information
CBIN (Compiled Binary) files are a binary storage container for configuration data.
The file stores data using indexed string tables and typed values (Integers, Floats, and Strings)
Strings are stored in a dedicated string table and referenced by ID throughout the file. 
Keys are stored in sequential order, along with the value params each key contains.
Value params stored in a separate Values table in sequential order, with each value indicating its type. Each key may have multiple values.

**Games:** `Comanche 4`, `Delta Force: Land Warrior`, `Delta Force: Task Force Dagger`, `Delta Force: Black Hawk Down`, `Delta Force: Black Hawk Down Team Sabre`, 
`Delta Force: Xtreme`, `Delta Force: X2`, `Joint Operations`, `Tachyon: The Fringe`

**Extensions:** (`.anm`), (`.bas`), (`.bdf`), (`.box`), (`.cfg`), (`.def`), (`.des`), (`.hud`), (`.ics`), (`.itm`), (`.job`), (`.kda`), (`.mnu`), (`.mpc`), (`.nws`), (`.ocf`), (`.scr`), (`.sen`), (`.txt`), (`.wng`)

**Encryption:** CBIN files are encrypted (obfuscated).

1. The **Header** (first 20 bytes) is **Unencrypted**.
2. The **Payload** (everything after the header) is **Encrypted**.

**Encryption Algorithm:** The payload uses a rolling XOR cipher.  
* **Key:** Defined in the Header (usually `0x01E177CE`).  
* **Algorithm:** For every byte in the payload, the key is rotated left by 7 bits, and the byte is XORed with the lowest 8 bits of the key.  

## CBIN Parsed Format
CBIN files can be parsed into a structure similar to a common INI file. Each value within a key is comma separated, with strings wrapped in quotes.  

`[GROUP1]`  
`KEY=50,1.5,"STRING"`  
`KEY=10.0,1.5,"STRING"`  
`....`  

`[GROUP2]`  
`KEY="STRING",10`
`KEY="STRING","STRING","STRING"`  
`KEY=5,10,8`  
`....`  

## CBIN Structure
All files follow the below sequential structure.  
*Note: All offsets and data following the Header are relative to the decrypted payload.*  

### [Header]
Size: `20 Bytes`  

| Field | Type | Description |
| --- | --- | --- |
| MagicBytes | byte[4] | File Signature |
| StringTableOffset | uint32 | Absolute offset to the StringTable |
| StringTableLength | uint32 | Total bytes of the StringTable |
| StringTableCount | uint32 | Number of strings in the table |
| EncryptionKey | uint32 | Key used to decrypt the payload (e.g., 0x01E177CE) |

---

### [GroupCount]
Size: `4 Bytes`  

| Field | Type | Description |
| --- | --- | --- |
| Count | uint32 | Total number of Groups |

---

### [GroupsTable]
Size: `8 Bytes * GroupCount`  

| Field | Type | Description |
| --- | --- | --- |
| StringId | uint32 | ID of the Group Name in the StringTable |
| EntryCount | uint32 | Number of Keys in this group |

---

### [KeysTable]
Size: `Variable`  
*Notes: This table iterates through every Group defined above. If a Group has `EntryCount > 0`, the keys are listed, followed immediately by 8 bytes of padding.*  

**Per Key Entry (Repeated for EntryCount):**  

| Field                 | Type      | Description                                      |
| :-------------------- | :-------- | :----------------------------------------------- |
| StringId              | uint32    | ID of the Key Name in the `StringTable`            |
| RefValueCount         | uint32    | Number of Values assigned to this Key            |

**Padding (Occurs once after the keys for a specific Group, if Group `EntryCount > 0`):**  

| Field                 | Type      | Description                                      |
| :-------------------- | :-------- | :----------------------------------------------- |
| Padding               | byte[8]   | 8 Empty bytes (0x00)                             |

---

### [ValuesTable]
Size: `8 Bytes * TotalValues`  
*Notes: This table lists values sequentially for every Key.*  

| Field | Type | Description |
| --- | --- | --- |
| Value | uint32 | The data. If type is `String`, this is the `StringId` |
| ValueType | uint32 | The data type (See table below) |

**Value Types:**  
  
| ID | Type   | Description                                           |
| :--| :----- | :---------------------------------------------------- |
| 1  | Int    | Value is a standard integer                           |
| 2  | Float  | Value is a float (cast the uint32 to float)           |
| 4  | String | Value is an index (ID) pointing to the `StringTable`  |

---

### [StringTable]
Size: `StringTableLength`  
*Notes: Located at `StringTableOffset`. Contains a list of null-terminated strings. String IDs are 1-based indices corresponding to the order the strings appear in this table.*  

| Field | Type | Description |
| --- | --- | --- |
| String | string | Null terminated string |