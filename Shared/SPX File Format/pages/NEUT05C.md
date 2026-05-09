# Tachyon: The Fringe NEUT05C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT05C.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 4 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 5 |
| Entities | 15 |
| Events | 14 |
| Waypoints | 5 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Hvy_Freighter`, `1: Bora_Light_Freighter`, `2: Medical_Frigate`, `3: Star_Patrol_Capital_Ship`, `4: Star_Patrol_Enforcer` |
| Scripts | `AOBUL.SCR` |
| Scenes | None |
| Labels | `aobul` |
| Aliases | `bagel`, `bagel_1`, `bagel_2`, `oside`, `oside_1`, `oside_2`, `Will_01`, `SHIP1_HYPER`, `ohshit`, `SHIP3_HYPER`, `SHIP2_HYPER` |
| Groups | `FG_SIROCCO`, `FG_BOLT`, `FG_QUAKE`, `HURRICANE`, `GALE`, `DROMEDARY`, `CONT_002`, `FINDER`, `CONT_030`, `TRAVELER`, `CONT_028`, `BOLD`, `CONT_004` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Variable comparison: subject variable group 21, variable 2, op 0, value 1

**Action**

- Object spawn/action: Medical_Frigate (object 11, id 1365), subtype 3

### Event 1

**Trigger**

- Variable comparison: subject variable group 21, variable 3, op 0, value 1

**Action**

- Object spawn/action: Bora_Hvy_Freighter (object 14, id 86), subtype 3

### Event 2

**Trigger**

- Variable comparison: subject variable group 21, variable 4, op 0, value 1

**Action**

- Object spawn/action: Bora_Hvy_Freighter (object 13, id 77), subtype 3

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Gate state/action: param 7, subtype 2, param 0
- Object spawn/action: Star_Patrol_Capital_Ship (object 9, id 771), subtype 3
- Object spawn/action: Star_Patrol_Capital_Ship (object 10, id 784), subtype 5
- Gate state/action: param 6, subtype 3, param 0
- Play dialog: AOBUL.SCR, line/variant 14
- Show/update HUD contact: contact/list 0, subtype 9, param 19
- Show/update HUD contact: contact/list 0, subtype 9, param 22
- Show/update HUD contact: contact/list 0, subtype 9, param 23

### Event 4

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 14

**Action**

- Object spawn/action: Medical_Frigate (object 11, id 1365), subtype 4
- Object spawn/action: Bora_Hvy_Freighter (object 13, id 77), subtype 4
- Object spawn/action: Bora_Hvy_Freighter (object 14, id 86), subtype 4
- Gate state/action: param 6, subtype 2, param 0

### Event 5

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 192, subtype 3, param 6
- Group/spawn-list action: spawn list/group 141, subtype 3, param 6

### Event 6

**Trigger**

- Object event: subject Medical_Frigate (object 11, id 1365), op 8, value 0

**Action**

- Set/add variable: variable group 21, variable 5, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 19

### Event 7

**Trigger**

- Object event: subject Bora_Hvy_Freighter (object 13, id 77), op 8, value 0

**Action**

- Set/add variable: variable group 21, variable 6, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 22

### Event 8

**Trigger**

- Object event: subject Bora_Hvy_Freighter (object 14, id 86), op 8, value 0

**Action**

- Set/add variable: variable group 21, variable 7, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 23

### Event 9

**Trigger**

- Object event: subject Bora_Light_Freighter (object 12, id 1366), op 10, value 0

**Action**

- Play dialog: AOBUL.SCR, line/variant 16
- Object spawn/action: Bora_Light_Freighter (object 12, id 1366), subtype 5

### Event 10

**Trigger**

- Object event: subject Bora_Light_Freighter (object 12, id 1366), op 10, value 0

**Action**

- Group/spawn-list action: spawn list/group 141, subtype 4, param 9
- Group/spawn-list action: spawn list/group 192, subtype 4, param 9
- Group/spawn-list action: spawn list/group 121, subtype 4, param 9
- Object spawn/action: Star_Patrol_Capital_Ship (object 9, id 771), subtype 8, param 9
- Object spawn/action: id 858, subtype 8, param 9
- Object spawn/action: Star_Patrol_Capital_Ship (object 10, id 784), subtype 8, param 9

### Event 11

**Trigger**

- Variable comparison: subject variable group 21, variable 33, op 1, value 1

**Action**

- Object spawn/action: Bora_Light_Freighter (object 12, id 1366), subtype 3

### Event 12

**Trigger**

- Object event: subject Bora_Light_Freighter (object 12, id 1366), op 8, value 0

**Action**

- Set/add variable: variable group 21, variable 34, subtype 0, value 1

### Event 13

**Trigger**

- Object event: subject Bora_Hvy_Freighter (object 13, id 77), op 14, value 9 (join 2)
- Object event: subject Bora_Hvy_Freighter (object 14, id 86), op 14, value 9 (join 2)
- Object event: subject Medical_Frigate (object 11, id 1365), op 14, value 4 (join 2)

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 34
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 13, variable 410, subtype 0, value 1
- Set/add variable: variable group 13, variable 411, subtype 0, value 1

## Waypoints

### Waypoint 0

- Tag: `201`
- Members: `Bora_Light_Freighter (object 12, id 1366, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (186.56, 245.37, -545.75) | on arrival activate current object (raw param -1 ignored) |
| 1 | (642.51, 245.37, 690.21) | None |
| 2 | (906.96, 245.37, 1006.61) | None |
| 3 | (578.68, 245.37, 2212.89) | on arrival action 1, param -1 |

### Waypoint 1

- Tag: `21`
- Members: `Star_Patrol_Capital_Ship (object 10, id 784, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-407.02, 317.84, 1731.20) | None |
| 1 | (64.78, 317.84, 2072.74) | on arrival action 1, param -1 |

### Waypoint 2

- Tag: `6`
- Members: `Star_Patrol_Enforcer (object 0, id 797, starts at point 0)`, `Star_Patrol_Enforcer (object 1, id 798, starts at point 0)`, `Star_Patrol_Enforcer (object 2, id 799, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (286.63, 246.24, 129.94) | None |
| 1 | (237.65, 246.24, 819.44) | None |
| 2 | (681.73, 249.13, 1309.91) | None |
| 3 | (1123.27, 246.24, 714.54) | None |
| 4 | (683.17, 249.13, 345.70) | on arrival redirect to Waypoint 2 (tag 6), point 0 |

### Waypoint 3

- Tag: `3`
- Members: `Star_Patrol_Enforcer (object 6, id 803, starts at point 0)`, `Star_Patrol_Enforcer (object 7, id 804, starts at point 0)`, `Star_Patrol_Enforcer (object 8, id 805, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-442.99, 31.73, 2706.54) | None |
| 1 | (-671.29, 31.73, 3171.75) | None |
| 2 | (-1056.54, 31.73, 2896.07) | None |
| 3 | (-901.43, 31.73, 2258.00) | on arrival redirect to Waypoint 3 (tag 3), point 0 |

### Waypoint 4

- Tag: `2`
- Members: `Star_Patrol_Enforcer (object 3, id 800, starts at point -1)`, `Star_Patrol_Enforcer (object 4, id 801, starts at point 0)`, `Star_Patrol_Enforcer (object 5, id 802, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1518.25, 414.73, 1942.49) | None |
| 1 | (1989.11, 414.73, 2356.01) | None |
| 2 | (2273.41, 414.73, 1421.03) | None |
| 3 | (2116.46, 414.73, 783.52) | None |
| 4 | (1602.79, 414.73, 955.83) | on arrival redirect to Waypoint 4 (tag 2), point 0 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Star_Patrol_Enforcer` | 797 | Interactive | 217.54,246.24,-275.03 | 511,0,0 | group/role: FG_SIROCCO / 0; alias: bagel; waypoint: Waypoint 2 (tag 6, 5 point(s)), starting point 0, arrival event value 393216 |
| 1 | `Star_Patrol_Enforcer` | 798 | Interactive | 354.54,246.24,-296.58 | 511,0,0 | group/role: FG_SIROCCO / 0; alias: bagel_1; waypoint: Waypoint 2 (tag 6, 5 point(s)), starting point 0, arrival event value 393216 |
| 2 | `Star_Patrol_Enforcer` | 799 | Interactive | 260.80,246.24,-388.13 | 511,0,0 | group/role: FG_SIROCCO / 0; alias: bagel_2; waypoint: Waypoint 2 (tag 6, 5 point(s)), starting point 0, arrival event value 393216 |
| 3 | `Star_Patrol_Enforcer` | 800 | Interactive | 1599.84,414.73,1641.99 | 0,0,0 | group/role: FG_BOLT / 0; waypoint: Waypoint 4 (tag 2, 5 point(s)), starting point -1 |
| 4 | `Star_Patrol_Enforcer` | 801 | Interactive | 1590.22,414.73,1512.73 | 0,0,0 | group/role: FG_BOLT / 0; waypoint: Waypoint 4 (tag 2, 5 point(s)), starting point 0, arrival event value 131072 |
| 5 | `Star_Patrol_Enforcer` | 802 | Interactive | 1664.73,414.73,1434.64 | 0,0,0 | group/role: FG_BOLT / 0; waypoint: Waypoint 4 (tag 2, 5 point(s)), starting point 0, arrival event value 131072 |
| 6 | `Star_Patrol_Enforcer` | 803 | Interactive | -448.33,31.73,2491.02 | 0,0,0 | group/role: FG_QUAKE / 0; alias: oside; waypoint: Waypoint 3 (tag 3, 4 point(s)), starting point 0, arrival event value 196608 |
| 7 | `Star_Patrol_Enforcer` | 804 | Interactive | -510.85,31.73,2366.32 | 0,0,0 | group/role: FG_QUAKE / 0; alias: oside_1; waypoint: Waypoint 3 (tag 3, 4 point(s)), starting point 0, arrival event value 196608 |
| 8 | `Star_Patrol_Enforcer` | 805 | Interactive | -410.22,31.73,2356.07 | 0,0,0 | group/role: FG_QUAKE / 0; alias: oside_2; waypoint: Waypoint 3 (tag 3, 4 point(s)), starting point 0, arrival event value 196608 |
| 9 | `Star_Patrol_Capital_Ship` | 771 | Interactive | 1420.74,303.35,861.13 | 465,0,0 | secondary groups: none, HURRICANE |
| 10 | `Star_Patrol_Capital_Ship` | 784 | Interactive | -1060.61,233.57,1104.79 | 63,0,0 | secondary groups: none, GALE; waypoint: Waypoint 1 (tag 21, 2 point(s)), starting point 0, arrival event value 1376256 |
| 11 | `Medical_Frigate` | 1365 | Interactive | 678.11,244.55,749.39 | 0,0,0 | alias: SHIP1_HYPER; secondary groups: CONT_002, DROMEDARY |
| 12 | `Bora_Light_Freighter` | 1366 | Interactive | 266.45,125.62,-1000.66 | 0,0,0 | alias: ohshit; secondary groups: CONT_030, FINDER; waypoint: Waypoint 0 (tag 201, 4 point(s)), starting point -1 |
| 13 | `Bora_Hvy_Freighter` | 77 | Interactive | 485.37,246.24,753.71 | 1,0,0 | alias: SHIP3_HYPER; secondary groups: CONT_028, TRAVELER |
| 14 | `Bora_Hvy_Freighter` | 86 | Interactive | 890.29,246.24,752.55 | 508,0,0 | alias: SHIP2_HYPER; secondary groups: CONT_004, BOLD |
