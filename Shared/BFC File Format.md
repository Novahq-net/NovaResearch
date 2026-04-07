# NovaLogic BFC File Format
Visit [https://novahq.net](https://novahq.net) for more information on NovaLogic file formats and tools to work with these files. 

## BFC Information
BFC (Binary File Container) is a compressed file format probably implimented to reduce the size of game assets.

**Games:** `Delta Force: Xtreme`, `Delta Force: X2`, `Joint Operations`

**Extensions:** (`.dds`), (`.mdt`), (`.wav`) 

**Compression:** BFC files use standard ZLIB compression (RFC 1950).  
1. The **Header** (first 8 bytes) contains the signature and the size of the data *before* compression.  
2. The **Payload** is a standard ZLIB stream containing the compressed data and a checksum.  

**Encoding:** The file uses standard Deflate compression (usually with a 32K window size). The ZLIB header typically defaults to `0x78 0x9C` (Default Compression), and the stream ends with an Adler-32 checksum.  

## BFC Structure
All files follow this sequential structure:  

### [Header]
Size: `8 Bytes`  

| Field                 | Type      | Description                                      |
| :-------------------- | :-------- | :----------------------------------------------- |
| MagicBytes            | byte[4]   | "BFC1" (0x42 0x46 0x43 0x31)                     |
| UncompressedSize      | uint32    | The size of the file in bytes when decompressed  |

---

### [ZlibBlock]
Size: `Variable (Remaining file size)`      
*Notes: This block is a standard ZLIB stream. It can be decompressed using any standard ZLIB library (e.g., `zlib`, `SharpZipLib`, or .NET `DeflateStream` after stripping the 2-byte header).*  

| Field                 | Type      | Description                                      |
| :-------------------- | :-------- | :----------------------------------------------- |
| ZlibHeader            | byte[2]   | Compression Flags (Usually `0x78 0x9C`)          |
| CompressedData        | byte[]    | Raw Deflate compressed stream                    |
| Adler32               | uint32    | Checksum of the uncompressed data (Big Endian)   |