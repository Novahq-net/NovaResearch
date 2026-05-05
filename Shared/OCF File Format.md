# NovaLogic OCF File Format
Visit [https://novahq.net](https://novahq.net) for more information on NovaLogic file formats and tools to work with these files.  

This information was gathered from reverse engineering the formats statically and while loaded in-game. Some of the entries are best guesses based on behaviour after loading into the engine or inferred from the data. While researching, some of the fields were renamed or re-identified and may be inconsistent across versions. If you have any corrections or insights, please create an issue or submit a pull request.

## OCF Information
The `.OCF` file is the top-level composition manifest used by `Tachyon: The Fringe` to combine several `.PAK` files into one single model.

**Encryption:** OCF files are stored as encrypted CBIN-format binaries. See [CBIN file format](./CBIN%20File%20Format.md)

## OCF Format
```
File
  [header]                  metadata
  [paks]                    PAK refs
  [part_00]                 root part (no parent)
  [part_01]                 child part with ATTACH = "part_00", ...
  [part_02]                 []...
  ...
```

## OCF Structure

### [header]

| Key | Type | Description |
| --- | --- | --- |
| NAME | string | Model name (e.g. `"THREGATON"`, `"MULTIBGROID"`) |
| NUMPAKS | int | Number of `PAK` files referenced |
| NUMPARTS | int | Number of `part_NN` sections |

---

### [paks]

**`PAK` entry:** comma-separated value list
```
PAK = "pak_name", "filename.PAK", "palette.PAL", vertex_hint, type_flag
```

| Field | Type | Description |
| --- | --- | --- |
| PAKName | string | Used by `part_NN` `PAK =` fields to bind a part to this PAK |
| Filename | string | 3DPK model filename to load |
| Palette | string | `.PAL` palette filename |
| VertexHint | int | Vertex count |
| TypeFlag | int | Sub-type  `0` (static), `2` (turret), `4` (generator), `5` (shield), `9` (power) |

The PAK file itself follows the [PAK File Format](./PAK%20File%20Format.md). TTF uses PAK v0x2003.

---

### [part_NN]
*Notes: One per part instance, with `NN` zero-padded (`part_00`, `part_01`, ...). `part_00` is the root part; it has no `ATTACH` and is positioned at the OCF's local origin `(0, 0, 0)`. All other parts must declare an `ATTACH` referencing an earlier-numbered part.*

| Key | Type | Description |
| --- | --- | --- |
| NAME | string | Unique part instance name |
| PAK | string | PAK name |
| SCALE | float | Scale factor |
| ANGLES | float[3] | Initial orientation `(X, Y, Z)` in degrees |
| ROTATE | float[3] | Additional rotation `(X, Y, Z)` in degrees |
| ATTACH | string, int, int | Parent part name, parent attach-point index, child attach-point index |
| TYPE | int | `0` = structural, `2` = turret / weapon, `4` = shield, `6` = engine |
| SUB_TYPE | int | `0` = default, `4` = heavy turret, `6` = beam weapon, `7` = defense turret |
| PART_ID | int | Gameplay-side part identifier |
| HITPOINTS | int | Destructible part health |
| DOCK | int, float | Dock id, dock distance |
| LAUNCH_DOCK | int | Launch bay dock id |
| LAND_DOCK | int, float | Dock id, distance |
| RELOAD_DOCK | int, float | Dock id, distance |
| CREDIT_POWERPLANT | int | Power-plant flag |
| SOUND_LOOP | string | Ambient sound name |

---

## Position Assembly
Each part's world-space position is computed once at OCF load time by walking the `ATTACH` tree from `part_00` outward. Each part stores its own world position. The renderer uses each part's local rotation when drawing its geometry but does **not** inherit parent rotations into the child's transform.

For a non-root part, the position is:

```
parent_attach_world = parent.world_pos + R(parent.angles) * (parent.attach[parent_idx] * parent.scale)
child_attach_local  = R(child.angles)  * (child.attach[child_idx]  * child.scale)
child.world_pos     = parent_attach_world - child_attach_local
```

Where `R(angles)` is the orientation matrix described below, and `parent.attach[i]` is the i-th attachment point of the PAK referenced by the parent.

**Each part keeps its own facing direction.** Spinning the parent moves the child's position (because the parent's attachment point is rotated with it) but does not rotate the child's geometry. Each child's `ANGLES` are set to the orientation it should have in world coordinates, regardless of the parent's orientation.

---

## Attachment Points
Each PAK's embedded 3DO model carries an array of **attachment points** immediately after its `Hardpoints` array. The 3DO header field at offset `0x40` holds the attachment-point count, and each attachment point is a 16-byte record:

| Field | Type | Description |
| --- | --- | --- |
| X | int32 | Position X |
| Y | int32 | Position Y |
| Z | int32 | Position Z |
| Radius | uint32 | Snap / collision radius |

---

## Coordinate System and Rotation Matrix

`ANGLES` and `ROTATE` are stored as floats in degrees in the OCF file. The engine converts them to a per-part orientation matrix at load time. The rotation order combines all three axes in a single composite transform:

```
V' = R_y(ANGLES[0]) * R_x_LH(ANGLES[1]) * R_z(ANGLES[2]) * V
```

- `ANGLES[0]` rotates around the Y axis (outermost step)
- `ANGLES[1]` rotates around the X axis with left-handed sign convention
- `ANGLES[2]` rotates around the Z axis (innermost step)

`SCALE` is a uniform multiplier applied before the rotation.

**Coordinate axis swap (PAK loader):** the 3DPK loader applies a fixed `(X, Y, Z) -> (X, Z, -Y)` swap to all 3DO vertex positions, normals, mesh entries, and attachment points as it loads each PAK. OCF `ANGLES` values are set in the **post-swap** coordinate space. 