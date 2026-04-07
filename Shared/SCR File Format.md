# NovaLogic SCR1 File Format
Visit [https://novahq.net](https://novahq.net) for more information on NovaLogic file formats and tools to work with these files. 

## SCR1 Information
SCR1 (Script file) files are a text file that stores configuration data.

**Games:**  `Comanche 4`, `Delta Force 1`, `Delta Force 2`, `Delta Force: Land Warrior`, `Delta Force: Task Force Dagger`, `Delta Force: Black Hawk Down`, `Delta Force: Black Hawk Down Team Sabre`, 
`Delta Force: Xtreme`, `Delta Force: X2`, `Joint Operations`

**Extensions:** (`.aca`), (`.adm`), (`.aip`), (`.anm`), (`.bin`), (`.end`), (`.def`), (`.fx`), (`.ldo`), (`.csv`), (`.ptg`), (`.ptl`), (`.ptu`), (`.txt`)

**Encryption:** SCR1 files are encrypted (obfuscated) using an ARX (Add-Rotate-XOR) stream cipher.  

## Encryption Keys
The 32-bit key continuously scrambles itself by adding a rotated copy of itself, rotating the result, and flipping the lowest bit; the bottom 8 bits of this new state are then XORed with each byte of the data.

| Game                         | Key
| :--------------------------- | :---------- |
| DF1                          | 0x04960552  |
| DF2, LW, TFD, C4             | 0x01234567  |
| BHD, BHDTS, DFX, DFX2, JOCA  | 0x2A5A8EAD  |
| DFX, DFX2, JOCA (.fx files)  | 0xA55B1EED  |
| JO DEMO / JOE                | 0xABEEFACE  |

## SCR1 Structure
All files follow this sequential structure:  

### [Header]
Size: `4 Bytes`  
*Notes: DF1 does not contain a MagicBytes field, the whole file is encrypted with the key.* 

| Field                 | Type      | Description                                      |
| :-------------------- | :-------- | :----------------------------------------------- |
| MagicBytes            | byte[4]   | "SCR1" ( 0x53, 0x43, 0x52, 0x01)                 |

---

### [Encrypted Payload]
Size: `Variable (Remaining file size)`      

| Field                 | Type      | Description                                      |
| :-------------------- | :-------- | :----------------------------------------------- |
| Payload               | byte[N]   | Encrypted text data to EOF                       |