# Tachyon: The Fringe EARTH03A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH03A.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `(none)` |
| Region | 0 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 3 |
| Events | 11 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 4 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Heavy_Freighter`, `1: Generic_Light_Freighter`, `2: Shuttle_Medium` |
| Scripts | `DILL.SCR`, `FRGT.SCR`, `CPSH.SCR`, `SHUT.SCR` |
| Scenes | None |
| Labels | `SHUT`, `bfnf_03`, `PLAYER`, `ORION03`, `ORION02`, `ORION01`, `PEGASUS01`, `PEGASUS02`, `PEGASUS03`, `MAKO01`, `MAKO03`, `PIRANHA01`, `PIRANHA02`, `PIRANHA03`, `PIRANHA04`, `DART01`, `DART02`, `DART03`, `DART04`, `FRGT`, `CPSH`, `SAMA`, `FREIGHT01` |
| Aliases | `fred2`, `fred1`, `fred3` |
| Groups | `FERNANDO`, `CONT_026`, `TORRENCE`, `CONT_006`, `BRIGHTSTAR_TRADER`, `CONT_021` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0
- Mission objective/state: param 5, subtype 0, param 0
- Gate state/action: param 1, subtype 2, param 0
- Gate state/action: param 301, subtype 2, param 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 4

**Action**

- Play dialog: DILL.SCR, line/variant 6

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 45

**Action**

- Object spawn/action: GalSpan_Heavy_Freighter (object 2, id 885), subtype 3

### Event 3

**Trigger**

- Object arrival: Generic_Light_Freighter (object 1, id 343) reached Waypoint 0 (tag 3), point 2 (raw value 196610)

**Action**

- Object spawn/action: Generic_Light_Freighter (object 1, id 343), subtype 4

### Event 4

**Trigger**

- Object arrival: Generic_Light_Freighter (object 1, id 343) reached Waypoint 0 (tag 3), point 0 (raw value 196608)

**Action**

- Play dialog: FRGT.SCR, line/variant 0

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 55

**Action**

- Play dialog: CPSH.SCR, line/variant 0

### Event 6

**Trigger**

- Object event: subject Generic_Light_Freighter (object 1, id 343), op 4, value 10

**Action**

- Play dialog: FRGT.SCR, line/variant 1

### Event 7

**Trigger**

- Object event: subject GalSpan_Heavy_Freighter (object 2, id 885), op 4, value 10

**Action**

- Play dialog: CPSH.SCR, line/variant 1

### Event 8

**Trigger**

- Object event: subject Shuttle_Medium (object 0, id 309), op 4, value 10

**Action**

- Play dialog: SHUT.SCR, line/variant 0

### Event 9

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 12, variable 4, op 1, value 2
- Variable comparison: subject variable group 12, variable 0, op 1, value 1 (join 2)

**Action**

- Set runtime trigger variable: variable group 20, variable 31, subtype 0, value 0

### Event 10

**Trigger**

- Variable comparison: subject variable group 20, variable 31, op 1, value 4

**Action**

- Play dialog: DILL.SCR, line/variant 3

## Waypoints

### Waypoint 0

- Tag: `3`
- Members: `Generic_Light_Freighter (object 1, id 343, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1588.76, 0.00, 48.35) | None; listened by Event 4 for Generic_Light_Freighter (object 1, id 343) |
| 1 | (-572.14, 0.00, 731.71) | None |
| 2 | (125.50, 693.00, 5327.66) | on arrival action 1, param -1; listened by Event 3 for Generic_Light_Freighter (object 1, id 343) |

### Waypoint 1

- Tag: `2`
- Members: `GalSpan_Heavy_Freighter (object 2, id 885, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1082.41, 775.32, 5415.75) | None |
| 1 | (1050.46, 575.90, 853.18) | None |
| 2 | (578.16, 578.90, 446.10) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 2

- Tag: `1`
- Members: `Shuttle_Medium (object 0, id 309, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (711.85, 247.93, -413.10) | None |
| 1 | (785.47, 247.93, 218.61) | None |
| 2 | (298.78, 247.93, 547.89) | None |
| 3 | (-257.76, 247.93, 214.07) | None |
| 4 | (-1614.13, 247.93, -702.52) | None |
| 5 | (214.87, 247.93, -544.62) | None |
| 6 | (-328.14, 247.93, -1450.56) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Shuttle_Medium` | 309 | Interactive | -250.33,247.93,-1412.82 | 0,0,0 | label: SHUT; secondary groups: CONT_026, FERNANDO; waypoint: Waypoint 2 (tag 1, 7 point(s)), starting point 0, arrival event value 65536 |
| 1 | `Generic_Light_Freighter` | 343 | Interactive | -2003.45,0.00,170.32 | 146,0,0 | label: FRGT; secondary groups: CONT_006, TORRENCE; waypoint: Waypoint 0 (tag 3, 3 point(s)), starting point 0, arrival event value 196608 |
| 2 | `GalSpan_Heavy_Freighter` | 885 | Interactive | 1022.92,915.32,5993.36 | 256,503,0 | label: CPSH; secondary groups: CONT_021, BRIGHTSTAR_TRADER; waypoint: Waypoint 1 (tag 2, 3 point(s)), starting point 0, arrival event value 131072 |
