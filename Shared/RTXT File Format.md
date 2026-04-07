# NovaLogic RTXT File Format
Visit [https://novahq.net](https://novahq.net) for more information on NovaLogic file formats and tools to work with these files.  

## RTXT Information
RTXT (Resource Text) files are a binary storage container for configuration data.
The file stores data either as a value only list (no keys/groups) or as grouped key/value pairs.

**Games:** `Armored Fist 3`, `Comanche 4`, `Delta Force 1`, `Delta Force 2`, `Delta Force: Land Warrior`, `Delta Force: Task Force Dagger`, `Delta Force: Black Hawk Down`, `Delta Force: Black Hawk Down Team Sabre`, 
`Delta Force: Xtreme`, `Delta Force: X2`, `F16 Multirole Fighter`, `F22 Lightning 3`, `F22 Raptor`, `F22 Raptor IBS`, `Joint Operations`, `MiG-29 Fulcrum`, `Tachyon: The Fringe`

**Extensions:** (`.bin`)  

**Encryption:** RTXT files have no encryption or obfuscation.

## RTXT Parsed Format
RTXT files can be parsed into a structure similar to a common INI file. Values can have special chars or new lines.  

The type of list can be determined by reading GroupCount in the GroupsTable or the size of GroupsTableLength.
If GroupCount or GroupsTableLength is zero, the file ends immediately after GroupCount.   

`[GROUP1]`  
`KEY=VALUE`  
  
`[GROUP2]`  
`KEY=VALUE`  
`....`  

If there are no groups, the structure is simply:  

`VALUE`  
`VALUE`  
`VALUE`  
`....`  

## RTXT Structure
All files follow the below sequential structure.  

### [Header]
Size: `16 Bytes`  

| Field                 | Type      | Description                                      |
| :-------------------- | :-------- | :----------------------------------------------- |
| MagicBytes            | byte[4]   | "RTXT"                                           |
| GroupTableOffset      | uint32    | Absolute offset to the `GroupsTable`             |
| GroupsTableLength     | uint32    | Total bytes of the `GroupsTable`                 |
| RefTableCount         | uint32    | Number of entries in the `RefTable`              |

---

### [RefTable]
Size: `16 Bytes * RefTableCount`  
*Notes: Reference table starts immediately after `Header`*  

| Field                 | Type      | Description                                      |
| :-------------------- | :-------- | :----------------------------------------------- |
| ValueOffset           | uint32    | Relative from (`RefTableCount * 16`)             |
| OffsetX               | short     | Display offset X?                                |
| OffsetY               | short     | Display offset Y?                                |
| GroupId               | short     | `GroupId`, -1 for no group                       |
| Padding               | byte[6]   | 6 bytes of padding                               |

---

### [ValueTable]
Size: `strlen * RefTableCount`  
*Notes: Value (string) table starts immediately after `RefTable`* 

| Field                 | Type      | Description                                      |
| :-------------------- | :-------- | :----------------------------------------------- |
| String                | string    | Null terminated strings                          |

---

### [GroupCount]
Size: `4 Bytes`  
*Notes: Start of GroupTable*  

| Field                 | Type      | Description                                      |
| :-------------------- | :-------- | :----------------------------------------------- |
| GroupCount           | uint32     | Number of groups                                 |

---

### [GroupsHeader]
Size: `8 Bytes * GroupCount`  

| Field                 | Type      | Description                                      |
| :-------------------- | :-------- | :----------------------------------------------- |
| KeysOffset            | uint32    | Relative offset from start of `GroupHeader`      |
| EntryCount            | uint32    | Number of keys in group                          |

---

### [GroupNames]
Size: `strlen * EntryCount`  
*Notes: Null terminated string immediately following the `GroupHeader`*   

| Field                 | Type      | Description                                      |
| :-------------------- | :-------- | :----------------------------------------------- |
| String                | string    | Null terminated strings                          |

---

### [GroupKeysTable]
Size: `strlen * EntryCount`  
*Notes: Keys are matched with string values in order as they appear.*  

| Field                 | Type      | Description                                      |
| :-------------------- | :-------- | :----------------------------------------------- |
| String                | string    | Null terminated strings                          |