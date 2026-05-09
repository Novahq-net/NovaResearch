# Tachyon: The Fringe DISP02F.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP02F.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 9 |
| Events | 5 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Warhammer`, `1: Bora_Mace`, `2: Bora_Battleaxe` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFGE_03`, `BFGF_03`, `MERC_17`, `BFNE_01`, `CLEON`, `Patrol1`, `Patrol2`, `SPIKE`, `Redemption` |
| Aliases | `BC10_Claymore1`, `BC10_Claymore2`, `BC10_Claymore3`, `BC10_Claymore4`, `Coward`, `BC10_Waraxe`, `BC10_Mace1`, `BC10_Mace2`, `BC10_Mace3`, `BC10_Mace4`, `BC10_Warhammer1`, `BC10_Warhammer2`, `BC10_Warhammer3`, `BC10_Warhammer4`, `SPIKE`, `Stocks01` |
| Groups | `FG_CLAW`, `FG_VALOR`, `FG_MAUL`, `FG_SWORD` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Group/spawn-list action: spawn list/group 30, subtype 2
- Play dialog: PLAYER.SCR, line/variant 116

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 8, variable 3, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 56, subtype 0
- Play dialog: PLAYER.SCR, line/variant 168
- Set runtime trigger variable: variable group 20, variable 2, subtype 0, value 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 300 (extra 1, 2; flags 2)
- Variable comparison: subject variable group 8, variable 3, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 169

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 4

**Action**

- Group/spawn-list action: spawn list/group 46, subtype 0

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 4

**Action**

- Group/spawn-list action: spawn list/group 85, subtype 1, param 2
- Play dialog: PLAYER.SCR, line/variant 192

## Waypoints

### Waypoint 0

- Tag: `351`
- Members: `Bora_Battleaxe (object 0, id 1797, starts at point 0)`, `Bora_Battleaxe (object 1, id 1798, starts at point 0)`, `Bora_Battleaxe (object 2, id 1799, starts at point 0)`, `Bora_Mace (object 3, id 1879, starts at point 1)`, `Bora_Mace (object 4, id 1880, starts at point 1)`, `Bora_Warhammer (object 5, id 1800, starts at point 1)`, `Bora_Warhammer (object 6, id 1801, starts at point 1)`, `Bora_Mace (object 7, id 1877, starts at point 1)`, `Bora_Mace (object 8, id 1878, starts at point 1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1887.35, 0.00, -4371.02) | None |
| 1 | (-1688.70, 0.00, 2001.17) | on arrival redirect to Waypoint 0 (tag 351), point 0 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Bora_Battleaxe` | 1797 | Interactive | 1980.08,0.00,-4497.93 | 448,0,0 | group/role: FG_CLAW / 1; waypoint: Waypoint 0 (tag 351, 2 point(s)), starting point 0, arrival event value 23003136 |
| 1 | `Bora_Battleaxe` | 1798 | Interactive | 2014.66,0.00,-4638.61 | 448,0,0 | group/role: FG_CLAW / 2; waypoint: Waypoint 0 (tag 351, 2 point(s)), starting point 0, arrival event value 23003136 |
| 2 | `Bora_Battleaxe` | 1799 | Interactive | 2094.75,0.00,-4498.33 | 448,0,0 | group/role: FG_CLAW / 3; waypoint: Waypoint 0 (tag 351, 2 point(s)), starting point 0, arrival event value 23003136 |
| 3 | `Bora_Mace` | 1879 | Interactive | 208.91,0.00,-1410.42 | 0,0,0 | group/role: FG_VALOR / 1; waypoint: Waypoint 0 (tag 351, 2 point(s)), starting point 1, arrival event value 23003137 |
| 4 | `Bora_Mace` | 1880 | Interactive | 260.34,0.00,-1412.81 | 0,0,0 | group/role: FG_VALOR / 2; waypoint: Waypoint 0 (tag 351, 2 point(s)), starting point 1, arrival event value 23003137 |
| 5 | `Bora_Warhammer` | 1800 | Interactive | -361.14,-6.25,-470.83 | 0,0,0 | group/role: FG_MAUL / 1; waypoint: Waypoint 0 (tag 351, 2 point(s)), starting point 1, arrival event value 23003137 |
| 6 | `Bora_Warhammer` | 1801 | Interactive | -330.34,-6.25,-530.95 | 0,0,0 | group/role: FG_MAUL / 2; waypoint: Waypoint 0 (tag 351, 2 point(s)), starting point 1, arrival event value 23003137 |
| 7 | `Bora_Mace` | 1877 | Interactive | -2264.16,0.00,2577.53 | 0,0,0 | group/role: FG_SWORD / 1; waypoint: Waypoint 0 (tag 351, 2 point(s)), starting point 1, arrival event value 23003137 |
| 8 | `Bora_Mace` | 1878 | Interactive | -2215.42,0.00,2577.53 | 0,0,0 | group/role: FG_SWORD / 2; waypoint: Waypoint 0 (tag 351, 2 point(s)), starting point 1, arrival event value 23003137 |
