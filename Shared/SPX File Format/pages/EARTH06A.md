# Tachyon: The Fringe EARTH06A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH06A.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `(none)` |
| Region | 0 |
| Sector ID | 5 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 16 |
| Events | 17 |
| Waypoints | 7 |
| Child Sectors | 0 |
| Scripts | 4 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Minelayer`, `1: AGT_Orion`, `2: Independent_Merc_Dart`, `3: Spy_Probe` |
| Scripts | `PLAYER.SCR`, `mine.scr`, `ARI2.SCR`, `AGTF.SCR` |
| Scenes | None |
| Labels | `STPF`, `ARI2`, `bfne_08`, `bfne_01`, `PIRA`, `PIRB`, `MINE`, `FRTB` |
| Aliases | None |
| Groups | `FG_GALSPAN1`, `FG_BORA6`, `FG_AGT_RIVAL3`, `FG_AGT_RIVAL2`, `FG_AGT5`, `FG_AGT_RIVAL1`, `CONT_005` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Play scene: unknown index 0, param 0
- Show/update HUD contact: contact/list 0, subtype 1, param 33
- Set runtime trigger variable: variable group 20, variable 13, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 13, op 1, value 7

**Action**

- Play dialog: PLAYER.SCR, line/variant 5
- Set runtime trigger variable: variable group 20, variable 13, subtype 1, value 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 900 (extra 1, 481; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 900 (extra 1, 483; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 900 (extra 1, 1154; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 900 (extra 1, 1788; join 2; flags 2)

**Action**

- Set/add variable: variable group 21, variable 26, subtype 0, value 1

### Event 3

**Trigger**

- Group/spawn-list event: subject 33, op 1, value 50

**Action**

- Set runtime trigger variable: variable group 20, variable 20, subtype 0, value 0

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 20, op 1, value 7

**Action**

- Group/spawn-list action: spawn list/group 11, subtype 0
- Show/update HUD contact: contact/list 0, subtype 1, param 11
- Set runtime trigger variable: variable group 20, variable 20, subtype 1, value 0

### Event 5

**Trigger**

- Object event: subject Generic_Minelayer (object 15, id 1779), op 0, value 0 (join 2; flags 2)
- Object event: subject Generic_Minelayer (object 15, id 1779), op 4, value 10 (join 2)

**Action**

- Set runtime trigger variable: variable group 20, variable 13, subtype 0, value 0
- Group/spawn-list action: spawn list/group 24, subtype 1, param 1779
- Show/update HUD contact: contact/list 0, subtype 1, param 24
- Group/spawn-list action: spawn list/group 5, subtype 1, param 2
- Play dialog: mine.scr, line/variant 1

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 13, op 1, value 20

**Action**

- Play dialog: ARI2.SCR, line/variant 1

### Event 7

**Trigger**

- Object event: subject Independent_Merc_Dart (object 5, id 1155), op 2, value 0 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 51

### Event 8

**Trigger**

- Group/spawn-list event: subject 33, op 0, value 0
- Group/spawn-list event: subject 24, op 0, value 0
- Object event: subject Generic_Minelayer (object 15, id 1779), op 2, value 0
- Group/spawn-list event: subject 11, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Set/add variable: variable group 12, variable 0, subtype 0, value 1
- Set/add variable: variable group 12, variable 4, subtype 0, value 2
- Play dialog: PLAYER.SCR, line/variant 26
- Group/spawn-list action: spawn list/group 5, subtype 3, param 2
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 30

### Event 9

**Trigger**

- Object event: subject Independent_Merc_Dart (object 6, id 1156), op 4, value 50

**Action**

- Play dialog: ARI2.SCR, line/variant 0

### Event 10

**Trigger**

- Object event: subject Generic_Minelayer (object 15, id 1779), op 3, value 80

**Action**

- Play dialog: mine.scr, line/variant 0

### Event 11

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 1050 (extra 1, 1779; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 138

### Event 12

**Trigger**

- Variable comparison: subject variable group 21, variable 26, op 1, value 1
- Variable comparison: subject variable group 21, variable 27, op 1, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 12

### Event 13

**Trigger**

- Object event: subject Generic_Minelayer (object 15, id 1779), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 27, subtype 0, value 1

### Event 14

**Trigger**

- Sector/startup condition family: subject 2, op 0, value 1

**Action**

- Play dialog: AGTF.SCR, line/variant 31

### Event 15

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 12

**Action**

- Show/update HUD contact: contact/list 0, subtype 0, param 1779

### Event 16

**Trigger**

- Object event: subject Generic_Minelayer (object 15, id 1779), op 2, value 0

**Action**

- Object spawn/action: Generic_Minelayer (object 15, id 1779), subtype 21, param 6

## Waypoints

### Waypoint 0

- Tag: `101`
- Members: `AGT_Orion (object 9, id 2838, starts at point 0)`, `AGT_Orion (object 10, id 2839, starts at point 0)`, `AGT_Orion (object 11, id 2840, starts at point 0)`, `AGT_Orion (object 12, id 2843, starts at point 0)`, `AGT_Orion (object 14, id 2852, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-589.45, 379.34, 840.77) | None |

### Waypoint 1

- Tag: `6`
- Members: `Spy_Probe (object 2, id 481, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (3321.09, -1210.00, 1003.97) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 2

- Tag: `4`
- Members: `Spy_Probe (object 1, id 483, starts at point 0)`, `Independent_Merc_Dart (object 3, id 2747, starts at point 0)`, `Independent_Merc_Dart (object 4, id 2748, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1983.99, 0.00, -343.99) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 3

- Tag: `3`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-335.89, 0.00, 3063.58) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 4

- Tag: `2`
- Members: `Generic_Minelayer (object 15, id 1779, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1041.95, 530.91, -611.66) | None |
| 1 | (438.50, 528.93, 296.86) | None |
| 2 | (-1334.47, 494.71, 1067.94) | None |
| 3 | (-2129.50, 494.71, 956.70) | None |
| 4 | (-2651.46, 494.71, 74.27) | None |
| 5 | (-2405.66, 494.71, -1709.95) | None |
| 6 | (-1150.43, 494.71, -2291.64) | None |
| 7 | (885.84, 494.71, -2101.68) | on arrival redirect to Waypoint 4 (tag 2), point 0 |

### Waypoint 5

- Tag: `9`
- Members: `Independent_Merc_Dart (object 5, id 1155, starts at point 0)`, `Independent_Merc_Dart (object 6, id 1156, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-33.78, 573.00, 616.83) | None |

### Waypoint 6

- Tag: `1`
- Members: `Independent_Merc_Dart (object 7, id 2728, starts at point 0)`, `Independent_Merc_Dart (object 8, id 2729, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1408.44, -1489.00, 753.29) | None |
| 1 | (837.17, 0.00, 2274.52) | None |
| 2 | (251.01, 0.00, 1068.79) | on arrival redirect to Waypoint 6 (tag 1), point 0 |

## Spawn Lists

### Spawn List 0

- ID: `11`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 5 | spawn list 5 | None |

### Spawn List 1

- ID: `12`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 5 | spawn list 5 | None |
| 1 | 0 | none | None |

### Spawn List 2

- ID: `24`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 5 | spawn list 5 | None |
| 1 | 0 | none | None |

### Spawn List 3

- ID: `5`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 5 | spawn list 11 | None |
| 2 | 5 | id 23 | None |
| 3 | 5 | spawn list 24 | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Spy_Probe` | 1788 | Interactive | -350.21,0.00,3105.40 | 0,0,0 | group/role: FG_GALSPAN1 / 2 |
| 1 | `Spy_Probe` | 483 | Interactive | 732.83,371.00,3083.41 | 0,0,0 | group/role: FG_GALSPAN1 / 1; waypoint: Waypoint 2 (tag 4, 1 point(s)), starting point 0, arrival event value 262144 |
| 2 | `Spy_Probe` | 481 | Interactive | 3285.88,-1423.00,1055.22 | 0,0,0 | group/role: FG_GALSPAN1 / 3; waypoint: Waypoint 1 (tag 6, 1 point(s)), starting point 0, arrival event value 393216 |
| 3 | `Independent_Merc_Dart` | 2747 | Interactive | 1150.14,0.00,-552.76 | 0,0,0 | label: ARI2; group/role: FG_BORA6 / 0; waypoint: Waypoint 2 (tag 4, 1 point(s)), starting point 0, arrival event value 262144 |
| 4 | `Independent_Merc_Dart` | 2748 | Interactive | 1205.61,0.00,-552.76 | 0,0,0 | label: bfne_08; group/role: FG_BORA6 / 0; waypoint: Waypoint 2 (tag 4, 1 point(s)), starting point 0, arrival event value 262144 |
| 5 | `Independent_Merc_Dart` | 1155 | Interactive | -314.20,885.00,-391.16 | 128,0,0 | group/role: FG_AGT_RIVAL3 / 0; waypoint: Waypoint 5 (tag 9, 1 point(s)), starting point 0, arrival event value 589824 |
| 6 | `Independent_Merc_Dart` | 1156 | Interactive | -457.33,885.00,91.92 | 128,0,0 | group/role: FG_AGT_RIVAL3 / 1; waypoint: Waypoint 5 (tag 9, 1 point(s)), starting point 0, arrival event value 589824 |
| 7 | `Independent_Merc_Dart` | 2728 | Interactive | 806.04,-1210.00,24.14 | 85,0,0 | group/role: FG_AGT_RIVAL2 / 0; waypoint: Waypoint 6 (tag 1, 3 point(s)), starting point 0, arrival event value 65536 |
| 8 | `Independent_Merc_Dart` | 2729 | Interactive | 806.34,-1210.00,-40.03 | 92,0,0 | label: bfne_01; group/role: FG_AGT_RIVAL2 / 2; waypoint: Waypoint 6 (tag 1, 3 point(s)), starting point 0, arrival event value 65536 |
| 9 | `AGT_Orion` | 2838 | Interactive | -1212.10,0.00,1676.29 | 0,0,0 | group/role: FG_AGT5 / 1; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 10 | `AGT_Orion` | 2839 | Interactive | -1298.57,0.00,1597.84 | 0,0,0 | group/role: FG_AGT5 / 2; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 11 | `AGT_Orion` | 2840 | Interactive | -1164.65,0.00,1564.07 | 0,0,0 | group/role: FG_AGT5 / 3; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 12 | `AGT_Orion` | 2843 | Interactive | -1224.35,0.00,1491.36 | 0,0,0 | group/role: FG_AGT5 / 4; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 13 | `Spy_Probe` | 1154 | Interactive | 2148.29,-849.00,686.47 | 0,0,0 | group/role: FG_GALSPAN1 / 2 |
| 14 | `AGT_Orion` | 2852 | Interactive | -1164.44,0.00,1408.03 | 0,0,0 | group/role: FG_AGT5 / 5; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 15 | `Generic_Minelayer` | 1779 | Interactive | 1950.92,545.07,-1970.06 | 469,0,0 | label: MINE; group/role: FG_AGT_RIVAL1 / 0; secondary groups: CONT_005, none; waypoint: Waypoint 4 (tag 2, 8 point(s)), starting point 0, arrival event value 131072 |
