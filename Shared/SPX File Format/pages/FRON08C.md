# Tachyon: The Fringe FRON08C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON08C.SPX` |
| Sector | `QUAD_08` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 7 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 10 |
| Events | 7 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Hajod_Fighter_2`, `1: Ice_Roid_2`, `2: Asteroid_1` |
| Scripts | `PLAYER.SCR`, `HMSLA.SCR` |
| Scenes | None |
| Labels | `bfne_03`, `bfne_01`, `HSLAV`, `BFGE_01`, `CHAPEL` |
| Aliases | `Jerome01`, `Jerome02`, `Jerome03`, `Jerome04`, `Jerome05`, `Jerome06`, `bc05_2`, `bc05_1`, `bc05_4`, `bc05_5`, `BC05_Sistine_Chapel` |
| Groups | `FG_PUNISHER`, `FG_DESPOT` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 24, op 1, value 1

**Action**

- Set runtime trigger variable: variable group 20, variable 14, subtype 0, value 0
- Group/spawn-list action: spawn list/group 135, subtype 4, param 4
- Object spawn/action: id 996, subtype 8, param 4
- Gate state/action: param 2, subtype 3, param 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 14, op 1, value 10

**Action**

- Play dialog: PLAYER.SCR, line/variant 6

### Event 2

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 6

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 34
- Object spawn/action: id 1120, subtype 14

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 8, value 0 (extra 1, 1120; flags 2)

**Action**

- Play scene: unknown index 0, param 1
- Set runtime trigger variable: variable group 20, variable 15, subtype 0, value 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 34

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 15, op 1, value 10

**Action**

- Play dialog: PLAYER.SCR, line/variant 8

### Event 5

**Trigger**

- Object event: subject 852, op 0, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 86, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 87, op 4, value 0 (join 2; flags 2)
- Object event: subject 34, op 0, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 20, op 4, value 0 (flags 2)

**Action**

- Group/spawn-list action: spawn list/group 86, subtype 4, param 1
- Group/spawn-list action: spawn list/group 87, subtype 7
- Play dialog: HMSLA.SCR, line/variant 4
- Group/spawn-list action: spawn list/group 87, subtype 4, param 1

### Event 6

**Trigger**

- Variable comparison: subject variable group 21, variable 23, op 1, value 1

**Action**

- Gate state/action: param 2, subtype 2, param 0

## Waypoints

### Waypoint 0

- Tag: `10`
- Members: `Hajod_Fighter_2 (object 3, id 860, starts at point 6)`, `Hajod_Fighter_2 (object 4, id 861, starts at point 6)`, `Hajod_Fighter_2 (object 5, id 862, starts at point 6)`, `Hajod_Fighter_2 (object 6, id 863, starts at point 6)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-526.36, 76.83, -1218.08) | None |
| 1 | (-730.11, 222.83, -1476.22) | None |
| 2 | (4.57, 222.83, -2121.18) | None |
| 3 | (415.68, 0.00, -1565.55) | None |
| 4 | (-525.22, 0.00, -709.12) | None |
| 5 | (-915.69, 0.00, -1247.20) | on arrival redirect to Waypoint 0 (tag 10), point 1 |

### Waypoint 1

- Tag: `8`
- Members: `Hajod_Fighter_2 (object 7, id 866, starts at point 0)`, `Hajod_Fighter_2 (object 8, id 864, starts at point 0)`, `Hajod_Fighter_2 (object 9, id 865, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-476.70, 245.92, 283.38) | None |
| 1 | (-806.74, 245.92, -196.68) | None |
| 2 | (-853.48, 245.92, -715.86) | None |
| 3 | (800.86, 245.92, -2013.79) | None |
| 4 | (1520.55, 245.92, -948.35) | None |
| 5 | (1523.35, 245.92, -261.01) | None |
| 6 | (1009.29, 245.92, 822.48) | on arrival redirect to Waypoint 1 (tag 8), point 0 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Asteroid_1` | 1020 | Object | -1801.22,0.00,840.90 | 0,0,0 | Scale/Radius: 1.00 |
| 1 | `Ice_Roid_2` | 1024 | Object | -1804.73,0.00,838.49 | 0,0,0 | Scale/Radius: 1.00 |
| 2 | `Ice_Roid_2` | 1025 | Object | -1804.82,0.00,843.95 | 0,0,0 | Scale/Radius: 1.00 |
| 3 | `Hajod_Fighter_2` | 860 | Interactive | -493.45,37.69,-1136.95 | 58,0,0 | group/role: FG_PUNISHER / 0; waypoint: Waypoint 0 (tag 10, 6 point(s)), starting point 6 |
| 4 | `Hajod_Fighter_2` | 861 | Interactive | -449.46,37.69,-1131.36 | 58,0,0 | group/role: FG_PUNISHER / 0; waypoint: Waypoint 0 (tag 10, 6 point(s)), starting point 6 |
| 5 | `Hajod_Fighter_2` | 862 | Interactive | -448.23,37.69,-1172.88 | 58,0,0 | label: BFGE_01; group/role: FG_PUNISHER / 0; waypoint: Waypoint 0 (tag 10, 6 point(s)), starting point 6 |
| 6 | `Hajod_Fighter_2` | 863 | Interactive | -411.19,37.69,-1172.88 | 58,0,0 | label: BFGE_01; group/role: FG_PUNISHER / 0; waypoint: Waypoint 0 (tag 10, 6 point(s)), starting point 6 |
| 7 | `Hajod_Fighter_2` | 866 | Interactive | 416.41,245.92,696.59 | 384,0,0 | label: BFGE_01; group/role: FG_DESPOT / 3; waypoint: Waypoint 1 (tag 8, 7 point(s)), starting point 0, arrival event value 524288 |
| 8 | `Hajod_Fighter_2` | 864 | Interactive | 353.33,245.92,773.31 | 384,0,0 | label: BFGE_01; group/role: FG_DESPOT / 1; waypoint: Waypoint 1 (tag 8, 7 point(s)), starting point 0, arrival event value 524288 |
| 9 | `Hajod_Fighter_2` | 865 | Interactive | 420.37,245.92,856.58 | 384,0,0 | group/role: FG_DESPOT / 2; waypoint: Waypoint 1 (tag 8, 7 point(s)), starting point 0, arrival event value 524288 |
