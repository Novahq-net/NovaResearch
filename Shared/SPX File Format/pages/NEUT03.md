# Tachyon: The Fringe NEUT03.SPX - Advance with Courage; Deja Vu

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT03.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `NEUTRA3.BDF` |
| Region | 1 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 3 |
| Events | 2 |
| Waypoints | 0 |
| Child Sectors | 1 |
| Scripts | 1 |
| Scenes | 1 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Spcargo_Mining`, `1: Mega_Gate`, `2: Hyper_Gate` |
| Scripts | `PLAYER.SCR` |
| Scenes | `H3GC020A.SEN` |
| Labels | `OBULO`, `BFIGH`, `G02BFA`, `BFGE_07`, `G02BRB`, `HERID` |
| Aliases | `fred_fighter1`, `fred_fighter2`, `fred_freighter1`, `fred_freighter2` |
| Groups | `CONT_027` |
| Child Sectors | [neut03A.spx](NEUT03A.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 1555; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 126
- Set/add variable: variable group 13, variable 807, subtype 0, value 1

### Event 1

**Trigger**

- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Object spawn/action: Spcargo_Mining (object 2, id 1555), subtype 0

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1040 | Gate | 4165.50,224.92,-3842.95 | 492,487,0 | Gate SPX: [neut02.spx](NEUT02.md) |
| 1 | `Mega_Gate` | 1041 | Gate | -77.17,0.00,10597.82 | 256,0,0 | Gate SPX: [bora03.spx](BORA03.md) |
| 2 | `Spcargo_Mining` | 1555 | Interactive | -257.13,-28.96,10845.38 | 329,111,169 | secondary groups: CONT_027, none |
