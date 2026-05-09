# Tachyon: The Fringe FRON04A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON04A.SPX` |
| Sector | `QUAD_04` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 3 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 9 |
| Events | 17 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Skav_Pirate_Manta`, `1: Star_Patrol_Enforcer` |
| Scripts | `PLAYER.SCR`, `SPBLT.SCR` |
| Scenes | None |
| Labels | `BFGF_05`, `bfne_01`, `BFGE_01`, `BFNE_06`, `BFGE_05` |
| Aliases | `Jerome13`, `Kimodo 2`, `Kimodo 1`, `Kimodo 3`, `Kimodo 4`, `Python 1`, `Python 2`, `Python 3`, `Python 4`, `Aphid2`, `Aphid1`, `Mantis1`, `Mantis2`, `Cephius` |
| Groups | `FG_BOLT`, `FG_GNAT`, `FG_DRAGONFLY` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (join 1)
- Group/spawn-list event: subject 121, op 3, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 104

### Event 1

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Group/spawn-list event: subject 121, op 3, value 0

**Action**

- Group/spawn-list action: spawn list/group 134, subtype 2

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1 (join 1)
- Object event: subject Star_Patrol_Enforcer (object 0, id 397), op 2, value 0

**Action**

- Play dialog: SPBLT.SCR, line/variant 2
- Object spawn/action: id 862, subtype 6

### Event 3

**Trigger**

- Group/spawn-list event: subject 134, op 4, value 0 (extra 5, 121; flags 2)

**Action**

- Group/spawn-list action: spawn list/group 140, subtype 7

### Event 4

**Trigger**

- Group/spawn-list event: subject 134, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 140, op 4, value 0 (flags 2)

**Action**

- Group/spawn-list action: spawn list/group 134, subtype 4, param 9
- Group/spawn-list action: spawn list/group 140, subtype 4, param 9
- Set runtime trigger variable: variable group 20, variable 14, subtype 0, value 0

### Event 5

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 1, id 408), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 12, subtype 1, value 1

### Event 6

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 2, id 409), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 12, subtype 1, value 1
- Play dialog: PLAYER.SCR, line/variant 163

### Event 7

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 3, id 410), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 12, subtype 1, value 1

### Event 8

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 4, id 411), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 12, subtype 1, value 1

### Event 9

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 5, id 412), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 12, subtype 1, value 1

### Event 10

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 6, id 413), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 12, subtype 1, value 1

### Event 11

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 7, id 414), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 12, subtype 1, value 1

### Event 12

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 8, id 416), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 12, subtype 1, value 1

### Event 13

**Trigger**

- Variable comparison: subject variable group 21, variable 12, op 1, value 7
- Variable comparison: subject variable group 20, variable 14, op 2, value 100 (join 1)
- Object event: subject Star_Patrol_Enforcer (object 0, id 397), op 2, value 0

**Action**

- Set/add variable: variable group 16, variable 417, subtype 0, value 2

### Event 14

**Trigger**

- Variable comparison: subject variable group 21, variable 12, op 1, value 7
- Variable comparison: subject variable group 20, variable 14, op 2, value 100 (join 1)
- Object event: subject Star_Patrol_Enforcer (object 0, id 397), op 2, value 0

**Action**

- Play dialog: SPBLT.SCR, line/variant 3
- Object spawn/action: Star_Patrol_Enforcer (object 0, id 397), subtype 2, param 1

### Event 15

**Trigger**

- Object event: subject Star_Patrol_Enforcer (object 0, id 397), op 2, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 121

### Event 16

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 50

**Action**

- Play dialog: PLAYER.SCR, line/variant 190

## Waypoints

### Waypoint 0

- Tag: `2`
- Members: `Skav_Pirate_Manta (object 1, id 408, starts at point 0)`, `Skav_Pirate_Manta (object 2, id 409, starts at point 0)`, `Skav_Pirate_Manta (object 3, id 410, starts at point 0)`, `Skav_Pirate_Manta (object 4, id 411, starts at point 0)`, `Skav_Pirate_Manta (object 5, id 412, starts at point 0)`, `Skav_Pirate_Manta (object 6, id 413, starts at point 0)`, `Skav_Pirate_Manta (object 7, id 414, starts at point 0)`, `Skav_Pirate_Manta (object 8, id 416, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (887.11, 507.43, -1218.27) | None |
| 1 | (37.14, 0.00, -1246.81) | None |
| 2 | (-897.47, 0.00, -1057.45) | None |
| 3 | (-914.50, 0.00, -247.19) | on arrival redirect to Waypoint 0 (tag 2), point 1 |

### Waypoint 1

- Tag: `1`
- Members: `Star_Patrol_Enforcer (object 0, id 397, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (115.55, 0.00, -483.13) | None |
| 1 | (-829.69, 0.00, -49.06) | None |
| 2 | (-1510.94, 0.00, -164.81) | None |
| 3 | (-1766.41, 0.00, -666.40) | None |
| 4 | (-872.27, 0.00, -1418.79) | None |
| 5 | (353.98, 0.00, -1544.19) | None |

## Spawn Lists

### Spawn List 0

- ID: `140`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 1 | id 121 | None |

### Spawn List 1

- ID: `134`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 1 | id 121 | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Star_Patrol_Enforcer` | 397 | Interactive | 1115.65,0.00,-1916.75 | 415,0,0 | group/role: FG_BOLT / 0; alias: Jerome13; waypoint: Waypoint 1 (tag 1, 6 point(s)), starting point 0, arrival event value 65536 |
| 1 | `Skav_Pirate_Manta` | 408 | Interactive | 602.17,1200.98,81.59 | 384,0,0 | label: bfne_01; group/role: FG_GNAT / 0; waypoint: Waypoint 0 (tag 2, 4 point(s)), starting point 0, arrival event value 131072 |
| 2 | `Skav_Pirate_Manta` | 409 | Interactive | 593.65,1200.98,14.28 | 384,0,0 | group/role: FG_GNAT / 0; waypoint: Waypoint 0 (tag 2, 4 point(s)), starting point 0, arrival event value 131072 |
| 3 | `Skav_Pirate_Manta` | 410 | Interactive | 661.78,1200.98,81.80 | 384,0,0 | group/role: FG_GNAT / 0; waypoint: Waypoint 0 (tag 2, 4 point(s)), starting point 0, arrival event value 131072 |
| 4 | `Skav_Pirate_Manta` | 411 | Interactive | 653.26,1200.98,4.63 | 0,0,0 | group/role: FG_GNAT / 0; waypoint: Waypoint 0 (tag 2, 4 point(s)), starting point 0, arrival event value 131072 |
| 5 | `Skav_Pirate_Manta` | 412 | Interactive | 1210.64,320.18,-937.79 | 313,0,0 | group/role: FG_DRAGONFLY / 0; waypoint: Waypoint 0 (tag 2, 4 point(s)), starting point 0, arrival event value 131072 |
| 6 | `Skav_Pirate_Manta` | 413 | Interactive | 1177.95,317.97,-883.04 | 317,0,0 | label: bfne_01; group/role: FG_DRAGONFLY / 0; waypoint: Waypoint 0 (tag 2, 4 point(s)), starting point 0, arrival event value 131072 |
| 7 | `Skav_Pirate_Manta` | 414 | Interactive | 1237.62,317.97,-883.04 | 317,0,0 | group/role: FG_DRAGONFLY / 0; waypoint: Waypoint 0 (tag 2, 4 point(s)), starting point 0, arrival event value 131072 |
| 8 | `Skav_Pirate_Manta` | 416 | Interactive | 1252.85,317.97,-931.92 | 314,0,0 | label: bfne_01; group/role: FG_DRAGONFLY / 0; waypoint: Waypoint 0 (tag 2, 4 point(s)), starting point 0, arrival event value 131072 |
