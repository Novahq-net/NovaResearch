# Tachyon: The Fringe BORA01A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `BORA01A.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 3 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 7 |
| Events | 3 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Battleaxe`, `1: Bora_Mace`, `2: Bora_Shuttle_Medium`, `3: Bora_Cutlass` |
| Scripts | `CHAAS.SCR` |
| Scenes | None |
| Labels | `chaas` |
| Aliases | `frank01`, `frank04`, `frank03`, `frank02` |
| Groups | `FG_CLAW`, `CONT_033`, `FG_BORA7` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Group/spawn-list action: spawn list/group 30, subtype 2
- Object spawn/action: Bora_Shuttle_Medium (object 1, id 1671), subtype 0
- Group/spawn-list action: spawn list/group 25, subtype 1, param 1006
- Set runtime trigger variable: variable group 20, variable 10, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 10, op 1, value 12

**Action**

- Play dialog: CHAAS.SCR, line/variant 0

### Event 2

**Trigger**

- Object event: subject Bora_Cutlass (object 0, id 1664), op 7, value 0
- Object event: subject Bora_Battleaxe (object 6, id 1665), op 7, value 0
- Object event: subject Bora_Battleaxe (object 5, id 1666), op 7, value 0
- Object event: subject Bora_Battleaxe (object 4, id 1866), op 7, value 0

**Action**

- Set/add variable: variable group 21, variable 21, subtype 1, value 1

## Waypoints

### Waypoint 0

- Tag: `103`
- Members: `Bora_Mace (object 2, id 1675, starts at point 0)`, `Bora_Mace (object 3, id 1674, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1413.10, 0.00, 1014.10) | on arrival redirect to Waypoint 2 (tag 102), point 0 |

### Waypoint 1

- Tag: `101`
- Members: `Bora_Shuttle_Medium (object 1, id 1671, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1701.44, 0.00, -1026.70) | on arrival play dialog/script or enter gate, param 1007 |

### Waypoint 2

- Tag: `102`
- Members: `Bora_Cutlass (object 0, id 1664, starts at point 0)`, `Bora_Battleaxe (object 4, id 1866, starts at point 0)`, `Bora_Battleaxe (object 5, id 1666, starts at point 0)`, `Bora_Battleaxe (object 6, id 1665, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1063.24, 225.15, -1911.73) | None |
| 1 | (-699.97, 223.95, -2365.38) | on arrival play dialog/script or enter gate, param 1004 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Bora_Cutlass` | 1664 | Interactive | -1269.68,226.16,-1715.54 | 216,0,0 | label: chaas; group/role: FG_CLAW / 1; alias: frank01; waypoint: Waypoint 2 (tag 102, 2 point(s)), starting point 0, arrival event value 6684672 |
| 1 | `Bora_Shuttle_Medium` | 1671 | Interactive | -1561.14,0.00,1418.67 | 316,0,0 | secondary groups: CONT_033, none; waypoint: Waypoint 1 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 2 | `Bora_Mace` | 1675 | Interactive | 2570.68,0.00,-2148.00 | 0,0,0 | group/role: FG_BORA7 / 2; waypoint: Waypoint 0 (tag 103, 1 point(s)), starting point 0, arrival event value 6750208 |
| 3 | `Bora_Mace` | 1674 | Interactive | 2406.86,0.00,-2192.41 | 0,0,0 | group/role: FG_BORA7 / 1; waypoint: Waypoint 0 (tag 103, 1 point(s)), starting point 0, arrival event value 6750208 |
| 4 | `Bora_Battleaxe` | 1866 | Interactive | -1361.29,226.15,-1571.01 | 213,0,0 | group/role: FG_CLAW / 4; alias: frank04; waypoint: Waypoint 2 (tag 102, 2 point(s)), starting point 0, arrival event value 6684672 |
| 5 | `Bora_Battleaxe` | 1666 | Interactive | -1277.86,226.15,-1616.83 | 218,0,0 | group/role: FG_CLAW / 3; alias: frank03; waypoint: Waypoint 2 (tag 102, 2 point(s)), starting point 0, arrival event value 6684672 |
| 6 | `Bora_Battleaxe` | 1665 | Interactive | -1336.60,226.15,-1690.36 | 218,0,0 | group/role: FG_CLAW / 2; alias: frank02; waypoint: Waypoint 2 (tag 102, 2 point(s)), starting point 0, arrival event value 6684672 |
