# Tachyon: The Fringe BORA07.SPX - Sour Colony

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `BORA07.SPX` |
| Sector | `QUAD_07` |
| Backdrop | `BORA7.BDF` |
| Region | 3 |
| Sector ID | 6 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 4 |
| Events | 2 |
| Waypoints | 0 |
| Child Sectors | 2 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Spcargo_Credits`, `1: Hyper_Gate` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | None |
| Aliases | None |
| Groups | `CONT_067` |
| Child Sectors | [bora07A.spx](BORA07A.md), [bora07B.spx](BORA07B.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 7; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 128
- Set/add variable: variable group 0, variable 2, subtype 1, value 250
- Show/update HUD contact: contact/list 0, subtype 9, param 22
- Set/add variable: variable group 15, variable 807, subtype 0, value 1
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 32, op 2, value 10

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 22
- Set/add variable: variable group 20, variable 32, subtype 0, value 0

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 4 | Gate | 961.67,0.00,549.89 | 313,0,0 | Gate SPX: [bora06.spx](BORA06.md) |
| 1 | `Hyper_Gate` | 5 | Gate | 81.88,0.00,-1800.81 | 57,0,0 | Gate SPX: [bora01.spx](BORA01.md) |
| 2 | `Hyper_Gate` | 6 | Gate | 2457.10,0.00,-937.28 | 448,0,0 | Gate SPX: [bora08.spx](BORA08.md) |
| 3 | `Spcargo_Credits` | 7 | Interactive | 1156.02,-1100.00,-900.82 | 64,441,405 | secondary groups: CONT_067, none |
