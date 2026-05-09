# Tachyon: The Fringe MYST04.SPX - Descent into Madness; Final Retribution

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST04.SPX` |
| Sector | `QUAD_04` |
| Backdrop | `MYSTER4.BDF` |
| Region | 5 |
| Sector ID | 3 |
| SectorHazardFlags | Twilight fog / fog-radar impairment (0x00000002) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 4 |
| Events | 1 |
| Waypoints | 0 |
| Child Sectors | 1 |
| Scripts | 1 |
| Scenes | 1 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Cassitor_Control_Array`, `1: Cassitor_Production_Facility`, `2: Spcargo_Parts`, `3: Hyper_Gate` |
| Scripts | `PLAYER.SCR` |
| Scenes | `M4GC060A.SEN` |
| Labels | None |
| Aliases | None |
| Groups | `CONT_060` |
| Child Sectors | [myst04A.spx](MYST04A.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 259; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 133
- Set/add variable: variable group 17, variable 803, subtype 0, value 1

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 2 | Gate | -1820.31,642.64,2086.41 | 244,0,0 | Gate SPX: [myst03.spx](MYST03.md) |
| 1 | `Spcargo_Parts` | 259 | Interactive | -4002.32,-619.65,254.94 | 0,0,449 | secondary groups: CONT_060, none |
| 2 | `Cassitor_Production_Facility` | 190 | Interactive | -2165.38,0.00,899.75 | 0,0,0 | None |
| 3 | `Cassitor_Control_Array` | 191 | Interactive | -55.74,-170.08,-149.63 | 0,0,0 | None |
