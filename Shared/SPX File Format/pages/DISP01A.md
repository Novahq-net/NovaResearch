# Tachyon: The Fringe DISP01A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP01A.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 14 |
| Events | 8 |
| Waypoints | 0 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Deliverance_BC10_Only`, `1: Bora_Battleaxe`, `2: Susan_Bradley_Waraxe`, `3: Bora_Claymore` |
| Scripts | `ANNAH.SCR` |
| Scenes | None |
| Labels | `TNSA`, `SPIKE`, `capb` |
| Aliases | `BC10_Claymore4`, `BC10_Claymore1`, `BC10_Claymore3`, `BC10_Claymore2`, `BC10_Waraxe`, `tnsa`, `BC10_Mace4`, `BC10_Mace2`, `BC10_Mace1`, `BC10_Mace3`, `BC10_Warhammer3`, `BC10_Warhammer2`, `BC10_Warhammer4`, `BC10_Warhammer1`, `SPIKE`, `Stocks01` |
| Groups | `FG_SWORD`, `FG_LANCE`, `WAR_AXE`, `FG_MORNING_STAR`, `FG_TRIDENT`, `DELIVERANCE`, `CONT_024` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 13, subtype 0, value 0
- Mission objective/state: param 393217, subtype 0, param 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 13, op 1, value 6

**Action**

- Play dialog: ANNAH.SCR, line/variant 2

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Area/player/sector/dock/time event: subject 0, op 9, value 0

**Action**

- Play dialog: ANNAH.SCR, line/variant 3
- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0
- Play scene: unknown index 0, param 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 38

**Action**

- Group/spawn-list action: spawn list/group 124, subtype 3, param 8

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 41

**Action**

- Group/spawn-list action: spawn list/group 47, subtype 3, param 8

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 42

**Action**

- Group/spawn-list action: spawn list/group 57, subtype 3, param 8

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 43

**Action**

- Group/spawn-list action: spawn list/group 56, subtype 3, param 8

### Event 7

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 54

**Action**

- Object spawn/action: Deliverance_BC10_Only (object 13, id 526), subtype 4

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Bora_Claymore` | 105 | Interactive | -1441.67,0.00,-3716.04 | 131,0,0 | group/role: FG_SWORD / 0; alias: BC10_Claymore4 |
| 1 | `Bora_Claymore` | 106 | Interactive | -1441.24,0.00,-3468.85 | 132,0,0 | group/role: FG_SWORD / 0; alias: BC10_Claymore1 |
| 2 | `Bora_Claymore` | 107 | Interactive | -1440.35,0.00,-3636.37 | 139,0,0 | group/role: FG_SWORD / 0; alias: BC10_Claymore3 |
| 3 | `Bora_Claymore` | 108 | Interactive | -1436.46,0.00,-3553.97 | 131,0,0 | group/role: FG_SWORD / 0; alias: BC10_Claymore2 |
| 4 | `Susan_Bradley_Waraxe` | 68 | Interactive | -1070.31,0.00,-3586.92 | 124,0,0 | group/role: FG_LANCE / 0; alias: BC10_Waraxe; secondary groups: none, WAR_AXE |
| 5 | `Bora_Battleaxe` | 513 | Interactive | -1210.83,0.00,-3707.24 | 135,0,0 | group/role: FG_MORNING_STAR / 0; alias: BC10_Mace4 |
| 6 | `Bora_Battleaxe` | 514 | Interactive | -1209.71,0.00,-3561.35 | 129,0,0 | group/role: FG_MORNING_STAR / 0; alias: BC10_Mace2 |
| 7 | `Bora_Battleaxe` | 515 | Interactive | -1209.71,0.00,-3494.49 | 129,0,0 | group/role: FG_MORNING_STAR / 0; alias: BC10_Mace1 |
| 8 | `Bora_Battleaxe` | 516 | Interactive | -1208.59,0.00,-3629.43 | 129,0,0 | group/role: FG_MORNING_STAR / 0; alias: BC10_Mace3 |
| 9 | `Bora_Battleaxe` | 101 | Interactive | -1318.29,0.00,-3632.33 | 122,0,0 | group/role: FG_TRIDENT / 0; alias: BC10_Warhammer3 |
| 10 | `Bora_Battleaxe` | 102 | Interactive | -1316.15,0.00,-3551.98 | 126,0,0 | group/role: FG_TRIDENT / 0; alias: BC10_Warhammer2 |
| 11 | `Bora_Battleaxe` | 103 | Interactive | -1318.78,0.00,-3729.18 | 127,0,0 | group/role: FG_TRIDENT / 0; alias: BC10_Warhammer4 |
| 12 | `Bora_Battleaxe` | 104 | Interactive | -1309.81,0.00,-3466.25 | 122,0,0 | group/role: FG_TRIDENT / 0; alias: BC10_Warhammer1 |
| 13 | `Deliverance_BC10_Only` | 526 | Interactive | -1206.66,0.00,-4178.67 | 129,0,0 | alias: Stocks01; secondary groups: CONT_024, DELIVERANCE |
