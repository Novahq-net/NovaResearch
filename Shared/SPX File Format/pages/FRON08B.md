# Tachyon: The Fringe FRON08B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON08B.SPX` |
| Sector | `QUAD_08` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 7 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 15 |
| Events | 18 |
| Waypoints | 4 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Hajod_Fighter_2`, `1: Hajod_Fighter_1`, `2: Shuttle_Small` |
| Scripts | `PLAYER.SCR`, `ESCSL.SCR` |
| Scenes | None |
| Labels | `bfne_03`, `bfne_01`, `HSLAV`, `BFGE_01`, `CHAPEL` |
| Aliases | `Jerome01`, `Jerome02`, `Jerome03`, `Jerome04`, `Jerome05`, `Jerome06`, `bc05_2`, `bc05_1`, `bc05_4`, `bc05_5`, `BC05_Sistine_Chapel` |
| Groups | `FG_TYRANT`, `FG_DISCIPLINE`, `FG_PUNISHER`, `FG_DESPOT` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 36
- Set runtime trigger variable: variable group 20, variable 29, subtype 0, value 0
- Object spawn/action: Shuttle_Small (object 2, id 791), subtype 14

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 29, op 1, value 3

**Action**

- Play dialog: PLAYER.SCR, line/variant 130

### Event 2

**Trigger**

- Group/spawn-list event: subject 132, op 2, value 393216 (Waypoint 3 (tag 6), point 0) (join 2)
- Group/spawn-list event: subject 132, op 0, value 0 (join 2)
- Group/spawn-list event: subject 132, op 4, value 0 (join 2; flags 2)

**Action**

- Group/spawn-list action: spawn list/group 132, subtype 4, param 9
- Object spawn/action: id 996, subtype 8, param 9
- Show/update HUD contact: contact/list 0, subtype 1, param 132
- Hide/remove HUD contact: contact/list 0, subtype 9, param 36
- Object spawn/action: Shuttle_Small (object 2, id 791), subtype 15

### Event 3

**Trigger**

- Group/spawn-list event: subject 132, op 4, value 0 (join 2; flags 2)
- Object event: subject Hajod_Fighter_1 (object 14, id 1064), op 2, value 0 (join 2)
- Object event: subject Hajod_Fighter_1 (object 6, id 797), op 2, value 0 (join 2)
- Object event: subject Hajod_Fighter_1 (object 7, id 798), op 2, value 0 (join 2)
- Object event: subject Hajod_Fighter_1 (object 8, id 799), op 2, value 0 (join 2)

**Action**

- Group/spawn-list action: spawn list/group 86, subtype 1, param 996
- Show/update HUD contact: contact/list 0, subtype 1, param 86

### Event 4

**Trigger**

- Group/spawn-list event: subject 86, op 0, value 0
- Group/spawn-list event: subject 132, op 0, value 0

**Action**

- Group/spawn-list action: spawn list/group 131, subtype 7
- Group/spawn-list action: spawn list/group 131, subtype 4, param 12
- Show/update HUD contact: contact/list 0, subtype 7, param 131
- Play dialog: ESCSL.SCR, line/variant 1
- Object spawn/action: Shuttle_Small (object 2, id 791), subtype 14

### Event 5

**Trigger**

- Group/spawn-list event: subject 131, op 2, value 262145 (Waypoint 2 (tag 4), point 1)

**Action**

- Group/spawn-list action: spawn list/group 87, subtype 1, param 996
- Hide/remove HUD contact: contact/list 0, subtype 7, param 131
- Show/update HUD contact: contact/list 0, subtype 3, param 131
- Play dialog: PLAYER.SCR, line/variant 133

### Event 6

**Trigger**

- Object event: subject Shuttle_Small (object 0, id 789), op 7, value 0 (join 2)
- Object event: subject Shuttle_Small (object 1, id 790), op 7, value 0 (join 2)
- Object event: subject Shuttle_Small (object 2, id 791), op 7, value 0 (join 2)
- Object event: subject Shuttle_Small (object 3, id 792), op 7, value 0 (join 2)
- Object event: subject Shuttle_Small (object 4, id 793), op 7, value 0 (join 2)
- Object event: subject Shuttle_Small (object 5, id 794), op 7, value 0 (join 2)

**Action**

- Mission objective/state: param 262144, subtype 0, param 0
- Hide/remove HUD contact: contact/list 0, subtype 3, param 131

### Event 7

**Trigger**

- Object event: subject Shuttle_Small (object 0, id 789), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 8

**Trigger**

- Object event: subject Shuttle_Small (object 1, id 790), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 9

**Trigger**

- Object event: subject Shuttle_Small (object 2, id 791), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 10

**Trigger**

- Object event: subject Shuttle_Small (object 3, id 792), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 11

**Trigger**

- Object event: subject Shuttle_Small (object 4, id 793), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 12

**Trigger**

- Object event: subject Shuttle_Small (object 5, id 794), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 13

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 2, value 2

**Action**

- Play dialog: PLAYER.SCR, line/variant 136
- Mark/flash contact: contact/list 0, subtype 3, param 131
- Show/update HUD contact: contact/list 0, subtype 11, param 38
- Set/add variable: variable group 16, variable 428, subtype 0, value 1
- Set/add variable: variable group 16, variable 429, subtype 0, value 1

### Event 14

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Play dialog: ESCSL.SCR, line/variant 3

### Event 15

**Trigger**

- Object event: subject Hajod_Fighter_2 (object 11, id 800), op 2, value 0 (join 2)
- Object event: subject Hajod_Fighter_2 (object 12, id 801), op 2, value 0 (join 2)
- Object event: subject Hajod_Fighter_2 (object 13, id 802), op 2, value 0 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 185

### Event 16

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 50 (flags 1)

**Action**

- Play dialog: PLAYER.SCR, line/variant 189

### Event 17

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 189

**Action**

- Play dialog: PLAYER.SCR, line/variant 172

## Waypoints

### Waypoint 0

- Tag: `7`
- Members: `Hajod_Fighter_2 (object 9, id 803, starts at point 0)`, `Hajod_Fighter_2 (object 10, id 804, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (505.89, 52.02, 523.22) | None |
| 1 | (-28.18, 93.22, 260.09) | None |
| 2 | (-886.34, 277.39, -300.83) | None |

### Waypoint 1

- Tag: `5`
- Members: `Hajod_Fighter_2 (object 11, id 800, starts at point 0)`, `Hajod_Fighter_2 (object 12, id 801, starts at point 0)`, `Hajod_Fighter_2 (object 13, id 802, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (516.47, 52.02, 497.98) | None |
| 1 | (-883.26, 293.27, -520.10) | None |

### Waypoint 2

- Tag: `4`
- Members: `Shuttle_Small (object 0, id 789, starts at point 0)`, `Shuttle_Small (object 1, id 790, starts at point 0)`, `Shuttle_Small (object 2, id 791, starts at point 0)`, `Shuttle_Small (object 3, id 792, starts at point 0)`, `Shuttle_Small (object 4, id 793, starts at point 0)`, `Shuttle_Small (object 5, id 794, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-139.78, 153.88, -1864.47) | None |
| 1 | (-379.98, 233.07, -1658.22) | None |
| 2 | (-1152.64, 295.71, -191.67) | None |
| 3 | (-1620.14, 293.74, 741.60) | on arrival play dialog/script or enter gate, param 1 |

### Waypoint 3

- Tag: `6`
- Members: `Hajod_Fighter_1 (object 6, id 797, starts at point 0)`, `Hajod_Fighter_1 (object 7, id 798, starts at point 0)`, `Hajod_Fighter_1 (object 8, id 799, starts at point 0)`, `Hajod_Fighter_1 (object 14, id 1064, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (879.41, 232.86, -2073.60) | None |
| 1 | (-903.91, 431.18, -859.49) | on arrival activate current object (raw param -1 ignored) |

## Spawn Lists

### Spawn List 0

- ID: `132`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 5 | id 131 | None |
| 1 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Shuttle_Small` | 789 | Interactive | -18.52,36.92,-1595.18 | 314,0,0 | group/role: FG_TYRANT / 0; alias: Jerome01; waypoint: Waypoint 2 (tag 4, 4 point(s)), starting point 0, arrival event value 262144 |
| 1 | `Shuttle_Small` | 790 | Interactive | 16.61,36.92,-1623.67 | 311,0,0 | group/role: FG_TYRANT / 0; alias: Jerome02; waypoint: Waypoint 2 (tag 4, 4 point(s)), starting point 0, arrival event value 262144 |
| 2 | `Shuttle_Small` | 791 | Interactive | 24.61,36.92,-1542.90 | 319,0,0 | group/role: FG_TYRANT / 0; alias: Jerome03; waypoint: Waypoint 2 (tag 4, 4 point(s)), starting point 0, arrival event value 262144 |
| 3 | `Shuttle_Small` | 792 | Interactive | 60.47,36.92,-1570.53 | 314,0,0 | group/role: FG_TYRANT / 0; alias: Jerome04; waypoint: Waypoint 2 (tag 4, 4 point(s)), starting point 0, arrival event value 262144 |
| 4 | `Shuttle_Small` | 793 | Interactive | 71.32,36.92,-1489.71 | 314,0,0 | group/role: FG_TYRANT / 0; alias: Jerome05; waypoint: Waypoint 2 (tag 4, 4 point(s)), starting point 0, arrival event value 262144 |
| 5 | `Shuttle_Small` | 794 | Interactive | 104.13,36.92,-1518.36 | 316,0,0 | group/role: FG_TYRANT / 0; alias: Jerome06; waypoint: Waypoint 2 (tag 4, 4 point(s)), starting point 0, arrival event value 262144 |
| 6 | `Hajod_Fighter_1` | 797 | Interactive | 1841.83,351.38,-1303.15 | 326,475,0 | label: bfne_03; group/role: FG_DISCIPLINE / 0; waypoint: Waypoint 3 (tag 6, 2 point(s)), starting point 0, arrival event value 393216 |
| 7 | `Hajod_Fighter_1` | 798 | Interactive | 1791.45,350.59,-1311.60 | 326,475,0 | group/role: FG_DISCIPLINE / 0; waypoint: Waypoint 3 (tag 6, 2 point(s)), starting point 0, arrival event value 393216 |
| 8 | `Hajod_Fighter_1` | 799 | Interactive | 1835.18,348.12,-1245.81 | 329,475,0 | label: bfne_03; group/role: FG_DISCIPLINE / 0; waypoint: Waypoint 3 (tag 6, 2 point(s)), starting point 0, arrival event value 393216 |
| 9 | `Hajod_Fighter_2` | 803 | Interactive | 853.95,0.00,669.34 | 311,0,0 | group/role: FG_PUNISHER / 0; waypoint: Waypoint 0 (tag 7, 3 point(s)), starting point 0, arrival event value 458752 |
| 10 | `Hajod_Fighter_2` | 804 | Interactive | 929.21,0.00,682.33 | 311,0,0 | label: bfne_01; group/role: FG_PUNISHER / 0; waypoint: Waypoint 0 (tag 7, 3 point(s)), starting point 0, arrival event value 458752 |
| 11 | `Hajod_Fighter_2` | 800 | Interactive | 858.80,0.00,756.47 | 311,0,0 | label: bfne_01; group/role: FG_DESPOT / 0; waypoint: Waypoint 1 (tag 5, 2 point(s)), starting point 0, arrival event value 327680 |
| 12 | `Hajod_Fighter_2` | 801 | Interactive | 923.31,0.00,769.45 | 311,0,0 | group/role: FG_DESPOT / 0; waypoint: Waypoint 1 (tag 5, 2 point(s)), starting point 0, arrival event value 327680 |
| 13 | `Hajod_Fighter_2` | 802 | Interactive | 998.58,0.00,769.45 | 311,0,0 | group/role: FG_DESPOT / 0; waypoint: Waypoint 1 (tag 5, 2 point(s)), starting point 0, arrival event value 327680 |
| 14 | `Hajod_Fighter_1` | 1064 | Interactive | 1899.27,351.38,-1280.26 | 325,475,0 | group/role: FG_DISCIPLINE / 0; waypoint: Waypoint 3 (tag 6, 2 point(s)), starting point 0, arrival event value 393216 |
