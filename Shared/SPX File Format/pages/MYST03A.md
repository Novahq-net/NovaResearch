# Tachyon: The Fringe MYST03A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST03A.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `(none)` |
| Region | 5 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 15 |
| Events | 5 |
| Waypoints | 4 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Cassitor_Assault_Drone` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFNE_06` |
| Aliases | `Will_02` |
| Groups | `FG_STRAIN_RHO`, `FG_STRAIN_TAU`, `FG_STRAIN_IOTA`, `FG_STRAIN_KAPPA` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 2

**Action**

- Play dialog: PLAYER.SCR, line/variant 36

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 17, variable 404, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 205, subtype 0
- Set runtime trigger variable: variable group 20, variable 10, subtype 0, value 0
- Group/spawn-list action: spawn list/group 211, subtype 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 10, op 1, value 5

**Action**

- Play dialog: PLAYER.SCR, line/variant 44

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Gate state/action: param 3, subtype 0, param 0

## Waypoints

### Waypoint 0

- Tag: `4`
- Members: `Cassitor_Assault_Drone (object 9, id 207, starts at point 0)`, `Cassitor_Assault_Drone (object 10, id 208, starts at point 0)`, `Cassitor_Assault_Drone (object 11, id 209, starts at point 0)`, `Cassitor_Assault_Drone (object 12, id 221, starts at point 0)`, `Cassitor_Assault_Drone (object 13, id 222, starts at point 0)`, `Cassitor_Assault_Drone (object 14, id 223, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-827.25, 0.00, -448.28) | None |
| 1 | (-93.05, 0.00, -933.95) | None |
| 2 | (-914.99, 0.00, 292.74) | None |
| 3 | (-1159.72, 0.00, 272.71) | None |
| 4 | (-951.93, 0.00, 493.01) | on arrival redirect to Waypoint 0 (tag 4), point 2 |

### Waypoint 1

- Tag: `3`
- Members: `Cassitor_Assault_Drone (object 6, id 12, starts at point 0)`, `Cassitor_Assault_Drone (object 7, id 13, starts at point 0)`, `Cassitor_Assault_Drone (object 8, id 14, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (454.18, 0.00, -338.69) | None |
| 1 | (-816.15, 0.00, 252.63) | None |
| 2 | (-343.61, 0.00, -980.57) | None |
| 3 | (171.89, 0.00, -1444.78) | None |
| 4 | (232.04, 0.00, -877.41) | on arrival redirect to Waypoint 1 (tag 3), point 2 |

### Waypoint 2

- Tag: `2`
- Members: `Cassitor_Assault_Drone (object 3, id 7, starts at point 0)`, `Cassitor_Assault_Drone (object 4, id 8, starts at point 0)`, `Cassitor_Assault_Drone (object 5, id 9, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (390.98, 0.00, 397.99) | None |
| 1 | (-927.84, 0.00, 435.50) | None |
| 2 | (-4.24, 0.00, -961.81) | None |
| 3 | (296.47, 0.00, -1055.59) | None |
| 4 | (124.64, 0.00, -1322.87) | None |
| 5 | (-300.65, 0.00, -1191.57) | on arrival redirect to Waypoint 2 (tag 2), point 2 |

### Waypoint 3

- Tag: `1`
- Members: `Cassitor_Assault_Drone (object 0, id 4, starts at point 0)`, `Cassitor_Assault_Drone (object 1, id 5, starts at point 0)`, `Cassitor_Assault_Drone (object 2, id 6, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-519.74, 0.00, -361.63) | None |
| 1 | (-1048.12, 0.00, 341.72) | None |
| 2 | (-77.27, 0.00, -1022.77) | None |
| 3 | (-163.18, 0.00, -1327.55) | None |
| 4 | (287.88, 0.00, -1135.31) | on arrival redirect to Waypoint 3 (tag 1), point 2 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Cassitor_Assault_Drone` | 4 | Interactive | -462.47,0.00,-496.22 | 448,0,0 | group/role: FG_STRAIN_RHO / 0; waypoint: Waypoint 3 (tag 1, 5 point(s)), starting point 0, arrival event value 65536 |
| 1 | `Cassitor_Assault_Drone` | 5 | Interactive | -390.32,0.00,-394.29 | 448,0,0 | group/role: FG_STRAIN_RHO / 0; waypoint: Waypoint 3 (tag 1, 5 point(s)), starting point 0, arrival event value 65536 |
| 2 | `Cassitor_Assault_Drone` | 6 | Interactive | -470.96,0.00,-408.19 | 448,0,0 | group/role: FG_STRAIN_RHO / 0; waypoint: Waypoint 3 (tag 1, 5 point(s)), starting point 0, arrival event value 65536 |
| 3 | `Cassitor_Assault_Drone` | 7 | Interactive | 474.81,0.00,409.37 | 384,0,0 | group/role: FG_STRAIN_TAU / 0; waypoint: Waypoint 2 (tag 2, 6 point(s)), starting point 0, arrival event value 131072 |
| 4 | `Cassitor_Assault_Drone` | 8 | Interactive | 555.46,0.00,325.98 | 384,0,0 | group/role: FG_STRAIN_TAU / 0; waypoint: Waypoint 2 (tag 2, 6 point(s)), starting point 0, arrival event value 131072 |
| 5 | `Cassitor_Assault_Drone` | 9 | Interactive | 542.72,0.00,488.13 | 384,0,0 | group/role: FG_STRAIN_TAU / 0; waypoint: Waypoint 2 (tag 2, 6 point(s)), starting point 0, arrival event value 131072 |
| 6 | `Cassitor_Assault_Drone` | 12 | Interactive | 612.21,67.44,-376.20 | 448,457,0 | waypoint: Waypoint 1 (tag 3, 5 point(s)), starting point 0, arrival event value 196608 |
| 7 | `Cassitor_Assault_Drone` | 13 | Interactive | 693.83,67.44,-315.25 | 448,457,0 | waypoint: Waypoint 1 (tag 3, 5 point(s)), starting point 0, arrival event value 196608 |
| 8 | `Cassitor_Assault_Drone` | 14 | Interactive | 625.10,67.44,-488.74 | 448,457,0 | waypoint: Waypoint 1 (tag 3, 5 point(s)), starting point 0, arrival event value 196608 |
| 9 | `Cassitor_Assault_Drone` | 207 | Interactive | -1035.05,0.00,-453.29 | 384,0,0 | group/role: FG_STRAIN_IOTA / 0; waypoint: Waypoint 0 (tag 4, 5 point(s)), starting point 0, arrival event value 262144 |
| 10 | `Cassitor_Assault_Drone` | 208 | Interactive | -1113.55,0.00,-533.40 | 384,0,0 | group/role: FG_STRAIN_IOTA / 0; waypoint: Waypoint 0 (tag 4, 5 point(s)), starting point 0, arrival event value 262144 |
| 11 | `Cassitor_Assault_Drone` | 209 | Interactive | -1099.69,0.00,-373.18 | 384,0,0 | group/role: FG_STRAIN_IOTA / 0; waypoint: Waypoint 0 (tag 4, 5 point(s)), starting point 0, arrival event value 262144 |
| 12 | `Cassitor_Assault_Drone` | 221 | Interactive | -849.36,0.00,-206.29 | 384,0,0 | group/role: FG_STRAIN_KAPPA / 0; waypoint: Waypoint 0 (tag 4, 5 point(s)), starting point 0, arrival event value 262144 |
| 13 | `Cassitor_Assault_Drone` | 222 | Interactive | -924.41,0.00,-277.51 | 384,0,0 | group/role: FG_STRAIN_KAPPA / 0; waypoint: Waypoint 0 (tag 4, 5 point(s)), starting point 0, arrival event value 262144 |
| 14 | `Cassitor_Assault_Drone` | 223 | Interactive | -933.80,0.00,-119.82 | 384,0,0 | group/role: FG_STRAIN_KAPPA / 0; waypoint: Waypoint 0 (tag 4, 5 point(s)), starting point 0, arrival event value 262144 |
