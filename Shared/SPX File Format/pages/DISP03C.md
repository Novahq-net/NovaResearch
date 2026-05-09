# Tachyon: The Fringe DISP03C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP03C.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 7 |
| Entities | 32 |
| Events | 13 |
| Waypoints | 10 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Deliverance_BC10_Only`, `1: Bora_Battleaxe`, `2: Bora_Claymore`, `3: Hyper_Gate`, `4: GalSpan_Orion`, `5: GalSpan_Merc_Corvus`, `6: Susan_Bradley_Waraxe` |
| Scripts | `PLAYER.SCR`, `SUSAN.SCR` |
| Scenes | None |
| Labels | `BFGE_02`, `BFBE_07`, `TNSA`, `BFBE_09`, `adder1`, `BFBF_07`, `ROSS`, `SPIKE`, `atkin`, `cruiser1` |
| Aliases | `fake_2`, `BC10_Waraxe`, `Coward`, `spy_1`, `fake_1`, `tnsa`, `BC10_Claymore4`, `BC10_Claymore3`, `BC10_Claymore2`, `BC10_Claymore1`, `BC10_Warhammer4`, `BC10_Warhammer3`, `BC10_Warhammer2`, `BC10_Warhammer1`, `BC10_Mace3`, `BC10_Mace4`, `BC10_Mace1`, `BC10_Mace2`, `Galileo`, `SPIKE`, `zeus`, `Stocks01` |
| Groups | `FG_LANCE`, `WAR_AXE`, `FG_COLUMBA`, `FG_COLCHIS`, `FG_COLONAE`, `FG_CYCNUS`, `FG_CAELUM`, `FG_SWORD`, `FG_TRIDENT`, `FG_MORNING_STAR`, `DELIVERANCE` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Gate state/action: param 10203, subtype 3, param 0
- Show/update HUD contact: contact/list 0, subtype 1, param 273
- Show/update HUD contact: contact/list 0, subtype 1, param 274
- Show/update HUD contact: contact/list 0, subtype 1, param 278
- Show/update HUD contact: contact/list 0, subtype 1, param 277
- Show/update HUD contact: contact/list 0, subtype 1, param 216
- Play dialog: PLAYER.SCR, line/variant 157
- Set runtime trigger variable: variable group 20, variable 2, subtype 1, value 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Group/spawn-list action: spawn list/group 216, subtype 0
- Group/spawn-list action: spawn list/group 273, subtype 0
- Group/spawn-list action: spawn list/group 274, subtype 0
- Group/spawn-list action: spawn list/group 278, subtype 0
- Group/spawn-list action: spawn list/group 277, subtype 0

### Event 2

**Trigger**

- Variable comparison: subject variable group 21, variable 2, op 1, value 1
- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Object spawn/action: Deliverance_BC10_Only (object 31, id 10953), subtype 3
- Object spawn/action: Deliverance_BC10_Only (object 31, id 10953), subtype 18
- Set/add variable: variable group 20, variable 2, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 6, param 10953

### Event 3

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 157

**Action**

- Group/spawn-list action: spawn list/group 273, subtype 2
- Group/spawn-list action: spawn list/group 274, subtype 2
- Group/spawn-list action: spawn list/group 278, subtype 2
- Group/spawn-list action: spawn list/group 277, subtype 2
- Group/spawn-list action: spawn list/group 216, subtype 2

### Event 4

**Trigger**

- Global enemy/object-count event: subject 0, op 0, value 0

**Action**

- Play dialog: SUSAN.SCR, line/variant 13
- Set/add variable: variable group 21, variable 19, subtype 0, value 1
- Mission objective/state: param 393224, subtype 0, param 0

### Event 5

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 13

**Action**

- Gate state/action: param 10203, subtype 2, param 0

### Event 6

**Trigger**

- Unknown runtime event: subject 10203, op 0, value 0
- Variable comparison: subject variable group 21, variable 19, op 1, value 1

**Action**

- Set runtime trigger variable: variable group 20, variable 2, subtype 0, value 0

### Event 7

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 23

**Action**

- Group/spawn-list action: spawn list/group 124, subtype 3, param 10203
- Object spawn/action: Deliverance_BC10_Only (object 31, id 10953), subtype 4
- Hide/remove HUD contact: contact/list 0, subtype 6, param 10953
- Set/add variable: variable group 21, variable 2, subtype 0, value 2

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 23

**Action**

- Group/spawn-list action: spawn list/group 47, subtype 3, param 10203

### Event 9

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 23

**Action**

- Group/spawn-list action: spawn list/group 57, subtype 3, param 10203

### Event 10

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 23

**Action**

- Group/spawn-list action: spawn list/group 56, subtype 3, param 10203

### Event 11

**Trigger**

- Group/spawn-list event: subject 273, op 1, value 70

**Action**

- Play dialog: PLAYER.SCR, line/variant 154

### Event 12

**Trigger**

- Group/spawn-list event: subject 216, op 1, value 70

**Action**

- Play dialog: PLAYER.SCR, line/variant 172

## Waypoints

### Waypoint 0

- Tag: `210`
- Members: `GalSpan_Merc_Corvus (object 15, id 10969, starts at point 0)`, `GalSpan_Merc_Corvus (object 16, id 10970, starts at point 0)`, `GalSpan_Merc_Corvus (object 17, id 10971, starts at point 0)`, `GalSpan_Merc_Corvus (object 18, id 10972, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-29.43, 44.00, 1675.07) | None |
| 1 | (-300.80, 44.00, 1746.64) | None |
| 2 | (-685.86, 44.00, 1818.21) | on arrival redirect to Waypoint 6 (tag 204), point 0 |

### Waypoint 1

- Tag: `209`
- Members: `Bora_Battleaxe (object 27, id 10956, starts at point 0)`, `Bora_Battleaxe (object 28, id 10957, starts at point 0)`, `Bora_Battleaxe (object 29, id 10954, starts at point 0)`, `Bora_Battleaxe (object 30, id 10955, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (952.65, 0.00, 1684.48) | None |

### Waypoint 2

- Tag: `208`
- Members: `Bora_Claymore (object 19, id 11402, starts at point 0)`, `Bora_Claymore (object 20, id 11403, starts at point 0)`, `Bora_Claymore (object 21, id 11404, starts at point 0)`, `Bora_Claymore (object 22, id 11405, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1176.51, 0.00, 1624.02) | None |

### Waypoint 3

- Tag: `207`
- Members: `Bora_Battleaxe (object 23, id 11406, starts at point 0)`, `Bora_Battleaxe (object 24, id 11407, starts at point 0)`, `Bora_Battleaxe (object 25, id 11408, starts at point 0)`, `Bora_Battleaxe (object 26, id 11409, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1144.52, 0.00, 1686.02) | None |

### Waypoint 4

- Tag: `206`
- Members: `Susan_Bradley_Waraxe (object 0, id 8767, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1095.24, 0.00, 1734.01) | None |

### Waypoint 5

- Tag: `205`
- Members: `GalSpan_Merc_Corvus (object 7, id 10138, starts at point 2)`, `GalSpan_Merc_Corvus (object 8, id 10139, starts at point 2)`, `GalSpan_Merc_Corvus (object 9, id 10140, starts at point 2)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-701.08, -74.81, 2056.21) | on arrival activate current object (raw param -1 ignored) |
| 1 | (-827.73, -34.84, 2123.96) | None |
| 2 | (-1004.22, -17.42, 2251.06) | on arrival redirect to Waypoint 6 (tag 204), point 0 |

### Waypoint 6

- Tag: `204`
- Members: `GalSpan_Merc_Corvus (object 1, id 10130, starts at point 0)`, `GalSpan_Merc_Corvus (object 2, id 10131, starts at point 0)`, `GalSpan_Merc_Corvus (object 3, id 10133, starts at point 0)`, `GalSpan_Merc_Corvus (object 14, id 10998, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1052.69, 0.00, 1592.59) | None |
| 1 | (-1304.88, 0.00, 1781.49) | on arrival activate current object (raw param -1 ignored) |
| 2 | (-1513.06, 0.00, 1966.04) | on arrival redirect to Waypoint 5 (tag 205), point 0 |

### Waypoint 7

- Tag: `203`
- Members: `GalSpan_Merc_Corvus (object 4, id 10134, starts at point 0)`, `GalSpan_Merc_Corvus (object 5, id 10135, starts at point 0)`, `GalSpan_Merc_Corvus (object 6, id 10136, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (263.00, 49.47, 1968.95) | None |
| 1 | (92.20, 29.82, 2069.18) | None |
| 2 | (-22.41, 21.01, 2135.25) | on arrival redirect to Waypoint 6 (tag 204), point 0 |

### Waypoint 8

- Tag: `202`
- Members: `GalSpan_Orion (object 10, id 10143, starts at point 0)`, `GalSpan_Orion (object 11, id 10144, starts at point 0)`, `GalSpan_Orion (object 12, id 10145, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-735.45, 0.00, 1538.46) | None |
| 1 | (-881.41, 0.00, 1642.15) | on arrival activate current object (raw param -1 ignored) |
| 2 | (-1121.37, 0.00, 1815.87) | on arrival redirect to Waypoint 7 (tag 203), point 0 |

### Waypoint 9

- Tag: `201`
- Members: `Deliverance_BC10_Only (object 31, id 10953, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-553.86, -305.00, 15.22) | None |
| 1 | (444.65, -182.00, 386.58) | None |
| 2 | (1199.30, 0.00, 657.82) | None |

## Spawn Lists

### Spawn List 0

- ID: `273`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 6 | Deliverance_BC10_Only (object 31, id 10953) | None |

### Spawn List 1

- ID: `274`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 6 | Deliverance_BC10_Only (object 31, id 10953) | None |

### Spawn List 2

- ID: `278`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 6 | Deliverance_BC10_Only (object 31, id 10953) | None |

### Spawn List 3

- ID: `277`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 6 | Deliverance_BC10_Only (object 31, id 10953) | None |

### Spawn List 4

- ID: `216`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 6 | Deliverance_BC10_Only (object 31, id 10953) | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Susan_Bradley_Waraxe` | 8767 | Interactive | -1873.34,0.00,2769.00 | 166,0,0 | group/role: FG_LANCE / 0; alias: BC10_Waraxe; secondary groups: none, WAR_AXE; waypoint: Waypoint 4 (tag 206, 1 point(s)), starting point 0, arrival event value 13500416 |
| 1 | `GalSpan_Merc_Corvus` | 10130 | Interactive | -979.70,39.00,1458.90 | 442,0,0 | group/role: FG_COLUMBA / 0; waypoint: Waypoint 6 (tag 204, 3 point(s)), starting point 0, arrival event value 13369344 |
| 2 | `GalSpan_Merc_Corvus` | 10131 | Interactive | -928.58,23.40,1501.45 | 439,0,0 | label: BFBE_07; group/role: FG_COLUMBA / 0; waypoint: Waypoint 6 (tag 204, 3 point(s)), starting point 0, arrival event value 13369344 |
| 3 | `GalSpan_Merc_Corvus` | 10133 | Interactive | -992.16,0.00,1517.52 | 441,0,0 | group/role: FG_COLUMBA / 0; waypoint: Waypoint 6 (tag 204, 3 point(s)), starting point 0, arrival event value 13369344 |
| 4 | `GalSpan_Merc_Corvus` | 10134 | Interactive | 350.26,66.00,1977.20 | 425,0,0 | group/role: FG_COLCHIS / 0; waypoint: Waypoint 7 (tag 203, 3 point(s)), starting point 0, arrival event value 13303808 |
| 5 | `GalSpan_Merc_Corvus` | 10135 | Interactive | 310.25,-43.00,1909.82 | 439,0,0 | group/role: FG_COLCHIS / 0; waypoint: Waypoint 7 (tag 203, 3 point(s)), starting point 0, arrival event value 13303808 |
| 6 | `GalSpan_Merc_Corvus` | 10136 | Interactive | 267.33,13.00,1847.33 | 432,0,0 | label: BFBE_07; group/role: FG_COLCHIS / 0; waypoint: Waypoint 7 (tag 203, 3 point(s)), starting point 0, arrival event value 13303808 |
| 7 | `GalSpan_Merc_Corvus` | 10138 | Interactive | -564.30,0.00,2005.85 | 442,0,0 | group/role: FG_COLONAE / 0; waypoint: Waypoint 5 (tag 205, 3 point(s)), starting point 2, arrival event value 13434882 |
| 8 | `GalSpan_Merc_Corvus` | 10139 | Interactive | -602.56,35.00,1969.19 | 441,0,0 | group/role: FG_COLONAE / 0; waypoint: Waypoint 5 (tag 205, 3 point(s)), starting point 2, arrival event value 13434882 |
| 9 | `GalSpan_Merc_Corvus` | 10140 | Interactive | -524.25,-52.00,1973.64 | 466,0,0 | label: BFBE_07; group/role: FG_COLONAE / 0; waypoint: Waypoint 5 (tag 205, 3 point(s)), starting point 2, arrival event value 13434882 |
| 10 | `GalSpan_Orion` | 10143 | Interactive | -553.65,-56.00,1408.49 | 432,0,0 | group/role: FG_CYCNUS / 0; waypoint: Waypoint 8 (tag 202, 3 point(s)), starting point 0, arrival event value 13238272 |
| 11 | `GalSpan_Orion` | 10144 | Interactive | -483.07,0.00,1375.65 | 424,0,0 | group/role: FG_CYCNUS / 0; waypoint: Waypoint 8 (tag 202, 3 point(s)), starting point 0, arrival event value 13238272 |
| 12 | `GalSpan_Orion` | 10145 | Interactive | -520.43,-64.00,1448.30 | 425,0,0 | label: BFBE_07; group/role: FG_CYCNUS / 0; waypoint: Waypoint 8 (tag 202, 3 point(s)), starting point 0, arrival event value 13238272 |
| 13 | `Hyper_Gate` | 10203 | Gate | 1002.55,0.00,1483.65 | 385,0,0 | Gate SPX: [disp09.spx](DISP09.md) |
| 14 | `GalSpan_Merc_Corvus` | 10998 | Interactive | -915.82,0.00,1446.95 | 435,0,0 | group/role: FG_COLUMBA / 0; waypoint: Waypoint 6 (tag 204, 3 point(s)), starting point 0, arrival event value 13369344 |
| 15 | `GalSpan_Merc_Corvus` | 10969 | Interactive | 111.15,39.00,1584.14 | 411,0,0 | group/role: FG_CAELUM / 0; waypoint: Waypoint 0 (tag 210, 3 point(s)), starting point 0, arrival event value 13762560 |
| 16 | `GalSpan_Merc_Corvus` | 10970 | Interactive | 173.74,39.00,1618.07 | 411,0,0 | label: BFBE_07; group/role: FG_CAELUM / 0; waypoint: Waypoint 0 (tag 210, 3 point(s)), starting point 0, arrival event value 13762560 |
| 17 | `GalSpan_Merc_Corvus` | 10971 | Interactive | 223.81,39.00,1645.22 | 411,0,0 | group/role: FG_CAELUM / 0; waypoint: Waypoint 0 (tag 210, 3 point(s)), starting point 0, arrival event value 13762560 |
| 18 | `GalSpan_Merc_Corvus` | 10972 | Interactive | 217.55,39.00,1563.78 | 411,0,0 | group/role: FG_CAELUM / 0; waypoint: Waypoint 0 (tag 210, 3 point(s)), starting point 0, arrival event value 13762560 |
| 19 | `Bora_Claymore` | 11402 | Interactive | -2191.58,0.00,2863.78 | 176,0,0 | group/role: FG_SWORD / 0; alias: BC10_Claymore4; waypoint: Waypoint 2 (tag 208, 1 point(s)), starting point 0, arrival event value 13631488 |
| 20 | `Bora_Claymore` | 11403 | Interactive | -2160.35,0.00,2908.94 | 171,0,0 | group/role: FG_SWORD / 0; alias: BC10_Claymore3; waypoint: Waypoint 2 (tag 208, 1 point(s)), starting point 0, arrival event value 13631488 |
| 21 | `Bora_Claymore` | 11404 | Interactive | -2123.16,0.00,2963.77 | 176,0,0 | group/role: FG_SWORD / 0; alias: BC10_Claymore2; waypoint: Waypoint 2 (tag 208, 1 point(s)), starting point 0, arrival event value 13631488 |
| 22 | `Bora_Claymore` | 11405 | Interactive | -2081.52,0.00,3010.54 | 181,0,0 | group/role: FG_SWORD / 0; alias: BC10_Claymore1; waypoint: Waypoint 2 (tag 208, 1 point(s)), starting point 0, arrival event value 13631488 |
| 23 | `Bora_Battleaxe` | 11406 | Interactive | -2101.98,0.00,2801.41 | 164,0,0 | group/role: FG_TRIDENT / 0; alias: BC10_Warhammer4; waypoint: Waypoint 3 (tag 207, 1 point(s)), starting point 0, arrival event value 13565952 |
| 24 | `Bora_Battleaxe` | 11407 | Interactive | -2073.72,0.00,2853.02 | 174,0,0 | group/role: FG_TRIDENT / 0; alias: BC10_Warhammer3; waypoint: Waypoint 3 (tag 207, 1 point(s)), starting point 0, arrival event value 13565952 |
| 25 | `Bora_Battleaxe` | 11408 | Interactive | -2046.95,0.00,2901.40 | 166,0,0 | group/role: FG_TRIDENT / 0; alias: BC10_Warhammer2; waypoint: Waypoint 3 (tag 207, 1 point(s)), starting point 0, arrival event value 13565952 |
| 26 | `Bora_Battleaxe` | 11409 | Interactive | -2006.79,0.00,2946.55 | 168,0,0 | group/role: FG_TRIDENT / 0; alias: BC10_Warhammer1; waypoint: Waypoint 3 (tag 207, 1 point(s)), starting point 0, arrival event value 13565952 |
| 27 | `Bora_Battleaxe` | 10956 | Interactive | -1954.15,0.00,2856.10 | 193,0,0 | label: BFBF_07; group/role: FG_MORNING_STAR / 0; alias: BC10_Mace3; waypoint: Waypoint 1 (tag 209, 1 point(s)), starting point 0, arrival event value 13697024 |
| 28 | `Bora_Battleaxe` | 10957 | Interactive | -1923.88,0.00,2894.90 | 193,0,0 | group/role: FG_MORNING_STAR / 0; alias: BC10_Mace4; waypoint: Waypoint 1 (tag 209, 1 point(s)), starting point 0, arrival event value 13697024 |
| 29 | `Bora_Battleaxe` | 10954 | Interactive | -2022.97,0.00,2754.62 | 193,0,0 | group/role: FG_MORNING_STAR / 0; alias: BC10_Mace1; waypoint: Waypoint 1 (tag 209, 1 point(s)), starting point 0, arrival event value 13697024 |
| 30 | `Bora_Battleaxe` | 10955 | Interactive | -1987.19,0.00,2811.33 | 193,0,0 | group/role: FG_MORNING_STAR / 0; alias: BC10_Mace2; waypoint: Waypoint 1 (tag 209, 1 point(s)), starting point 0, arrival event value 13697024 |
| 31 | `Deliverance_BC10_Only` | 10953 | Interactive | -1448.88,-425.26,-251.48 | 107,14,0 | alias: Stocks01; secondary groups: none, DELIVERANCE; waypoint: Waypoint 9 (tag 201, 3 point(s)), starting point 0, arrival event value 13172736 |
