# Tachyon: The Fringe FRON12.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON12.SPX` |
| Sector | `QUAD_12` |
| Backdrop | `FRONTI12.BDF` |
| Region | 4 |
| Sector ID | 11 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 5 |
| Entities | 11 |
| Events | 8 |
| Waypoints | 1 |
| Child Sectors | 5 |
| Scripts | 0 |
| Scenes | 1 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Redship_Casino_Station`, `1: GalSpan_Cruiser`, `2: Spcargo_Credits`, `3: Spcargo_Contraband`, `4: Hyper_Gate` |
| Scripts | None |
| Scenes | `F12BC02A.SEN` |
| Labels | `BFNF_01`, `BFGE_01`, `BFNE_02` |
| Aliases | `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1`, `Stocks01` |
| Groups | `CONT_029`, `CONT_066`, `PERSEPHONE`, `CONT_034` |
| Child Sectors | [fron12A.spx](FRON12A.md), [fron12B.spx](FRON12B.md), [fron12C.spx](FRON12C.md), [fron12D.spx](FRON12D.md), [fron12E.spx](FRON12E.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 7, op 1, value 1
- Variable comparison: subject variable group 0, variable 4, op 1, value 4025

**Action**

- Object spawn/action: GalSpan_Cruiser (object 9, id 1333), subtype 20
- Object spawn/action: GalSpan_Cruiser (object 9, id 1333), subtype 17
- Object spawn/action: GalSpan_Cruiser (object 9, id 1333), subtype 5

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 1440; flags 2)

**Action**

- Object spawn/action: Redship_Casino_Station (object 10, id 1366), subtype 8, param 9
- Set/add variable: variable group 16, variable 804, subtype 0, value 1

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 1441; flags 2)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 100
- Object spawn/action: Redship_Casino_Station (object 10, id 1366), subtype 8, param 9
- Show/update HUD contact: contact/list 0, subtype 9, param 41
- Set/add variable: variable group 16, variable 811, subtype 0, value 1
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 1443; flags 2)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 100
- Object spawn/action: Redship_Casino_Station (object 10, id 1366), subtype 8, param 9
- Set/add variable: variable group 16, variable 812, subtype 0, value 1

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 1445; flags 2)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 100
- Object spawn/action: Redship_Casino_Station (object 10, id 1366), subtype 8, param 9
- Set/add variable: variable group 16, variable 813, subtype 0, value 1

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 1447; flags 2)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 100
- Object spawn/action: Redship_Casino_Station (object 10, id 1366), subtype 8, param 9
- Set/add variable: variable group 16, variable 814, subtype 0, value 1

### Event 6

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 1449; flags 2)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 100
- Object spawn/action: Redship_Casino_Station (object 10, id 1366), subtype 8, param 9
- Set/add variable: variable group 16, variable 815, subtype 0, value 1

### Event 7

**Trigger**

- Variable comparison: subject variable group 20, variable 32, op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 41
- Set/add variable: variable group 20, variable 32, subtype 0, value 0

## Waypoints

### Waypoint 0

- Tag: `51`
- Members: `GalSpan_Cruiser (object 9, id 1333, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1870.36, 227.00, 329.68) | None |
| 1 | (-1657.65, 257.00, 442.32) | None |
| 2 | (-1462.98, 303.00, 548.36) | on arrival action 1, param -1 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | 184.88,0.00,-772.37 | 0,0,0 | Gate SPX: [fron11.spx](FRON11.md) |
| 1 | `Hyper_Gate` | 2 | Gate | -2848.07,0.00,-2.14 | 119,0,0 | Gate SPX: [fron07.spx](FRON07.md) |
| 2 | `Hyper_Gate` | 3 | Gate | 3593.73,0.00,1925.93 | 0,0,0 | Gate SPX: [fron07.spx](FRON07.md) |
| 3 | `Spcargo_Contraband` | 1440 | Interactive | 3089.31,-310.12,272.12 | 0,0,0 | secondary groups: CONT_029, none |
| 4 | `Spcargo_Credits` | 1441 | Interactive | 2570.51,336.45,824.63 | 0,0,0 | secondary groups: CONT_066, none |
| 5 | `Spcargo_Credits` | 1443 | Interactive | 2571.26,337.99,824.61 | 0,0,0 | secondary groups: CONT_066, none |
| 6 | `Spcargo_Credits` | 1445 | Interactive | 2572.02,336.45,824.63 | 0,0,0 | secondary groups: CONT_066, none |
| 7 | `Spcargo_Credits` | 1447 | Interactive | 2550.77,336.47,862.56 | 0,0,0 | secondary groups: CONT_066, none |
| 8 | `Spcargo_Credits` | 1449 | Interactive | 2537.29,336.47,826.60 | 0,0,0 | secondary groups: CONT_066, none |
| 9 | `GalSpan_Cruiser` | 1333 | Interactive | -2845.95,196.23,7.80 | 105,0,0 | alias: Stocks01; secondary groups: CONT_034, PERSEPHONE; waypoint: Waypoint 0 (tag 51, 3 point(s)), starting point 0, arrival event value 3342336 |
| 10 | `Redship_Casino_Station` | 1366 | Interactive | 2067.29,0.00,993.78 | 28,0,0 | None |
