# Tachyon: The Fringe DISP02E.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP02E.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 9 |
| Entities | 33 |
| Events | 13 |
| Waypoints | 7 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Carrier`, `1: GalSpan_Cruiser`, `2: Bora_Destroyer`, `3: Bora_Claymore`, `4: GalSpan_Phoenix`, `5: GalSpan_Pegasus`, `6: GalSpan_Archangel`, `7: Bora_Mace`, `8: Bora_Warhammer` |
| Scripts | `YOUNG.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFGE_03`, `BFGF_03`, `MERC_17`, `BFNE_01`, `CLEON`, `Patrol1`, `Patrol2`, `SPIKE`, `Redemption` |
| Aliases | `BC10_Claymore1`, `BC10_Claymore2`, `BC10_Claymore3`, `BC10_Claymore4`, `Coward`, `BC10_Waraxe`, `BC10_Mace1`, `BC10_Mace2`, `BC10_Mace3`, `BC10_Mace4`, `BC10_Warhammer1`, `BC10_Warhammer2`, `BC10_Warhammer3`, `BC10_Warhammer4`, `SPIKE`, `Stocks01` |
| Groups | `FG_SCOUT`, `FG_MUTINY`, `FG_JANUS`, `FG_PICTOR`, `FG_ARES`, `FG_RIGHTEOUS`, `FG_SEXTANS`, `FG_ASTERION`, `FG_INSURRECTION`, `FG_JACKHAMMER`, `FORTITUDE`, `PYXIS`, `GALLANT` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Object spawn/action: Bora_Carrier (object 32, id 395), subtype 21, param 6
- Set runtime trigger variable: variable group 20, variable 20, subtype 0, value 0
- Play dialog: YOUNG.SCR, line/variant 1
- Show/update HUD contact: contact/list 0, subtype 0, param 380
- Object spawn/action: Bora_Destroyer (object 30, id 380), subtype 14

### Event 1

**Trigger**

- Object event: subject Bora_Destroyer (object 30, id 380), op 3, value 60
- Variable comparison: subject variable group 21, variable 12, op 3, value 2

**Action**

- Play dialog: YOUNG.SCR, line/variant 3

### Event 2

**Trigger**

- Object event: subject Bora_Destroyer (object 30, id 380), op 2, value 0
- Variable comparison: subject variable group 21, variable 12, op 3, value 2

**Action**

- Play dialog: PLAYER.SCR, line/variant 108
- Object spawn/action: GalSpan_Cruiser (object 31, id 381), subtype 17

### Event 3

**Trigger**

- Object event: subject Bora_Destroyer (object 30, id 380), op 16, value 0
- Variable comparison: subject variable group 21, variable 12, op 3, value 2

**Action**

- Set/add variable: variable group 18, variable 414, subtype 0, value 1
- Set/add variable: variable group 18, variable 415, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 24
- Set runtime trigger variable: variable group 20, variable 28, subtype 0, value 0
- Set/add variable: variable group 21, variable 17, subtype 0, value 1

### Event 4

**Trigger**

- Object event: subject GalSpan_Cruiser (object 31, id 381), op 2, value 0
- Variable comparison: subject variable group 21, variable 17, op 3, value 1

**Action**

- Set/add variable: variable group 21, variable 12, subtype 0, value 2
- Set/add variable: variable group 18, variable 414, subtype 0, value 1
- Set/add variable: variable group 18, variable 415, subtype 0, value 1
- Play dialog: YOUNG.SCR, line/variant 7
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Hide/remove HUD contact: contact/list 0, subtype 0, param 380
- Show/update HUD contact: contact/list 0, subtype 11, param 25

### Event 5

**Trigger**

- Object arrival: GalSpan_Cruiser (object 31, id 381) reached Waypoint 4 (tag 304), point 1 (raw value 19922945)

**Action**

- Play dialog: YOUNG.SCR, line/variant 4
- Set runtime trigger variable: variable group 20, variable 18, subtype 0, value 0

### Event 6

**Trigger**

- Object arrival: GalSpan_Cruiser (object 31, id 381) reached Waypoint 4 (tag 304), point 2 (raw value 19922946)

**Action**

- Object spawn/action: GalSpan_Cruiser (object 31, id 381), subtype 18

### Event 7

**Trigger**

- Global enemy/object-count event: subject 0, op 0, value 0

**Action**

- Group/spawn-list action: spawn list/group 16, subtype 5, param 381
- Group/spawn-list action: spawn list/group 149, subtype 5, param 381
- Group/spawn-list action: spawn list/group 197, subtype 5, param 381
- Group/spawn-list action: spawn list/group 198, subtype 5, param 381
- Group/spawn-list action: spawn list/group 149, subtype 5, param 381

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 28, op 1, value 60

**Action**

- Object spawn/action: GalSpan_Cruiser (object 31, id 381), subtype 4

### Event 9

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 100

**Action**

- Play dialog: PLAYER.SCR, line/variant 150

### Event 10

**Trigger**

- Object event: subject GalSpan_Cruiser (object 31, id 381), op 4, value 100

**Action**

- Play dialog: YOUNG.SCR, line/variant 6

### Event 11

**Trigger**

- Variable comparison: subject variable group 20, variable 18, op 1, value 25

**Action**

- Group/spawn-list action: spawn list/group 102, subtype 0
- Group/spawn-list action: spawn list/group 103, subtype 0
- Play dialog: YOUNG.SCR, line/variant 5

### Event 12

**Trigger**

- Object event: subject Bora_Destroyer (object 30, id 380), op 2, value 0

**Action**

- Object spawn/action: Bora_Destroyer (object 30, id 380), subtype 21, param 8

## Waypoints

### Waypoint 0

- Tag: `308`
- Members: `Bora_Mace (object 2, id 410, starts at point 0)`, `Bora_Mace (object 3, id 411, starts at point 0)`, `Bora_Mace (object 4, id 412, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1116.34, 377.00, -6089.85) | None |
| 1 | (1285.40, 377.00, -5784.33) | None |
| 2 | (1557.77, 377.00, -5784.33) | None |

### Waypoint 1

- Tag: `307`
- Members: `Bora_Mace (object 13, id 404, starts at point 0)`, `Bora_Mace (object 14, id 402, starts at point 0)`, `Bora_Mace (object 15, id 403, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1910.89, 346.00, -6812.73) | None |
| 1 | (1953.45, 346.00, -6425.09) | None |
| 2 | (2200.29, 346.00, -6289.73) | None |

### Waypoint 2

- Tag: `306`
- Members: `Bora_Claymore (object 20, id 1724, starts at point 0)`, `Bora_Claymore (object 21, id 1725, starts at point 0)`, `Bora_Claymore (object 22, id 1726, starts at point 0)`, `Bora_Claymore (object 23, id 1727, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (345.01, 0.00, -7733.93) | None |
| 1 | (1183.14, 0.00, -6918.09) | None |
| 2 | (1998.37, 0.00, -6179.20) | None |

### Waypoint 3

- Tag: `305`
- Members: `Bora_Claymore (object 24, id 1728, starts at point 0)`, `Bora_Claymore (object 25, id 1729, starts at point 0)`, `Bora_Claymore (object 26, id 1730, starts at point 0)`, `Bora_Claymore (object 27, id 1731, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (530.08, 0.00, -7955.18) | None |
| 1 | (972.32, 0.00, -7359.67) | None |
| 2 | (1462.58, 0.00, -6756.50) | None |
| 3 | (2013.78, 0.00, -6235.19) | None |

### Waypoint 4

- Tag: `304`
- Members: `GalSpan_Cruiser (object 31, id 381, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1742.98, 0.00, -5544.73) | None |
| 1 | (2057.97, 0.00, -5894.40) | None; listened by Event 5 for GalSpan_Cruiser (object 31, id 381) |
| 2 | (2277.54, 0.00, -6170.25) | on arrival activate current object (raw param -1 ignored); listened by Event 6 for GalSpan_Cruiser (object 31, id 381) |

### Waypoint 5

- Tag: `303`
- Members: `GalSpan_Phoenix (object 19, id 1701, starts at point 0)`, `GalSpan_Phoenix (object 29, id 1929, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2833.81, 349.00, -5439.21) | None |
| 1 | (3289.56, 301.00, -6061.87) | None |
| 2 | (3646.50, 248.00, -6775.52) | None |
| 3 | (4015.36, 266.00, -7611.66) | None |

### Waypoint 6

- Tag: `301`
- Members: `GalSpan_Phoenix (object 18, id 418, starts at point 0)`, `GalSpan_Phoenix (object 28, id 1928, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2458.18, 0.00, -5608.35) | None |
| 1 | (2774.20, 204.00, -6371.93) | None |
| 2 | (3208.21, 320.00, -7178.26) | None |
| 3 | (3661.81, 294.00, -7761.70) | on arrival activate current object (raw param -1 ignored) |

## Spawn Lists

### Spawn List 0

- ID: `103`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | GalSpan_Cruiser (object 31, id 381) | None |

### Spawn List 1

- ID: `102`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | GalSpan_Cruiser (object 31, id 381) | None |

### Spawn List 2

- ID: `149`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Bora_Destroyer (object 30, id 380) | None |

### Spawn List 3

- ID: `198`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | id 379 | None |
| 1 | 6 | Bora_Destroyer (object 30, id 380) | None |

### Spawn List 4

- ID: `197`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Bora_Destroyer (object 30, id 380) | None |

### Spawn List 5

- ID: `83`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 6

- ID: `133`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 7

- ID: `53`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 8

- ID: `16`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 1 | spawn list 133 | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Bora_Warhammer` | 406 | Interactive | 1812.74,122.00,-7031.63 | 361,0,0 | label: BFGE_03; group/role: FG_SCOUT / 0 |
| 1 | `Bora_Warhammer` | 407 | Interactive | 1878.84,122.00,-6980.43 | 361,0,0 | group/role: FG_SCOUT / 0 |
| 2 | `Bora_Mace` | 410 | Interactive | 1188.30,305.00,-6434.21 | 0,0,0 | group/role: FG_MUTINY / 0; waypoint: Waypoint 0 (tag 308, 3 point(s)), starting point 0, arrival event value 20185088 |
| 3 | `Bora_Mace` | 411 | Interactive | 1235.52,305.00,-6393.25 | 0,0,0 | group/role: FG_MUTINY / 0; waypoint: Waypoint 0 (tag 308, 3 point(s)), starting point 0, arrival event value 20185088 |
| 4 | `Bora_Mace` | 412 | Interactive | 1282.73,305.00,-6342.05 | 0,0,0 | label: BFGE_03; group/role: FG_MUTINY / 0; waypoint: Waypoint 0 (tag 308, 3 point(s)), starting point 0, arrival event value 20185088 |
| 5 | `GalSpan_Archangel` | 416 | Interactive | 2075.09,339.56,-6656.11 | 247,14,0 | group/role: FG_JANUS / 0 |
| 6 | `GalSpan_Archangel` | 417 | Interactive | 2122.30,339.56,-6604.90 | 247,14,0 | label: BFGF_03; group/role: FG_JANUS / 0 |
| 7 | `GalSpan_Pegasus` | 423 | Interactive | 1303.84,349.08,-6063.95 | 269,486,0 | group/role: FG_PICTOR / 0 |
| 8 | `GalSpan_Pegasus` | 424 | Interactive | 1368.50,349.08,-6056.06 | 269,486,0 | group/role: FG_PICTOR / 0 |
| 9 | `GalSpan_Pegasus` | 425 | Interactive | 1442.59,349.08,-6053.09 | 269,486,0 | label: BFGF_03; group/role: FG_PICTOR / 0 |
| 10 | `GalSpan_Pegasus` | 1610 | Interactive | 1518.41,132.56,-6924.82 | 252,0,0 | group/role: FG_ARES / 0 |
| 11 | `GalSpan_Pegasus` | 1611 | Interactive | 1591.49,132.56,-6924.82 | 252,0,0 | group/role: FG_ARES / 0 |
| 12 | `GalSpan_Pegasus` | 1612 | Interactive | 1652.38,132.56,-6924.82 | 252,0,0 | label: BFGF_03; group/role: FG_ARES / 0 |
| 13 | `Bora_Mace` | 404 | Interactive | 2069.79,278.00,-7018.59 | 0,501,0 | label: BFGE_03; group/role: FG_RIGHTEOUS / 0; waypoint: Waypoint 1 (tag 307, 3 point(s)), starting point 0, arrival event value 20119552 |
| 14 | `Bora_Mace` | 402 | Interactive | 1937.57,278.00,-7172.20 | 0,0,0 | group/role: FG_RIGHTEOUS / 0; waypoint: Waypoint 1 (tag 307, 3 point(s)), starting point 0, arrival event value 20119552 |
| 15 | `Bora_Mace` | 403 | Interactive | 2013.13,278.00,-7121.00 | 0,0,0 | group/role: FG_RIGHTEOUS / 0; waypoint: Waypoint 1 (tag 307, 3 point(s)), starting point 0, arrival event value 20119552 |
| 16 | `Bora_Warhammer` | 1619 | Interactive | 1927.78,122.00,-7034.62 | 361,0,0 | group/role: FG_SCOUT / 0 |
| 17 | `GalSpan_Archangel` | 1662 | Interactive | 2168.52,339.56,-6662.63 | 236,14,0 | group/role: FG_JANUS / 0 |
| 18 | `GalSpan_Phoenix` | 418 | Interactive | 2207.86,61.56,-5311.58 | 208,0,0 | group/role: FG_SEXTANS / 0; waypoint: Waypoint 6 (tag 301, 4 point(s)), starting point 0, arrival event value 19726336 |
| 19 | `GalSpan_Phoenix` | 1701 | Interactive | 2584.93,64.00,-4937.18 | 226,0,0 | group/role: FG_ASTERION / 0; waypoint: Waypoint 5 (tag 303, 4 point(s)), starting point 0, arrival event value 19857408 |
| 20 | `Bora_Claymore` | 1724 | Interactive | 135.43,0.00,-7924.43 | 49,0,0 | group/role: FG_INSURRECTION / 0; waypoint: Waypoint 2 (tag 306, 3 point(s)), starting point 0, arrival event value 20054016 |
| 21 | `Bora_Claymore` | 1725 | Interactive | 195.36,0.00,-7916.30 | 49,0,0 | group/role: FG_INSURRECTION / 0; waypoint: Waypoint 2 (tag 306, 3 point(s)), starting point 0, arrival event value 20054016 |
| 22 | `Bora_Claymore` | 1726 | Interactive | 285.25,0.00,-7916.30 | 48,0,0 | label: BFGE_03; group/role: FG_INSURRECTION / 0; waypoint: Waypoint 2 (tag 306, 3 point(s)), starting point 0, arrival event value 20054016 |
| 23 | `Bora_Claymore` | 1727 | Interactive | 232.82,0.00,-7956.92 | 49,0,0 | group/role: FG_INSURRECTION / 0; waypoint: Waypoint 2 (tag 306, 3 point(s)), starting point 0, arrival event value 20054016 |
| 24 | `Bora_Claymore` | 1728 | Interactive | 328.32,0.00,-8151.20 | 60,0,0 | group/role: FG_JACKHAMMER / 0; waypoint: Waypoint 3 (tag 305, 4 point(s)), starting point 0, arrival event value 19988480 |
| 25 | `Bora_Claymore` | 1729 | Interactive | 395.74,0.00,-8151.20 | 60,0,0 | group/role: FG_JACKHAMMER / 0; waypoint: Waypoint 3 (tag 305, 4 point(s)), starting point 0, arrival event value 19988480 |
| 26 | `Bora_Claymore` | 1730 | Interactive | 455.67,0.00,-8151.20 | 60,0,0 | label: BFGE_03; group/role: FG_JACKHAMMER / 0; waypoint: Waypoint 3 (tag 305, 4 point(s)), starting point 0, arrival event value 19988480 |
| 27 | `Bora_Claymore` | 1731 | Interactive | 425.71,0.00,-8240.55 | 60,0,0 | group/role: FG_JACKHAMMER / 0; waypoint: Waypoint 3 (tag 305, 4 point(s)), starting point 0, arrival event value 19988480 |
| 28 | `GalSpan_Phoenix` | 1928 | Interactive | 2247.63,0.00,-5287.15 | 202,0,0 | label: BFGF_03; group/role: FG_SEXTANS / 0; waypoint: Waypoint 6 (tag 301, 4 point(s)), starting point 0, arrival event value 19726336 |
| 29 | `GalSpan_Phoenix` | 1929 | Interactive | 2632.67,0.00,-4920.65 | 208,0,0 | label: BFGF_03; group/role: FG_ASTERION / 0; waypoint: Waypoint 5 (tag 303, 4 point(s)), starting point 0, arrival event value 19857408 |
| 30 | `Bora_Destroyer` | 380 | Interactive | 4399.01,223.96,-8151.45 | 38,495,0 | label: BFGE_03; secondary groups: none, FORTITUDE |
| 31 | `GalSpan_Cruiser` | 381 | Interactive | 757.22,158.08,-4586.74 | 195,505,0 | secondary groups: none, PYXIS; waypoint: Waypoint 4 (tag 304, 3 point(s)), starting point 0, arrival event value 19922944 |
| 32 | `Bora_Carrier` | 395 | Interactive | 1503.27,535.41,-3421.25 | 183,501,0 | secondary groups: none, GALLANT |
