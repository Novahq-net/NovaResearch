# Tachyon: The Fringe NEUT01H.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT01H.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 5 |
| Events | 4 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 0 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Science_Vessel`, `1: Generic_Light_Freighter`, `2: Shuttle_Small`, `3: Shuttle_Medium` |
| Scripts | None |
| Scenes | None |
| Labels | `MISHK`, `FakeJake`, `Daymir` |
| Aliases | `Courage`, `kwi03_7`, `Jerome26`, `Jerome25`, `Jerome24`, `Jerome22`, `Jerome21`, `Jerome20`, `kevin01`, `Intrepid`, `kwI03_10`, `SHIP1_HYPER`, `ohshit`, `SHIP2_HYPER`, `SHIP3_HYPER` |
| Groups | None |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Gate state/action: param 67, subtype 3, param 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 26, subtype 0, value 0

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 26, op 1, value 8

**Action**

- Object spawn/action: Shuttle_Medium (object 0, id 484), subtype 1, param 64

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 26, op 1, value 17

**Action**

- Object spawn/action: Shuttle_Medium (object 1, id 485), subtype 1, param 64
- Set runtime trigger variable: variable group 20, variable 26, subtype 1, value 0

## Waypoints

### Waypoint 0

- Tag: `453`
- Members: `Shuttle_Small (object 2, id 543, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (3928.20, 112.45, -6327.67) | None |
| 1 | (3966.49, 0.00, -6813.33) | None |
| 2 | (3998.75, -85.29, -6358.82) | None |
| 3 | (4171.40, -75.12, -6574.72) | None |
| 4 | (4181.76, 77.69, -6842.96) | None |
| 5 | (3932.57, 84.88, -6583.15) | on arrival redirect to Waypoint 0 (tag 453), point 0 |

### Waypoint 1

- Tag: `452`
- Members: `Shuttle_Medium (object 1, id 485, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (7113.50, 0.00, -5529.83) | None |
| 1 | (6707.50, 666.28, -8372.57) | None |
| 2 | (1361.83, 407.44, -9778.07) | None |

### Waypoint 2

- Tag: `451`
- Members: `Shuttle_Medium (object 0, id 484, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (6735.80, 470.91, -5018.39) | None |
| 1 | (2397.60, 415.87, -4423.92) | on arrival activate current object (raw param -1 ignored) |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Shuttle_Medium` | 484 | Interactive | 9151.61,0.00,-4641.71 | 341,0,0 | waypoint: Waypoint 2 (tag 451, 2 point(s)), starting point 0, arrival event value 29556736 |
| 1 | `Shuttle_Medium` | 485 | Interactive | 9241.08,0.00,-4449.29 | 327,0,0 | waypoint: Waypoint 1 (tag 452, 3 point(s)), starting point 0, arrival event value 29622272 |
| 2 | `Shuttle_Small` | 543 | Interactive | 4077.81,165.37,-6042.16 | 256,0,0 | waypoint: Waypoint 0 (tag 453, 6 point(s)), starting point 0, arrival event value 29687808 |
| 3 | `Generic_Light_Freighter` | 483 | Interactive | 4326.38,516.53,-10494.58 | 156,0,0 | None |
| 4 | `Science_Vessel` | 542 | Interactive | 4088.43,-27.11,-6662.54 | 0,0,0 | None |
