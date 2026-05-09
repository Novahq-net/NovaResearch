# Tachyon: The Fringe FRON04B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON04B.SPX` |
| Sector | `QUAD_04` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 3 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 18 |
| Events | 14 |
| Waypoints | 11 |
| Child Sectors | 0 |
| Scripts | 4 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Cruiser`, `1: Skav_Pirate_Manta`, `2: Void_Pirate_Fighter` |
| Scripts | `CEPHS.SCR`, `VOIDP.SCR`, `SKAVP.SCR`, `G03SKA.SCR` |
| Scenes | None |
| Labels | `BFGF_05`, `bfne_01`, `BFGE_01`, `BFNE_06`, `BFGE_05` |
| Aliases | `Jerome13`, `Kimodo 2`, `Kimodo 1`, `Kimodo 3`, `Kimodo 4`, `Python 1`, `Python 2`, `Python 3`, `Python 4`, `Aphid2`, `Aphid1`, `Mantis1`, `Mantis2`, `Cephius` |
| Groups | `FG_KOMODO`, `FG_PYTHON`, `FG_APHID`, `FG_HORNET`, `CEPHIUS`, `CEPHEUS` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Object event: subject GalSpan_Cruiser (object 16, id 906), op 9, value 0

**Action**

- Set/add variable: variable group 20, variable 0, subtype 1, value 1
- Show/update HUD contact: contact/list 0, subtype 6, param 906

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 1, subtype 0, value 0
- Set/add variable: variable group 21, variable 5, subtype 1, value 1
- Set/add variable: variable group 21, variable 2, subtype 0, value 1
- Set/add variable: variable group 20, variable 0, subtype 0, value 0
- Mission objective/state: param 262147, subtype 0, param 0
- Object spawn/action: GalSpan_Cruiser (object 16, id 906), subtype 14

### Event 2

**Trigger**

- Variable comparison: subject variable group 21, variable 2, op 1, value 1

**Action**

- Object spawn/action: GalSpan_Cruiser (object 16, id 906), subtype 3

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 2, op 1, value 1

**Action**

- Play dialog: CEPHS.SCR, line/variant 5

### Event 4

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 5

**Action**

- Play dialog: VOIDP.SCR, line/variant 1

### Event 5

**Trigger**

- Variable comparison: subject variable group 21, variable 5, op 1, value 2

**Action**

- Object spawn/action: GalSpan_Cruiser (object 16, id 906), subtype 4

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 30

**Action**

- Group/spawn-list action: spawn list/group 229, subtype 8, param 9895938 (Waypoint 2 (tag 151), point 2)
- Group/spawn-list action: spawn list/group 228, subtype 8, param 9895938 (Waypoint 2 (tag 151), point 2)

### Event 7

**Trigger**

- Object event: subject GalSpan_Cruiser (object 16, id 906), op 0, value 0 (extra 5, 72; flags 2)

**Action**

- Play dialog: SKAVP.SCR, line/variant 0

### Event 8

**Trigger**

- Group/spawn-list event: subject 73, op 4, value 0 (flags 2)

**Action**

- Play dialog: G03SKA.SCR, line/variant 1

### Event 9

**Trigger**

- Object arrival: GalSpan_Cruiser (object 16, id 906) reached Waypoint 3 (tag 156), point 1 (raw value 10223617)

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Mission objective/state: param 262148, subtype 0, param 0

### Event 10

**Trigger**

- Variable comparison: subject variable group 21, variable 2, op 1, value 1
- Global enemy/object-count event: subject 0, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Mission objective/state: param 262148, subtype 0, param 0

### Event 11

**Trigger**

- Object event: subject GalSpan_Cruiser (object 16, id 906), op 8, value 0 (flags 1)

**Action**

- Set/add variable: variable group 21, variable 2, subtype 1, value 1

### Event 12

**Trigger**

- Variable comparison: subject variable group 21, variable 2, op 1, value 3

**Action**

- Object spawn/action: GalSpan_Cruiser (object 17, id 917), subtype 3
- Group/spawn-list action: spawn list/group 229, subtype 8, param 10289152 (Waypoint 0 (tag 157), point 0)
- Hide/remove HUD contact: contact/list 0, subtype 9, param 42
- Group/spawn-list action: spawn list/group 228, subtype 8, param 10289152 (Waypoint 0 (tag 157), point 0)

### Event 13

**Trigger**

- Object event: subject GalSpan_Cruiser (object 16, id 906), op 2, value 0 (join 2)
- Object event: subject GalSpan_Cruiser (object 16, id 906), op 6, value 0 (join 2)
- Object event: subject GalSpan_Cruiser (object 17, id 917), op 2, value 0 (join 2)
- Object event: subject GalSpan_Cruiser (object 17, id 917), op 6, value 0 (join 2)

**Action**

- Set/add variable: variable group 16, variable 409, subtype 0, value 1

## Waypoints

### Waypoint 0

- Tag: `157`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (83.65, 0.00, -3240.15) | None |
| 1 | (-2965.13, 0.00, -1415.36) | on arrival play dialog/script or enter gate, param 2 |

### Waypoint 1

- Tag: `8`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2159.69, 0.00, -78.10) | None |
| 1 | (-1280.13, 0.00, 452.76) | None |
| 2 | (-633.68, 0.00, 56.98) | None |

### Waypoint 2

- Tag: `151`
- Members: `Void_Pirate_Fighter (object 0, id 417, starts at point -1)`, `Void_Pirate_Fighter (object 1, id 418, starts at point -1)`, `Void_Pirate_Fighter (object 2, id 419, starts at point -1)`, `Void_Pirate_Fighter (object 3, id 420, starts at point -1)`, `Void_Pirate_Fighter (object 4, id 421, starts at point -1)`, `Void_Pirate_Fighter (object 5, id 422, starts at point -1)`, `Void_Pirate_Fighter (object 6, id 423, starts at point -1)`, `Void_Pirate_Fighter (object 7, id 424, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2383.25, 0.00, -144.30) | None |
| 1 | (-1893.79, 0.00, -681.95) | None |
| 2 | (293.04, 0.00, -2013.03) | None |
| 3 | (1341.14, 0.00, -2237.22) | on arrival play dialog/script or enter gate, param 1 |

### Waypoint 3

- Tag: `156`
- Members: `GalSpan_Cruiser (object 16, id 906, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1174.05, 0.00, -1666.98) | None |
| 1 | (2208.81, 0.00, -3660.87) | on arrival action 1, param -1; listened by Event 9 for GalSpan_Cruiser (object 16, id 906) |

### Waypoint 4

- Tag: `153`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-3736.87, 0.00, -1723.37) | None |
| 1 | (894.39, 0.00, -4488.33) | on arrival action 1, param -1 |

### Waypoint 5

- Tag: `154`
- Members: `Skav_Pirate_Manta (object 8, id 894, starts at point -1)`, `Skav_Pirate_Manta (object 9, id 895, starts at point -1)`, `Skav_Pirate_Manta (object 10, id 896, starts at point -1)`, `Skav_Pirate_Manta (object 11, id 897, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-19.42, 0.00, -2559.52) | None |
| 1 | (-259.40, 0.00, -1989.03) | None |
| 2 | (-1586.77, 0.00, -1213.79) | None |

### Waypoint 6

- Tag: `155`
- Members: `Skav_Pirate_Manta (object 12, id 898, starts at point -1)`, `Skav_Pirate_Manta (object 13, id 899, starts at point -1)`, `Skav_Pirate_Manta (object 14, id 900, starts at point -1)`, `Skav_Pirate_Manta (object 15, id 901, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (552.13, 0.00, 1368.72) | None |
| 1 | (-1481.03, 0.00, 1355.95) | None |
| 2 | (-2335.71, 1208.40, 382.79) | None |

### Waypoint 7

- Tag: `12`
- Members: `GalSpan_Cruiser (object 17, id 917, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (75.28, 2282.06, -3629.44) | None |
| 1 | (-1713.43, 2282.06, -2514.76) | on arrival action 1, param -1 |

### Waypoint 8

- Tag: `13`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (484.08, 2282.06, -2577.97) | None |
| 1 | (-3205.13, 2282.06, -359.96) | on arrival action 1, param -1 |

### Waypoint 9

- Tag: `11`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-540.92, 2282.06, -4394.88) | None |
| 1 | (-4422.58, 2282.06, -2195.83) | on arrival action 1, param -1 |

### Waypoint 10

- Tag: `152`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-3033.18, 0.00, -220.52) | None |
| 1 | (1595.61, 0.00, -2981.87) | on arrival action 1, param -1 |

## Spawn Lists

### Spawn List 0

- ID: `72`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | GalSpan_Cruiser (object 16, id 906) | None |

### Spawn List 1

- ID: `228`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 7 | id 227 | None |
| 1 | 5 | spawn list 72 | None |
| 2 | 5 | spawn list 73 | None |

### Spawn List 2

- ID: `229`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 3

- ID: `73`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Void_Pirate_Fighter` | 417 | Interactive | -5083.30,0.00,1702.49 | 0,0,0 | group/role: FG_KOMODO / 0; alias: Kimodo 2; waypoint: Waypoint 2 (tag 151, 4 point(s)), starting point -1 |
| 1 | `Void_Pirate_Fighter` | 418 | Interactive | -5032.67,0.00,1763.63 | 0,0,0 | label: BFGF_05; group/role: FG_KOMODO / 0; alias: Kimodo 1; waypoint: Waypoint 2 (tag 151, 4 point(s)), starting point -1 |
| 2 | `Void_Pirate_Fighter` | 419 | Interactive | -4973.61,0.00,1702.49 | 0,0,0 | label: BFGF_05; group/role: FG_KOMODO / 0; alias: Kimodo 3; waypoint: Waypoint 2 (tag 151, 4 point(s)), starting point -1 |
| 3 | `Void_Pirate_Fighter` | 420 | Interactive | -5032.67,0.00,1641.36 | 0,0,0 | group/role: FG_KOMODO / 0; alias: Kimodo 4; waypoint: Waypoint 2 (tag 151, 4 point(s)), starting point -1 |
| 4 | `Void_Pirate_Fighter` | 421 | Interactive | -4762.67,0.00,1794.18 | 0,0,0 | label: BFGF_05; group/role: FG_PYTHON / 0; alias: Python 1; waypoint: Waypoint 2 (tag 151, 4 point(s)), starting point -1 |
| 5 | `Void_Pirate_Fighter` | 422 | Interactive | -4813.30,0.00,1722.87 | 0,0,0 | label: BFGF_05; group/role: FG_PYTHON / 0; alias: Python 2; waypoint: Waypoint 2 (tag 151, 4 point(s)), starting point -1 |
| 6 | `Void_Pirate_Fighter` | 423 | Interactive | -4712.05,0.00,1733.06 | 0,0,0 | group/role: FG_PYTHON / 0; alias: Python 3; waypoint: Waypoint 2 (tag 151, 4 point(s)), starting point -1 |
| 7 | `Void_Pirate_Fighter` | 424 | Interactive | -4762.67,0.00,1651.55 | 0,0,0 | group/role: FG_PYTHON / 0; alias: Python 4; waypoint: Waypoint 2 (tag 151, 4 point(s)), starting point -1 |
| 8 | `Skav_Pirate_Manta` | 894 | Interactive | 169.98,0.00,-4337.20 | 0,0,0 | label: BFGE_05; group/role: FG_APHID / 0; waypoint: Waypoint 5 (tag 154, 3 point(s)), starting point -1 |
| 9 | `Skav_Pirate_Manta` | 895 | Interactive | 229.21,0.00,-4337.20 | 0,0,0 | label: BFGE_05; group/role: FG_APHID / 0; waypoint: Waypoint 5 (tag 154, 3 point(s)), starting point -1 |
| 10 | `Skav_Pirate_Manta` | 896 | Interactive | 288.45,0.00,-4329.64 | 0,0,0 | group/role: FG_APHID / 0; waypoint: Waypoint 5 (tag 154, 3 point(s)), starting point -1 |
| 11 | `Skav_Pirate_Manta` | 897 | Interactive | 382.54,0.00,-4329.64 | 0,0,0 | group/role: FG_APHID / 0; waypoint: Waypoint 5 (tag 154, 3 point(s)), starting point -1 |
| 12 | `Skav_Pirate_Manta` | 898 | Interactive | 1538.21,1158.21,1497.95 | 0,0,0 | label: BFGE_05; group/role: FG_HORNET / 0; waypoint: Waypoint 6 (tag 155, 3 point(s)), starting point -1 |
| 13 | `Skav_Pirate_Manta` | 899 | Interactive | 1557.65,1158.21,1497.51 | 0,0,0 | group/role: FG_HORNET / 0; waypoint: Waypoint 6 (tag 155, 3 point(s)), starting point -1 |
| 14 | `Skav_Pirate_Manta` | 900 | Interactive | 1534.07,1158.21,1465.03 | 0,0,0 | label: BFGE_05; group/role: FG_HORNET / 0; waypoint: Waypoint 6 (tag 155, 3 point(s)), starting point -1 |
| 15 | `Skav_Pirate_Manta` | 901 | Interactive | 1561.95,1158.21,1465.02 | 0,0,0 | group/role: FG_HORNET / 0; waypoint: Waypoint 6 (tag 155, 3 point(s)), starting point -1 |
| 16 | `GalSpan_Cruiser` | 906 | Interactive | -4174.99,0.00,-4.26 | 164,0,0 | alias: Cephius; secondary groups: none, CEPHIUS; waypoint: Waypoint 3 (tag 156, 2 point(s)), starting point -1 |
| 17 | `GalSpan_Cruiser` | 917 | Interactive | 1517.98,2282.06,-4582.34 | 427,0,0 | alias: Cephius; secondary groups: none, CEPHEUS; waypoint: Waypoint 7 (tag 12, 2 point(s)), starting point -1 |
