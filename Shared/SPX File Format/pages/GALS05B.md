# Tachyon: The Fringe GALS05B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `GALS05B.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `(none)` |
| Region | 2 |
| Sector ID | 4 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 6 |
| Events | 7 |
| Waypoints | 4 |
| Child Sectors | 0 |
| Scripts | 0 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Lt_Freighter`, `1: GalSpan_Carrier`, `2: GalSpan_Orion`, `3: GalSpan_Shuttle_Medium` |
| Scripts | None |
| Scenes | None |
| Labels | `bfne_02`, `BFGE_04`, `bfne_03`, `bfgf_02`, `bfne_08`, `bfge_02` |
| Aliases | `wing_man` |
| Groups | `CONT_002`, `FG_HADES` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 26, subtype 0, value 0

### Event 1

**Trigger**

- Object arrival: GalSpan_Shuttle_Medium (object 0, id 19) reached Waypoint 3 (tag 151), point 1 (raw value 9895937)

**Action**

- Object spawn/action: GalSpan_Shuttle_Medium (object 0, id 19), subtype 2, param 1

### Event 2

**Trigger**

- Object arrival: GalSpan_Carrier (object 4, id 62) reached Waypoint 2 (tag 152), point 0 (raw value 9961472)

**Action**

- Object spawn/action: GalSpan_Carrier (object 4, id 62), subtype 4

### Event 3

**Trigger**

- Variable comparison: subject variable group 14, variable 402, op 1, value 1
- Variable comparison: subject variable group 14, variable 403, op 1, value 2

**Action**

- Object spawn/action: GalSpan_Lt_Freighter (object 5, id 66), subtype 0

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 26, op 1, value 10

**Action**

- Group/spawn-list action: spawn list/group 157, subtype 1, param 2

### Event 5

**Trigger**

- Group/spawn-list event: subject 157, op 2, value 10092546 (Waypoint 0 (tag 154), point 2)

**Action**

- Group/spawn-list action: spawn list/group 157, subtype 3, param 1

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 26, op 1, value 38

**Action**

- Object spawn/action: GalSpan_Carrier (object 4, id 62), subtype 5

## Waypoints

### Waypoint 0

- Tag: `154`
- Members: `GalSpan_Orion (object 1, id 67, starts at point 0)`, `GalSpan_Orion (object 2, id 68, starts at point 0)`, `GalSpan_Orion (object 3, id 69, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (742.70, 0.00, 530.21) | None |
| 1 | (286.54, 0.00, 859.96) | None |
| 2 | (-467.12, 0.00, 622.35) | None |

### Waypoint 1

- Tag: `153`
- Members: `GalSpan_Lt_Freighter (object 5, id 66, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1104.92, -161.98, 333.94) | None |
| 1 | (419.11, -218.68, 1644.28) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 2

- Tag: `152`
- Members: `GalSpan_Carrier (object 4, id 62, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2089.75, 902.48, 4431.48) | None; listened by Event 2 for GalSpan_Carrier (object 4, id 62) |

### Waypoint 3

- Tag: `151`
- Members: `GalSpan_Shuttle_Medium (object 0, id 19, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (186.18, -579.20, 1073.32) | None |
| 1 | (-354.19, -277.78, 546.54) | None; listened by Event 1 for GalSpan_Shuttle_Medium (object 0, id 19) |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `GalSpan_Shuttle_Medium` | 19 | Interactive | 244.85,-576.04,2229.22 | 266,0,0 | secondary groups: CONT_002, none; waypoint: Waypoint 3 (tag 151, 2 point(s)), starting point 0, arrival event value 9895936 |
| 1 | `GalSpan_Orion` | 67 | Interactive | 769.54,0.00,-66.24 | 0,0,0 | group/role: FG_HADES / 0; waypoint: Waypoint 0 (tag 154, 3 point(s)), starting point 0, arrival event value 10092544 |
| 2 | `GalSpan_Orion` | 68 | Interactive | 720.34,0.00,-129.27 | 0,0,0 | group/role: FG_HADES / 2; waypoint: Waypoint 0 (tag 154, 3 point(s)), starting point 0, arrival event value 10092544 |
| 3 | `GalSpan_Orion` | 69 | Interactive | 805.31,0.00,-129.27 | 0,0,0 | group/role: FG_HADES / 3; waypoint: Waypoint 0 (tag 154, 3 point(s)), starting point 0, arrival event value 10092544 |
| 4 | `GalSpan_Carrier` | 62 | Interactive | 1747.71,0.00,2366.35 | 14,36,156 | waypoint: Waypoint 2 (tag 152, 1 point(s)), starting point 0, arrival event value 9961472 |
| 5 | `GalSpan_Lt_Freighter` | 66 | Interactive | 1289.35,-161.98,-39.69 | 469,0,0 | waypoint: Waypoint 1 (tag 153, 2 point(s)), starting point 0, arrival event value 10027008 |
