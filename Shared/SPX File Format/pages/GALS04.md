# Tachyon: The Fringe GALS04.SPX - Pirate Attack

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `GALS04.SPX` |
| Sector | `QUAD_04` |
| Backdrop | `GALSPA4.BDF` |
| Region | 2 |
| Sector ID | 3 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 3 |
| Events | 2 |
| Waypoints | 0 |
| Child Sectors | 1 |
| Scripts | 0 |
| Scenes | 1 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Outpost`, `1: Spcargo_Credits`, `2: Hyper_Gate` |
| Scripts | None |
| Scenes | `G4DOC02.SEN` |
| Labels | `bfge_03` |
| Aliases | `frank11` |
| Groups | `CONT_068` |
| Child Sectors | [gals04A.spx](GALS04A.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 19; flags 2)

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 23
- Set/add variable: variable group 0, variable 2, subtype 1, value 500
- Set/add variable: variable group 14, variable 806, subtype 0, value 1
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 32, op 2, value 10

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 23
- Set/add variable: variable group 20, variable 32, subtype 0, value 0

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 5 | Gate | 126.76,0.00,-94.91 | 0,0,0 | Gate SPX: [Gals01.spx](GALS01.md) |
| 1 | `Spcargo_Credits` | 19 | Interactive | -907.34,-52.02,2619.11 | 284,284,284 | secondary groups: CONT_068, none |
| 2 | `GalSpan_Outpost` | 14 | Interactive | -931.60,0.00,2513.04 | 0,0,0 | None |
