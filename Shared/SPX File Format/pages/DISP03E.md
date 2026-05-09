# Tachyon: The Fringe DISP03E.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP03E.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 2 |
| Events | 6 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 0 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Minelayer`, `1: Leoff_Coward_Destructable` |
| Scripts | None |
| Scenes | None |
| Labels | `BFGE_02`, `BFBE_07`, `TNSA`, `BFBE_09`, `adder1`, `BFBF_07`, `ROSS`, `SPIKE`, `atkin`, `cruiser1` |
| Aliases | `fake_2`, `BC10_Waraxe`, `Coward`, `spy_1`, `fake_1`, `tnsa`, `BC10_Claymore4`, `BC10_Claymore3`, `BC10_Claymore2`, `BC10_Claymore1`, `BC10_Warhammer4`, `BC10_Warhammer3`, `BC10_Warhammer2`, `BC10_Warhammer1`, `BC10_Mace3`, `BC10_Mace4`, `BC10_Mace1`, `BC10_Mace2`, `Galileo`, `SPIKE`, `zeus`, `Stocks01` |
| Groups | `FG_AMBER`, `LEON`, `COBALT_SPIKE`, `CONT_025` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Variable comparison: subject variable group 21, variable 2, op 1, value 1 (flags 1)

**Action**

- Object spawn/action: Generic_Minelayer (object 1, id 9054), subtype 3
- Set runtime trigger variable: variable group 20, variable 20, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 6, param 9054

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 20, op 1, value 90

**Action**

- Object spawn/action: Generic_Minelayer (object 1, id 9054), subtype 4
- Set runtime trigger variable: variable group 20, variable 20, subtype 1, value 0
- Set/add variable: variable group 20, variable 20, subtype 0, value 0
- Set/add variable: variable group 21, variable 2, subtype 1, value 1

### Event 2

**Trigger**

- Object event: subject Generic_Minelayer (object 1, id 9054), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 21, subtype 0, value 1

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Variable comparison: subject variable group 0, variable 0, op 1, value 1 (flags 1)

**Action**

- Object spawn/action: Leoff_Coward_Destructable (object 0, id 9226), subtype 8, param 9

### Event 4

**Trigger**

- Object event: subject Leoff_Coward_Destructable (object 0, id 9226), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 22, subtype 0, value 1

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 21, op 1, value 1
- Variable comparison: subject variable group 0, variable 0, op 0, value 1

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Mission objective/state: param 393223, subtype 0, param 0

## Waypoints

### Waypoint 0

- Tag: `301`
- Members: `Leoff_Coward_Destructable (object 0, id 9226, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1161.10, 0.00, 1217.48) | on arrival play dialog/script or enter gate, param 3 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Leoff_Coward_Destructable` | 9226 | Interactive | -1935.03,0.00,2681.66 | 0,0,0 | group/role: FG_AMBER / 0; alias: Coward; secondary groups: none, LEON; waypoint: Waypoint 0 (tag 301, 1 point(s)), starting point -1 |
| 1 | `Generic_Minelayer` | 9054 | Interactive | -621.79,0.00,-33.90 | 171,0,0 | label: SPIKE; alias: SPIKE; secondary groups: CONT_025, COBALT_SPIKE |
