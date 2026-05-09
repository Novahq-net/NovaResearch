# Tachyon: The Fringe BORA08.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `BORA08.SPX` |
| Sector | `QUAD_08` |
| Backdrop | `BORA8.BDF` |
| Region | 3 |
| Sector ID | 7 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 5 |
| Entities | 8 |
| Events | 2 |
| Waypoints | 0 |
| Child Sectors | 1 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Colony_Station`, `1: Bora_Indep_Mining_Facility`, `2: Spcargo_Food`, `3: Mega_Gate`, `4: Hyper_Gate` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFBE_08` |
| Aliases | None |
| Groups | `CONT_063`, `DARKSTONE_MINING`, `NEW_DOVER_MINING`, `NEW_GAIA`, `NEW_ATLANTIS` |
| Child Sectors | [bora08A.spx](BORA08A.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 43; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 64
- Set/add variable: variable group 15, variable 803, subtype 0, value 1

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 44; flags 2)

**Action**

- Set/add variable: variable group 15, variable 804, subtype 0, value 1

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 3 | Gate | 291.17,0.00,-729.74 | 0,0,0 | Gate SPX: [bora07.spx](BORA07.md) |
| 1 | `Mega_Gate` | 4 | Gate | -1257.86,0.00,-1734.17 | 75,0,0 | Gate SPX: [disp01.spx](DISP01.md) |
| 2 | `Spcargo_Food` | 43 | Interactive | 2354.18,432.86,-2194.61 | 0,0,0 | secondary groups: CONT_063, none |
| 3 | `Spcargo_Food` | 44 | Interactive | 2676.77,432.96,-1257.21 | 0,0,0 | secondary groups: CONT_063, none |
| 4 | `Bora_Indep_Mining_Facility` | 5 | Interactive | -2207.83,0.00,3368.75 | 0,0,0 | secondary groups: none, DARKSTONE_MINING |
| 5 | `Bora_Indep_Mining_Facility` | 6 | Interactive | 2521.88,0.00,-1699.24 | 154,0,0 | secondary groups: none, NEW_DOVER_MINING |
| 6 | `Generic_Colony_Station` | 7 | Interactive | 2838.98,0.00,4700.63 | 385,0,0 | secondary groups: none, NEW_GAIA |
| 7 | `Generic_Colony_Station` | 8 | Interactive | -3427.51,0.00,-702.40 | 210,0,0 | secondary groups: none, NEW_ATLANTIS |
