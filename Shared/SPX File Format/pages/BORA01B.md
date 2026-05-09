# Tachyon: The Fringe BORA01B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `BORA01B.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 3 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 7 |
| Events | 3 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 0 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Hvy_Freighter`, `1: Bora_Destroyer`, `2: Bora_Mace`, `3: Bora_Warhammer` |
| Scripts | None |
| Scenes | None |
| Labels | `chaas` |
| Aliases | `frank01`, `frank04`, `frank03`, `frank02` |
| Groups | `FG_TRIDENT`, `FG_INSURRECTION`, `JUDGEMENT`, `CONT_023`, `PILE_DRIVER`, `CONT_021` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 7

**Action**

- Object spawn/action: Bora_Destroyer (object 5, id 1079), subtype 4

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 21, op 1, value 2

**Action**

- Broadcast HUD contact action: contact/list 0, subtype 0, param 9
- Object spawn/action: id 1007, subtype 14
- Mission objective/state: param 196612, subtype 0, param 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 2

**Action**

- Broadcast HUD contact action: contact/list 0, subtype 0, param 8
- Object spawn/action: id 1005, subtype 14
- Mission objective/state: param 196611, subtype 0, param 0
- Set/add variable: variable group 21, variable 22, subtype 0, value 1

## Waypoints

### Waypoint 0

- Tag: `1`
- Members: `Bora_Warhammer (object 0, id 1088, starts at point 2)`, `Bora_Warhammer (object 1, id 1089, starts at point 2)`, `Bora_Mace (object 2, id 1090, starts at point 0)`, `Bora_Mace (object 3, id 1091, starts at point 0)`, `Bora_Mace (object 4, id 1092, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (961.94, 55.18, -1356.47) | None |
| 1 | (2687.69, 415.24, 608.39) | None |
| 2 | (1235.08, 415.24, 3618.14) | None |
| 3 | (-685.22, 415.24, 3973.51) | None |
| 4 | (-2445.48, 415.24, 861.46) | None |
| 5 | (-1300.06, 55.18, -1514.38) | on arrival redirect to Waypoint 0 (tag 1), point 0 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Bora_Warhammer` | 1088 | Interactive | 2386.51,431.85,1300.38 | 461,0,0 | group/role: FG_TRIDENT / 0; waypoint: Waypoint 0 (tag 1, 6 point(s)), starting point 2, arrival event value 65538 |
| 1 | `Bora_Warhammer` | 1089 | Interactive | 2402.49,431.85,1170.64 | 468,0,0 | group/role: FG_TRIDENT / 0; waypoint: Waypoint 0 (tag 1, 6 point(s)), starting point 2, arrival event value 65538 |
| 2 | `Bora_Mace` | 1090 | Interactive | -1558.16,0.00,-1916.60 | 64,0,0 | group/role: FG_INSURRECTION / 0; waypoint: Waypoint 0 (tag 1, 6 point(s)), starting point 0, arrival event value 65536 |
| 3 | `Bora_Mace` | 1091 | Interactive | -1417.06,0.00,-2076.43 | 64,0,0 | group/role: FG_INSURRECTION / 0; waypoint: Waypoint 0 (tag 1, 6 point(s)), starting point 0, arrival event value 65536 |
| 4 | `Bora_Mace` | 1092 | Interactive | -1667.91,0.00,-2094.19 | 0,0,0 | group/role: FG_INSURRECTION / 0; waypoint: Waypoint 0 (tag 1, 6 point(s)), starting point 0, arrival event value 65536 |
| 5 | `Bora_Destroyer` | 1079 | Interactive | -1372.23,-29.52,-2678.67 | 309,13,0 | secondary groups: CONT_023, JUDGEMENT |
| 6 | `Bora_Hvy_Freighter` | 1656 | Interactive | 1252.20,-355.31,-532.27 | 47,0,0 | secondary groups: CONT_021, PILE_DRIVER |
