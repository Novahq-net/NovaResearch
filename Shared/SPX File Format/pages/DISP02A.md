# Tachyon: The Fringe DISP02A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP02A.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 5 |
| Entities | 28 |
| Events | 31 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 5 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Mace`, `1: Susan_Bradley_Waraxe`, `2: GalSpan_Merc_Corvus`, `3: Bora_Battleaxe`, `4: Satellite` |
| Scripts | `PLAYER.SCR`, `SUSAN.SCR`, `BOACE.SCR`, `MERCB.SCR`, `MERCA.SCR` |
| Scenes | None |
| Labels | `BFGE_03`, `BFGF_03`, `MERC_17`, `BFNE_01`, `CLEON`, `Patrol1`, `Patrol2`, `SPIKE`, `Redemption` |
| Aliases | `BC10_Claymore1`, `BC10_Claymore2`, `BC10_Claymore3`, `BC10_Claymore4`, `Coward`, `BC10_Waraxe`, `BC10_Mace1`, `BC10_Mace2`, `BC10_Mace3`, `BC10_Mace4`, `BC10_Warhammer1`, `BC10_Warhammer2`, `BC10_Warhammer3`, `BC10_Warhammer4`, `SPIKE`, `Stocks01` |
| Groups | `FG_BACKBONE`, `FG_PAVO`, `FG_TEGEA`, `FG_LEPUS`, `FG_IXION`, `FG_FORNAX`, `FG_VELA`, `FG_GRACE`, `SUSAN_BRADLEY`, `FG_RESOLVE`, `FG_BRAVERY` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Object spawn/action: Satellite (object 0, id 109), subtype 7
- Object spawn/action: Satellite (object 1, id 110), subtype 7
- Player inventory/default-state: param 0, subtype 1, param 10
- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 5 (join 2)

**Action**

- Gate state/action: param 1, subtype 3, param 0

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 10

**Action**

- Play scene: unknown index 0, param 0
- Group/spawn-list action: spawn list/group 174, subtype 1, param 2
- Play dialog: PLAYER.SCR, line/variant 15

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 20

**Action**

- Group/spawn-list action: spawn list/group 173, subtype 1, param 2

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 30

**Action**

- Group/spawn-list action: spawn list/group 175, subtype 1, param 2
- Play dialog: PLAYER.SCR, line/variant 15

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 40

**Action**

- Group/spawn-list action: spawn list/group 176, subtype 1, param 2

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 50

**Action**

- Group/spawn-list action: spawn list/group 178, subtype 1, param 2

### Event 7

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 50

**Action**

- Group/spawn-list action: spawn list/group 177, subtype 1, param 2

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 56 (join 2)

**Action**

- Gate state/action: param 2, subtype 3, param 0
- Object spawn/action: Satellite (object 2, id 111), subtype 7
- Object spawn/action: Satellite (object 3, id 112), subtype 7
- Set runtime trigger variable: variable group 20, variable 0, subtype 1, value 0
- Broadcast hide/remove contact: contact/list 0, subtype 0, param 9
- Show/update HUD contact: contact/list 0, subtype 9, param 12

### Event 9

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 50

**Action**

- Set/add variable: variable group 21, variable 20, subtype 0, value 1

### Event 10

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Area/player/sector/dock/time event: subject 0, op 0, value 70

**Action**

- Set/add variable: variable group 21, variable 21, subtype 0, value 1

### Event 11

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 1
- Area/player/sector/dock/time event: subject 0, op 0, value 90

**Action**

- Set/add variable: variable group 21, variable 22, subtype 0, value 1

### Event 12

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Variable comparison: subject variable group 21, variable 21, op 1, value 1
- Variable comparison: subject variable group 21, variable 22, op 1, value 1 (join 1)
- Variable comparison: subject variable group 21, variable 23, op 1, value 1 (join 1)

**Action**

- Gate state/action: param 2, subtype 2, param 0
- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0

### Event 13

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 61

**Action**

- Group/spawn-list action: spawn list/group 171, subtype 1, param 2
- Group/spawn-list action: spawn list/group 170, subtype 1, param 2
- Group/spawn-list action: spawn list/group 179, subtype 1, param 2
- Group/spawn-list action: spawn list/group 172, subtype 1, param 2
- Play dialog: SUSAN.SCR, line/variant 0
- Set runtime trigger variable: variable group 20, variable 0, subtype 1, value 0

### Event 14

**Trigger**

- Global enemy/object-count event: subject 0, op 0, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Gate state/action: param 1, subtype 2, param 0
- Set/add variable: variable group 18, variable 402, subtype 0, value 1
- Set/add variable: variable group 18, variable 403, subtype 0, value 2
- Play dialog: SUSAN.SCR, line/variant 2
- Hide/remove HUD contact: contact/list 0, subtype 9, param 12
- Show/update HUD contact: contact/list 0, subtype 12, param 24

### Event 15

**Trigger**

- Object event: subject Susan_Bradley_Waraxe (object 19, id 372), op 0, value 0 (flags 2)

**Action**

- Play dialog: SUSAN.SCR, line/variant 5

### Event 16

**Trigger**

- Object event: subject Bora_Battleaxe (object 4, id 374), op 0, value 0 (flags 2)

**Action**

- Play dialog: BOACE.SCR, line/variant 0

### Event 17

**Trigger**

- Object event: subject GalSpan_Merc_Corvus (object 9, id 138), op 3, value 20 (join 2)
- Object event: subject GalSpan_Merc_Corvus (object 8, id 123), op 3, value 20 (join 2)
- Object event: subject GalSpan_Merc_Corvus (object 10, id 124), op 3, value 20 (join 2)
- Object event: subject 118, op 3, value 20 (join 2)
- Object event: subject GalSpan_Merc_Corvus (object 18, id 121), op 3, value 20 (join 2)
- Object event: subject 115, op 3, value 20 (join 2)

**Action**

- Play dialog: MERCB.SCR, line/variant 1

### Event 18

**Trigger**

- Object event: subject GalSpan_Merc_Corvus (object 14, id 122), op 4, value 50 (join 2)
- Object event: subject GalSpan_Merc_Corvus (object 15, id 139), op 4, value 70 (join 2)
- Object event: subject GalSpan_Merc_Corvus (object 16, id 125), op 4, value 70 (join 2)
- Object event: subject GalSpan_Merc_Corvus (object 17, id 117), op 4, value 70 (join 2)
- Object event: subject GalSpan_Merc_Corvus (object 12, id 120), op 4, value 70 (join 2)
- Object event: subject GalSpan_Merc_Corvus (object 7, id 113), op 4, value 70 (join 2)

**Action**

- Play dialog: MERCA.SCR, line/variant 2

### Event 19

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 70

**Action**

- Play dialog: PLAYER.SCR, line/variant 22

### Event 20

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 22
- Area/player/sector/dock/time event: subject 0, op 0, value 100

**Action**

- Play dialog: PLAYER.SCR, line/variant 21

### Event 21

**Trigger**

- Group/spawn-list event: subject 172, op 3, value 0
- Group/spawn-list event: subject 170, op 3, value 0
- Group/spawn-list event: subject 171, op 3, value 0
- Group/spawn-list event: subject 179, op 3, value 0

**Action**

- Gate state/action: param 2, subtype 3, param 0

### Event 22

**Trigger**

- Variable comparison: subject variable group 21, variable 23, op 1, value 1 (join 1)
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Gate state/action: param 2, subtype 2, param 0
- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0

### Event 23

**Trigger**

- Group/spawn-list event: subject 173, op 1, value 50

**Action**

- Set/add variable: variable group 21, variable 12, subtype 0, value 1

### Event 24

**Trigger**

- Group/spawn-list event: subject 175, op 1, value 50

**Action**

- Set/add variable: variable group 21, variable 13, subtype 0, value 1

### Event 25

**Trigger**

- Group/spawn-list event: subject 177, op 1, value 50

**Action**

- Set/add variable: variable group 21, variable 14, subtype 0, value 1

### Event 26

**Trigger**

- Group/spawn-list event: subject 174, op 1, value 50

**Action**

- Set/add variable: variable group 21, variable 15, subtype 0, value 1

### Event 27

**Trigger**

- Group/spawn-list event: subject 176, op 1, value 50

**Action**

- Set/add variable: variable group 21, variable 16, subtype 0, value 1

### Event 28

**Trigger**

- Group/spawn-list event: subject 178, op 1, value 50

**Action**

- Set/add variable: variable group 21, variable 17, subtype 0, value 1

### Event 29

**Trigger**

- Variable comparison: subject variable group 21, variable 12, op 1, value 1
- Variable comparison: subject variable group 21, variable 13, op 1, value 1
- Variable comparison: subject variable group 21, variable 14, op 1, value 1
- Variable comparison: subject variable group 21, variable 15, op 1, value 1
- Variable comparison: subject variable group 21, variable 16, op 1, value 1
- Variable comparison: subject variable group 21, variable 17, op 1, value 1

**Action**

- Set/add variable: variable group 21, variable 23, subtype 0, value 1

### Event 30

**Trigger**

- Runtime condition family: subject 0, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 11, param 0

## Waypoints

### Waypoint 0

- Tag: `3`
- Members: `GalSpan_Merc_Corvus (object 7, id 113, starts at point 0)`, `GalSpan_Merc_Corvus (object 12, id 120, starts at point 0)`, `GalSpan_Merc_Corvus (object 13, id 114, starts at point 0)`, `GalSpan_Merc_Corvus (object 18, id 121, starts at point 0)`, `Susan_Bradley_Waraxe (object 19, id 372, starts at point 0)`, `Bora_Battleaxe (object 23, id 371, starts at point 0)`, `Bora_Battleaxe (object 24, id 373, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2141.23, 0.00, -4265.54) | None |
| 1 | (983.34, 0.00, -2035.25) | None |
| 2 | (-140.66, 0.00, -1065.51) | None |
| 3 | (-1430.92, 0.00, -483.45) | None |
| 4 | (1310.12, 0.00, 1032.22) | None |
| 5 | (804.94, 0.00, -1024.81) | on arrival redirect to Waypoint 1 (tag 2), point 1 |

### Waypoint 1

- Tag: `2`
- Members: `Bora_Battleaxe (object 4, id 374, starts at point 0)`, `Bora_Battleaxe (object 5, id 375, starts at point 0)`, `Bora_Battleaxe (object 6, id 376, starts at point 0)`, `GalSpan_Merc_Corvus (object 8, id 123, starts at point 0)`, `GalSpan_Merc_Corvus (object 9, id 138, starts at point 0)`, `GalSpan_Merc_Corvus (object 14, id 122, starts at point 0)`, `GalSpan_Merc_Corvus (object 15, id 139, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1774.46, 0.00, -4354.04) | None |
| 1 | (943.74, 0.00, -2468.80) | None |
| 2 | (-953.10, 0.00, -1736.01) | None |
| 3 | (-2180.42, 0.00, -475.26) | None |
| 4 | (-1109.72, 0.00, 701.50) | on arrival redirect to Waypoint 2 (tag 1), point 2 |

### Waypoint 2

- Tag: `1`
- Members: `GalSpan_Merc_Corvus (object 10, id 124, starts at point 0)`, `GalSpan_Merc_Corvus (object 11, id 116, starts at point 0)`, `GalSpan_Merc_Corvus (object 16, id 125, starts at point 0)`, `GalSpan_Merc_Corvus (object 17, id 117, starts at point 0)`, `Bora_Mace (object 20, id 1888, starts at point 0)`, `Bora_Mace (object 21, id 1889, starts at point 0)`, `Bora_Mace (object 22, id 1890, starts at point 0)`, `Bora_Mace (object 25, id 368, starts at point 0)`, `Bora_Mace (object 26, id 369, starts at point 0)`, `Bora_Mace (object 27, id 370, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2386.11, 0.00, -4124.80) | None |
| 1 | (1291.10, 0.00, -1509.44) | None |
| 2 | (1653.11, 0.00, -368.07) | None |
| 3 | (1713.84, 0.00, 1371.57) | None |
| 4 | (-334.65, 0.00, 1115.80) | on arrival redirect to Waypoint 0 (tag 3), point 1 |

## Spawn Lists

### Spawn List 0

- ID: `179`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 1

- ID: `172`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 1 | id 246 | None |
| 1 | 1 | id 244 | None |

### Spawn List 2

- ID: `171`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 1 | id 247 | None |
| 1 | 1 | id 245 | None |

### Spawn List 3

- ID: `170`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 1 | id 243 | None |
| 1 | 1 | id 242 | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Satellite` | 109 | Interactive | -1822.03,0.00,2281.75 | 0,0,0 | None |
| 1 | `Satellite` | 110 | Interactive | -1877.86,0.00,2259.06 | 0,0,0 | None |
| 2 | `Satellite` | 111 | Interactive | 2116.83,0.00,-4793.38 | 0,0,0 | None |
| 3 | `Satellite` | 112 | Interactive | 2288.11,0.00,-4700.11 | 0,0,0 | None |
| 4 | `Bora_Battleaxe` | 374 | Interactive | 2181.26,0.00,-4832.75 | 0,0,0 | group/role: FG_BACKBONE / 0; waypoint: Waypoint 1 (tag 2, 5 point(s)), starting point 0, arrival event value 131072 |
| 5 | `Bora_Battleaxe` | 375 | Interactive | 2155.25,0.00,-4888.62 | 0,0,0 | group/role: FG_BACKBONE / 0; waypoint: Waypoint 1 (tag 2, 5 point(s)), starting point 0, arrival event value 131072 |
| 6 | `Bora_Battleaxe` | 376 | Interactive | 2200.78,0.00,-4888.61 | 0,0,0 | group/role: FG_BACKBONE / 0; waypoint: Waypoint 1 (tag 2, 5 point(s)), starting point 0, arrival event value 131072 |
| 7 | `GalSpan_Merc_Corvus` | 113 | Interactive | 2261.01,0.00,-4867.83 | 0,0,0 | group/role: FG_PAVO / 0; waypoint: Waypoint 0 (tag 3, 6 point(s)), starting point 0, arrival event value 196608 |
| 8 | `GalSpan_Merc_Corvus` | 123 | Interactive | 2103.38,0.00,-5070.31 | 0,0,0 | group/role: FG_TEGEA / 0; waypoint: Waypoint 1 (tag 2, 5 point(s)), starting point 0, arrival event value 131072 |
| 9 | `GalSpan_Merc_Corvus` | 138 | Interactive | 2060.32,0.00,-4932.66 | 0,0,0 | group/role: FG_LEPUS / 0; waypoint: Waypoint 1 (tag 2, 5 point(s)), starting point 0, arrival event value 131072 |
| 10 | `GalSpan_Merc_Corvus` | 124 | Interactive | 2438.12,0.00,-5042.34 | 0,0,0 | group/role: FG_IXION / 0; waypoint: Waypoint 2 (tag 1, 5 point(s)), starting point 0, arrival event value 65536 |
| 11 | `GalSpan_Merc_Corvus` | 116 | Interactive | 2433.04,0.00,-4872.70 | 0,0,0 | group/role: FG_FORNAX / 0; waypoint: Waypoint 2 (tag 1, 5 point(s)), starting point 0, arrival event value 65536 |
| 12 | `GalSpan_Merc_Corvus` | 120 | Interactive | 2190.93,0.00,-4723.53 | 0,0,0 | group/role: FG_VELA / 0; waypoint: Waypoint 0 (tag 3, 6 point(s)), starting point 0, arrival event value 196608 |
| 13 | `GalSpan_Merc_Corvus` | 114 | Interactive | 2294.21,0.00,-4864.96 | 0,0,0 | group/role: FG_PAVO / 0; waypoint: Waypoint 0 (tag 3, 6 point(s)), starting point 0, arrival event value 196608 |
| 14 | `GalSpan_Merc_Corvus` | 122 | Interactive | 2131.63,0.00,-5070.16 | 0,0,0 | label: MERC_17; group/role: FG_TEGEA / 0; waypoint: Waypoint 1 (tag 2, 5 point(s)), starting point 0, arrival event value 131072 |
| 15 | `GalSpan_Merc_Corvus` | 139 | Interactive | 2091.33,0.00,-4931.80 | 0,0,0 | group/role: FG_LEPUS / 0; waypoint: Waypoint 1 (tag 2, 5 point(s)), starting point 0, arrival event value 131072 |
| 16 | `GalSpan_Merc_Corvus` | 125 | Interactive | 2470.99,0.00,-5041.67 | 0,0,0 | group/role: FG_IXION / 0; waypoint: Waypoint 2 (tag 1, 5 point(s)), starting point 0, arrival event value 65536 |
| 17 | `GalSpan_Merc_Corvus` | 117 | Interactive | 2468.62,0.00,-4872.70 | 0,0,0 | group/role: FG_FORNAX / 0; waypoint: Waypoint 2 (tag 1, 5 point(s)), starting point 0, arrival event value 65536 |
| 18 | `GalSpan_Merc_Corvus` | 121 | Interactive | 2226.84,0.00,-4723.37 | 0,0,0 | group/role: FG_VELA / 0; waypoint: Waypoint 0 (tag 3, 6 point(s)), starting point 0, arrival event value 196608 |
| 19 | `Susan_Bradley_Waraxe` | 372 | Interactive | 2339.45,0.00,-4716.14 | 0,0,0 | group/role: FG_GRACE / 0; secondary groups: none, SUSAN_BRADLEY; waypoint: Waypoint 0 (tag 3, 6 point(s)), starting point 0, arrival event value 196608 |
| 20 | `Bora_Mace` | 1888 | Interactive | 2264.24,0.00,-5002.44 | 0,0,0 | group/role: FG_RESOLVE / 0; waypoint: Waypoint 2 (tag 1, 5 point(s)), starting point 0, arrival event value 65536 |
| 21 | `Bora_Mace` | 1889 | Interactive | 2292.03,0.00,-5002.44 | 0,0,0 | group/role: FG_RESOLVE / 0; waypoint: Waypoint 2 (tag 1, 5 point(s)), starting point 0, arrival event value 65536 |
| 22 | `Bora_Mace` | 1890 | Interactive | 2277.21,0.00,-5034.58 | 0,0,0 | group/role: FG_RESOLVE / 0; waypoint: Waypoint 2 (tag 1, 5 point(s)), starting point 0, arrival event value 65536 |
| 23 | `Bora_Battleaxe` | 371 | Interactive | 2317.77,0.00,-4789.01 | 0,0,0 | group/role: FG_GRACE / 0; waypoint: Waypoint 0 (tag 3, 6 point(s)), starting point 0, arrival event value 196608 |
| 24 | `Bora_Battleaxe` | 373 | Interactive | 2356.79,0.00,-4798.72 | 0,0,0 | group/role: FG_GRACE / 0; waypoint: Waypoint 0 (tag 3, 6 point(s)), starting point 0, arrival event value 196608 |
| 25 | `Bora_Mace` | 368 | Interactive | 1992.56,0.00,-4786.64 | 0,0,0 | group/role: FG_BRAVERY / 0; waypoint: Waypoint 2 (tag 1, 5 point(s)), starting point 0, arrival event value 65536 |
| 26 | `Bora_Mace` | 369 | Interactive | 2033.75,0.00,-4791.49 | 0,0,0 | group/role: FG_BRAVERY / 0; waypoint: Waypoint 2 (tag 1, 5 point(s)), starting point 0, arrival event value 65536 |
| 27 | `Bora_Mace` | 370 | Interactive | 2016.41,0.00,-4723.49 | 0,0,0 | group/role: FG_BRAVERY / 0; waypoint: Waypoint 2 (tag 1, 5 point(s)), starting point 0, arrival event value 65536 |
