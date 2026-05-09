# Tachyon: The Fringe FRON01A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON01A.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 10 |
| Events | 9 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Cruiser`, `1: Void_Pirate_Fighter` |
| Scripts | `TRISH.SCR`, `CEPHS.SCR` |
| Scenes | None |
| Labels | `BFGF_05`, `BFNE_03`, `BFNF_03`, `BFGE_01`, `BFGF_01`, `bfne_05` |
| Aliases | `Python 4`, `Python 3`, `Python 1`, `Python 2`, `Kimodo 1`, `Jerome02`, `Jerome03`, `Jerome04`, `Jerome05`, `Jerome06`, `Jerome01`, `BC05_sistine_chapel`, `bc05_1`, `bc05_2`, `bc05_4`, `bc05_5`, `Mantis1`, `Mantis2`, `Mantis3`, `Mantis4`, `Aphid1`, `Aphid2`, `Aphid3`, `Aphid4`, `Python1`, `Python2`, `Python3`, `Python4`, `Komodo1`, `Komodo2`, `Komodo3`, `Komodo4`, `Kimodo 2`, `Kimodo 3`, `Kimodo 4`, `Cephius`, `Stocks01` |
| Groups | `FG_PYTHON`, `FG_KOMODO`, `CEPHIUS` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 6, param 474
- Set/add variable: variable group 21, variable 20, subtype 0, value 0
- Set/add variable: variable group 21, variable 5, subtype 0, value 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 10

**Action**

- Group/spawn-list action: spawn list/group 229, subtype 1, param 2
- Object spawn/action: GalSpan_Cruiser (object 8, id 474), subtype 14

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 22

**Action**

- Play dialog: TRISH.SCR, line/variant 2
- Group/spawn-list action: spawn list/group 228, subtype 1, param 2

### Event 4

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 2

**Action**

- Play dialog: CEPHS.SCR, line/variant 3

### Event 5

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 3

**Action**

- Play dialog: CEPHS.SCR, line/variant 4

### Event 6

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 4 (join 2)
- Variable comparison: subject variable group 21, variable 5, op 1, value 1

**Action**

- Object spawn/action: GalSpan_Cruiser (object 8, id 474), subtype 4
- Set/add variable: variable group 21, variable 2, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Mission objective/state: param 262148, subtype 0, param 0
- Object spawn/action: GalSpan_Cruiser (object 8, id 474), subtype 15

### Event 7

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 2
- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)

**Action**

- Set/add variable: variable group 16, variable 409, subtype 0, value 1

### Event 8

**Trigger**

- Variable comparison: subject variable group 21, variable 2, op 1, value 5

**Action**

- Object spawn/action: GalSpan_Cruiser (object 9, id 492), subtype 3

## Waypoints

### Waypoint 0

- Tag: `10`
- Members: `Void_Pirate_Fighter (object 4, id 79, starts at point -1)`, `Void_Pirate_Fighter (object 5, id 760, starts at point -1)`, `Void_Pirate_Fighter (object 6, id 761, starts at point -1)`, `Void_Pirate_Fighter (object 7, id 762, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1321.68, 0.00, 3189.91) | None |
| 1 | (1047.37, 0.00, 2805.70) | None |
| 2 | (1102.24, 0.00, 2659.75) | None |
| 3 | (1234.10, 0.00, 2394.87) | None |
| 4 | (1383.19, 14.00, 2545.87) | None |
| 5 | (1460.94, 0.00, 2656.69) | on arrival play dialog/script or enter gate, param 3 |

### Waypoint 1

- Tag: `1`
- Members: `Void_Pirate_Fighter (object 0, id 74, starts at point -1)`, `Void_Pirate_Fighter (object 1, id 76, starts at point -1)`, `Void_Pirate_Fighter (object 2, id 77, starts at point -1)`, `Void_Pirate_Fighter (object 3, id 78, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1250.25, 0.00, 3203.45) | None |
| 1 | (935.01, 0.00, 2815.57) | None |
| 2 | (1022.14, 0.00, 2586.72) | None |
| 3 | (1125.72, 0.00, 2410.94) | None |
| 4 | (1263.17, 14.00, 2548.78) | None |
| 5 | (1348.59, 0.00, 2660.30) | on arrival play dialog/script or enter gate, param 3 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Void_Pirate_Fighter` | 74 | Interactive | 1252.84,0.00,3601.51 | 0,0,0 | group/role: FG_PYTHON / 4; alias: Python 4; waypoint: Waypoint 1 (tag 1, 6 point(s)), starting point -1 |
| 1 | `Void_Pirate_Fighter` | 76 | Interactive | 1277.37,0.00,3639.59 | 0,0,0 | label: BFGF_05; group/role: FG_PYTHON / 3; alias: Python 3; waypoint: Waypoint 1 (tag 1, 6 point(s)), starting point -1 |
| 2 | `Void_Pirate_Fighter` | 77 | Interactive | 1252.84,0.00,3681.89 | 0,0,0 | label: BFGF_05; group/role: FG_PYTHON / 1; alias: Python 1; waypoint: Waypoint 1 (tag 1, 6 point(s)), starting point -1 |
| 3 | `Void_Pirate_Fighter` | 78 | Interactive | 1228.32,0.00,3639.59 | 0,0,0 | group/role: FG_PYTHON / 2; alias: Python 2; waypoint: Waypoint 1 (tag 1, 6 point(s)), starting point -1 |
| 4 | `Void_Pirate_Fighter` | 79 | Interactive | 1212.79,0.00,3574.70 | 0,0,0 | label: BFGF_05; group/role: FG_KOMODO / 1; alias: Kimodo 1; waypoint: Waypoint 0 (tag 10, 6 point(s)), starting point -1 |
| 5 | `Void_Pirate_Fighter` | 760 | Interactive | 1228.62,0.00,3561.34 | 0,0,0 | label: BFGF_05; group/role: FG_KOMODO / 2; alias: Kimodo 2; waypoint: Waypoint 0 (tag 10, 6 point(s)), starting point -1 |
| 6 | `Void_Pirate_Fighter` | 761 | Interactive | 1242.34,0.00,3548.95 | 0,0,0 | group/role: FG_KOMODO / 3; alias: Kimodo 3; waypoint: Waypoint 0 (tag 10, 6 point(s)), starting point -1 |
| 7 | `Void_Pirate_Fighter` | 762 | Interactive | 1256.68,0.00,3534.07 | 0,0,0 | group/role: FG_KOMODO / 4; alias: Kimodo 4; waypoint: Waypoint 0 (tag 10, 6 point(s)), starting point -1 |
| 8 | `GalSpan_Cruiser` | 474 | Interactive | 2043.53,404.63,3829.51 | 256,0,0 | alias: Cephius; secondary groups: none, CEPHIUS |
| 9 | `GalSpan_Cruiser` | 492 | Interactive | 1937.69,0.00,1220.77 | 0,0,0 | alias: Cephius; secondary groups: none, CEPHIUS |
