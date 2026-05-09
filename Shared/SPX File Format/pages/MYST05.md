# Tachyon: The Fringe MYST05.SPX - Lost To The Fog

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST05.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `MYSTER5.BDF` |
| Region | 5 |
| Sector ID | 4 |
| SectorHazardFlags | Radiation hazard, Twilight fog / fog-radar impairment (0x00000003) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 5 |
| Entities | 5 |
| Events | 1 |
| Waypoints | 0 |
| Child Sectors | 2 |
| Scripts | 0 |
| Scenes | 1 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: AI_Landing_Platform`, `1: Mad_Pirate_Platform`, `2: Cassitor_Main_Station`, `3: Spcargo_Art`, `4: Hyper_Gate` |
| Scripts | None |
| Scenes | `M5LAN01.SEN` |
| Labels | `WRKR1`, `WRKR2` |
| Aliases | `Will_02` |
| Groups | `CONT_061` |
| Child Sectors | [myst05A.spx](MYST05A.md), [myst05B.spx](MYST05B.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 76; flags 2)

**Action**

- Set/add variable: variable group 17, variable 802, subtype 0, value 1

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | -924.38,1346.49,88.94 | 0,456,0 | Gate SPX: [myst03.spx](MYST03.md) |
| 1 | `Spcargo_Art` | 76 | Interactive | -311.02,1979.60,2937.38 | 0,0,0 | secondary groups: CONT_061, none |
| 2 | `Cassitor_Main_Station` | 10 | Interactive | -302.45,1867.31,2955.61 | 0,0,0 | None |
| 3 | `Mad_Pirate_Platform` | 34 | Interactive | -912.04,360.24,1307.57 | 64,0,0 | None |
| 4 | `AI_Landing_Platform` | 41 | Interactive | 225.25,360.07,1307.60 | 448,0,0 | None |
