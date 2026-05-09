# Tachyon: The Fringe NEUT03A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT03A.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 20 |
| Events | 31 |
| Waypoints | 16 |
| Child Sectors | 0 |
| Scripts | 4 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Destroyer`, `1: Bora_Hvy_Freighter`, `2: Bora_Cutlass`, `3: Star_Patrol_Enforcer` |
| Scripts | `PLAYER.SCR`, `G02BFB.SCR`, `TRISH.SCR`, `G02BRB.SCR` |
| Scenes | None |
| Labels | `OBULO`, `BFIGH`, `G02BFA`, `BFGE_07`, `G02BRB`, `HERID` |
| Aliases | `fred_fighter1`, `fred_fighter2`, `fred_freighter1`, `fred_freighter2` |
| Groups | `FG_TORNADO`, `FG_MUTINY`, `FG_VALOR`, `CAMEL_47`, `CONT_018`, `VICTORY`, `CONT_021`, `INSPIRATION`, `CONT_041`, `BURROW`, `CONT_043`, `EXPLORATION`, `CONT_028`, `HOPE`, `CONT_004`, `PROMISE`, `CONT_006`, `HERIDES`, `PAN`, `HERCULES`, `PILGRIM`, `CONT_039`, `EXEMPTION`, `CONT_020`, `TRAVELER`, `CONT_022` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 11
- Gate state/action: param 1041, subtype 3, param 0
- Set/add variable: variable group 21, variable 26, subtype 0, value 1
- Set runtime trigger variable: variable group 20, variable 15, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 15, op 1, value 3

**Action**

- Play dialog: PLAYER.SCR, line/variant 54
- Set runtime trigger variable: variable group 20, variable 15, subtype 1, value 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Object spawn/action: Bora_Hvy_Freighter (object 7, id 1042), subtype 5
- Object spawn/action: Bora_Hvy_Freighter (object 8, id 1059), subtype 5
- Object spawn/action: Bora_Hvy_Freighter (object 9, id 1067), subtype 5
- Object spawn/action: Bora_Hvy_Freighter (object 10, id 1075), subtype 5
- Object spawn/action: Bora_Hvy_Freighter (object 11, id 1083), subtype 5
- Object spawn/action: Bora_Hvy_Freighter (object 12, id 1107), subtype 5
- Object spawn/action: Bora_Hvy_Freighter (object 13, id 1116), subtype 5
- Object spawn/action: Bora_Hvy_Freighter (object 18, id 1050), subtype 5

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Object spawn/action: Bora_Hvy_Freighter (object 17, id 1126), subtype 5
- Object spawn/action: Bora_Hvy_Freighter (object 19, id 1136), subtype 5

### Event 4

**Trigger**

- Variable comparison: subject variable group 21, variable 2, op 0, value 1

**Action**

- Object spawn/action: Bora_Hvy_Freighter (object 7, id 1042), subtype 3

### Event 5

**Trigger**

- Variable comparison: subject variable group 21, variable 3, op 0, value 1

**Action**

- Object spawn/action: Bora_Hvy_Freighter (object 18, id 1050), subtype 3

### Event 6

**Trigger**

- Object event: subject Bora_Hvy_Freighter (object 10, id 1075), op 10, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 57
- Hide/remove HUD contact: contact/list 0, subtype 9, param 11
- Show/update HUD contact: contact/list 0, subtype 9, param 12
- Set/add variable: variable group 21, variable 30, subtype 0, value 1

### Event 7

**Trigger**

- Object event: subject Bora_Cutlass (object 5, id 1163), op 2, value 0 (join 2)
- Object event: subject Bora_Cutlass (object 6, id 1164), op 2, value 0

**Action**

- Play dialog: G02BFB.SCR, line/variant 1

### Event 8

**Trigger**

- Object event: subject 1165, op 2, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 55

### Event 9

**Trigger**

- Variable comparison: subject variable group 21, variable 33, op 1, value 0
- Variable comparison: subject variable group 21, variable 34, op 1, value 1
- Variable comparison: subject variable group 21, variable 32, op 1, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 56

### Event 10

**Trigger**

- Object event: subject Bora_Hvy_Freighter (object 10, id 1075), op 2, value 0

**Action**

- Play dialog: TRISH.SCR, line/variant 5

### Event 11

**Trigger**

- Object event: subject Bora_Hvy_Freighter (object 10, id 1075), op 8, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 59

### Event 12

**Trigger**

- Object event: subject Bora_Hvy_Freighter (object 10, id 1075), op 2, value 0 (join 2)
- Object event: subject Bora_Hvy_Freighter (object 10, id 1075), op 8, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Set runtime trigger variable: variable group 20, variable 31, subtype 0, value 0

### Event 13

**Trigger**

- Variable comparison: subject variable group 20, variable 31, op 1, value 1

**Action**

- Set/add variable: variable group 13, variable 406, subtype 0, value 1
- Set/add variable: variable group 13, variable 407, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 11
- Hide/remove HUD contact: contact/list 0, subtype 9, param 12
- Show/update HUD contact: contact/list 0, subtype 11, param 34
- Set runtime trigger variable: variable group 20, variable 31, subtype 1, value 0

### Event 14

**Trigger**

- Object event: subject Bora_Hvy_Freighter (object 10, id 1075), op 14, value 9

**Action**

- Play dialog: G02BRB.SCR, line/variant 2
- Hide/remove HUD contact: contact/list 0, subtype 9, param 12
- Set runtime trigger variable: variable group 20, variable 4, subtype 0, value 0

### Event 15

**Trigger**

- Variable comparison: subject variable group 20, variable 4, op 1, value 25 (join 2)
- Sector/startup condition family: subject 3, op 0, value 2

**Action**

- Set/add variable: variable group 21, variable 32, subtype 0, value 1
- Set runtime trigger variable: variable group 20, variable 4, subtype 1, value 0

### Event 16

**Trigger**

- Variable comparison: subject variable group 21, variable 32, op 1, value 1
- Variable comparison: subject variable group 21, variable 33, op 1, value 1

**Action**

- Set/add variable: variable group 38, variable 5, subtype 0, value 1

### Event 17

**Trigger**

- Variable comparison: subject variable group 21, variable 32, op 1, value 1
- Variable comparison: subject variable group 21, variable 33, op 1, value 1

**Action**

- Set/add variable: variable group 13, variable 406, subtype 0, value 1
- Set/add variable: variable group 13, variable 407, subtype 0, value 2
- Set runtime trigger variable: variable group 20, variable 18, subtype 0, value 0
- Play dialog: G02BRB.SCR, line/variant 3
- Play scene: unknown index 0, param 0
- Object spawn/action: GalSpan_Destroyer (object 14, id 1436), subtype 3
- Object spawn/action: GalSpan_Destroyer (object 15, id 1448), subtype 3
- Object spawn/action: GalSpan_Destroyer (object 16, id 1460), subtype 3

### Event 18

**Trigger**

- Variable comparison: subject variable group 20, variable 18, op 1, value 3

**Action**

- Group/spawn-list action: spawn list/group 256, subtype 1, param 1040
- Hide/remove HUD contact: contact/list 0, subtype 10, param 0

### Event 19

**Trigger**

- Sector/startup condition family: subject 3, op 0, value 3 (join 2)
- Runtime condition family: subject 0, op 0, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 24, subtype 0, value 0

### Event 20

**Trigger**

- Variable comparison: subject variable group 20, variable 24, op 1, value 2

**Action**

- Play dialog: TRISH.SCR, line/variant 8
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 33

### Event 21

**Trigger**

- Object event: subject Bora_Hvy_Freighter (object 7, id 1042), op 0, value 0 (join 2; flags 2)
- Object event: subject Bora_Hvy_Freighter (object 8, id 1059), op 0, value 0 (join 2; flags 2)
- Object event: subject Bora_Hvy_Freighter (object 9, id 1067), op 0, value 0 (join 2; flags 2)
- Object event: subject Bora_Hvy_Freighter (object 10, id 1075), op 0, value 0 (join 2; flags 2)
- Object event: subject Bora_Hvy_Freighter (object 11, id 1083), op 0, value 0 (join 2; flags 2)
- Object event: subject Bora_Hvy_Freighter (object 12, id 1107), op 0, value 0 (join 2; flags 2)
- Object event: subject Bora_Hvy_Freighter (object 13, id 1116), op 0, value 0 (join 2; flags 2)
- Object event: subject Bora_Hvy_Freighter (object 18, id 1050), op 0, value 0 (join 2; flags 2)

**Action**

- Set/add variable: variable group 21, variable 29, subtype 0, value 1

### Event 22

**Trigger**

- Object event: subject Bora_Hvy_Freighter (object 17, id 1126), op 0, value 0 (join 2; flags 2)
- Object event: subject Bora_Hvy_Freighter (object 19, id 1136), op 0, value 0 (join 2; flags 2)
- Object event: subject Bora_Hvy_Freighter (object 10, id 1075), op 14, value 9

**Action**

- Set/add variable: variable group 21, variable 29, subtype 0, value 1

### Event 23

**Trigger**

- Variable comparison: subject variable group 21, variable 29, op 1, value 1

**Action**

- Play dialog: G02BRB.SCR, line/variant 0
- Group/spawn-list action: spawn list/group 85, subtype 0
- Show/update HUD contact: contact/list 0, subtype 1, param 85

### Event 24

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 900 (extra 1, 1163; flags 2)

**Action**

- Play dialog: G02BFB.SCR, line/variant 0

### Event 25

**Trigger**

- Group/spawn-list event: subject 85, op 0, value 0 (join 2)
- Group/spawn-list event: subject 85, op 6, value 0 (join 2)

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 85
- Set/add variable: variable group 21, variable 33, subtype 0, value 1

### Event 26

**Trigger**

- Group/spawn-list event: subject 83, op 0, value 0 (join 2)
- Group/spawn-list event: subject 83, op 6, value 0 (join 2)

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 83
- Set/add variable: variable group 21, variable 34, subtype 0, value 1

### Event 27

**Trigger**

- Group/spawn-list event: subject 83, op 3, value 0
- Variable comparison: subject variable group 21, variable 34, op 1, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 1, param 83

### Event 28

**Trigger**

- Object event: subject GalSpan_Destroyer (object 14, id 1436), op 15, value 0

**Action**

- Object spawn/action: GalSpan_Destroyer (object 14, id 1436), subtype 18

### Event 29

**Trigger**

- Object event: subject GalSpan_Destroyer (object 15, id 1448), op 15, value 0

**Action**

- Object spawn/action: GalSpan_Destroyer (object 15, id 1448), subtype 18

### Event 30

**Trigger**

- Object event: subject GalSpan_Destroyer (object 16, id 1460), op 15, value 0

**Action**

- Object spawn/action: GalSpan_Destroyer (object 16, id 1460), subtype 18

## Waypoints

### Waypoint 0

- Tag: `17`
- Members: `Star_Patrol_Enforcer (object 0, id 1491, starts at point 0)`, `Star_Patrol_Enforcer (object 1, id 1492, starts at point 0)`, `Star_Patrol_Enforcer (object 2, id 1493, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (3991.10, 0.00, -2840.40) | None |
| 1 | (2794.39, 0.00, 3904.06) | None |
| 2 | (4002.13, 0.00, -3202.50) | on arrival play dialog/script or enter gate, param 1040 |

### Waypoint 1

- Tag: `16`
- Members: `Bora_Cutlass (object 3, id 1472, starts at point 0)`, `Bora_Cutlass (object 4, id 1473, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (3949.02, 0.00, -2945.58) | None |
| 1 | (3489.92, 0.00, -1057.17) | None |
| 2 | (-896.56, 0.00, 11007.88) | on arrival redirect to Waypoint 1 (tag 16), point 1 |

### Waypoint 2

- Tag: `15`
- Members: `Bora_Hvy_Freighter (object 18, id 1050, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (3786.22, 0.00, -2395.04) | on arrival activate current object (raw param -1 ignored) |
| 1 | (3699.45, 0.00, -984.77) | None |
| 2 | (-837.03, 0.00, 11094.56) | on arrival action 1, param -1 |

### Waypoint 3

- Tag: `14`
- Members: `Bora_Hvy_Freighter (object 7, id 1042, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (3284.75, 0.00, -2395.29) | on arrival activate current object (raw param -1 ignored) |
| 1 | (3192.20, 0.00, -1429.15) | None |
| 2 | (-1689.29, 0.00, 11173.76) | on arrival action 1, param -1 |

### Waypoint 4

- Tag: `13`
- Members: `Bora_Hvy_Freighter (object 10, id 1075, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (3648.59, 0.00, -1039.71) | None |
| 1 | (-1260.21, 0.00, 11137.73) | on arrival action 1, param -1 |

### Waypoint 5

- Tag: `12`
- Members: `Bora_Hvy_Freighter (object 13, id 1116, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (3197.37, 0.00, -1338.61) | None |
| 1 | (-1573.77, 0.00, 10849.52) | on arrival action 1, param -1 |

### Waypoint 6

- Tag: `11`
- Members: `Bora_Hvy_Freighter (object 17, id 1126, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (3374.64, 0.00, -433.93) | None |
| 1 | (-1050.27, 0.00, 10985.95) | on arrival action 1, param -1 |

### Waypoint 7

- Tag: `10`
- Members: `Bora_Hvy_Freighter (object 8, id 1059, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (3041.32, 0.00, -890.82) | None |
| 1 | (-1567.57, 0.00, 11009.51) | on arrival action 1, param -1 |

### Waypoint 8

- Tag: `9`
- Members: `Bora_Hvy_Freighter (object 19, id 1136, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2679.18, 0.00, 976.98) | None |
| 1 | (-1135.65, 0.00, 11012.51) | on arrival action 1, param -1 |

### Waypoint 9

- Tag: `8`
- Members: `Bora_Hvy_Freighter (object 9, id 1067, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2161.96, 0.00, 1026.07) | None |
| 1 | (-1720.33, 0.00, 10975.69) | on arrival action 1, param -1 |

### Waypoint 10

- Tag: `7`
- Members: `GalSpan_Destroyer (object 16, id 1460, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (4764.93, 0.00, -720.00) | None |
| 1 | (3978.08, 0.00, 1108.47) | None |
| 2 | (2044.60, 0.00, 6146.23) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 11

- Tag: `6`
- Members: `GalSpan_Destroyer (object 15, id 1448, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (4125.52, 0.00, -1354.61) | None |
| 1 | (2798.50, 0.00, 1769.61) | None |
| 2 | (1130.72, 0.00, 5914.46) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 12

- Tag: `5`
- Members: `GalSpan_Destroyer (object 14, id 1436, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (3916.41, 0.00, -108.86) | None |
| 1 | (3493.78, 0.00, 930.28) | None |
| 2 | (1248.07, 0.00, 6745.00) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 13

- Tag: `3`
- Members: `Bora_Cutlass (object 5, id 1163, starts at point 0)`, `Bora_Cutlass (object 6, id 1164, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-29.44, 0.00, 3918.90) | None |
| 1 | (4011.83, 0.00, -2781.13) | None |
| 2 | (3125.34, 0.00, 494.48) | None |
| 3 | (1660.96, 0.00, 4162.41) | None |
| 4 | (-81.85, 0.00, 8936.65) | on arrival redirect to Waypoint 13 (tag 3), point 2 |

### Waypoint 14

- Tag: `2`
- Members: `Bora_Hvy_Freighter (object 12, id 1107, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2095.26, 0.00, 2223.39) | None |
| 1 | (-1008.35, 0.00, 11093.70) | on arrival action 1, param -1 |

### Waypoint 15

- Tag: `1`
- Members: `Bora_Hvy_Freighter (object 11, id 1083, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1805.67, 0.00, 1741.86) | None |
| 1 | (-1394.17, 0.00, 11073.25) | on arrival action 1, param -1 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Star_Patrol_Enforcer` | 1491 | Interactive | 4130.68,0.00,-4178.48 | 492,0,0 | label: OBULO; group/role: FG_TORNADO / 0; waypoint: Waypoint 0 (tag 17, 3 point(s)), starting point 0, arrival event value 1114112 |
| 1 | `Star_Patrol_Enforcer` | 1492 | Interactive | 4260.88,0.00,-4340.20 | 492,0,0 | group/role: FG_TORNADO / 1; waypoint: Waypoint 0 (tag 17, 3 point(s)), starting point 0, arrival event value 1114112 |
| 2 | `Star_Patrol_Enforcer` | 1493 | Interactive | 4431.80,0.00,-4504.71 | 492,0,0 | group/role: FG_TORNADO / 2; waypoint: Waypoint 0 (tag 17, 3 point(s)), starting point 0, arrival event value 1114112 |
| 3 | `Bora_Cutlass` | 1472 | Interactive | 3949.02,0.00,-3394.71 | 0,0,0 | label: BFIGH; group/role: FG_MUTINY / 0; alias: fred_fighter1; waypoint: Waypoint 1 (tag 16, 3 point(s)), starting point 0, arrival event value 1048576 |
| 4 | `Bora_Cutlass` | 1473 | Interactive | 3819.21,0.00,-3553.57 | 0,0,0 | label: G02BFA; group/role: FG_MUTINY / 1; alias: fred_fighter2; waypoint: Waypoint 1 (tag 16, 3 point(s)), starting point 0, arrival event value 1048576 |
| 5 | `Bora_Cutlass` | 1163 | Interactive | -16.91,0.00,4110.74 | 253,0,0 | label: BFGE_07; group/role: FG_VALOR / 0; waypoint: Waypoint 13 (tag 3, 5 point(s)), starting point 0, arrival event value 196608 |
| 6 | `Bora_Cutlass` | 1164 | Interactive | -253.30,0.00,4232.13 | 253,0,0 | label: BFGE_07; group/role: FG_VALOR / 1; waypoint: Waypoint 13 (tag 3, 5 point(s)), starting point 0, arrival event value 196608 |
| 7 | `Bora_Hvy_Freighter` | 1042 | Interactive | 3285.90,0.00,-2538.80 | 0,0,0 | alias: fred_freighter1; secondary groups: CONT_018, CAMEL_47; waypoint: Waypoint 3 (tag 14, 3 point(s)), starting point 0, arrival event value 917504 |
| 8 | `Bora_Hvy_Freighter` | 1059 | Interactive | 3228.50,0.00,-1625.55 | 506,0,0 | secondary groups: CONT_021, VICTORY; waypoint: Waypoint 7 (tag 10, 2 point(s)), starting point 0, arrival event value 655360 |
| 9 | `Bora_Hvy_Freighter` | 1067 | Interactive | 3104.51,0.00,-1104.34 | 488,0,0 | secondary groups: CONT_041, INSPIRATION; waypoint: Waypoint 9 (tag 8, 2 point(s)), starting point 0, arrival event value 524288 |
| 10 | `Bora_Hvy_Freighter` | 1075 | Interactive | 3764.49,0.00,-2114.02 | 506,0,0 | label: G02BRB; secondary groups: CONT_043, BURROW; waypoint: Waypoint 4 (tag 13, 2 point(s)), starting point 0, arrival event value 851968 |
| 11 | `Bora_Hvy_Freighter` | 1083 | Interactive | 2993.75,0.00,-742.75 | 486,0,0 | secondary groups: CONT_028, EXPLORATION; waypoint: Waypoint 15 (tag 1, 2 point(s)), starting point 0, arrival event value 65536 |
| 12 | `Bora_Hvy_Freighter` | 1107 | Interactive | 3453.30,0.00,-627.38 | 486,0,0 | secondary groups: CONT_004, HOPE; waypoint: Waypoint 14 (tag 2, 2 point(s)), starting point 0, arrival event value 131072 |
| 13 | `Bora_Hvy_Freighter` | 1116 | Interactive | 3263.45,0.00,-2091.55 | 506,0,0 | secondary groups: CONT_006, PROMISE; waypoint: Waypoint 5 (tag 12, 2 point(s)), starting point 0, arrival event value 786432 |
| 14 | `GalSpan_Destroyer` | 1436 | Interactive | 4584.05,0.00,-1426.50 | 469,0,0 | label: HERID; secondary groups: none, HERIDES; waypoint: Waypoint 12 (tag 5, 3 point(s)), starting point 0, arrival event value 327680 |
| 15 | `GalSpan_Destroyer` | 1448 | Interactive | 4677.06,0.00,-2456.91 | 470,0,0 | secondary groups: none, PAN; waypoint: Waypoint 11 (tag 6, 3 point(s)), starting point 0, arrival event value 393216 |
| 16 | `GalSpan_Destroyer` | 1460 | Interactive | 5369.90,0.00,-2233.01 | 470,0,0 | secondary groups: none, HERCULES; waypoint: Waypoint 10 (tag 7, 3 point(s)), starting point 0, arrival event value 458752 |
| 17 | `Bora_Hvy_Freighter` | 1126 | Interactive | 3718.27,0.00,-1571.89 | 499,0,0 | secondary groups: CONT_039, PILGRIM; waypoint: Waypoint 6 (tag 11, 2 point(s)), starting point 0, arrival event value 720896 |
| 18 | `Bora_Hvy_Freighter` | 1050 | Interactive | 3790.83,0.00,-2522.86 | 509,0,0 | alias: fred_freighter2; secondary groups: CONT_020, EXEMPTION; waypoint: Waypoint 2 (tag 15, 3 point(s)), starting point 0, arrival event value 983040 |
| 19 | `Bora_Hvy_Freighter` | 1136 | Interactive | 3590.80,0.00,-990.28 | 484,0,0 | secondary groups: CONT_022, TRAVELER; waypoint: Waypoint 8 (tag 9, 2 point(s)), starting point 0, arrival event value 589824 |
