# Tachyon: The Fringe BORA05.SPX - Gate Blueprints

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `BORA05.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `BORA5.BDF` |
| Region | 3 |
| Sector ID | 4 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 5 |
| Events | 1 |
| Waypoints | 1 |
| Child Sectors | 2 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Indep_Research_Facility`, `1: Spcargo_Medical`, `2: Bora_Shuttle_Medium`, `3: Hyper_Gate` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `bfbe_08`, `bfbf_08` |
| Aliases | None |
| Groups | `FG_BORA5`, `CONT_004`, `CONT_038`, `CONT_002`, `NEW_DAWN_STATION` |
| Child Sectors | [bora05A.spx](BORA05A.md), [bora05B.spx](BORA05B.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 2166; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 63
- Set/add variable: variable group 15, variable 805, subtype 0, value 1

## Waypoints

### Waypoint 0

- Tag: `2`
- Members: `Bora_Shuttle_Medium (object 1, id 253, starts at point 0)`, `Bora_Shuttle_Medium (object 2, id 254, starts at point 4)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (686.48, 1354.78, 370.34) | None |
| 1 | (1338.37, 374.78, 1612.07) | None |
| 2 | (1980.50, -920.88, 2967.71) | None |
| 3 | (1386.80, -910.18, 4381.57) | None |
| 4 | (-1145.77, -910.18, 4344.25) | None |
| 5 | (-2514.36, -920.89, 3038.42) | None |
| 6 | (-887.55, -551.95, 811.47) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 2 | Gate | -1885.14,0.00,592.04 | 78,0,0 | Gate SPX: [bora01.spx](BORA01.md) |
| 1 | `Bora_Shuttle_Medium` | 253 | Interactive | 442.93,1317.08,262.59 | 128,0,0 | group/role: FG_BORA5 / 0; secondary groups: CONT_004, none; waypoint: Waypoint 0 (tag 2, 7 point(s)), starting point 0, arrival event value 131072 |
| 2 | `Bora_Shuttle_Medium` | 254 | Interactive | -763.16,-899.47,4515.55 | 0,0,0 | group/role: FG_BORA5 / 0; secondary groups: CONT_038, none; waypoint: Waypoint 0 (tag 2, 7 point(s)), starting point 4, arrival event value 131076 |
| 3 | `Spcargo_Medical` | 2166 | Interactive | 393.84,32.05,3733.66 | 0,0,0 | secondary groups: CONT_002, none |
| 4 | `Bora_Indep_Research_Facility` | 255 | Interactive | 8.11,0.00,3373.23 | 0,0,0 | secondary groups: none, NEW_DAWN_STATION |
