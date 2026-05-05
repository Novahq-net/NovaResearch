# NovaLogic PAK File Format (v2001 and v2003)
Visit [https://novahq.net](https://novahq.net) for more information on NovaLogic file formats and tools to work with these files.  

This information was gathered from reverse engineering the formats statically and while loaded in-game. Some of the entries are best guesses based on behaviour after loading into the engine or inferred from the data. While researching, some of the fields were renamed or re-identified and may be inconsistent across versions. If you have any corrections or insights, please create an issue or submit a pull request.

## PAK Information
The `.PAK` (3DPK) format is NovaLogic's binary 3D model archive container used by `F-16 Multirole Fighter`, `MiG-29 Fulcrum`, `F-22 Raptor`, `F-22 Lightning 3`, and `Tachyon: The Fringe`. The 3DO model blocks embedded inside a `.PAK` use the [3DO File Format](./3DO%20File%20Format.md).

**Versions:**
- v2001: `F-16 Multirole Fighter`, `MiG-29 Fulcrum`, `F-22 Raptor`
- v2003: `Tachyon: The Fringe`, `F-22 Lightning 3`

## PAK Format
```
File
  Header                          72 B (v0x2001) or 96 B (v0x2003)
  LodDirectory[LodCount]
  LodDataBlocks[]
    BlockHeader
    PartEntries[]                 each references one embedded 3DO model
  Embedded3DOModels[]             one per part per LOD
  CollisionPayload                v0x2003 only, when flag 0x01 set
  AnimationPayload                v0x2003 only, when flag 0x04 set
  Textures[]                      embedded paletted pixel data + RGB palette
```

## PAK Structure
All files follow the below sequential structure. All offsets and counts are little-endian.

### [Header]
Size: `72 Bytes` (v0x2001) or `96 Bytes` (v0x2003)  

| Field | Type | Description |
| --- | --- | --- |
| Magic | char[4] | Always `"3DPK"` |
| Version | uint32 | (`0x2001`) or (`0x2003`) |
| Name | char[32] | Space-padded, null-terminated model name |
| Flags | uint32 | Payload selectors. `0` in v0x2001 |
| LodCount | uint32 | Number of LODs (`1`-`6`) |
| BoundingRadius | uint32 | Bounding sphere radius |
| Unknown | uint32 | |
| LodDirOffset | uint32 | (`0x48`) in v0x2001, (`0x60`) in v0x2003 |
| TextureDataOffset | uint32 | File offset to `Textures` section |
| FileSize | uint32 | Total file size |
| Unknown | uint32 | |
| CollisionOffset | uint32 | **(v0x2003 only)** File offset to collision payload |
| AnimationOffset | uint32 | **(v0x2003 only)** File offset to animation payload |
| Unknown | byte[16] | **(v0x2003 only)** Always `0` |

**Header Flags** (v0x2003 only):

| Bit | Mask | Name | Description |
| --- | --- | --- | --- |
| 0 | 0x01 | HasCollision | Collision payload exists at `CollisionOffset` |
| 1 | 0x02 | Remapped | Palette was remapped (TTF-only) |
| 2 | 0x04 | HasAnimation | Animation payload exists at `AnimationOffset` |

---

### [LodDirectory]
Size: `LodCount * 8 Bytes`  

| Field | Type | Description |
| --- | --- | --- |
| Distance | uint32 | LOD switch distance |
| LodDataOffset | uint32 | File offset to `LodDataBlock` |

---

### [LodDataBlock]
Size: `Variable`  

**Block Header:** `12 Bytes`

| Field | Type | Description |
| --- | --- | --- |
| Scale | uint32 | Always `0x00010000` (`1.0`) |
| PartCount | uint32 | Number of `PartEntry` records  |
| FirstPartOffset | uint32 | Always `12` |

**PartEntry:** `44 Bytes per entry`

| Field | Type | Description |
| --- | --- | --- |
| ModelOffset | uint32 | File offset to 3DO model block |
| Unknown | byte[12] | Always `0` |
| Flags | uint32 | Per-part flags |
| EntryStride | uint32 | Always `44` |
| Unknown | byte[8] | |
| NextLodOffset | uint32 | Relative offset to next-lower LOD |
| ChildOffset | uint32 | Byte offset to first child entry |
| Unknown | uint32 |  |

**Multi-part composites:** when `PartCount > 1`, the part entries form a tree defined by `ChildOffset`. The engine walks the tree at draw time and uses each embedded 3DO's `MeshEntries[]` to position child parts relative to the parent. The first 3DO is sometimes an empty root with zero geometry that just anchors the composite (Tachyon typically has an empty root part followed by 1-N geometry parts, see [OCF File Format](./OCF%20File%20Format.md)).

---

### [Embedded3DOModels]
Size: `Variable`  
*Notes: The 3DO magic / version / array layout is documented in the [3DO File Format](./3DO%20File%20Format.md).*

---

### [CollisionPayload]
Size: `Variable`  
*Notes: v0x2003 only. Present when `Flags & 0x01` is set. Located at the header's `CollisionOffset`. Not yet documented*

---

### [AnimationPayload]
Size: `Variable`  
*Notes: v0x2003 only. Present when `Flags & 0x04` is set. Located at the header's `AnimationOffset`. Not yet documented*

---

### [Textures]
Size: `Variable`  

**Section Header:** `4 Bytes`

| Field | Type | Description |
| --- | --- | --- |
| TextureCount | uint32 | Number of `Texture` entries |

**Texture:** `Variable size per entry`

| Field | Type | Description |
| --- | --- | --- |
| Filename | char[12] | Texture filename (e.g. `"IAARM_H.PCX"`) |
| HasPalette | uint16 | `0x0100` = a 768-byte palette. `0x0000` = no embedded palette |
| Unknown | uint16 | Flags |
| Width | uint32 | Width |
| Height | uint32 | Height |
| PixelDataSize | uint32 | Size of pixel data in bytes |
| PixelData | byte[PixelDataSize] | Pixel data |
| Palette | byte[768] | `256` entries of `R, G, B` |

**Palette fallback:** when a texture has no embedded palette, the game selects a palette in this order:

1. `.PAL` file with the same basename as the `.PAK`
2. `GENPAK.PCX` / `GENPAK.PAL`
3. Grayscale