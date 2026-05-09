# Tachyon: The Fringe DISP02B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP02B.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 3 |
| Events | 2 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Minelayer`, `1: Bora_Battleaxe` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFGE_03`, `BFGF_03`, `MERC_17`, `BFNE_01`, `CLEON`, `Patrol1`, `Patrol2`, `SPIKE`, `Redemption` |
| Aliases | `BC10_Claymore1`, `BC10_Claymore2`, `BC10_Claymore3`, `BC10_Claymore4`, `Coward`, `BC10_Waraxe`, `BC10_Mace1`, `BC10_Mace2`, `BC10_Mace3`, `BC10_Mace4`, `BC10_Warhammer1`, `BC10_Warhammer2`, `BC10_Warhammer3`, `BC10_Warhammer4`, `SPIKE`, `Stocks01` |
| Groups | `FG_NOBLE`, `REDEMPTION` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 27, op 1, value 1 (join 2)

**Action**

- Play scene: unknown index 0, param 1
- Set runtime trigger variable: variable group 20, variable 7, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 7, op 1, value 3

**Action**

- Play dialog: PLAYER.SCR, line/variant 10

## Waypoints

### Waypoint 0

- Tag: `151`
- Members: `Bora_Battleaxe (object 0, id 475, starts at point -1)`, `Bora_Battleaxe (object 1, id 476, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (577.50, 0.00, -4380.41) | None |
| 1 | (3149.45, 0.00, -3193.96) | None |
| 2 | (825.67, 0.00, -1775.12) | on arrival redirect to Waypoint 0 (tag 151), point 0 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Bora_Battleaxe` | 475 | Interactive | -702.63,0.00,-4026.99 | 256,0,0 | label: Patrol1; group/role: FG_NOBLE / 0; waypoint: Waypoint 0 (tag 151, 3 point(s)), starting point -1 |
| 1 | `Bora_Battleaxe` | 476 | Interactive | -612.77,0.00,-3994.51 | 256,0,0 | label: Patrol2; group/role: FG_NOBLE / 0; waypoint: Waypoint 0 (tag 151, 3 point(s)), starting point -1 |
| 2 | `Bora_Minelayer` | 1795 | Interactive | -603.56,142.15,-2674.68 | 0,0,0 | label: Redemption; secondary groups: none, REDEMPTION |
