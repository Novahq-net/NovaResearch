# NovaLogic PFF File Format
Visit [https://novahq.net](https://novahq.net) for more information on NovaLogic file formats and tools to work with these files.

## PFF Information
PFF archives are containers for smaller files.  

There is no special encoding or encryption methods used to decode these files.

## PFF Structure
All PFF versions follow this general sequential structure:  
1.  [Header]: Contains versioning and table offsets. Always 20 bytes regardless of version  
2.  [EntryDataBlobs]: The actual raw data of the archived files  
3.  [EntryTable]: A directory of entries defining the files stored in the blobs  
4.  [Footer]: Metadata or padding (varies by version)  

---

## PFF0
Version Identifier: PFF0 (Hex: 50 46 46 30)  
*Supported Games: F22R(Non-IBS)*

### [Header]
| Field            | Type      | Description                                |
| :--------------- | :-------- | :----------------------------------------- |
| Length           | uint32    | Length of header                           |
| Version          | byte[4]   | "PFF0"                   |
| EntryCount       | uint32    | Number of files in the archive             |
| EntryLength      | uint32    | Size of each entry in the table            |
| EntryTableOffset | uint32    | Offset to the start of the Entry Table     |

### [Entry Definition]
Entry Size: 32 Bytes  
*Note: PFF0 does not use DeadSpaceFlags because pack-pff0.exe removes the data and rebuilds the file* 

| Field            | Type      | Description                                |
| :--------------- | :-------- | :----------------------------------------- |
| ZeroPad          | uint32    | Record starts with padding                 |
| DataOffset       | uint32    | Offset to the file data                    |
| DataSize         | uint32    | Length of the file data                    |
| Timestamp        | uint32    | Unix Epoch timestamp                       |
| FileName         | byte[15]  | Always 15 bytes + null terminator          |
|                  |           | "&lt;DEAD SPACE&gt;" signifies deleted     |

### [Footer]
* None

---

## PFF2
Version Identifier: PFF2 (Hex: 50 46 46 32)  
*Supported Games: C3G* 

### [Header]
| Field            | Type      | Description                                |
| :--------------- | :-------- | :----------------------------------------- |
| Length           | uint32    | Total file size                            |
| Version          | byte[4]   | "PFF2"                                     |
| EntryCount       | uint32    | Number of files in the archive             |
| EntryLength      | uint32    | Size of each entry in the table            |
| EntryTableOffset | uint32    | Offset to the start of the Entry Table     |

### [Entry Definition]
Entry Size: 32 Bytes  
*Note: PFF2 does not use DeadSpaceFlags because pack-pff2.exe removes the data and rebuilds the file* 

| Field            | Type      | Description                                |
| :--------------- | :-------- | :----------------------------------------- |
| CRC              | uint32    | Checksum for the entry                     |
| DataOffset       | uint32    | Offset to the file data                    |
| DataSize         | uint32    | Length of the file data                    |
| Timestamp        | uint32    | Unix Epoch timestamp                       |
| FileName         | byte[15]  | Always 15 bytes + null terminator          |
|                  |           | "&lt;DEAD SPACE&gt;" signifies deleted           |

### [Footer]
Size: 4 Bytes

| Field            | Type      | Description                                |
| :--------------- | :-------- | :----------------------------------------- |
| EntryTableCRC    | uint32    | (Unconfirmed) Changes every time a file is |
|                  |           | added or removed from the EntryTable       |

---

## PFF3
Version Identifier: PFF3 (Hex: 50 46 46 33) or F4 (Hex: 01 00 46 34)  
*Supported Games: Entry Variants Listed Below* 

### [Header]
| Field            | Type      | Description                                |
| :--------------- | :-------- | :----------------------------------------- |
| Length           | uint32    | Total file size                            |
| Version          | byte[4]   | "PFF3/  F4"                                |
| EntryCount       | uint32    | Number of files in the archive             |
| EntryLength      | uint32    | Always 32 or 36 bytes                      |
| EntryTableOffset | uint32    | Offset to the start of the Entry Table     |

### [Entry Definition (Variant 1)] 
Entry Size: 32 Bytes (Leaves out CRC)  
*Supported Games: AF3, F16, F22R-IBS, L3, M29, TTF, DF1, DF2*   

| Field            | Type      | Description                                |
| :--------------- | :-------- | :----------------------------------------- |
| DeadSpaceFlags   | uint32    | If 1, then FileName is set to &lt;DEAD SPACE&gt; |
| DataOffset       | uint32    | Offset to the file data                    |
| DataSize         | uint32    | Length of the file data                    |
| Timestamp        | uint32    | Unix Epoch timestamp                       |
| FileName         | byte[15]  | Always 15 bytes + null terminator          |

### [Entry Definition (Variant 2)]
Entry Size: 36 Bytes (Includes CRC)  
*Supported Games: C4, LW, TFD, BHD, JO, DFX*  

| Field            | Type      | Description                                |
| :--------------- | :-------- | :----------------------------------------- |
| *Standard Fields*| *N/A* | Includes all fields from 32-byte version   |
| CRC              | uint32    | CRC remains unchanged even if              |
|                  |           | DeadSpaceFlags = 1 and FileName = &lt;DEAD SPACE&gt; |

### [Footer]
Size: Usually 12 Bytes  
*Note: F16.pff and Mig29.pff have a 0-byte footer despite being PFF3*  

| Field            | Type      | Description                                |
| :--------------- | :-------- | :----------------------------------------- |
| LAP_IP           | uint32    | Local IP address?                          |
| ZeroPadding      | uint32    | Usually all zeros. Exception:              |
|                  |           | PFF3-Raptor-Common.pff has bytes CC F2 AC DF |
| Signature        | uint32    | Always "KING" (Hex: 4B 49 4E 47)           |

---

## PFF4
Version Identifier: PFF4 (Hex: 50 46 46 34)  
*Supported Games: DFX2* 

### [Header]
| Field            | Type      | Description                                |
| :--------------- | :-------- | :----------------------------------------- |
| Length           | uint32    | Total file size                            |
| Version          | byte[4]   | "PFF4"                                     |
| EntryCount       | uint32    | Number of files in the archive             |
| EntryLength      | uint32    | Always 36 bytes                            |
| EntryTableOffset | uint32    | Offset to the start of the Entry Table     |

### [Entry Definition]
Entry Size: 36 Bytes

| Field            | Type      | Description                                |
| :--------------- | :-------- | :----------------------------------------- |
| DeadSpaceFlags   | uint32    | If 1, then FileName is set to &lt;DEAD SPACE&gt; |
| DataOffset       | uint32    | Offset to the file data                    |
| DataSize         | uint32    | Length of the file data                    |
| Timestamp        | uint32    | Unix Epoch timestamp                       |
| FileName         | byte[15]  | Always 15 bytes + null terminator          |
| CRC              | uint32    | CRC remains unchanged even if              |
|                  |           | DeadSpaceFlags = 1 and FileName = &lt;DEAD SPACE&gt; |

### [Footer]
Size: 12 Bytes

| Field            | Type      | Description                                |
| :--------------- | :-------- | :----------------------------------------- |
| IpAddress        | uint32    | Network IP address                        |
| ZeroPadding      | uint32    | Always zeros?                              |
| Signature        | uint32    | Always "KING" (Hex: 4B 49 4E 47)          |