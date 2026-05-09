# Tachyon: The Fringe DISP02C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP02C.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 5 |
| Entities | 18 |
| Events | 11 |
| Waypoints | 10 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Deliverance_BC10_Only`, `1: Bora_Battleaxe`, `2: GalSpan_Orion`, `3: Susan_Bradley_Waraxe`, `4: Bora_Claymore` |
| Scripts | `B10GPB.SCR`, `DELIV.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFGE_03`, `BFGF_03`, `MERC_17`, `BFNE_01`, `CLEON`, `Patrol1`, `Patrol2`, `SPIKE`, `Redemption` |
| Aliases | `BC10_Claymore1`, `BC10_Claymore2`, `BC10_Claymore3`, `BC10_Claymore4`, `Coward`, `BC10_Waraxe`, `BC10_Mace1`, `BC10_Mace2`, `BC10_Mace3`, `BC10_Mace4`, `BC10_Warhammer1`, `BC10_Warhammer2`, `BC10_Warhammer3`, `BC10_Warhammer4`, `SPIKE`, `Stocks01` |
| Groups | `FG_SWORD`, `FG_LANCE`, `WAR_AXE`, `FG_DRACONIS`, `FG_MORNING_STAR`, `FG_TRIDENT`, `DELIVERANCE`, `CONT_024` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Group/spawn-list action: spawn list/group 272, subtype 2
- Gate state/action: param 2, subtype 3, param 0
- Object spawn/action: Deliverance_BC10_Only (object 17, id 1936), subtype 3
- Object spawn/action: Deliverance_BC10_Only (object 17, id 1936), subtype 18
- Set runtime trigger variable: variable group 20, variable 28, subtype 0, value 0
- Set runtime trigger variable: variable group 20, variable 5, subtype 1, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 28, op 1, value 2

**Action**

- Group/spawn-list action: spawn list/group 124, subtype 2
- Group/spawn-list action: spawn list/group 57, subtype 2
- Group/spawn-list action: spawn list/group 47, subtype 2
- Show/update HUD contact: contact/list 0, subtype 6, param 1936
- Object spawn/action: Deliverance_BC10_Only (object 17, id 1936), subtype 14

### Event 2

**Trigger**

- Group/spawn-list event: subject 272, op 2, value 13172736 (Waypoint 6 (tag 201), point 0)

**Action**

- Play dialog: B10GPB.SCR, line/variant 0
- Set/add variable: variable group 20, variable 5, subtype 0, value 0

### Event 3

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 0

**Action**

- Group/spawn-list action: spawn list/group 272, subtype 2
- Show/update HUD contact: contact/list 0, subtype 1, param 272

### Event 4

**Trigger**

- Group/spawn-list event: subject 272, op 0, value 0

**Action**

- Mission objective/state: param 393218, subtype 0, param 0
- Set/add variable: variable group 21, variable 29, subtype 0, value 1
- Object spawn/action: id 2, subtype 14

### Event 5

**Trigger**

- Global enemy/object-count event: subject 0, op 0, value 0

**Action**

- Play dialog: DELIV.SCR, line/variant 1
- Set runtime trigger variable: variable group 20, variable 31, subtype 0, value 0

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 31, op 1, value 18

**Action**

- Play dialog: DELIV.SCR, line/variant 2
- Gate state/action: param 2, subtype 2, param 0
- Set/add variable: variable group 21, variable 11, subtype 0, value 1

### Event 7

**Trigger**

- Unknown runtime event: subject 2, op 0, value 0
- Variable comparison: subject variable group 21, variable 11, op 1, value 1

**Action**

- Set runtime trigger variable: variable group 20, variable 5, subtype 0, value 0

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 5, op 1, value 8

**Action**

- Group/spawn-list action: spawn list/group 124, subtype 3, param 2
- Group/spawn-list action: spawn list/group 47, subtype 3, param 2
- Group/spawn-list action: spawn list/group 56, subtype 3, param 2
- Group/spawn-list action: spawn list/group 57, subtype 3, param 2
- Object spawn/action: Deliverance_BC10_Only (object 17, id 1936), subtype 4
- Set/add variable: variable group 21, variable 2, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 6, param 1936

### Event 9

**Trigger**

- Object event: subject GalSpan_Orion (object 8, id 1769), op 0, value 0 (flags 2)
- Object event: subject GalSpan_Orion (object 8, id 1769), op 2, value 0 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 153

### Event 10

**Trigger**

- Object event: subject GalSpan_Orion (object 6, id 1767), op 0, value 0 (flags 2)
- Object event: subject GalSpan_Orion (object 6, id 1767), op 2, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 180

## Waypoints

### Waypoint 0

- Tag: `207`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1629.32, 0.00, -4537.37) | None |

### Waypoint 1

- Tag: `210`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2051.09, 0.00, -5396.77) | None |

### Waypoint 2

- Tag: `209`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1691.60, 0.00, -5224.89) | None |

### Waypoint 3

- Tag: `208`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1538.74, 0.00, -4816.67) | None |

### Waypoint 4

- Tag: `206`
- Members: `Bora_Battleaxe (object 9, id 1909, starts at point 0)`, `Bora_Battleaxe (object 10, id 1910, starts at point 0)`, `Bora_Battleaxe (object 11, id 1911, starts at point 0)`, `Bora_Battleaxe (object 12, id 1912, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1930.98, 0.00, 2379.17) | on arrival activate current object (raw param -1 ignored) |
| 1 | (2014.67, 0.00, -5075.58) | on arrival redirect to Waypoint 0 (tag 207), point 0 |

### Waypoint 5

- Tag: `205`
- Members: `Deliverance_BC10_Only (object 17, id 1936, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1162.52, 0.00, -650.70) | None |
| 1 | (-292.63, 0.00, -1774.57) | None |
| 2 | (586.32, 0.00, -2914.92) | None |
| 3 | (1420.36, 0.00, -4353.30) | None |

### Waypoint 6

- Tag: `201`
- Members: `GalSpan_Orion (object 5, id 1766, starts at point 0)`, `GalSpan_Orion (object 6, id 1767, starts at point 0)`, `GalSpan_Orion (object 7, id 1768, starts at point 0)`, `GalSpan_Orion (object 8, id 1769, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (4009.09, 0.00, -6135.15) | None |
| 1 | (2933.30, 0.00, -4898.58) | None |
| 2 | (2399.96, 0.00, -4259.97) | None |
| 3 | (1900.13, 0.00, -3701.01) | None |
| 4 | (1496.97, 0.00, -3265.49) | None |
| 5 | (1117.54, 0.00, -2834.57) | None |

### Waypoint 7

- Tag: `202`
- Members: `Bora_Claymore (object 0, id 296, starts at point 0)`, `Bora_Claymore (object 1, id 297, starts at point 0)`, `Bora_Claymore (object 2, id 298, starts at point 0)`, `Bora_Claymore (object 3, id 299, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1873.74, 0.00, 2409.56) | None |
| 1 | (2408.02, 0.00, -4993.25) | on arrival redirect to Waypoint 2 (tag 209), point 0 |

### Waypoint 8

- Tag: `203`
- Members: `Susan_Bradley_Waraxe (object 4, id 351, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1955.36, 0.00, 2363.13) | on arrival activate current object (raw param -1 ignored) |
| 1 | (2270.49, 0.00, -5274.82) | on arrival redirect to Waypoint 3 (tag 208), point 0 |

### Waypoint 9

- Tag: `204`
- Members: `Bora_Battleaxe (object 13, id 344, starts at point 0)`, `Bora_Battleaxe (object 14, id 345, starts at point 0)`, `Bora_Battleaxe (object 15, id 346, starts at point 0)`, `Bora_Battleaxe (object 16, id 347, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1904.73, 0.00, 2394.59) | on arrival activate current object (raw param -1 ignored) |
| 1 | (2598.12, 7.00, -5179.77) | on arrival redirect to Waypoint 1 (tag 210), point 0 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Bora_Claymore` | 296 | Interactive | -1335.66,0.00,2203.40 | 256,0,0 | group/role: FG_SWORD / 0; alias: BC10_Claymore1; waypoint: Waypoint 7 (tag 202, 2 point(s)), starting point 0, arrival event value 13238272 |
| 1 | `Bora_Claymore` | 297 | Interactive | -1269.48,0.00,2203.40 | 256,0,0 | group/role: FG_SWORD / 0; alias: BC10_Claymore2; waypoint: Waypoint 7 (tag 202, 2 point(s)), starting point 0, arrival event value 13238272 |
| 2 | `Bora_Claymore` | 298 | Interactive | -1198.20,0.00,2208.88 | 256,0,0 | group/role: FG_SWORD / 0; alias: BC10_Claymore3; waypoint: Waypoint 7 (tag 202, 2 point(s)), starting point 0, arrival event value 13238272 |
| 3 | `Bora_Claymore` | 299 | Interactive | -1121.83,0.00,2208.88 | 256,0,0 | group/role: FG_SWORD / 0; alias: BC10_Claymore4; waypoint: Waypoint 7 (tag 202, 2 point(s)), starting point 0, arrival event value 13238272 |
| 4 | `Susan_Bradley_Waraxe` | 351 | Interactive | -1244.36,0.00,1885.14 | 256,0,0 | group/role: FG_LANCE / 0; alias: BC10_Waraxe; secondary groups: none, WAR_AXE; waypoint: Waypoint 8 (tag 203, 2 point(s)), starting point 0, arrival event value 13303808 |
| 5 | `GalSpan_Orion` | 1766 | Interactive | 4350.16,0.00,-6509.75 | 439,0,0 | group/role: FG_DRACONIS / 0; waypoint: Waypoint 6 (tag 201, 6 point(s)), starting point 0, arrival event value 13172736 |
| 6 | `GalSpan_Orion` | 1767 | Interactive | 4406.25,0.00,-6520.92 | 449,0,0 | group/role: FG_DRACONIS / 0; waypoint: Waypoint 6 (tag 201, 6 point(s)), starting point 0, arrival event value 13172736 |
| 7 | `GalSpan_Orion` | 1768 | Interactive | 4441.12,0.00,-6573.83 | 432,0,0 | group/role: FG_DRACONIS / 0; waypoint: Waypoint 6 (tag 201, 6 point(s)), starting point 0, arrival event value 13172736 |
| 8 | `GalSpan_Orion` | 1769 | Interactive | 4368.58,0.00,-6564.54 | 437,0,0 | group/role: FG_DRACONIS / 0; waypoint: Waypoint 6 (tag 201, 6 point(s)), starting point 0, arrival event value 13172736 |
| 9 | `Bora_Battleaxe` | 1909 | Interactive | -1342.33,0.00,2001.04 | 253,0,0 | group/role: FG_MORNING_STAR / 0; alias: BC10_Mace1; waypoint: Waypoint 4 (tag 206, 2 point(s)), starting point 0, arrival event value 13500416 |
| 10 | `Bora_Battleaxe` | 1910 | Interactive | -1263.76,0.00,2003.88 | 253,0,0 | group/role: FG_MORNING_STAR / 0; alias: BC10_Mace2; waypoint: Waypoint 4 (tag 206, 2 point(s)), starting point 0, arrival event value 13500416 |
| 11 | `Bora_Battleaxe` | 1911 | Interactive | -1206.14,0.00,2003.88 | 253,0,0 | group/role: FG_MORNING_STAR / 0; alias: BC10_Mace3; waypoint: Waypoint 4 (tag 206, 2 point(s)), starting point 0, arrival event value 13500416 |
| 12 | `Bora_Battleaxe` | 1912 | Interactive | -1138.04,0.00,1998.20 | 253,0,0 | group/role: FG_MORNING_STAR / 0; alias: BC10_Mace4; waypoint: Waypoint 4 (tag 206, 2 point(s)), starting point 0, arrival event value 13500416 |
| 13 | `Bora_Battleaxe` | 344 | Interactive | -1334.96,0.00,2104.74 | 256,0,0 | group/role: FG_TRIDENT / 0; alias: BC10_Warhammer1; waypoint: Waypoint 9 (tag 204, 2 point(s)), starting point 0, arrival event value 13369344 |
| 14 | `Bora_Battleaxe` | 345 | Interactive | -1271.31,0.00,2104.74 | 256,0,0 | group/role: FG_TRIDENT / 0; alias: BC10_Warhammer2; waypoint: Waypoint 9 (tag 204, 2 point(s)), starting point 0, arrival event value 13369344 |
| 15 | `Bora_Battleaxe` | 346 | Interactive | -1197.73,0.00,2106.88 | 256,0,0 | group/role: FG_TRIDENT / 0; alias: BC10_Warhammer3; waypoint: Waypoint 9 (tag 204, 2 point(s)), starting point 0, arrival event value 13369344 |
| 16 | `Bora_Battleaxe` | 347 | Interactive | -1122.16,0.00,2106.88 | 256,0,0 | group/role: FG_TRIDENT / 0; alias: BC10_Warhammer4; waypoint: Waypoint 9 (tag 204, 2 point(s)), starting point 0, arrival event value 13369344 |
| 17 | `Deliverance_BC10_Only` | 1936 | Interactive | -1928.34,0.00,40.40 | 185,0,0 | alias: Stocks01; secondary groups: CONT_024, DELIVERANCE; waypoint: Waypoint 5 (tag 205, 4 point(s)), starting point -1 |
