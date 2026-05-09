# Tachyon: The Fringe NEUT05.SPX - Recoil; Hospital Emergency; The Rory Sting

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT05.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `NEUTRA5.BDF` |
| Region | 1 |
| Sector ID | 4 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 4 |
| Events | 2 |
| Waypoints | 0 |
| Child Sectors | 8 |
| Scripts | 0 |
| Scenes | 1 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Star_Patrol_Station`, `1: Spcargo_Medical`, `2: Hyper_Gate` |
| Scripts | None |
| Scenes | `H1BC012A.SEN` |
| Labels | `aobul` |
| Aliases | `bagel`, `bagel_1`, `bagel_2`, `oside`, `oside_1`, `oside_2`, `Will_01`, `SHIP1_HYPER`, `ohshit`, `SHIP3_HYPER`, `SHIP2_HYPER` |
| Groups | `CONT_002` |
| Child Sectors | [neut05A.spx](NEUT05A.md), [neut05B.spx](NEUT05B.md), [neut05C.spx](NEUT05C.md), [neut05D.spx](NEUT05D.md), [neut05E.spx](NEUT05E.md), [neut05F.spx](NEUT05F.md), [neut05G.spx](NEUT05G.md), [neut05H.spx](NEUT05H.md) |

## Events

### Event 0

**Trigger**

- Variable comparison: subject variable group 0, variable 0, op 1, value 2 (join 2)

**Action**

- Object spawn/action: Spcargo_Medical (object 2, id 1385), subtype 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 1385; flags 2)

**Action**

- Set/add variable: variable group 13, variable 806, subtype 0, value 1

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 6 | Gate | 470.74,0.00,2806.05 | 257,0,0 | Gate SPX: [neut06.spx](NEUT06.md) |
| 1 | `Hyper_Gate` | 7 | Gate | 409.79,0.00,-843.42 | 0,0,0 | Gate SPX: [neut01.spx](NEUT01.md) |
| 2 | `Spcargo_Medical` | 1385 | Interactive | 434.25,-1060.00,1315.80 | 0,0,0 | secondary groups: CONT_002, none |
| 3 | `Star_Patrol_Station` | 858 | Interactive | 434.93,-247.02,1315.39 | 0,0,0 | None |
