# Tachyon: The Fringe EARTH10G.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH10G.SPX` |
| Sector | `QUAD_10` |
| Backdrop | `(none)` |
| Region | 0 |
| Sector ID | 9 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 1 |
| Events | 4 |
| Waypoints | 0 |
| Child Sectors | 0 |
| Scripts | 0 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Sol_Training_Course` |
| Scripts | None |
| Scenes | None |
| Labels | None |
| Aliases | None |
| Groups | None |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 0, value 1

### Event 1

**Trigger**

- Variable comparison: subject variable group 0, variable 21, op 2, value 4

**Action**

- Show/update HUD contact: contact/list 0, subtype 12, param 30

### Event 2

**Trigger**

- Variable comparison: subject variable group 0, variable 21, op 2, value 4

**Action**

- Set/add variable: variable group 21, variable 20, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 0, variable 21, op 2, value 0

**Action**

- Set/add variable: variable group 12, variable 200, subtype 0, value 1
- Set/add variable: variable group 12, variable 201, subtype 0, value 2

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Sol_Training_Course` | 2 | Interactive | 879.51,0.00,2689.92 | 0,0,0 | None |
