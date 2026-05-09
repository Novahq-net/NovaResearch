# Tachyon: The Fringe NEUT01F.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT01F.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 5 |
| Events | 8 |
| Waypoints | 4 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Lt_Freighter`, `1: Wingman_Mishka`, `2: Shuttle_Medium`, `3: Shuttle_Small` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `MISHK`, `FakeJake`, `Daymir` |
| Aliases | `Courage`, `kwi03_7`, `Jerome26`, `Jerome25`, `Jerome24`, `Jerome22`, `Jerome21`, `Jerome20`, `kevin01`, `Intrepid`, `kwI03_10`, `SHIP1_HYPER`, `ohshit`, `SHIP2_HYPER`, `SHIP3_HYPER` |
| Groups | `MISHKA_DWEATHERS`, `HESPERIDES`, `CONT_044` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Gate state/action: param 67, subtype 3, param 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 13, variable 412, op 1, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 20, subtype 0, value 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 9, value 0

**Action**

- Object spawn/action: GalSpan_Lt_Freighter (object 4, id 581), subtype 5

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 20, op 1, value 15

**Action**

- Object spawn/action: Shuttle_Small (object 0, id 390), subtype 1, param 64
- Set runtime trigger variable: variable group 20, variable 20, subtype 1, value 0

### Event 4

**Trigger**

- Object arrival: GalSpan_Lt_Freighter (object 4, id 581) reached Waypoint 0 (tag 353), point 1 (raw value 23134209)
- Sector/startup condition family: subject 0, op 0, value 78

**Action**

- Object spawn/action: GalSpan_Lt_Freighter (object 4, id 581), subtype 4

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 3600 (extra 1, 581; flags 2)
- Area/player/sector/dock/time event: subject 0, op 9, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 78

### Event 6

**Trigger**

- Object event: subject Wingman_Mishka (object 3, id 459), op 2, value 0

**Action**

- Set/add variable: variable group 13, variable 801, subtype 0, value 0

### Event 7

**Trigger**

- Object event: subject Wingman_Mishka (object 3, id 459), op 2, value 0
- Variable comparison: subject variable group 13, variable 413, op 0, value 3

**Action**

- Set/add variable: variable group 13, variable 413, subtype 0, value 2

## Waypoints

### Waypoint 0

- Tag: `353`
- Members: `GalSpan_Lt_Freighter (object 4, id 581, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (6435.89, 412.23, -9254.91) | None |
| 1 | (7376.62, 261.98, -10166.51) | None; listened by Event 4 for GalSpan_Lt_Freighter (object 4, id 581) |

### Waypoint 1

- Tag: `352`
- Members: `Wingman_Mishka (object 3, id 459, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (5446.04, -6.12, -8771.65) | None |
| 1 | (1194.08, 515.70, -8286.82) | None |
| 2 | (756.85, 446.94, -8298.03) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 2

- Tag: `351`
- Members: `Shuttle_Small (object 0, id 390, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (7828.05, -413.25, -4675.80) | None |
| 1 | (6188.12, -427.50, -7147.87) | None |
| 2 | (5148.50, -285.00, -7246.75) | None |

### Waypoint 3

- Tag: `99`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2998.26, 0.00, -8331.36) | None |
| 1 | (3005.50, 669.66, -11111.18) | None |
| 2 | (2986.38, 6119.70, -11830.52) | on arrival action 1, param -1 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Shuttle_Small` | 390 | Interactive | 9657.79,0.00,-5134.05 | 0,0,0 | waypoint: Waypoint 2 (tag 351, 3 point(s)), starting point 0, arrival event value 23003136 |
| 1 | `Shuttle_Medium` | 511 | Interactive | 1309.57,300.91,-9854.26 | 7,0,0 | None |
| 2 | `Shuttle_Medium` | 512 | Interactive | 1275.95,301.24,-9617.67 | 192,0,0 | None |
| 3 | `Wingman_Mishka` | 459 | Interactive | 7501.07,0.00,-10854.56 | 0,0,0 | label: MISHK; alias: kwi03_7; secondary groups: none, MISHKA_DWEATHERS; waypoint: Waypoint 1 (tag 352, 3 point(s)), starting point 0, arrival event value 23068672 |
| 4 | `GalSpan_Lt_Freighter` | 581 | Interactive | 5570.78,519.50,-8169.30 | 199,498,0 | alias: kwI03_10; secondary groups: CONT_044, HESPERIDES; waypoint: Waypoint 0 (tag 353, 2 point(s)), starting point 0, arrival event value 23134208 |
