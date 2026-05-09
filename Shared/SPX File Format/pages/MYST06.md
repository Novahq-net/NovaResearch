# Tachyon: The Fringe MYST06.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST06.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `MYSTER6.BDF` |
| Region | 5 |
| Sector ID | 5 |
| SectorHazardFlags | Twilight fog / fog-radar impairment (0x00000002) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 4 |
| Events | 2 |
| Waypoints | 0 |
| Child Sectors | 4 |
| Scripts | 0 |
| Scenes | 2 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Mega_Gate`, `1: Hyper_Gate` |
| Scripts | None |
| Scenes | `M6BC041A.SEN`, `M6BC070A.SEN` |
| Labels | `PISCE`, `RALPH` |
| Aliases | `PISCES1`, `PISCES2`, `pisces3`, `pisces4`, `stocks02` |
| Groups | None |
| Child Sectors | [myst06A.spx](MYST06A.md), [myst06B.spx](MYST06B.md), [myst06C.spx](MYST06C.md), [myst06D.spx](MYST06D.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4024

**Action**

- Gate state/action: param 4, subtype 3, param 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 3007

**Action**

- Gate state/action: param 4, subtype 3, param 0

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | -616.73,200.00,364.79 | 162,469,0 | Gate SPX: [myst01.spx](MYST01.md) |
| 1 | `Hyper_Gate` | 2 | Gate | 485.96,0.00,477.25 | 368,0,0 | Gate SPX: [myst02.spx](MYST02.md) |
| 2 | `Hyper_Gate` | 3 | Gate | 654.77,-300.00,-544.69 | 0,43,0 | Gate SPX: [myst07.spx](MYST07.md) |
| 3 | `Mega_Gate` | 4 | Gate | -443.92,100.00,-448.68 | 65,498,0 | Gate SPX: [fron02.spx](FRON02.md) |
