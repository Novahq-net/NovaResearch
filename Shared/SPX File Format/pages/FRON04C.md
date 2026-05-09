# Tachyon: The Fringe FRON04C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON04C.SPX` |
| Sector | `QUAD_04` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 3 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 4 |
| Events | 6 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Skav_Pirate_Manta` |
| Scripts | `G03SKA.SCR` |
| Scenes | None |
| Labels | `BFGF_05`, `bfne_01`, `BFGE_01`, `BFNE_06`, `BFGE_05` |
| Aliases | `Jerome13`, `Kimodo 2`, `Kimodo 1`, `Kimodo 3`, `Kimodo 4`, `Python 1`, `Python 2`, `Python 3`, `Python 4`, `Aphid2`, `Aphid1`, `Mantis1`, `Mantis2`, `Cephius` |
| Groups | `FG_APHID`, `FG_MANTIS` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Gate state/action: param 1, subtype 3, param 0
- Gate state/action: param 2, subtype 2, param 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (join 2)

**Action**

- Set runtime trigger variable: variable group 20, variable 19, subtype 0, value 0

### Event 2

**Trigger**

- Group/spawn-list event: subject 72, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 74, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 73, op 4, value 0 (join 2; flags 2)
- Variable comparison: subject variable group 20, variable 19, op 1, value 55 (join 2)

**Action**

- Play dialog: G03SKA.SCR, line/variant 1

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 15

**Action**

- Play dialog: G03SKA.SCR, line/variant 0

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 90

**Action**

- Group/spawn-list action: spawn list/group 72, subtype 3, param 2
- Group/spawn-list action: spawn list/group 74, subtype 3, param 2

### Event 5

**Trigger**

- Variable comparison: subject variable group 21, variable 23, op 1, value 1

**Action**

- Gate state/action: param 1, subtype 2, param 0

## Waypoints

### Waypoint 0

- Tag: `5`
- Members: `Skav_Pirate_Manta (object 2, id 871, starts at point -1)`, `Skav_Pirate_Manta (object 3, id 872, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (434.42, 536.64, -625.71) | None |
| 1 | (-1785.88, -113.88, -572.46) | None |
| 2 | (-1802.93, -125.39, -1619.50) | None |
| 3 | (-1569.81, -29.56, -2254.30) | None |
| 4 | (-178.36, -406.75, -3107.94) | None |
| 5 | (1176.05, -1435.30, -2846.18) | None |
| 6 | (1252.72, -1602.56, -2349.54) | on arrival redirect to Waypoint 0 (tag 5), point 0 |

### Waypoint 1

- Tag: `4`
- Members: `Skav_Pirate_Manta (object 0, id 867, starts at point -1)`, `Skav_Pirate_Manta (object 1, id 868, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (642.35, 1471.30, 984.77) | None |
| 1 | (-309.37, 1471.30, 1149.82) | None |
| 2 | (-950.28, 1471.30, 571.78) | None |
| 3 | (88.97, 536.64, -1186.39) | None |
| 4 | (1144.55, 1471.30, -1588.79) | None |
| 5 | (1463.64, 1471.30, -750.06) | None |
| 6 | (1355.49, 1471.30, 163.13) | on arrival redirect to Waypoint 1 (tag 4), point 1 |

### Waypoint 2

- Tag: `3`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-743.55, 171.24, -1084.78) | None |
| 1 | (-345.16, 171.24, -733.52) | None |
| 2 | (-343.39, 171.24, 23.91) | None |
| 3 | (-1942.84, 0.00, 201.36) | on arrival redirect to Waypoint 2 (tag 3), point 0 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Skav_Pirate_Manta` | 867 | Interactive | 1227.37,1158.64,-187.51 | 0,0,0 | label: BFGE_01; group/role: FG_APHID / 0; alias: Aphid2; waypoint: Waypoint 1 (tag 4, 7 point(s)), starting point -1 |
| 1 | `Skav_Pirate_Manta` | 868 | Interactive | 1209.57,1158.64,-187.76 | 0,0,0 | label: BFGE_01; group/role: FG_APHID / 0; alias: Aphid1; waypoint: Waypoint 1 (tag 4, 7 point(s)), starting point -1 |
| 2 | `Skav_Pirate_Manta` | 871 | Interactive | 1178.80,1158.64,-301.26 | 0,0,0 | label: BFGE_01; group/role: FG_MANTIS / 0; alias: Mantis1; waypoint: Waypoint 0 (tag 5, 7 point(s)), starting point -1 |
| 3 | `Skav_Pirate_Manta` | 872 | Interactive | 1200.75,1158.64,-301.26 | 0,0,0 | label: BFGE_01; group/role: FG_MANTIS / 0; alias: Mantis2; waypoint: Waypoint 0 (tag 5, 7 point(s)), starting point -1 |
