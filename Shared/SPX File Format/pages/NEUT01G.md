# Tachyon: The Fringe NEUT01G.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT01G.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 4 |
| Events | 3 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Minetender`, `1: Luxury_Liner`, `2: Generic_Light_Freighter`, `3: Shuttle_Medium` |
| Scripts | `ANNAH.SCR` |
| Scenes | None |
| Labels | `MISHK`, `FakeJake`, `Daymir` |
| Aliases | `Courage`, `kwi03_7`, `Jerome26`, `Jerome25`, `Jerome24`, `Jerome22`, `Jerome21`, `Jerome20`, `kevin01`, `Intrepid`, `kwI03_10`, `SHIP1_HYPER`, `ohshit`, `SHIP2_HYPER`, `SHIP3_HYPER` |
| Groups | `CONT_033` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Gate state/action: param 67, subtype 3, param 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 1500 (extra 1, 66; flags 3)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Object spawn/action: Generic_Light_Freighter (object 1, id 435), subtype 1, param 64

### Event 2

**Trigger**

- Variable comparison: subject variable group 0, variable 4, op 1, value 4009
- Area/player/sector/dock/time event: subject 0, op 9, value 0

**Action**

- Play dialog: ANNAH.SCR, line/variant 5

## Waypoints

### Waypoint 0

- Tag: `402`
- Members: `Luxury_Liner (object 2, id 515, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (5828.21, 257.19, -11449.76) | None |
| 1 | (4401.16, 267.27, -9821.79) | None |
| 2 | (4376.86, 275.21, -7682.02) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 1

- Tag: `401`
- Members: `Generic_Light_Freighter (object 1, id 435, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (6705.97, -368.93, -5666.57) | None |
| 1 | (3076.74, 276.69, -5360.67) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Shuttle_Medium` | 414 | Interactive | 1955.07,139.45,-5330.59 | 386,491,84 | None |
| 1 | `Generic_Light_Freighter` | 435 | Interactive | 9180.58,0.00,-4210.73 | 323,0,98 | waypoint: Waypoint 1 (tag 401, 2 point(s)), starting point 0, arrival event value 26279936 |
| 2 | `Luxury_Liner` | 515 | Interactive | 6691.56,341.66,-12774.21 | 462,0,0 | secondary groups: CONT_033, none; waypoint: Waypoint 0 (tag 402, 3 point(s)), starting point 0, arrival event value 26345472 |
| 3 | `Generic_Minetender` | 670 | Interactive | 5736.13,0.00,-6070.19 | 128,0,0 | None |
