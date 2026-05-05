# NovaLogic 3DO File Format (v1.1)
Visit [https://novahq.net](https://novahq.net) for more information on NovaLogic file formats and tools to work with these files.  

This information was gathered from reverse engineering the formats statically and while loaded in-game. Some of the entries are best guesses based on behaviour after loading into the engine or inferred from the data. While researching, some of the fields were renamed or re-identified and may be inconsistent across versions. This was particularly true for the `3DO` format, where each game parses the format differently. If you have any corrections or insights, please create an issue or submit a pull request.

## 3DO Information
The `.3DO` format is NovaLogic's binary 3D model container used by `Armored Fist 3` and `Comanche 3 Gold`. Other games such as `F-16 Multirole Fighter`, `MiG-29 Fulcrum`, `F-22 Raptor`, `F-22 Lightning 3`, and `Tachyon: The Fringe` use embedded 3DO blocks within `.PAK` files (see [PAK File Format](./PAK%20File%20Format.md) for details).

## 3DO Format

```
File
  Header
  Textures[]
  Vertices[]                    position + UV per entry
  Triangles[]                   3-corner references into Vertices, Normals, Textures
  Normals[]
  MeshEntries[]                 sub-model offsets used by composite formats (PAK, AI, OCF)
  Hardpoints[]                  attachment offsets, located at `HardpointsOffset`
```

## 3DO Structure
All files follow the below sequential structure. All offsets and counts are little-endian.

### [Header]
Size: `92 Bytes`  

| Field | Type | Description |
| --- | --- | --- |
| Magic | char[4] | File signature, always `"3DO1"` |
| Version | uint32 | Format version, always `0x0101` |
| Name | char[8] | Space-padded, uppercase model name |
| BoundingRadius | int32 | bounding sphere radius (PAK-embedded only) |
| Bbox | int32[6] | Standalone: `MinX, MaxX, MinY, MaxY, MinZ, MaxZ`. PAK-embedded: `MinZ, MaxZ, MinY, MaxY, MinX, MaxX` |
| TextureCount | uint32 | Number of `Texture` entries |
| VertexCount | uint32 | Number of `Vertex` entries |
| TriangleCount | uint32 | Number of `Triangle` entries |
| NormalCount | uint32 | Number of `Normal` entries |
| MeshCount | uint32 | Number of `MeshEntry` entries |
| HardpointCount | uint32 | Number of `Hardpoint` entries |
| TexturesOffset | uint32 | Offset to `Textures` |
| VerticesOffset | uint32 | Offset to `Vertices` |
| TrianglesOffset | uint32 | Offset to `Triangles` |
| NormalsOffset | uint32 | Offset to `Normals` |
| MeshEntriesOffset | uint32 | Offset to `MeshEntries` |
| HardpointsOffset | uint32 | Offset to `Hardpoints` |

---

### [Texture]
Size: `28 Bytes per entry`  

| Field | Type | Description |
| --- | --- | --- |
| Filename | char[12] | Null-terminated texture filename |
| Unknown | byte | |
| Unknown | uint8 | |
| Unknown | uint8 | |
| Alpha | uint8 | `0x00` = opaque, `0x80` = alpha, other = mix |
| ColorR | uint8 | Flat-color R |
| ColorG | uint8 | Flat-color G |
| ColorB | uint8 | Flat-color B |
| Unknown | byte | |
| UvParamU | uint8 | UV repeat / shift U |
| UvParamV | uint8 | UV repeat / shift V |
| RenderFlags | uint16 | See below |
| Unknown | byte | |
| FrameCount | uint8 | Animation frame count |
| FrameIndex | uint8 | `0x7D` = LOD pair marker, `0x7F` = back-face material swap |
| Unknown | byte | |

**RenderFlags**:

| Bit | Mask | Name | Description |
| --- | --- | --- | --- |
| 3 | 0x0008 | HasTexture | Enables textured render |
| 6 | 0x0040 | DoubleSided | Render both faces |
| 7 | 0x0080 | PaletteKeyed | Applies a blend / brighten |
| 8 | 0x0100 | HiddenAtRest | Skip face when `Alpha` byte is `0x80` |
| 11 | 0x0800 | FlatColor | Use the `ColorR` / `ColorG` / `ColorB` bytes as a solid fill |
| 15 | 0x8000 | Unknown | |

---

### [Vertex]
Size: `44 Bytes per entry`  

| Field | Type | Description |
| --- | --- | --- |
| X | int32 | Position X |
| Y | int32 | Position Y |
| Z | int32 | Position Z |
| Unknown | byte[20] | |
| U | int32 | Texture U (divide by `65536`) |
| V | int32 | Texture V |
| Unknown | int32 | |

---

### [Triangle]
Size: `32 Bytes per entry`  

| Field | Type | Description |
| --- | --- | --- |
| Unknown | int32 | |
| TextureRef | int32 | Byte offset into `Textures` |
| VertexRefA | int32 | Byte offset into `Vertices` (corner 0) |
| VertexRefB | int32 | Byte offset into `Vertices` (corner 1) |
| VertexRefC | int32 | Byte offset into `Vertices` (corner 2) |
| NormalRefA | int32 | Byte offset into `Normals` (corner 0) |
| NormalRefB | int32 | Byte offset into `Normals` (corner 1) |
| NormalRefC | int32 | Byte offset into `Normals` (corner 2) |

---

### [Normal]
Size: `16 Bytes per entry`  

| Field | Type | Description |
| --- | --- | --- |
| Nx | int32 | Normal X component (divide by `32768`) |
| Ny | int32 | Normal Y component |
| Nz | int32 | Normal Z component |
| Unknown | int32 | |

---

### [MeshEntry]
Size: `12 Bytes per entry`  
*Notes: Sub-model offset triples used by composite formats (PAK, AI, OCF) to position child parts on a parent body.*

| Field | Type | Description |
| --- | --- | --- |
| X | int32 | Sub-model X offset |
| Y | int32 | Sub-model Y offset |
| Z | int32 | Sub-model Z offset |

---

### [Hardpoint]
Size: `16 Bytes per entry`  

| Field | Type | Description |
| --- | --- | --- |
| X | int32 | Hardpoint X offset |
| Y | int32 | Hardpoint Y offset |
| Z | int32 | Hardpoint Z offset |
| Unknown | byte[4] | |

---

## Coordinate System and Fixed-Point Encoding

*Notes: The load-time `<< 7` shift applies **only to vertex positions** and only in standalone use. PAK-embedded 3DOs are read without it.*

| Quantity | Type | Conversion to World Units |
| --- | --- | --- |
| Vertex X / Y / Z | int32 | Standalone: multiply by `128` (load-time `<< 7` shift). PAK-embedded: no shift |
| Normal X / Y / Z | int32 | divide by `32768` |
| UV U / V | int32 (16.16 FP) | divide by `65536` |
| Hardpoint X / Y / Z | int32 | direct |
| Bbox | int32 | direct |

