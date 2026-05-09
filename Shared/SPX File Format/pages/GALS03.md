# Tachyon: The Fringe GALS03.SPX - Color of the Nose.

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `GALS03.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `GALSPA3.BDF` |
| Region | 2 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 3 |
| Events | 1 |
| Waypoints | 0 |
| Child Sectors | 1 |
| Scripts | 1 |
| Scenes | 1 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Construction_Facility`, `1: Spcargo_Mining`, `2: Hyper_Gate` |
| Scripts | `PLAYER.SCR` |
| Scenes | `G3GC041A.SEN` |
| Labels | `BFGF_01`, `BFGE_01`, `explode` |
| Aliases | None |
| Groups | `CONT_027` |
| Child Sectors | [gals03A.spx](GALS03A.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 503; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 46
- Set/add variable: variable group 14, variable 803, subtype 0, value 1

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 4 | Gate | -2.15,0.00,-107.08 | 0,0,0 | Gate SPX: [Gals02.spx](GALS02.md) |
| 1 | `Spcargo_Mining` | 503 | Interactive | -393.09,503.06,4708.53 | 0,498,64 | secondary groups: CONT_027, none |
| 2 | `GalSpan_Construction_Facility` | 348 | Interactive | -1624.74,0.00,3787.44 | 81,0,0 | None |
