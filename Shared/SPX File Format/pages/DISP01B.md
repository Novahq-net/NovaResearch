# Tachyon: The Fringe DISP01B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP01B.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 6 |
| Entities | 10 |
| Events | 14 |
| Waypoints | 4 |
| Child Sectors | 0 |
| Scripts | 4 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Mad_Pirate_Platform`, `1: GalSpan_Cruiser`, `2: Bora_Destroyer`, `3: Bora_Mace`, `4: Bora_Battleaxe`, `5: TNS_Inquirer` |
| Scripts | `TNSA.SCR`, `CAPB.SCR`, `PLAYER.SCR`, `LIBER.SCR` |
| Scenes | None |
| Labels | `TNSA`, `SPIKE`, `capb` |
| Aliases | `BC10_Claymore4`, `BC10_Claymore1`, `BC10_Claymore3`, `BC10_Claymore2`, `BC10_Waraxe`, `tnsa`, `BC10_Mace4`, `BC10_Mace2`, `BC10_Mace1`, `BC10_Mace3`, `BC10_Warhammer3`, `BC10_Warhammer2`, `BC10_Warhammer4`, `BC10_Warhammer1`, `SPIKE`, `Stocks01` |
| Groups | `TNS_INQUIRER`, `CONT_005`, `FG_MORNING_STAR`, `FG_CATAPULT`, `INTEGRITY`, `CONT_023`, `CASSIOPEA` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Gate state/action: param 9, subtype 3, param 0
- Set runtime trigger variable: variable group 20, variable 10, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 19
- Object spawn/action: Mad_Pirate_Platform (object 9, id 511), subtype 14

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 10, op 1, value 3

**Action**

- Play dialog: TNSA.SCR, line/variant 6

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 10, op 1, value 19

**Action**

- Object spawn/action: GalSpan_Cruiser (object 8, id 140), subtype 3

### Event 3

**Trigger**

- Object event: subject GalSpan_Cruiser (object 8, id 140), op 9, value 0
- Variable comparison: subject variable group 20, variable 10, op 1, value 20

**Action**

- Play dialog: CAPB.SCR, line/variant 0
- Set runtime trigger variable: variable group 20, variable 10, subtype 1, value 0

### Event 4

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 0

**Action**

- Play dialog: CAPB.SCR, line/variant 1

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 511; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 92
- Play scene: unknown index 0, param 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 19
- Set/add variable: variable group 8, variable 3, subtype 1, value 1
- Show/update HUD contact: contact/list 0, subtype 9, param 23
- Object spawn/action: Mad_Pirate_Platform (object 9, id 511), subtype 15

### Event 6

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 5, value 0 (extra 1, 511; flags 2)

**Action**

- Object spawn/action: GalSpan_Cruiser (object 8, id 140), subtype 21, param 10

### Event 7

**Trigger**

- Object event: subject GalSpan_Cruiser (object 8, id 140), op 2, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 164
- Set runtime trigger variable: variable group 20, variable 11, subtype 0, value 0

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 11, op 1, value 12

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 23
- Show/update HUD contact: contact/list 0, subtype 9, param 28

### Event 9

**Trigger**

- Variable comparison: subject variable group 20, variable 11, op 1, value 13

**Action**

- Group/spawn-list action: spawn list/group 28, subtype 1, param 8
- Object spawn/action: Bora_Destroyer (object 7, id 72), subtype 3
- Mission objective/state: param 393218, subtype 0, param 0

### Event 10

**Trigger**

- Variable comparison: subject variable group 20, variable 11, op 1, value 14

**Action**

- Group/spawn-list action: spawn list/group 47, subtype 1, param 8
- Set runtime trigger variable: variable group 20, variable 11, subtype 1, value 0

### Event 11

**Trigger**

- Sector/startup condition family: subject 2, op 0, value 164

**Action**

- Play dialog: LIBER.SCR, line/variant 4

### Event 12

**Trigger**

- Object event: subject 10, op 4, value 10

**Action**

- Play dialog: LIBER.SCR, line/variant 2

### Event 13

**Trigger**

- Object event: subject 10, op 4, value 60

**Action**

- Play dialog: LIBER.SCR, line/variant 1

## Waypoints

### Waypoint 0

- Tag: `151`
- Members: `TNS_Inquirer (object 0, id 527, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1444.98, 0.00, -2859.34) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 1

- Tag: `153`
- Members: `Bora_Battleaxe (object 1, id 167, starts at point 0)`, `Bora_Battleaxe (object 2, id 168, starts at point 0)`, `Bora_Battleaxe (object 3, id 169, starts at point 0)`, `Bora_Battleaxe (object 4, id 170, starts at point 0)`, `Bora_Mace (object 5, id 171, starts at point 0)`, `Bora_Mace (object 6, id 172, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-0.32, 0.00, -3082.59) | None |
| 1 | (-825.75, 0.00, -2657.82) | None |
| 2 | (-1696.74, 0.00, -2118.86) | None |

### Waypoint 2

- Tag: `154`
- Members: `Bora_Destroyer (object 7, id 72, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1970.71, 0.00, -2574.35) | None |
| 1 | (1108.03, -235.46, -2385.86) | None |
| 2 | (-1152.45, -851.27, -1912.93) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 3

- Tag: `152`
- Members: `GalSpan_Cruiser (object 8, id 140, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2633.20, -61.51, 719.83) | None |
| 1 | (-2137.48, -61.51, -1070.38) | None |
| 2 | (-1337.29, -61.51, -1421.55) | on arrival activate current object (raw param -1 ignored) |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `TNS_Inquirer` | 527 | Interactive | 548.52,0.00,-3367.00 | 0,0,0 | label: TNSA; alias: tnsa; secondary groups: CONT_005, TNS_INQUIRER; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 1 | `Bora_Battleaxe` | 167 | Interactive | -656.91,316.71,-3297.65 | 0,0,0 | group/role: FG_MORNING_STAR / 1; waypoint: Waypoint 1 (tag 153, 3 point(s)), starting point 0, arrival event value 10027008 |
| 2 | `Bora_Battleaxe` | 168 | Interactive | -520.62,316.71,-3305.90 | 0,0,0 | group/role: FG_MORNING_STAR / 2; waypoint: Waypoint 1 (tag 153, 3 point(s)), starting point 0, arrival event value 10027008 |
| 3 | `Bora_Battleaxe` | 169 | Interactive | -399.15,316.71,-3298.66 | 0,0,0 | group/role: FG_MORNING_STAR / 3; waypoint: Waypoint 1 (tag 153, 3 point(s)), starting point 0, arrival event value 10027008 |
| 4 | `Bora_Battleaxe` | 170 | Interactive | -252.11,316.71,-3305.90 | 0,0,0 | group/role: FG_MORNING_STAR / 4; waypoint: Waypoint 1 (tag 153, 3 point(s)), starting point 0, arrival event value 10027008 |
| 5 | `Bora_Mace` | 171 | Interactive | -533.40,316.71,-3494.18 | 0,0,0 | group/role: FG_CATAPULT / 1; waypoint: Waypoint 1 (tag 153, 3 point(s)), starting point 0, arrival event value 10027008 |
| 6 | `Bora_Mace` | 172 | Interactive | -405.54,316.71,-3508.67 | 0,0,0 | group/role: FG_CATAPULT / 2; waypoint: Waypoint 1 (tag 153, 3 point(s)), starting point 0, arrival event value 10027008 |
| 7 | `Bora_Destroyer` | 72 | Interactive | 2392.91,0.00,-2701.15 | 400,0,0 | secondary groups: CONT_023, INTEGRITY; waypoint: Waypoint 2 (tag 154, 3 point(s)), starting point 0, arrival event value 10092544 |
| 8 | `GalSpan_Cruiser` | 140 | Interactive | -3043.90,-61.51,1720.78 | 223,0,0 | label: capb; secondary groups: CONT_023, CASSIOPEA; waypoint: Waypoint 3 (tag 152, 3 point(s)), starting point 0, arrival event value 9961472 |
| 9 | `Mad_Pirate_Platform` | 511 | Interactive | 743.16,-2534.55,-943.54 | 0,1,0 | None |
