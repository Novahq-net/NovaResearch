# Tachyon: The Fringe FRON09.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON09.SPX` |
| Sector | `QUAD_09` |
| Backdrop | `FRONTI9.BDF` |
| Region | 4 |
| Sector ID | 8 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 5 |
| Entities | 11 |
| Events | 1 |
| Waypoints | 0 |
| Child Sectors | 3 |
| Scripts | 0 |
| Scenes | 2 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Mad_Pirate_Platform`, `1: Gun_Platform1`, `2: Baron_Hajod_Station`, `3: Spcargo_Art`, `4: Hyper_Gate` |
| Scripts | None |
| Scenes | `F9GC030A.SEN`, `F9I1500A.SEN` |
| Labels | `BFNE_04`, `BFNE_02`, `BFNE_07` |
| Aliases | None |
| Groups | `CONT_061` |
| Child Sectors | [fron09B.spx](FRON09B.md), [fron09C.spx](FRON09C.md), [fron09D.spx](FRON09D.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 191; flags 2)

**Action**

- Set/add variable: variable group 16, variable 806, subtype 0, value 1

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | -605.63,0.00,818.41 | 385,511,476 | Gate SPX: [fron08.spx](FRON08.md) |
| 1 | `Spcargo_Art` | 191 | Interactive | -5708.34,-1360.72,986.27 | 107,0,0 | secondary groups: CONT_061, none |
| 2 | `Baron_Hajod_Station` | 2 | Interactive | -3752.65,-844.86,-400.03 | 118,0,0 | None |
| 3 | `Gun_Platform1` | 22 | Interactive | -880.39,1.37,1621.68 | 0,0,0 | None |
| 4 | `Gun_Platform1` | 26 | Interactive | -881.81,9.48,491.87 | 0,0,0 | None |
| 5 | `Gun_Platform1` | 27 | Interactive | -1697.42,48.56,491.87 | 0,0,0 | None |
| 6 | `Gun_Platform1` | 28 | Interactive | -2488.99,22.51,476.99 | 0,0,506 | None |
| 7 | `Gun_Platform1` | 29 | Interactive | -1625.95,0.00,1632.17 | 0,0,0 | None |
| 8 | `Gun_Platform1` | 30 | Interactive | -2334.81,0.00,1642.86 | 0,0,0 | None |
| 9 | `Gun_Platform1` | 121 | Interactive | -595.85,0.00,1041.09 | 0,0,128 | None |
| 10 | `Mad_Pirate_Platform` | 190 | Interactive | -3752.89,-315.63,-1173.28 | 374,0,0 | None |
