# Tachyon: The Fringe DISP01C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP01C.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 1 |
| Events | 3 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Light_Freighter` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `TNSA`, `SPIKE`, `capb` |
| Aliases | `BC10_Claymore4`, `BC10_Claymore1`, `BC10_Claymore3`, `BC10_Claymore2`, `BC10_Waraxe`, `tnsa`, `BC10_Mace4`, `BC10_Mace2`, `BC10_Mace1`, `BC10_Mace3`, `BC10_Warhammer3`, `BC10_Warhammer2`, `BC10_Warhammer4`, `BC10_Warhammer1`, `SPIKE`, `Stocks01` |
| Groups | None |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 10

**Action**

- Play dialog: PLAYER.SCR, line/variant 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 27, op 1, value 1

**Action**

- Set/add variable: variable group 18, variable 400, subtype 0, value 1
- Set/add variable: variable group 18, variable 401, subtype 0, value 2

## Waypoints

### Waypoint 0

- Tag: `210`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (719.68, 0.00, -3712.08) | None |
| 1 | (-3772.93, 0.00, -904.08) | None |
| 2 | (-3348.54, 0.00, 1739.87) | None |
| 3 | (2010.63, 0.00, 3131.63) | None |
| 4 | (3211.24, 0.00, -185.53) | on arrival redirect to Waypoint 0 (tag 210), point 4 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Generic_Light_Freighter` | 475 | Interactive | 943.41,0.00,-4165.56 | 0,0,0 | None |
