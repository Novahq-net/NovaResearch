# Tachyon: The Fringe DISP04A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP04A.SPX` |
| Sector | `QUAD_04` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 3 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 19 |
| Events | 19 |
| Waypoints | 5 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Navigational_Bouy`, `1: Bora_Dagger` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFNE_01`, `CLEON`, `SPIKE` |
| Aliases | `Coward`, `spy_1`, `SPIKE` |
| Groups | `FG_RECTITUDE`, `FG_METTLE`, `FG_STOUT`, `FG_FIDELITY`, `FG_FAITH` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Object spawn/action: Navigational_Bouy (object 15, id 155), subtype 14
- Show/update HUD contact: contact/list 0, subtype 9, param 18
- Group/spawn-list action: spawn list/group 266, subtype 1, param 2
- Play dialog: PLAYER.SCR, line/variant 124

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 154; flags 2)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Set/add variable: variable group 18, variable 406, subtype 0, value 1
- Set/add variable: variable group 18, variable 407, subtype 0, value 2
- Set/add variable: variable group 8, variable 8, subtype 0, value 0
- Play scene: unknown index 0, param 0
- Broadcast hide/remove contact: contact/list 0, subtype 0, param 11
- Set/add variable: variable group 38, variable 7, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 5, value 0 (extra 1, 154; flags 2)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 12, param 24
- Object spawn/action: Navigational_Bouy (object 15, id 155), subtype 15

### Event 3

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 262, subtype 0
- Group/spawn-list action: spawn list/group 265, subtype 0
- Group/spawn-list action: spawn list/group 263, subtype 0
- Group/spawn-list action: spawn list/group 264, subtype 0

### Event 4

**Trigger**

- Object event: subject Bora_Dagger (object 0, id 50), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Bora_Dagger (object 0, id 50), subtype 7

### Event 5

**Trigger**

- Object event: subject Bora_Dagger (object 1, id 51), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Bora_Dagger (object 1, id 51), subtype 7

### Event 6

**Trigger**

- Object event: subject Bora_Dagger (object 2, id 52), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Bora_Dagger (object 2, id 52), subtype 7

### Event 7

**Trigger**

- Object event: subject Bora_Dagger (object 3, id 54), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Bora_Dagger (object 3, id 54), subtype 7

### Event 8

**Trigger**

- Object event: subject Bora_Dagger (object 4, id 56), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Bora_Dagger (object 4, id 56), subtype 7

### Event 9

**Trigger**

- Object event: subject Bora_Dagger (object 5, id 57), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Bora_Dagger (object 5, id 57), subtype 7

### Event 10

**Trigger**

- Object event: subject Bora_Dagger (object 6, id 58), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Bora_Dagger (object 6, id 58), subtype 7

### Event 11

**Trigger**

- Object event: subject Bora_Dagger (object 7, id 59), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Bora_Dagger (object 7, id 59), subtype 7

### Event 12

**Trigger**

- Object event: subject Bora_Dagger (object 8, id 60), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Bora_Dagger (object 8, id 60), subtype 7

### Event 13

**Trigger**

- Object event: subject Bora_Dagger (object 9, id 62), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Bora_Dagger (object 9, id 62), subtype 7

### Event 14

**Trigger**

- Object event: subject Bora_Dagger (object 10, id 64), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Bora_Dagger (object 10, id 64), subtype 7

### Event 15

**Trigger**

- Object event: subject Bora_Dagger (object 11, id 65), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Bora_Dagger (object 11, id 65), subtype 7

### Event 16

**Trigger**

- Object event: subject Bora_Dagger (object 12, id 66), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Bora_Dagger (object 12, id 66), subtype 7

### Event 17

**Trigger**

- Object event: subject Bora_Dagger (object 13, id 68), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Bora_Dagger (object 13, id 68), subtype 7

### Event 18

**Trigger**

- Object event: subject Bora_Dagger (object 14, id 69), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Bora_Dagger (object 14, id 69), subtype 7

## Waypoints

### Waypoint 0

- Tag: `106`
- Members: `Bora_Dagger (object 3, id 54, starts at point -1)`, `Bora_Dagger (object 4, id 56, starts at point -1)`, `Bora_Dagger (object 5, id 57, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-818.31, 0.00, -605.28) | None |
| 1 | (-1083.51, 0.00, -780.05) | None |
| 2 | (-108.52, 0.00, -1444.19) | None |
| 3 | (640.28, 0.00, -1147.07) | None |
| 4 | (359.48, 0.00, -998.52) | None |

### Waypoint 1

- Tag: `104`
- Members: `Bora_Dagger (object 0, id 50, starts at point -1)`, `Bora_Dagger (object 1, id 51, starts at point -1)`, `Bora_Dagger (object 2, id 52, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (850.02, 0.00, -219.17) | None |
| 1 | (1138.42, 0.00, -403.80) | None |
| 2 | (985.39, 0.00, -918.15) | None |
| 3 | (520.41, 0.00, -812.65) | None |
| 4 | (67.20, 0.00, -904.97) | None |
| 5 | (-491.96, 0.00, -687.36) | None |
| 6 | (-750.94, 0.00, -364.24) | on arrival redirect to Waypoint 2 (tag 103), point 0 |

### Waypoint 2

- Tag: `103`
- Members: `Bora_Dagger (object 9, id 62, starts at point -1)`, `Bora_Dagger (object 10, id 64, starts at point -1)`, `Bora_Dagger (object 11, id 65, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-911.11, 0.00, 673.95) | None |
| 1 | (-1199.91, 0.00, 379.75) | None |
| 2 | (-1097.36, 0.00, 137.51) | None |
| 3 | (-685.35, 0.00, 335.34) | None |
| 4 | (-245.49, 0.00, 979.17) | None |
| 5 | (598.45, 0.00, 943.43) | None |
| 6 | (826.47, 0.00, 361.13) | on arrival redirect to Waypoint 1 (tag 104), point 0 |
| 7 | (1045.15, 0.00, -63.48) | on arrival redirect to Waypoint 1 (tag 104), point 0 |

### Waypoint 3

- Tag: `102`
- Members: `Bora_Dagger (object 12, id 66, starts at point -1)`, `Bora_Dagger (object 13, id 68, starts at point -1)`, `Bora_Dagger (object 14, id 69, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-169.33, 271.12, 503.65) | None |
| 1 | (-169.33, -105.86, 517.47) | None |
| 2 | (-169.33, -407.96, 487.51) | None |
| 3 | (0.00, -467.35, 64.53) | None |
| 4 | (280.45, -444.11, -246.20) | None |
| 5 | (280.45, -237.55, -342.99) | None |
| 6 | (280.45, 400.22, -338.38) | None |
| 7 | (0.00, 608.69, -205.12) | None |
| 8 | (-169.33, 591.08, 238.41) | on arrival redirect to Waypoint 4 (tag 101), point 0 |

### Waypoint 4

- Tag: `101`
- Members: `Bora_Dagger (object 6, id 58, starts at point -1)`, `Bora_Dagger (object 7, id 59, starts at point -1)`, `Bora_Dagger (object 8, id 60, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1.03, 215.21, 738.00) | None |
| 1 | (-474.09, 215.21, 463.26) | None |
| 2 | (-635.02, 215.21, -214.99) | None |
| 3 | (-6.64, 215.21, -627.09) | None |
| 4 | (614.08, 215.21, -360.94) | None |
| 5 | (568.10, 215.21, 403.17) | on arrival redirect to Waypoint 3 (tag 102), point 0 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Bora_Dagger` | 50 | Interactive | 920.59,0.00,-361.87 | 0,0,0 | group/role: FG_RECTITUDE / 0; waypoint: Waypoint 1 (tag 104, 7 point(s)), starting point -1 |
| 1 | `Bora_Dagger` | 51 | Interactive | 865.16,0.00,-361.87 | 0,0,0 | group/role: FG_RECTITUDE / 0; waypoint: Waypoint 1 (tag 104, 7 point(s)), starting point -1 |
| 2 | `Bora_Dagger` | 52 | Interactive | 859.00,0.00,-437.77 | 0,0,0 | group/role: FG_RECTITUDE / 0; waypoint: Waypoint 1 (tag 104, 7 point(s)), starting point -1 |
| 3 | `Bora_Dagger` | 54 | Interactive | -776.57,0.00,-900.50 | 0,0,0 | group/role: FG_METTLE / 0; waypoint: Waypoint 0 (tag 106, 5 point(s)), starting point -1 |
| 4 | `Bora_Dagger` | 56 | Interactive | -770.41,0.00,-969.51 | 0,0,0 | group/role: FG_METTLE / 0; waypoint: Waypoint 0 (tag 106, 5 point(s)), starting point -1 |
| 5 | `Bora_Dagger` | 57 | Interactive | -733.45,0.00,-969.51 | 0,0,0 | group/role: FG_METTLE / 0; waypoint: Waypoint 0 (tag 106, 5 point(s)), starting point -1 |
| 6 | `Bora_Dagger` | 58 | Interactive | 223.88,222.15,797.43 | 365,0,0 | group/role: FG_STOUT / 0; waypoint: Waypoint 4 (tag 101, 6 point(s)), starting point -1 |
| 7 | `Bora_Dagger` | 59 | Interactive | 273.16,222.15,804.33 | 365,0,0 | group/role: FG_STOUT / 0; waypoint: Waypoint 4 (tag 101, 6 point(s)), starting point -1 |
| 8 | `Bora_Dagger` | 60 | Interactive | 223.88,222.15,749.13 | 365,0,0 | group/role: FG_STOUT / 0; waypoint: Waypoint 4 (tag 101, 6 point(s)), starting point -1 |
| 9 | `Bora_Dagger` | 62 | Interactive | -610.72,0.00,763.97 | 332,0,0 | group/role: FG_FIDELITY / 0; waypoint: Waypoint 2 (tag 103, 8 point(s)), starting point -1 |
| 10 | `Bora_Dagger` | 64 | Interactive | -610.72,0.00,715.67 | 332,0,0 | group/role: FG_FIDELITY / 0; waypoint: Waypoint 2 (tag 103, 8 point(s)), starting point -1 |
| 11 | `Bora_Dagger` | 65 | Interactive | -561.45,0.00,694.97 | 332,0,0 | group/role: FG_FIDELITY / 0; waypoint: Waypoint 2 (tag 103, 8 point(s)), starting point -1 |
| 12 | `Bora_Dagger` | 66 | Interactive | 61.18,384.77,540.77 | 357,0,0 | group/role: FG_FAITH / 0; waypoint: Waypoint 3 (tag 102, 9 point(s)), starting point -1 |
| 13 | `Bora_Dagger` | 68 | Interactive | 48.86,384.77,478.67 | 357,0,0 | group/role: FG_FAITH / 0; waypoint: Waypoint 3 (tag 102, 9 point(s)), starting point -1 |
| 14 | `Bora_Dagger` | 69 | Interactive | 91.98,384.77,464.87 | 357,0,0 | group/role: FG_FAITH / 0; waypoint: Waypoint 3 (tag 102, 9 point(s)), starting point -1 |
| 15 | `Navigational_Bouy` | 155 | Interactive | -661.33,121.00,101.71 | 0,0,0 | None |
| 16 | `Navigational_Bouy` | 156 | Interactive | -661.82,121.00,-32.82 | 0,0,0 | None |
| 17 | `Navigational_Bouy` | 162 | Interactive | -585.14,120.00,36.83 | 383,0,0 | None |
| 18 | `Navigational_Bouy` | 163 | Interactive | -736.66,120.00,36.83 | 383,0,0 | None |
