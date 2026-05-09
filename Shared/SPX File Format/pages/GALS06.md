# Tachyon: The Fringe GALS06.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `GALS06.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `GALSPA6.BDF` |
| Region | 2 |
| Sector ID | 5 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 4 |
| Events | 1 |
| Waypoints | 0 |
| Child Sectors | 2 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Research_Facility`, `1: Spcargo_Food`, `2: Mega_Gate`, `3: Hyper_Gate` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | None |
| Aliases | `wing_man` |
| Groups | `CONT_063` |
| Child Sectors | [gals06A.spx](GALS06A.md), [gals06B.spx](GALS06B.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 120; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 47
- Set/add variable: variable group 14, variable 802, subtype 0, value 1

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | -1093.75,-127.50,887.88 | 146,0,0 | Gate SPX: [GAls05.spx](GALS05.md) |
| 1 | `Mega_Gate` | 2 | Gate | 100.95,323.02,-243.40 | 14,7,470 | Gate SPX: [Disp08.spx](DISP08.md) |
| 2 | `Spcargo_Food` | 120 | Interactive | 569.04,-259.40,1202.74 | 448,469,71 | secondary groups: CONT_063, none |
| 3 | `GalSpan_Research_Facility` | 43 | Interactive | 351.40,0.00,895.07 | 0,0,0 | None |
