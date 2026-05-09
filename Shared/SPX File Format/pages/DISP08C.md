# Tachyon: The Fringe DISP08C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP08C.SPX` |
| Sector | `QUAD_08` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 7 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 1 |
| Events | 5 |
| Waypoints | 0 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Minelayer` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `SPIKE` |
| Aliases | `spy_1`, `SPIKE` |
| Groups | `COBALT_SPIKE` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 9, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 1 (join 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Mission objective/state: param 393217, subtype 0, param 0
- Play dialog: PLAYER.SCR, line/variant 97

### Event 1

**Trigger**

- Variable comparison: subject variable group 21, variable 2, op 1, value 3

**Action**

- Object spawn/action: Generic_Minelayer (object 0, id 9), subtype 3

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 100 (extra 1, 10; flags 2)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Variable comparison: subject variable group 21, variable 21, op 1, value 0
- Variable comparison: subject variable group 21, variable 22, op 1, value 1
- Variable comparison: subject variable group 21, variable 2, op 1, value 3

**Action**

- Play dialog: PLAYER.SCR, line/variant 104
- Set/add variable: variable group 18, variable 413, subtype 0, value 2
- Set/add variable: variable group 18, variable 412, subtype 0, value 1

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 100 (extra 1, 10; flags 2)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Variable comparison: subject variable group 21, variable 21, op 1, value 1
- Variable comparison: subject variable group 21, variable 22, op 1, value 0

**Action**

- Set/add variable: variable group 18, variable 412, subtype 0, value 1
- Set/add variable: variable group 18, variable 413, subtype 0, value 1

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 100 (extra 1, 10; flags 2)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Variable comparison: subject variable group 21, variable 21, op 1, value 1
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Set/add variable: variable group 18, variable 413, subtype 0, value 3
- Set/add variable: variable group 18, variable 412, subtype 0, value 1

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Generic_Minelayer` | 9 | Interactive | -160.53,887.68,466.76 | 0,0,0 | label: SPIKE; alias: SPIKE; secondary groups: none, COBALT_SPIKE |
