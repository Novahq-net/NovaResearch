# Tachyon: The Fringe EARTH06B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH06B.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `(none)` |
| Region | 0 |
| Sector ID | 5 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 12 |
| Events | 16 |
| Waypoints | 5 |
| Child Sectors | 0 |
| Scripts | 4 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Luxury_Liner`, `1: Red_Pirate_Shrike`, `2: Pirate_Mine_HvyLaser`, `3: Star_Patrol_Enforcer` |
| Scripts | `PLAYER.SCR`, `pirb.scr`, `frtb.scr`, `STPF.SCR` |
| Scenes | None |
| Labels | `STPF`, `ARI2`, `bfne_08`, `bfne_01`, `PIRA`, `PIRB`, `MINE`, `FRTB` |
| Aliases | None |
| Groups | `FG_AGT5`, `FG_BORA7`, `CONT_034`, `FG_GALSPAN8`, `FG_GALSPAN7`, `TRIMURTI`, `CONT_032` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 44
- Show/update HUD contact: contact/list 0, subtype 1, param 25
- Set/add variable: variable group 21, variable 24, subtype 0, value 1

### Event 1

**Trigger**

- Group/spawn-list event: subject 25, op 0, value 0
- Variable comparison: subject variable group 21, variable 21, op 1, value 0

**Action**

- Group/spawn-list action: spawn list/group 40, subtype 1, param 2

### Event 2

**Trigger**

- Group/spawn-list event: subject 25, op 0, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 29, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Hide/remove HUD contact: contact/list 0, subtype 1, param 25
- Set/add variable: variable group 12, variable 11, subtype 0, value 1
- Set/add variable: variable group 12, variable 12, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 12, param 30

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 29, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 45
- Set runtime trigger variable: variable group 20, variable 29, subtype 1, value 0

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 29, op 1, value 1
- Variable comparison: subject variable group 21, variable 21, op 1, value 0

**Action**

- Group/spawn-list action: spawn list/group 39, subtype 1, param 2

### Event 5

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 45
- Variable comparison: subject variable group 21, variable 21, op 1, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 29, subtype 0, value 0

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 29, op 0, value 3
- Variable comparison: subject variable group 21, variable 21, op 1, value 0

**Action**

- Play dialog: pirb.scr, line/variant 0
- Set runtime trigger variable: variable group 20, variable 29, subtype 1, value 0

### Event 7

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 0 (join 1)
- Object event: subject Luxury_Liner (object 11, id 2690), op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 29, subtype 0, value 0

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 29, op 1, value 5
- Variable comparison: subject variable group 21, variable 21, op 1, value 0

**Action**

- Play dialog: frtb.scr, line/variant 0

### Event 9

**Trigger**

- Variable comparison: subject variable group 20, variable 29, op 1, value 80
- Variable comparison: subject variable group 21, variable 21, op 1, value 0

**Action**

- Group/spawn-list action: spawn list/group 5, subtype 1, param 2
- Play dialog: STPF.SCR, line/variant 0

### Event 10

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Variable comparison: subject variable group 21, variable 21, op 1, value 0

**Action**

- Group/spawn-list action: spawn list/group 5, subtype 1, param 2
- Play dialog: STPF.SCR, line/variant 1
- Set runtime trigger variable: variable group 20, variable 31, subtype 0, value 0
- Set runtime trigger variable: variable group 20, variable 29, subtype 1, value 0

### Event 11

**Trigger**

- Variable comparison: subject variable group 20, variable 31, op 1, value 30

**Action**

- Object spawn/action: Luxury_Liner (object 11, id 2690), subtype 4
- Group/spawn-list action: spawn list/group 5, subtype 3, param 2

### Event 12

**Trigger**

- Group/spawn-list event: subject 39, op 0, value 0
- Group/spawn-list event: subject 40, op 0, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 0, value 1

### Event 13

**Trigger**

- Object event: subject Luxury_Liner (object 11, id 2690), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 21, subtype 0, value 1

### Event 14

**Trigger**

- Object event: subject Red_Pirate_Shrike (object 8, id 2784), op 0, value 0 (join 2; flags 2)
- Object event: subject 2785, op 0, value 0 (join 2; flags 2)
- Object event: subject Red_Pirate_Shrike (object 9, id 2787), op 0, value 0 (join 2; flags 2)
- Object event: subject 2788, op 0, value 0 (join 2; flags 2)
- Object event: subject Red_Pirate_Shrike (object 10, id 2828), op 0, value 0 (join 2; flags 2)

**Action**

- Set/add variable: variable group 21, variable 22, subtype 0, value 1

### Event 15

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Variable comparison: subject variable group 21, variable 21, op 1, value 0
- Variable comparison: subject variable group 21, variable 22, op 1, value 1
- Variable comparison: subject variable group 21, variable 23, op 1, value 0

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 1000

## Waypoints

### Waypoint 0

- Tag: `151`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-68.80, 0.00, 2141.74) | on arrival action 1, param -1 |

### Waypoint 1

- Tag: `12`
- Members: `Red_Pirate_Shrike (object 9, id 2787, starts at point 0)`, `Red_Pirate_Shrike (object 10, id 2828, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (440.96, 0.00, 4107.69) | None |
| 1 | (-2004.92, 0.00, 1515.63) | None |
| 2 | (-1292.43, 0.00, 623.43) | None |
| 3 | (-319.97, 0.00, 509.10) | None |
| 4 | (283.43, 0.00, 483.69) | None |
| 5 | (1048.51, 0.00, 1595.29) | None |
| 6 | (931.15, 0.00, 2128.84) | None |
| 7 | (164.23, 0.00, 2704.14) | on arrival redirect to Waypoint 1 (tag 12), point 0 |

### Waypoint 2

- Tag: `8`
- Members: `Star_Patrol_Enforcer (object 0, id 2711, starts at point 0)`, `Star_Patrol_Enforcer (object 1, id 2712, starts at point 0)`, `Star_Patrol_Enforcer (object 2, id 2713, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (14.34, 0.00, 3990.77) | None |
| 1 | (-1519.47, 0.00, 458.87) | None |
| 2 | (-218.65, 0.00, 422.11) | None |
| 3 | (596.75, 0.00, 909.99) | None |
| 4 | (1107.83, 0.00, 2009.37) | None |
| 5 | (68.42, 0.00, 2894.53) | on arrival redirect to Waypoint 2 (tag 8), point 1 |

### Waypoint 3

- Tag: `7`
- Members: `Luxury_Liner (object 11, id 2690, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1687.73, 90.00, 4376.82) | None |
| 1 | (-445.13, 0.00, 4157.64) | None |
| 2 | (-1907.08, 0.00, 1836.61) | None |
| 3 | (-546.57, 0.00, 73.36) | None |
| 4 | (916.38, 0.00, 521.92) | None |
| 5 | (1518.72, 0.00, 1719.99) | on arrival activate current object (raw param -1 ignored) |
| 6 | (730.32, 0.00, 3787.32) | on arrival redirect to Waypoint 3 (tag 7), point 2 |

### Waypoint 4

- Tag: `11`
- Members: `Red_Pirate_Shrike (object 8, id 2784, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (278.18, -1210.00, 4176.62) | None |
| 1 | (-1978.09, 0.00, 1661.07) | None |
| 2 | (-566.34, 0.00, 840.83) | None |
| 3 | (636.23, 0.00, 731.73) | None |
| 4 | (904.54, 0.00, 2155.17) | on arrival redirect to waypoint tag 5, point 0 |

## Spawn Lists

### Spawn List 0

- ID: `40`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | Luxury_Liner (object 11, id 2690) | None |
| 1 | 0 | none | None |

### Spawn List 1

- ID: `39`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Luxury_Liner (object 11, id 2690) | None |
| 1 | 9 | none | None |

### Spawn List 2

- ID: `25`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Star_Patrol_Enforcer` | 2711 | Interactive | -592.54,0.00,1192.95 | 100,0,0 | label: STPF; group/role: FG_AGT5 / 1; waypoint: Waypoint 2 (tag 8, 6 point(s)), starting point 0, arrival event value 524288 |
| 1 | `Star_Patrol_Enforcer` | 2712 | Interactive | -587.23,0.00,1144.50 | 100,0,0 | group/role: FG_AGT5 / 2; waypoint: Waypoint 2 (tag 8, 6 point(s)), starting point 0, arrival event value 524288 |
| 2 | `Star_Patrol_Enforcer` | 2713 | Interactive | -557.70,0.00,1113.44 | 100,0,0 | group/role: FG_AGT5 / 3; waypoint: Waypoint 2 (tag 8, 6 point(s)), starting point 0, arrival event value 524288 |
| 3 | `Pirate_Mine_HvyLaser` | 2802 | Interactive | 999.81,-957.30,4932.81 | 457,142,272 | group/role: FG_BORA7 / 0; secondary groups: CONT_034, none |
| 4 | `Pirate_Mine_HvyLaser` | 2818 | Interactive | 1705.46,-957.30,3905.14 | 457,142,272 | group/role: FG_BORA7 / 0; secondary groups: CONT_034, none |
| 5 | `Pirate_Mine_HvyLaser` | 2779 | Interactive | 622.40,1441.45,3325.47 | 505,6,124 | group/role: FG_BORA7 / 0; secondary groups: CONT_034, none |
| 6 | `Pirate_Mine_HvyLaser` | 2803 | Interactive | -891.78,-957.30,3918.96 | 457,142,272 | group/role: FG_BORA7 / 0; secondary groups: CONT_034, none |
| 7 | `Pirate_Mine_HvyLaser` | 2816 | Interactive | -85.04,-957.30,4553.58 | 457,142,272 | group/role: FG_BORA7 / 0; secondary groups: CONT_034, none |
| 8 | `Red_Pirate_Shrike` | 2784 | Interactive | -1012.92,127.60,1324.06 | 0,0,0 | label: PIRA; group/role: FG_GALSPAN8 / 0; waypoint: Waypoint 4 (tag 11, 5 point(s)), starting point 0, arrival event value 720896 |
| 9 | `Red_Pirate_Shrike` | 2787 | Interactive | -992.16,0.00,1233.19 | 0,0,0 | label: PIRB; group/role: FG_GALSPAN7 / 0; waypoint: Waypoint 1 (tag 12, 8 point(s)), starting point 0, arrival event value 786432 |
| 10 | `Red_Pirate_Shrike` | 2828 | Interactive | -1019.12,0.00,1235.63 | 0,0,0 | group/role: FG_GALSPAN7 / 0; waypoint: Waypoint 1 (tag 12, 8 point(s)), starting point 0, arrival event value 786432 |
| 11 | `Luxury_Liner` | 2690 | Interactive | 2251.50,73.00,4471.58 | 371,0,0 | label: FRTB; secondary groups: CONT_032, TRIMURTI; waypoint: Waypoint 3 (tag 7, 7 point(s)), starting point 0, arrival event value 458752 |
