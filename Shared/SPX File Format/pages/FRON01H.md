# Tachyon: The Fringe FRON01H.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON01H.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 16 |
| Events | 4 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Void_Pirate_Fighter`, `1: Skav_Pirate_Manta` |
| Scripts | `TRISH.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFGF_05`, `BFNE_03`, `BFNF_03`, `BFGE_01`, `BFGF_01`, `bfne_05` |
| Aliases | `Python 4`, `Python 3`, `Python 1`, `Python 2`, `Kimodo 1`, `Jerome02`, `Jerome03`, `Jerome04`, `Jerome05`, `Jerome06`, `Jerome01`, `BC05_sistine_chapel`, `bc05_1`, `bc05_2`, `bc05_4`, `bc05_5`, `Mantis1`, `Mantis2`, `Mantis3`, `Mantis4`, `Aphid1`, `Aphid2`, `Aphid3`, `Aphid4`, `Python1`, `Python2`, `Python3`, `Python4`, `Komodo1`, `Komodo2`, `Komodo3`, `Komodo4`, `Kimodo 2`, `Kimodo 3`, `Kimodo 4`, `Cephius`, `Stocks01` |
| Groups | `FG_MANTIS`, `FG_APHID`, `FG_PYTHON`, `FG_KOMODO` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 43
- Set runtime trigger variable: variable group 20, variable 6, subtype 0, value 0
- Gate state/action: param 7, subtype 3, param 0
- Gate state/action: param 8, subtype 3, param 0
- Gate state/action: param 9, subtype 3, param 0
- Set/add variable: variable group 21, variable 20, subtype 0, value 0
- Mission objective/state: param 262149, subtype 0, param 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 9, value 0

**Action**

- Play dialog: TRISH.SCR, line/variant 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 24, op 1, value 1
- Variable comparison: subject variable group 21, variable 23, op 1, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 3
- Hide/remove HUD contact: contact/list 0, subtype 9, param 43

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 23, op 1, value 1

**Action**

- Set/add variable: variable group 16, variable 406, subtype 0, value 1
- Set/add variable: variable group 16, variable 407, subtype 0, value 2

## Waypoints

### Waypoint 0

- Tag: `452`
- Members: `Skav_Pirate_Manta (object 0, id 670, starts at point 2)`, `Skav_Pirate_Manta (object 1, id 671, starts at point 2)`, `Skav_Pirate_Manta (object 2, id 672, starts at point 2)`, `Skav_Pirate_Manta (object 3, id 673, starts at point 2)`, `Skav_Pirate_Manta (object 4, id 686, starts at point 2)`, `Skav_Pirate_Manta (object 5, id 687, starts at point 2)`, `Skav_Pirate_Manta (object 6, id 688, starts at point 2)`, `Skav_Pirate_Manta (object 7, id 689, starts at point 2)`, `Void_Pirate_Fighter (object 8, id 702, starts at point 1)`, `Void_Pirate_Fighter (object 9, id 703, starts at point 1)`, `Void_Pirate_Fighter (object 10, id 704, starts at point 1)`, `Void_Pirate_Fighter (object 11, id 705, starts at point 1)`, `Void_Pirate_Fighter (object 12, id 706, starts at point 1)`, `Void_Pirate_Fighter (object 13, id 707, starts at point 1)`, `Void_Pirate_Fighter (object 14, id 708, starts at point 1)`, `Void_Pirate_Fighter (object 15, id 709, starts at point 1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1237.02, 632.26, -2391.43) | None |
| 1 | (1506.88, 632.26, -2439.04) | None |
| 2 | (1462.98, 632.26, 60.14) | None |
| 3 | (-1280.93, 632.26, 131.54) | on arrival redirect to Waypoint 0 (tag 452), point 0 |

## Spawn Lists

### Spawn List 0

- ID: `229`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 1

- ID: `228`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 2

- ID: `72`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 3

- ID: `74`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Skav_Pirate_Manta` | 670 | Interactive | 1800.48,0.00,-1458.91 | 0,0,0 | label: BFGE_01; group/role: FG_MANTIS / 0; alias: Mantis1; waypoint: Waypoint 0 (tag 452, 4 point(s)), starting point 2, arrival event value 29622274 |
| 1 | `Skav_Pirate_Manta` | 671 | Interactive | 1774.56,0.00,-1495.27 | 0,0,0 | group/role: FG_MANTIS / 0; alias: Mantis2; waypoint: Waypoint 0 (tag 452, 4 point(s)), starting point 2, arrival event value 29622274 |
| 2 | `Skav_Pirate_Manta` | 672 | Interactive | 1830.96,0.00,-1498.58 | 0,0,0 | label: BFGE_01; group/role: FG_MANTIS / 0; alias: Mantis3; waypoint: Waypoint 0 (tag 452, 4 point(s)), starting point 2, arrival event value 29622274 |
| 3 | `Skav_Pirate_Manta` | 673 | Interactive | 1800.48,0.00,-1531.63 | 0,0,0 | group/role: FG_MANTIS / 0; alias: Mantis4; waypoint: Waypoint 0 (tag 452, 4 point(s)), starting point 2, arrival event value 29622274 |
| 4 | `Skav_Pirate_Manta` | 686 | Interactive | 1973.62,0.00,-1449.51 | 0,0,0 | label: BFGE_01; group/role: FG_APHID / 0; alias: Aphid1; waypoint: Waypoint 0 (tag 452, 4 point(s)), starting point 2, arrival event value 29622274 |
| 5 | `Skav_Pirate_Manta` | 687 | Interactive | 1945.57,0.00,-1485.63 | 0,0,0 | label: BFGE_01; group/role: FG_APHID / 0; alias: Aphid2; waypoint: Waypoint 0 (tag 452, 4 point(s)), starting point 2, arrival event value 29622274 |
| 6 | `Skav_Pirate_Manta` | 688 | Interactive | 2006.93,0.00,-1491.33 | 0,0,0 | group/role: FG_APHID / 0; alias: Aphid3; waypoint: Waypoint 0 (tag 452, 4 point(s)), starting point 2, arrival event value 29622274 |
| 7 | `Skav_Pirate_Manta` | 689 | Interactive | 1982.39,0.00,-1523.65 | 0,0,0 | group/role: FG_APHID / 0; alias: Aphid4; waypoint: Waypoint 0 (tag 452, 4 point(s)), starting point 2, arrival event value 29622274 |
| 8 | `Void_Pirate_Fighter` | 702 | Interactive | 1642.11,0.00,-803.49 | 0,0,0 | label: BFGF_01; group/role: FG_PYTHON / 0; alias: Python1; waypoint: Waypoint 0 (tag 452, 4 point(s)), starting point 1, arrival event value 29622273 |
| 9 | `Void_Pirate_Fighter` | 703 | Interactive | 1599.43,0.00,-856.38 | 0,0,0 | group/role: FG_PYTHON / 0; alias: Python2; waypoint: Waypoint 0 (tag 452, 4 point(s)), starting point 1, arrival event value 29622273 |
| 10 | `Void_Pirate_Fighter` | 704 | Interactive | 1687.84,0.00,-862.99 | 0,0,0 | label: BFGF_01; group/role: FG_PYTHON / 0; alias: Python3; waypoint: Waypoint 0 (tag 452, 4 point(s)), starting point 1, arrival event value 29622273 |
| 11 | `Void_Pirate_Fighter` | 705 | Interactive | 1639.06,0.00,-902.66 | 0,0,0 | group/role: FG_PYTHON / 0; alias: Python4; waypoint: Waypoint 0 (tag 452, 4 point(s)), starting point 1, arrival event value 29622273 |
| 12 | `Void_Pirate_Fighter` | 706 | Interactive | 1934.79,0.00,-777.04 | 0,0,0 | label: BFGF_01; group/role: FG_KOMODO / 0; alias: Komodo1; waypoint: Waypoint 0 (tag 452, 4 point(s)), starting point 1, arrival event value 29622273 |
| 13 | `Void_Pirate_Fighter` | 707 | Interactive | 1886.01,0.00,-849.77 | 0,0,0 | label: BFGF_01; group/role: FG_KOMODO / 0; alias: Komodo2; waypoint: Waypoint 0 (tag 452, 4 point(s)), starting point 1, arrival event value 29622273 |
| 14 | `Void_Pirate_Fighter` | 708 | Interactive | 1983.57,0.00,-862.99 | 0,0,0 | group/role: FG_KOMODO / 0; alias: Komodo3; waypoint: Waypoint 0 (tag 452, 4 point(s)), starting point 1, arrival event value 29622273 |
| 15 | `Void_Pirate_Fighter` | 709 | Interactive | 1943.94,0.00,-902.66 | 0,0,0 | group/role: FG_KOMODO / 0; alias: Komodo4; waypoint: Waypoint 0 (tag 452, 4 point(s)), starting point 1, arrival event value 29622273 |
