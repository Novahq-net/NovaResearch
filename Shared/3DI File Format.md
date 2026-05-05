# NovaLogic 3DI File Format (v5 through v10)
Visit [https://novahq.net](https://novahq.net) for more information on NovaLogic file formats and tools to work with these files.  

This information was gathered from reverse engineering the formats statically and while loaded in-game. Some of the entries are best guesses based on behaviour after loading into the engine or inferred from the data. While researching, some of the fields were renamed or re-identified and may be inconsistent across versions. If you have any corrections or insights, please create an issue or submit a pull request.

## 3DI Information
The `.3DI` format is NovaLogic's binary 3D model container used in the early `Delta Force` series. The file structure is largely consistent across versions, with later versions adding new sections and fields while maintaining most of the core layout. 

| Version | Game(s) |
| --- | --- |
| v5 | `Delta Force 1` |
| v8 | `Delta Force 2` |
| v10 | `Delta Force: Land Warrior`, `Delta Force: Task Force Dagger` |

***Note:*** BHD/C4/JOP/DFX/DFX2 use a different format even though they share the same (`.3DI`) extension. They are covered separately as they are unique formats.

## 3DI Format

```
File
  Header
  Portals[]                      (v10) optional; may be empty
  Textures[]                     embedded pixels (v5, v8) or external file refs (v10)
  LOD-Objects[1..4]               one per LOD (High, Medium, Low, Tiny)
    Vertices[]
    Normals[]
    Faces[]                      triangles, with UVs and per-vertex normal indices
    FaceColors[]                 (v10) optional per-face vertex-color triples
    Meshes[]                     parts; tree via ParentMeshIndex
    Hardpoints[]                 attachment points
    Planes[]                     (v8, v10) BSP / collision splitting planes
    CollisionVolumes[]           BSP tree
    Materials[]                  face shading, texture binding [, UV scale (v10)]
```

## Version Sizes

| Version | Header | TextureEntry | LOD-Object | Face | Mesh | CollisionVolume | Material |
| --- | --- | --- | --- | --- | --- | --- | --- |
| v5 | 124 | 36 + payload | 184 | 72 | 112 | 72 | 76 |
| v8 | 124 | 52 + payload | 192 | 72 | 112 | 80 | 120 |
| v10 | 160 | 80 (external) | 232 | 80 | 120 | 80 | 128 |

## 3DI Structure
All files follow the below sequential structure. All offsets and counts are little-endian.

### [Header] (v5 / v8)
Size: `124 Bytes`  

| Field | Type | Description |
| --- | --- | --- |
| Magic | byte[3] | Always `"3DI"` |
| Version | uint8 | Always `5` (v5) or `8` (v8) |
| Name | char[12] | Null-terminated model name |
| Unknown | uint32 | Always (`0` or `1`) |
| LodCount | uint32 | Number of LODs, 1 to 4 |
| LodDistance1 | uint32 | LOD switching distance |
| LodDistance2 | uint32 | LOD switching distance |
| LodDistance3 | uint32 | LOD switching distance |
| LodDistance4 | uint32 | LOD switching distance |
| RenderTags | char[4][4] | Four 4-character tags |
| Unknown | uint32 | Always `0` or `0x10` |
| Unknown | byte[64] | |

---

### [Header] (v10)
Size: `160 Bytes`  

| Field | Type | Description |
| --- | --- | --- |
| Magic | byte[3] | Always `"3DI"` |
| Version | uint8 | Always `10` |
| Name | char[12] | Null-terminated model name |
| Unknown | uint32 | Always (`0` or `1`) |
| LodCount | uint32 | Number of LODs, 1 to 4 |
| LodDistance1 | uint32 | LOD switching distance |
| LodDistance2 | uint32 | LOD switching distance |
| LodDistance3 | uint32 | LOD switching distance |
| LodDistance4 | uint32 | LOD switching distance |
| RenderTags | char[4][4] | Four 4-character tags |
| Unknown | uint32 | Always `0` or `0x10` |
| Unknown | byte[60] | |
| PortalCount | uint32 | Number of `Portal` records |
| Unknown | uint32 | |
| Unknown | byte[32] | |

---

### RenderTags

**RenderTags:** Four slots, one per environment / biome variant. Each slot holds a 4-character tag identifying the model class for that environment. Tags are stored little-endian, so reading the four bytes as ASCII gives the word reversed (e.g. `oleh` reads as `helo`). Slots can hold different tags within the same model, and unused slots may be zero. 

**v5 Tags:**

| Tag | Reads As | Class |
| --- | --- | --- |
| `crng` | gnrc | General |
| `0gro` | org0 | Characters |
| `tcfe` | efct | Effects |
| `drib` | bird | Birds |
| `pmal` | lamp | Lamps |
| `oleh` | helo | Helicopters |
| `eert` | tree | Trees |
| `d3fe` | ef3d | 3D effect |
| `mlap` | palm | Palms |
| `erit` | tire | Tires |
| `gnep` | peng | Penguin |

**v8 Tags:**

| Tag | Reads As | Class |
| --- | --- | --- |
| `crng` | gnrc | General |
| `gdlb` | bldg | Building |
| `0gro` | org0 | Characters |
| `tcfe` | efct | Effects |
| `2dlb` | bld2 | Building |
| `eert` | tree | Trees |
| `drib` | bird | Birds |
| `hsif` | fish | Fish |
| `d3fe` | ef3d | 3D effect |
| `npwe` | ewpn | Weapons |
| `oleh` | helo | Helicopters |
| `mlap` | palm | Palms |
| `mdrb` | brdm | BRDM vehicles |
| `knat` | tank | Tanks |
| `erit` | tire | Tires |
| `gnep` | peng | Penguin |
| `dnih` | hind | Hind helicopter |
| `gnup` | pung | Pungi |
| `92ak` | ka29 | KA29 helicopter |

**v10 Tags:**

| Tag | Reads As | Class |
| --- | --- | --- |
| `crng` | gnrc | General |
| `tcfe` | efct | Effects |
| `gdlb` | bldg | Building |
| `0gro` | org0 | Characters |
| `fltp` | ptlf | Portal flag |
| `2dlb` | bld2 | Building |
| `rood` | door | Doors |
| `eert` | tree | Trees |
| `erit` | tire | Tires |
| `1ltp` | ptl1 | Portal v1 |
| `d3fe` | ef3d | 3D effect |
| `npwe` | ewpn | Weapons |
| `oleh` | helo | Helicopters |
| `drib` | bird | Birds |
| `ecaf` | face | Faces |
| `92ak` | ka29 | KA29 helicopter |
| `mlap` | palm | Palms |
| `2ltp` | ptl2 | Portal v2 |
| `3ltp` | ptl3 | Portal v3 |
| `pmal` | lamp | Lamps |
| `knat` | tank | Tanks |

---

### [Portals] (v10)
Size: `PortalCount * 20 Bytes`  

**Portal Entry:** `20 Bytes`

| Field | Type | Description |
| --- | --- | --- |
| X | int16 | Portal X position |
| Y | int16 | Portal Y position |
| Z | int16 | Portal Z position |
| LinkCount | uint16 | (`1`, `2`, or `3`) |
| Width | uint16 | Portal opening width |
| Padding | byte[10] | Always `0` |

---

### [TextureCount]
Size: `4 Bytes`  

| Field | Type | Description |
| --- | --- | --- |
| Count | uint32 | Total number of texture entries |

---

### [TextureEntry] (v5)
Size: `Variable` (`36 + DataSize + 1024` bytes per entry)  

**Texture Header:** `36 Bytes`

| Field | Type | Description |
| --- | --- | --- |
| Name | char[12] | Texture name, null-terminated |
| Unknown | byte[4] | Always `0` |
| DataSize | uint32 | Pixel data block in bytes |
| Sequence | uint16 | Material sequence index |
| Flags | uint8 | Env / alpha flags |
| LodTag | uint8 | LOD index |
| Width | uint16 | Width (always 2^n) |
| Height | uint16 | Height (always 2^n) |
| Unknown | uint32 | |
| Unknown | uint32 | |

**Pixel Data:** `DataSize` bytes immediately after the header. 8-bit indexed color values. When `DataSize > Width * Height`, the texture stores multiple animation frames sharing a single palette (`FrameCount = DataSize / (Width * Height)`).

**Palette:** `1024 Bytes` immediately after the pixel data. 256 entries of 4 bytes each in `R, G, B, Pad` order.

---

### [TextureEntry] (v8)
Size: `Variable` (`52 + DataSize + 1024` bytes per entry)  

**Texture Header:** `52 Bytes`

| Field | Type | Description |
| --- | --- | --- |
| Name1 | char[12] | Texture name, null-terminated |
| Name2 | char[12] | Alternate / Alpha texture (not mask) |
| Unknown | byte[4] | Always `0` |
| DataSize | uint32 | Pixel data block in bytes |
| Sequence | uint16 | Material sequence index |
| Flags | uint8 | Env / alpha flags |
| LodTag | uint8 | LOD index |
| Width | uint16 | Width (always 2^n) |
| Height | uint16 | Height (always 2^n) |
| Unknown | uint32 | |
| Unknown | uint32 | |
| Unknown | uint32 | |

**Pixel Data:** `DataSize` bytes immediately after the header. Two layouts exist:
- **Standard 8-bit indexed:** `DataSize == Width * Height` (or a multiple, for animation frames sharing one palette). Each byte is a palette index.
- **Ratio-2 (per-pixel alpha):** `DataSize == 2 * Width * Height`. Each pixel is two bytes: byte 0 is the palette index, byte 1 is an alpha value (`0x00` = transparent, `0xFF` = opaque). 

When the data size is a multiple of `Width * Height` greater than 1 and not equal to 2, the texture stores multiple animation frames sharing a single palette (`FrameCount = DataSize / (Width * Height)`).

**Palette:** `1024 Bytes` immediately after the pixel data. 256 entries of 4 bytes each in `B, G, R, Pad` order.

---

### [TextureEntry] (v10)
Size: `80 Bytes per entry`  

| Field | Type | Description |
| --- | --- | --- |
| Name1 | char[16] | Texture filename |
| Name2 | char[16] | Alpha-mask filename |
| Unknown | byte[4] | Always `0` |
| DataSize | uint32 | Pixel data block in bytes |
| Sequence | uint16 | Material sequence index |
| Flags | uint16 | Texture flags |
| Width | uint16 | Width (always 2^n) |
| Height | uint16 | Height (always 2^n) |
| Unknown | byte[32] | |

**Name2 alpha mask** - when `Name2` is non-empty, the engine pairs `Name1` and `Name2` as a primary + cutout-mask pair. `Name1` supplies RGB, `Name2` supplies per-pixel alpha via texel brightness.

---

### Texture Flags (v5 / v8)

| Bit | Mask | Name | Description |
| --- | --- | --- | --- |
| 0 | 0x01 | Env0 | Texture is enabled in Env `0` |
| 1 | 0x02 | Env1 | Texture is enabled in Env `1` |
| 2 | 0x04 | Env2 | Texture is enabled in Env `2` |
| 3 | 0x08 | AlwaysLoad | Load regardless of env |
| 4 | 0x10 | PreservePalette | Skip palette optimizer |
| 5 | 0x20 | ColorKey | Palette index `0` is alpha key |
| 6 | 0x40 | Unknown | |
| 7 | 0x80 | Unknown | |

### Texture Flags (v10)

| Bit | Mask | Name | Description |
| --- | --- | --- | --- |
| 0 | 0x0001 | Env0 | Texture is enabled in Env `0` |
| 1 | 0x0002 | Env1 | Texture is enabled in Env `1` |
| 2 | 0x0004 | Env2 | Texture is enabled in Env `2` |
| 3 | 0x0008 | AlwaysLoad | Load regardless of env |
| 4 | 0x0010 | PreservePalette | Skip palette optimizer |
| 5 | 0x0020 | ColorKey | Palette index `0` is alpha key |
| 6 | 0x0040 | Unknown | |
| 7 | 0x0080 | Unknown | |
| 8 | 0x0100 | DedupMatch | Texture match |
| 9 | 0x0200 | CreateColorSurface | Engine allocate an RGB texture surface |
| 10 | 0x0400 | CreateAlphaSurface | Engine allocate an alpha texture surface |
| 11 | 0x0800 | Hidden | No-texture marker, skipped |
| 12-15 | 0x1000-0x8000 | Unknown | |

---

### [LodObject] (v5)
Size: `Variable`  

**LOD-Object Header:** `184 Bytes`

| Field | Type | Description |
| --- | --- | --- |
| NameArea | byte[16] | Model name + LOD suffix (` H`, ` M`, ` L`, ` T`) |
| Flags | uint32 | Bit `0`: vertex coordinates are mesh-relative |
| DataSize | uint32 | Total bytes of data arrays |
| Unknown | uint32 | |
| Bounding1 | int32 | Bounding sphere component |
| Bounding2 | int32 | Bounding sphere component |
| ModelRadius | int32 | Model radius |
| Bbox | int32[6] | `MinX, MaxX, MinY, MaxY, MinZ, MaxZ` |
| Unknown | uint32 | |
| Unknown | byte[60] | 3DSMax Metadata? |
| VertexCount | uint32 | Number of `Vertex` records |
| Unknown | uint32 | |
| NormalCount | uint32 | Number of `Normal` records |
| Unknown | uint32 | |
| FaceCount | uint32 | Number of `Face` records |
| Unknown | uint32 | |
| MeshCount | uint32 | Number of `Mesh` records |
| Unknown | uint32 | |
| HardpointCount | uint32 | Number of `Hardpoint` records |
| Unknown | uint32 | |
| MaterialCount | uint32 | Number of `Material` records |
| Unknown | uint32 | |
| CollisionVolumeCount | uint32 | Number of `CollisionVolume` records |
| Unknown | uint32 | |

---

### [LodObject] (v8)
Size: `Variable`  

**LOD-Object Header:** `192 Bytes`

| Field | Type | Description |
| --- | --- | --- |
| NameArea | byte[16] | Model name + LOD suffix (` H`, ` M`, ` L`, ` T`) |
| Flags | uint32 | Bit `0`: vertex coordinates are mesh-relative |
| DataSize | uint32 | Total bytes of data arrays |
| Unknown | uint32 | |
| Bounding1 | int32 | Bounding sphere component |
| Bounding2 | int32 | Bounding sphere component |
| ModelRadius | int32 | Model radius |
| Bbox | int32[6] | `MinX, MaxX, MinY, MaxY, MinZ, MaxZ` |
| Unknown | uint32 | |
| Unknown | byte[60] | 3DSMax Metadata? |
| VertexCount | uint32 | Number of `Vertex` records |
| Unknown | uint32 | |
| NormalCount | uint32 | Number of `Normal` records |
| Unknown | uint32 | |
| FaceCount | uint32 | Number of `Face` records |
| Unknown | uint32 | |
| MeshCount | uint32 | Number of `Mesh` records |
| Unknown | uint32 | |
| HardpointCount | uint32 | Number of `Hardpoint` records |
| Unknown | uint32 | |
| MaterialCount | uint32 | Number of `Material` records |
| Unknown | uint32 | |
| PlaneCount | uint32 | Number of `Plane` records |
| Unknown | uint32 | |
| CollisionVolumeCount | uint32 | Number of `CollisionVolume` records |
| Unknown | uint32 | |

---

### [LodObject] (v10)
Size: `Variable`  

**LOD-Object Header:** `232 Bytes`

| Field | Type | Description |
| --- | --- | --- |
| NameArea | byte[16] | Model name + LOD suffix (` H`, ` M`, ` L`, ` T`) |
| Flags | uint32 | Bit `0`: vertex coordinates are mesh-relative |
| DataSize | uint32 | Total bytes of data arrays |
| Unknown | uint32 | |
| Bounding1 | int32 | Bounding sphere component |
| Bounding2 | int32 | Bounding sphere component |
| ModelRadius | int32 | Model radius |
| Bbox | int32[6] | `MinX, MaxX, MinY, MaxY, MinZ, MaxZ` |
| Unknown | uint32 | |
| Unknown | byte[60] | 3DSMax Metadata? |
| VertexCount | uint32 | Number of `Vertex` records |
| Unknown | uint32 | |
| NormalCount | uint32 | Number of `Normal` records |
| Unknown | uint32 | |
| FaceCount | uint32 | Number of `Face` records |
| Unknown | uint32 | |
| FaceColorCount | uint32 | Number of `FaceColor` records |
| Unknown | uint32 | |
| MeshCount | uint32 | Number of `Mesh` records |
| Unknown | uint32 | |
| HardpointCount | uint32 | Number of `Hardpoint` records |
| Unknown | uint32 | |
| MaterialCount | uint32 | Number of `Material` records |
| Unknown | uint32 | |
| PlaneCount | uint32 | Number of `Plane` records |
| Unknown | uint32 | |
| CollisionVolumeCount | uint32 | Number of `CollisionVolume` records |
| Unknown | uint32 | |
| Unknown | byte[32] | |

---

### [Data]
Size: `DataSize`  

The bulk-data arrays appear in the order below. Arrays absent in a given version are omitted from the file.

**v5:**

| # | Array | Count Field | Bytes / Entry |
| --- | --- | --- | --- |
| 1 | Vertices | `VertexCount` | 8 |
| 2 | Normals | `NormalCount` | 8 |
| 3 | Faces | `FaceCount` | 72 |
| 4 | Meshes | `MeshCount` | 112 |
| 5 | Hardpoints | `HardpointCount` | 12 |
| 6 | CollisionVolumes | `CollisionVolumeCount` | 72 |
| 7 | Materials | `MaterialCount` | 76 |

**v8:**

| # | Array | Count Field | Bytes / Entry |
| --- | --- | --- | --- |
| 1 | Vertices | `VertexCount` | 8 |
| 2 | Normals | `NormalCount` | 8 |
| 3 | Faces | `FaceCount` | 72 |
| 4 | Meshes | `MeshCount` | 112 |
| 5 | Hardpoints | `HardpointCount` | 12 |
| 6 | Planes | `PlaneCount` | 8 |
| 7 | CollisionVolumes | `CollisionVolumeCount` | 80 |
| 8 | Materials | `MaterialCount` | 120 |

**v10:**

| # | Array | Count Field | Bytes / Entry |
| --- | --- | --- | --- |
| 1 | Vertices | `VertexCount` | 8 |
| 2 | Normals | `NormalCount` | 8 |
| 3 | Faces | `FaceCount` | 80 |
| 4 | FaceColors | `FaceColorCount` | 12 |
| 5 | Meshes | `MeshCount` | 120 |
| 6 | Hardpoints | `HardpointCount` | 12 |
| 7 | Planes | `PlaneCount` | 8 |
| 8 | CollisionVolumes | `CollisionVolumeCount` | 80 |
| 9 | Materials | `MaterialCount` | 128 |

---

### [Vertex]
Size: `8 Bytes`  

| Field | Type | Description |
| --- | --- | --- |
| X | int16 | X coordinate |
| Y | int16 | Y coordinate |
| Z | int16 | Z coordinate |
| MeshIndex | uint16 | Index of the owning `Mesh` record |

---

### [Normal]
Size: `8 Bytes`  

| Field | Type | Description |
| --- | --- | --- |
| Nx | int16 | Normal X component, 1.14 fixed-point (divide by `16384`) |
| Ny | int16 | Normal Y component, 1.14 fixed-point |
| Nz | int16 | Normal Z component, 1.14 fixed-point |
| Flags | int16 | |

---

### [Face] (v5 / v8)
Size: `72 Bytes`  

| Field | Type | Description |
| --- | --- | --- |
| Flags | uint16 | Bit `0`: smooth-shaded (use per-vertex normals) |
| FaceNormalIndex | int16 | Index into `Normals` for the flat (face) normal |
| U | int32[3] | U coordinates per corner, 16.16 fixed-point (divide by `65536`) |
| V | int32[3] | V coordinates per corner, 16.16 fixed-point |
| VertexIndex | int16[3] | Mesh-relative indices into `Vertices`, one per corner |
| NormalIndex | int16[3] | Mesh-relative indices into `Normals`, one per corner |
| PlaneDistance | int32 | Triangle plane distance from origin |
| Bbox | int32[6] | Triangle bounding box (used by raycast) |
| MaterialIndex | uint32 | Index into `Materials` |

---

### [Face] (v10)
Size: `80 Bytes`  

| Field | Type | Description |
| --- | --- | --- |
| Flags | uint16 | Bit `0`: smooth-shaded (use per-vertex normals) |
| FaceNormalIndex | int16 | Index into `Normals` for the flat (face) normal |
| U | int32[3] | U coordinates per corner, 16.16 fixed-point (divide by `65536`) |
| V | int32[3] | V coordinates per corner, 16.16 fixed-point |
| VertexIndex | int16[3] | Mesh-relative indices into `Vertices`, one per corner |
| NormalIndex | int16[3] | Mesh-relative indices into `Normals`, one per corner |
| Remap | uint16[3] | Render-vertex remap indices, one per corner |
| Unknown | uint16 | |
| PlaneDistance | int32 | Triangle plane distance from origin |
| Bbox | int32[6] | Triangle bounding box (used by raycast) |
| MaterialIndex | uint32 | Index into `Materials` |

---

### [FaceColor] (v10)
Size: `12 Bytes`  

| Field | Type | Description |
| --- | --- | --- |
| Color0 | uint32 | Packed RGB for corner 0 (`0x00RRGGBB` format) |
| Color1 | uint32 | Packed RGB for corner 1 |
| Color2 | uint32 | Packed RGB for corner 2 |

---

### [Mesh] (v5 / v8)
Size: `112 Bytes`  

| Field | Type | Description |
| --- | --- | --- |
| Flags | uint32 | Mesh flags |
| VertexCount | uint32 | Number of vertices owned by this mesh |
| Unknown | uint32 | |
| FaceCount | uint32 | Number of faces owned by this mesh |
| Unknown | uint32 | |
| NormalCount | uint32 | Number of normals owned by this mesh |
| Unknown | uint32 | |
| CollisionVolumeCount | uint32 | Per-mesh collision volume count |
| Unknown | uint32 | |
| ParentMeshIndex | uint32 | Index of parent mesh in this lod-object's mesh array |
| DeltaOrigin | int32[3] | Engine computed offset relative to parent |
| Origin | int32[3] | Mesh origin in fixed-point with 8 fractional bits (`>> 8` for world units) |
| Bbox | int32[6] | Mesh-local bounding box |
| BSphereCenter | int32[3] | Bounding sphere center (`Bbox` center) |
| BSphereRadiusH | int32 | Horizontal bounding radius |
| BSphereRadiusV | int32 | Vertical bounding radius |
| ScaleRadius | int32 | Per-mesh scale radius |

---

### [Mesh] (v10)
Size: `120 Bytes`  

| Field | Type | Description |
| --- | --- | --- |
| Flags | uint32 | Mesh flags |
| VertexCount | uint32 | Number of vertices owned by this mesh |
| Unknown | uint32 | |
| FaceCount | uint32 | Number of faces owned by this mesh |
| Unknown | uint32 | |
| FaceColorCount | uint32 | Number of face-color owned by this mesh |
| Unknown | uint32 | |
| NormalCount | uint32 | Number of normals owned by this mesh |
| Unknown | uint32 | |
| CollisionVolumeCount | uint32 | Per-mesh collision volume count |
| Unknown | uint32 | |
| ParentMeshIndex | uint32 | Index of parent mesh in this lod-object's mesh array |
| DeltaOrigin | int32[3] | Engine computed offset relative to parent |
| Origin | int32[3] | Mesh origin in fixed-point with 8 fractional bits (`>> 8` for world units) |
| Bbox | int32[6] | Mesh-local bounding box |
| BSphereCenter | int32[3] | Bounding sphere center (`Bbox` center) |
| BSphereRadiusH | int32 | Horizontal bounding radius |
| BSphereRadiusV | int32 | Vertical bounding radius |
| ScaleRadius | int32 | Per-mesh scale radius |

---

### [Hardpoint]
Size: `12 Bytes`  

| Field | Type | Description |
| --- | --- | --- |
| X | int32 | X position in fixed-point (`>> 8` for world units) |
| Y | int32 | Y position |
| Z | int32 | Z position |

---

### [Plane] (v8 / v10)
Size: `8 Bytes`  

| Field | Type | Description |
| --- | --- | --- |
| Nx | int16 | Plane normal X, 1.14 fixed-point (divide by `16384`) |
| Ny | int16 | Plane normal Y, 1.14 fixed-point |
| Nz | int16 | Plane normal Z, 1.14 fixed-point |
| D | int16 | Plane distance from origin |

---

### [CollisionVolume] (v5)
Size: `72 Bytes`  

| Field | Type | Description |
| --- | --- | --- |
| Flags | uint32 | Volume flags |
| Type | uint32 | Volume / node type |
| Bbox | int32[6] | `MinX, MaxX, MinY, MaxY, MinZ, MaxZ` |
| PlaneNx | int32 | Splitting plane normal X, 1.14 fixed-point |
| PlaneNy | int32 | Splitting plane normal Y |
| PlaneNz | int32 | Splitting plane normal Z |
| PlaneD | int32 | Splitting plane distance |
| ChildFront | int32 | Index of front BSP child (or sentinel) |
| ChildBack | int32 | Index of back BSP child |
| Unknown | byte[16] | |

---

### [CollisionVolume] (v8 / v10)
Size: `80 Bytes`  

| Field | Type | Description |
| --- | --- | --- |
| Flags | uint32 | Volume flags |
| Type | uint32 | Volume / node type |
| Bbox | int32[6] | `MinX, MaxX, MinY, MaxY, MinZ, MaxZ` |
| PlaneNx | int32 | Splitting plane normal X, 1.14 fixed-point |
| PlaneNy | int32 | Splitting plane normal Y |
| PlaneNz | int32 | Splitting plane normal Z |
| PlaneD | int32 | Splitting plane distance |
| ChildFront | int32 | Index of front BSP child (or sentinel) |
| ChildBack | int32 | Index of back BSP child |
| Unknown | byte[16] | |
| PlaneCount | uint32 | Number of `Plane` records referenced |
| Unknown | uint32 | |

---

### [Material] (v5)
Size: `76 Bytes`  

| Field | Type | Description |
| --- | --- | --- |
| Name | char[12] | Material name |
| Unknown | byte[4] | Always `0` |
| Flags | uint32 | Material flags |
| DiffuseColor | uint32 | Runtime packed BGRA |
| TextureIndex | int16 | Index into `Textures` array |
| Unknown | byte[2] | Always `0` |
| ScaleValue | int16 | Animated frame scale factor |
| FrameStep | int8 | Animated frame multiplier |
| FrameCount | int8 | Number of animation frames |
| WidthLog2 | int16 | Runtime `log2(TextureWidth)` |
| HeightLog2 | int16 | Runtime `log2(TextureHeight)` |
| WidthMask | int16 | Runtime `(1 << WidthLog2) - 1` |
| HeightMask | int16 | Runtime `(1 << HeightLog2) - 1` |
| EnvFillRgb | uint8[4][3] | Env solid fill color |
| EnvRefs | uint8[16] | Env texture sequence selectors |
| SpecularIntensity | int32 | Specular highlight strength |
| FlatColor | int32 | Lighting color, 16.16 fixed-point |

---

### [Material] (v8)
Size: `120 Bytes`  

| Field | Type | Description |
| --- | --- | --- |
| Name | char[12] | Material name |
| Unknown | byte[4] | Always `0` |
| Flags | uint32 | Material flags |
| DiffuseColor | uint32 | Runtime packed BGRA |
| TextureIndex | int16 | Index into `Textures` array |
| Unknown | byte[2] | Always `0` |
| ScaleValue | int16 | Animated frame scale factor |
| FrameStep | int8 | Animated frame multiplier |
| FrameCount | int8 | Number of animation frames |
| WidthLog2 | int16 | Runtime `log2(TextureWidth)` |
| HeightLog2 | int16 | Runtime `log2(TextureHeight)` |
| WidthMask | int16 | Runtime `(1 << WidthLog2) - 1` |
| HeightMask | int16 | Runtime `(1 << HeightLog2) - 1` |
| EnvFillRgb | uint8[4][3] | Env solid fill color |
| EnvRefs | uint8[16] | Env texture sequence selectors |
| Unknown | uint32 | |
| Unknown | uint32 | |
| Unknown | uint32 | |
| Unknown | uint32 | |
| HwDiffuseColor | uint32 | hardware-renderer copy of `DiffuseColor` |
| HwSizeLog2 | uint8[2] | hardware-renderer width / height log2 |
| Unknown | byte[2] | Always `0` |
| HwRenderMode | uint32 | hardware render-state flags |
| Unknown | byte[8] | Always `0` |
| Unknown | uint32 | |
| RenderFlags | uint32 | Runtime |
| Padding | byte[8] | Always `0` |

---

### [Material] (v10)
Size: `128 Bytes`  

| Field | Type | Description |
| --- | --- | --- |
| Name | char[12] | Material name |
| Unknown | byte[4] | Always `0` |
| Flags | uint32 | Material flags |
| DiffuseColor | uint32 | Runtime packed BGRA |
| TextureIndex | int16 | Index into `Textures` array |
| Unknown | byte[2] | Always `0` |
| ScaleValue | int16 | Animated frame scale factor |
| FrameStep | int8 | Animated frame multiplier |
| FrameCount | int8 | Number of animation frames |
| WidthLog2 | int16 | Runtime `log2(TextureWidth)` |
| HeightLog2 | int16 | Runtime `log2(TextureHeight)` |
| WidthMask | int16 | Runtime `(1 << WidthLog2) - 1` |
| HeightMask | int16 | Runtime `(1 << HeightLog2) - 1` |
| EnvFillRgb | uint8[4][3] | Env solid fill color |
| EnvRefs | uint8[16] | Env texture sequence selectors |
| Unknown | uint32 | |
| Unknown | uint32 | |
| Unknown | uint32 | |
| UvOffsetU | float32 | U offset |
| UvOffsetV | float32 | V offset |
| UvScaleU | float32 | UV tiling factor U |
| UvScaleV | float32 | UV tiling factor V |
| Unknown | byte[4] | Always `0` |
| Unknown | byte[4] | |
| Unknown | byte[4] | Always `0` |
| RenderFlags | uint32 | Runtime |
| BlendMode | uint8 | `0` = auto, `1` = opaque, `2`-`3` = alpha, `4` = add, `5` = sub |
| Padding | byte[15] | Always `0` |

---

### Material Flags (v5)

| Bit | Mask | Name | Description |
| --- | --- | --- | --- |
| 0 | 0x0001 | Textured | Material samples a texture for fill |
| 1 | 0x0002 | DoubleSided | Render both faces |
| 2 | 0x0004 | AltClut | light-darken effect on grayscale palettes |
| 3 | 0x0008 | Gouraud | Smooth shading |
| 5 | 0x0020 | FlatLit | Skip lighting |
| 6 | 0x0040 | DarkenShade | Darken the gouraud shade output |
| 7 | 0x0080 | Alpha50 | 50% alpha blend with palette index 0 color key |
| 9 | 0x0200 | ColorKey | Alpha `ColorKey` |
| 10 | 0x0400 | ShadowPriority | Shadow priority |
| 11 | 0x0800 | Hidden | Face skipped |
| 14 | 0x4000 | Animated | Cycle material frames |
| 15 | 0x8000 | AlphaBlend | Texel brightness as alpha |

### Material Flags (v8)

| Bit | Mask | Name | Description |
| --- | --- | --- | --- |
| 0 | 0x0001 | Textured | Material samples a texture for fill |
| 1 | 0x0002 | DoubleSided | Render both faces |
| 3 | 0x0008 | HiddenAuto | Bound texture missing |
| 5 | 0x0020 | FlatLit | Skip lighting |
| 7 | 0x0080 | SpecialBlend | Special alpha rendering |
| 9 | 0x0200 | ColorKey | Alpha `ColorKey` |
| 10 | 0x0400 | ShadowPriority | Shadow priority |
| 11 | 0x0800 | Hidden | Face skipped |
| 14 | 0x4000 | Animated | Cycle material frames |
| 15 | 0x8000 | AlphaBlend | Alpha blend mode |

### Material Flags (v10)

| Bit | Mask | Name | Description |
| --- | --- | --- | --- |
| 0 | 0x00000001 | Textured | Material samples a texture for fill |
| 1 | 0x00000002 | DoubleSided | Render both faces |
| 3 | 0x00000008 | Surface15Alt | Bullet impact surface type 15 |
| 4 | 0x00000010 | AlphaTest | Enable alpha test |
| 5 | 0x00000020 | FlatLit | Skip lighting |
| 7 | 0x00000080 | ConstantAlpha | Per-material constant alpha |
| 9 | 0x00000200 | NoBulletHit | Face is transparent to bullets and raycast |
| 11 | 0x00000800 | Hidden | Face skipped |
| 12 | 0x00001000 | ImpactFlag | OR'd into the runtime impact bits as `0x01000000` |
| 14 | 0x00004000 | Animated | Cycle material frames |
| 15 | 0x00008000 | AlphaBlend | Alpha blend mode (name2) |
| 16 | 0x00010000 | Surface14a | Bullet impact surface type 14 |
| 17 | 0x00020000 | Surface13 | Bullet impact surface type 13 |
| 18 | 0x00040000 | Surface12 | Bullet impact surface type 12 |
| 19 | 0x00080000 | Surface17 | Bullet impact surface type 17 (foliage / leaves) |
| 26 | 0x04000000 | Surface14b | Bullet impact surface type 14 (scope / window panes) |
| 27 | 0x08000000 | Surface16 | Bullet impact surface type 16 (cloth / flag textures) |
| 28 | 0x10000000 | Surface15 | Bullet impact surface type 15 (glass / wheel) |
| 29 | 0x20000000 | Unknown | |

---

## Coordinate System and Fixed-Point Encoding

| Quantity | Type | Conversion to World Units |
| --- | --- | --- |
| Vertex X / Y / Z | int16 | direct |
| Normal X / Y / Z | int16 (1.14 FP) | divide by `16384` |
| Mesh Origin | int32 (24.8 FP) | shift right by 8 |
| Hardpoint X / Y / Z | int32 (24.8 FP) | shift right by 8 |
| UV U / V (v5, v8) | int32 (16.16 FP) | divide by `65536` |
| UV U / V (v10) | int32 (16.16 FP) | divide by `65536` * (`UvScaleU` / `UvScaleV`) |
| Plane Normal (v8, v10) | int16 (1.14 FP) | divide by `16384` |
| Material UV Scale (v10) | float32 | direct |
| LOD Distance (v10) | uint32 (16.16 FP) | divide by `65536` |
