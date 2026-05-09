# Tachyon: The Fringe FRON09D.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON09D.SPX` |
| Sector | `QUAD_09` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 8 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 14 |
| Events | 17 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Hajod_Fighter_1` |
| Scripts | `PLAYER.SCR`, `HAJOD.SCR` |
| Scenes | None |
| Labels | `BFNE_04`, `BFNE_02`, `BFNE_07` |
| Aliases | None |
| Groups | `FG_DICTATOR`, `FG_DEUCE`, `FG_SOVEREIGN`, `FG_HELIOS` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 20, op 3, value 2

**Action**

- Show/update HUD contact: contact/list 0, subtype 1, param 195
- Show/update HUD contact: contact/list 0, subtype 1, param 257
- Play dialog: PLAYER.SCR, line/variant 99

### Event 1

**Trigger**

- Group/spawn-list event: subject 195, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 257, op 4, value 0 (flags 2)

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0
- Set/add variable: variable group 21, variable 20, subtype 0, value 1
- Play dialog: HAJOD.SCR, line/variant 20
- Object spawn/action: id 2, subtype 8, param 9

### Event 2

**Trigger**

- Object event: subject Hajod_Fighter_1 (object 4, id 145), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Hajod_Fighter_1 (object 4, id 145), subtype 7

### Event 3

**Trigger**

- Object event: subject Hajod_Fighter_1 (object 5, id 146), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Hajod_Fighter_1 (object 5, id 146), subtype 7

### Event 4

**Trigger**

- Object event: subject Hajod_Fighter_1 (object 6, id 147), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Hajod_Fighter_1 (object 6, id 147), subtype 7

### Event 5

**Trigger**

- Object event: subject Hajod_Fighter_1 (object 7, id 148), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Hajod_Fighter_1 (object 7, id 148), subtype 7

### Event 6

**Trigger**

- Object event: subject Hajod_Fighter_1 (object 2, id 80), op 0, value 0 (flags 2)
- Object event: subject Hajod_Fighter_1 (object 2, id 80), op 4, value 50

**Action**

- Object spawn/action: Hajod_Fighter_1 (object 2, id 80), subtype 7

### Event 7

**Trigger**

- Object event: subject Hajod_Fighter_1 (object 3, id 81), op 0, value 0 (flags 2)
- Object event: subject Hajod_Fighter_1 (object 3, id 81), op 4, value 50

**Action**

- Object spawn/action: Hajod_Fighter_1 (object 3, id 81), subtype 7

### Event 8

**Trigger**

- Object event: subject Hajod_Fighter_1 (object 0, id 83), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Hajod_Fighter_1 (object 0, id 83), subtype 7

### Event 9

**Trigger**

- Object event: subject Hajod_Fighter_1 (object 1, id 84), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Hajod_Fighter_1 (object 1, id 84), subtype 7

### Event 10

**Trigger**

- Group/spawn-list event: subject 195, op 1, value 50
- Group/spawn-list event: subject 257, op 1, value 50
- Sector/startup condition family: subject 1, op 0, value 20

**Action**

- Play dialog: PLAYER.SCR, line/variant 100

### Event 11

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 30

**Action**

- Group/spawn-list action: spawn list/group 195, subtype 7

### Event 12

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Group/spawn-list event: subject 195, op 0, value 0
- Group/spawn-list event: subject 257, op 0, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 101
- Set/add variable: variable group 16, variable 414, subtype 0, value 1
- Set/add variable: variable group 16, variable 415, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 12, param 37
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 21, variable 21, subtype 0, value 1
- Set/add variable: variable group 21, variable 20, subtype 0, value 0

### Event 13

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 101

**Action**

- Object spawn/action: id 121, subtype 5
- Object spawn/action: id 22, subtype 5
- Object spawn/action: id 26, subtype 5
- Object spawn/action: id 27, subtype 5
- Object spawn/action: id 28, subtype 5
- Object spawn/action: id 29, subtype 5
- Object spawn/action: id 30, subtype 5

### Event 14

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 101

**Action**

- Object spawn/action: id 121, subtype 8, param 9
- Object spawn/action: id 22, subtype 8, param 9
- Object spawn/action: id 26, subtype 8, param 9
- Object spawn/action: id 27, subtype 8, param 9
- Object spawn/action: id 28, subtype 8, param 9
- Object spawn/action: id 29, subtype 8, param 9
- Object spawn/action: id 30, subtype 8, param 9

### Event 15

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 101

**Action**

- Group/spawn-list action: spawn list/group 194, subtype 1, param 1
- Play dialog: HAJOD.SCR, line/variant 22

### Event 16

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 2

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 38
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Group/spawn-list action: spawn list/group 194, subtype 1, param 1
- Object spawn/action: id 121, subtype 5
- Object spawn/action: id 121, subtype 8, param 9
- Object spawn/action: id 26, subtype 5
- Object spawn/action: id 26, subtype 8, param 9

## Waypoints

### Waypoint 0

- Tag: `254`
- Members: `Hajod_Fighter_1 (object 12, id 204, starts at point -1)`, `Hajod_Fighter_1 (object 13, id 205, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (15348.03, 0.00, 7229.12) | None |
| 1 | (16637.02, 0.00, 3466.23) | None |
| 2 | (18025.15, 0.00, -1909.32) | None |
| 3 | (19016.68, 0.00, -12230.38) | None |
| 4 | (26651.44, 0.00, -8790.02) | None |

### Waypoint 1

- Tag: `252`
- Members: `Hajod_Fighter_1 (object 0, id 83, starts at point 0)`, `Hajod_Fighter_1 (object 1, id 84, starts at point 0)`, `Hajod_Fighter_1 (object 2, id 80, starts at point 0)`, `Hajod_Fighter_1 (object 3, id 81, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-4415.02, 95.01, -822.06) | None |
| 1 | (-2835.19, 0.00, -546.83) | None |
| 2 | (-2354.52, -2192.42, -293.30) | None |
| 3 | (-1377.35, 0.00, -67.03) | None |
| 4 | (-1790.17, -1464.94, 995.75) | None |
| 5 | (-2320.29, -1464.94, 1955.35) | None |
| 6 | (-4116.82, -1464.94, 1507.53) | None |
| 7 | (-4646.44, 0.00, 716.64) | None |
| 8 | (-2804.59, -1464.94, 923.63) | None |
| 9 | (-2818.81, 0.00, 388.63) | None |
| 10 | (-2117.26, -2192.42, -1436.98) | None |
| 11 | (-1489.55, -2192.42, -1060.79) | None |

### Waypoint 2

- Tag: `251`
- Members: `Hajod_Fighter_1 (object 8, id 160, starts at point 0)`, `Hajod_Fighter_1 (object 9, id 161, starts at point 0)`, `Hajod_Fighter_1 (object 10, id 162, starts at point 0)`, `Hajod_Fighter_1 (object 11, id 163, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-844.01, -97.00, 826.49) | None |
| 1 | (-832.88, -90.05, 208.88) | None |
| 2 | (-1657.27, 0.00, 1476.88) | None |
| 3 | (-2113.63, 0.00, -115.01) | None |

## Spawn Lists

### Spawn List 0

- ID: `195`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 1

- ID: `194`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hajod_Fighter_1` | 83 | Interactive | -3723.60,-270.98,-1123.88 | 128,0,0 | label: BFNE_02; group/role: FG_DICTATOR / 0; waypoint: Waypoint 1 (tag 252, 12 point(s)), starting point 0, arrival event value 16515072 |
| 1 | `Hajod_Fighter_1` | 84 | Interactive | -3713.48,-270.98,-1211.83 | 128,0,0 | group/role: FG_DICTATOR / 0; waypoint: Waypoint 1 (tag 252, 12 point(s)), starting point 0, arrival event value 16515072 |
| 2 | `Hajod_Fighter_1` | 80 | Interactive | -4686.30,-270.77,-711.41 | 384,0,0 | label: BFNE_02; group/role: FG_DICTATOR / 0; waypoint: Waypoint 1 (tag 252, 12 point(s)), starting point 0, arrival event value 16515072 |
| 3 | `Hajod_Fighter_1` | 81 | Interactive | -4663.53,-270.77,-815.84 | 384,0,0 | group/role: FG_DICTATOR / 0; waypoint: Waypoint 1 (tag 252, 12 point(s)), starting point 0, arrival event value 16515072 |
| 4 | `Hajod_Fighter_1` | 145 | Interactive | -4733.83,-272.17,-868.83 | 384,0,0 | group/role: FG_DEUCE / 0 |
| 5 | `Hajod_Fighter_1` | 146 | Interactive | -4733.83,-269.89,-789.22 | 384,0,0 | group/role: FG_DEUCE / 0 |
| 6 | `Hajod_Fighter_1` | 147 | Interactive | -3715.79,-269.39,-1269.32 | 128,0,0 | group/role: FG_DEUCE / 0 |
| 7 | `Hajod_Fighter_1` | 148 | Interactive | -3741.58,-269.39,-1070.11 | 128,0,0 | group/role: FG_DEUCE / 0 |
| 8 | `Hajod_Fighter_1` | 160 | Interactive | -13382.39,393.98,26.17 | 0,0,0 | label: BFNE_07; group/role: FG_SOVEREIGN / 0; waypoint: Waypoint 2 (tag 251, 4 point(s)), starting point 0, arrival event value 16449536 |
| 9 | `Hajod_Fighter_1` | 161 | Interactive | -13387.68,393.98,166.94 | 0,0,0 | group/role: FG_SOVEREIGN / 0; waypoint: Waypoint 2 (tag 251, 4 point(s)), starting point 0, arrival event value 16449536 |
| 10 | `Hajod_Fighter_1` | 162 | Interactive | -13392.96,393.98,314.89 | 0,0,0 | group/role: FG_SOVEREIGN / 0; waypoint: Waypoint 2 (tag 251, 4 point(s)), starting point 0, arrival event value 16449536 |
| 11 | `Hajod_Fighter_1` | 163 | Interactive | -13413.63,393.98,430.87 | 0,0,0 | label: BFNE_07; group/role: FG_SOVEREIGN / 0; waypoint: Waypoint 2 (tag 251, 4 point(s)), starting point 0, arrival event value 16449536 |
| 12 | `Hajod_Fighter_1` | 204 | Interactive | 14753.12,0.00,8304.22 | 0,0,0 | group/role: FG_HELIOS / 0; waypoint: Waypoint 0 (tag 254, 5 point(s)), starting point -1 |
| 13 | `Hajod_Fighter_1` | 205 | Interactive | 16141.25,0.00,8841.78 | 0,0,0 | group/role: FG_HELIOS / 0; waypoint: Waypoint 0 (tag 254, 5 point(s)), starting point -1 |
