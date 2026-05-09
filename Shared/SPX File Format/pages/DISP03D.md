# Tachyon: The Fringe DISP03D.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP03D.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 11 |
| Events | 19 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 4 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Dagger`, `1: Bora_Warhammer`, `2: Bora_Battleaxe`, `3: Bora_Mace` |
| Scripts | `SPY1W.SCR`, `PLAYER.SCR`, `ASVOX.SCR`, `SPY2W.SCR` |
| Scenes | None |
| Labels | `BFGE_02`, `BFBE_07`, `TNSA`, `BFBE_09`, `adder1`, `BFBF_07`, `ROSS`, `SPIKE`, `atkin`, `cruiser1` |
| Aliases | `fake_2`, `BC10_Waraxe`, `Coward`, `spy_1`, `fake_1`, `tnsa`, `BC10_Claymore4`, `BC10_Claymore3`, `BC10_Claymore2`, `BC10_Claymore1`, `BC10_Warhammer4`, `BC10_Warhammer3`, `BC10_Warhammer2`, `BC10_Warhammer1`, `BC10_Mace3`, `BC10_Mace4`, `BC10_Mace1`, `BC10_Mace2`, `Galileo`, `SPIKE`, `zeus`, `Stocks01` |
| Groups | `OBSIDIAN`, `QUASAR`, `GREYHOUND`, `FG_COBALT`, `FG_AMETHYST` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 142, subtype 0
- Group/spawn-list action: spawn list/group 143, subtype 1, param 3
- Play dialog: SPY1W.SCR, line/variant 5

### Event 1

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 5

**Action**

- Play dialog: PLAYER.SCR, line/variant 65

### Event 2

**Trigger**

- Group/spawn-list event: subject 143, op 0, value 0
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 67

### Event 3

**Trigger**

- Group/spawn-list event: subject 143, op 0, value 0
- Variable comparison: subject variable group 21, variable 23, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 67

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 21, op 1, value 1 (join 2)

**Action**

- Set/add variable: variable group 8, variable 16, subtype 0, value 0
- Set/add variable: variable group 8, variable 18, subtype 0, value 0
- Play dialog: ASVOX.SCR, line/variant 0
- Set/add variable: variable group 21, variable 24, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 9, param 34

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Play dialog: ASVOX.SCR, line/variant 0
- Set/add variable: variable group 21, variable 24, subtype 0, value 1
- Set/add variable: variable group 8, variable 16, subtype 0, value 0
- Set/add variable: variable group 8, variable 18, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 34

### Event 6

**Trigger**

- Sector/startup condition family: subject 2, op 0, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 71
- Show/update HUD contact: contact/list 0, subtype 9, param 31
- Hide/remove HUD contact: contact/list 0, subtype 9, param 34

### Event 7

**Trigger**

- Object event: subject Bora_Battleaxe (object 1, id 8933), op 2, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 68

### Event 8

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 1
- Sector/startup condition family: subject 1, op 0, value 71

**Action**

- Object spawn/action: Bora_Warhammer (object 2, id 8988), subtype 2, param 1
- Play dialog: SPY2W.SCR, line/variant 5

### Event 9

**Trigger**

- Variable comparison: subject variable group 21, variable 22, op 1, value 1
- Sector/startup condition family: subject 1, op 0, value 71

**Action**

- Object spawn/action: Bora_Mace (object 0, id 8989), subtype 2, param 1
- Play dialog: SPY1W.SCR, line/variant 8

### Event 10

**Trigger**

- Variable comparison: subject variable group 21, variable 23, op 1, value 1
- Object event: subject Bora_Battleaxe (object 1, id 8933), op 2, value 0

**Action**

- Set/add variable: variable group 18, variable 406, subtype 0, value 1
- Set/add variable: variable group 18, variable 407, subtype 0, value 1
- Broadcast hide/remove contact: contact/list 0, subtype 0, param 15
- Show/update HUD contact: contact/list 0, subtype 11, param 25

### Event 11

**Trigger**

- Object event: subject Bora_Battleaxe (object 1, id 8933), op 4, value 60
- Variable comparison: subject variable group 21, variable 20, op 1, value 1 (join 1)
- Variable comparison: subject variable group 21, variable 23, op 1, value 1 (join 1)

**Action**

- Play dialog: PLAYER.SCR, line/variant 65

### Event 12

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 8 (join 2)
- Sector/startup condition family: subject 3, op 0, value 5 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 66

### Event 13

**Trigger**

- Object event: subject Bora_Battleaxe (object 1, id 8933), op 15, value 0

**Action**

- Object spawn/action: Bora_Battleaxe (object 1, id 8933), subtype 2, param 3

### Event 14

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Gate state/action: param 3, subtype 2, param 0

### Event 15

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 22
- Hide/remove HUD contact: contact/list 0, subtype 9, param 31
- Object spawn/action: Bora_Battleaxe (object 1, id 8933), subtype 14

### Event 16

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 22
- Hide/remove HUD contact: contact/list 0, subtype 9, param 31
- Object spawn/action: Bora_Battleaxe (object 1, id 8933), subtype 14

### Event 17

**Trigger**

- Object event: subject Bora_Warhammer (object 2, id 8988), op 2, value 0 (join 2)
- Object event: subject Bora_Mace (object 0, id 8989), op 2, value 0 (join 2)

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 22
- Mission objective/state: param 393221, subtype 0, param 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 31

### Event 18

**Trigger**

- Object event: subject Bora_Battleaxe (object 1, id 8933), op 7, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 15

## Waypoints

### Waypoint 0

- Tag: `253`
- Members: `Bora_Mace (object 0, id 8989, starts at point -1)`, `Bora_Battleaxe (object 1, id 8933, starts at point 0)`, `Bora_Warhammer (object 2, id 8988, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-820.98, 0.00, -428.22) | None |
| 1 | (-576.72, 0.00, -88.90) | None |
| 2 | (193.38, 0.00, 41.72) | None |

### Waypoint 1

- Tag: `252`
- Members: `Bora_Dagger (object 3, id 8934, starts at point -1)`, `Bora_Dagger (object 4, id 8935, starts at point -1)`, `Bora_Dagger (object 5, id 8936, starts at point -1)`, `Bora_Dagger (object 6, id 8937, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (667.32, 0.00, -718.78) | None |
| 1 | (-159.32, 0.00, -837.90) | None |
| 2 | (-832.61, 0.00, -810.00) | None |

### Waypoint 2

- Tag: `251`
- Members: `Bora_Mace (object 7, id 8938, starts at point -1)`, `Bora_Mace (object 8, id 8939, starts at point -1)`, `Bora_Mace (object 9, id 8940, starts at point -1)`, `Bora_Mace (object 10, id 8941, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-760.44, 0.00, -629.20) | None |
| 1 | (-87.05, 0.00, -575.91) | None |
| 2 | (512.71, 0.00, -506.36) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Bora_Mace` | 8989 | Interactive | -986.04,0.00,-880.80 | 0,0,0 | alias: fake_2; secondary groups: none, OBSIDIAN; waypoint: Waypoint 0 (tag 253, 3 point(s)), starting point -1 |
| 1 | `Bora_Battleaxe` | 8933 | Interactive | -887.55,0.00,-884.75 | 0,0,0 | alias: spy_1; secondary groups: none, QUASAR; waypoint: Waypoint 0 (tag 253, 3 point(s)), starting point 0, arrival event value 16580608 |
| 2 | `Bora_Warhammer` | 8988 | Interactive | -939.96,0.00,-883.07 | 0,0,0 | label: BFGE_02; alias: fake_1; secondary groups: none, GREYHOUND; waypoint: Waypoint 0 (tag 253, 3 point(s)), starting point -1 |
| 3 | `Bora_Dagger` | 8934 | Interactive | -1365.67,0.00,-697.96 | 381,0,0 | group/role: FG_COBALT / 0; waypoint: Waypoint 1 (tag 252, 3 point(s)), starting point -1 |
| 4 | `Bora_Dagger` | 8935 | Interactive | -1134.38,0.00,-697.95 | 381,0,0 | group/role: FG_COBALT / 0; waypoint: Waypoint 1 (tag 252, 3 point(s)), starting point -1 |
| 5 | `Bora_Dagger` | 8936 | Interactive | -1224.79,0.00,-789.66 | 381,0,0 | group/role: FG_COBALT / 0; waypoint: Waypoint 1 (tag 252, 3 point(s)), starting point -1 |
| 6 | `Bora_Dagger` | 8937 | Interactive | -1260.89,0.00,-609.23 | 381,0,0 | label: BFGE_02; group/role: FG_COBALT / 0; waypoint: Waypoint 1 (tag 252, 3 point(s)), starting point -1 |
| 7 | `Bora_Mace` | 8938 | Interactive | 1162.10,0.00,-599.32 | 381,0,0 | group/role: FG_AMETHYST / 0; waypoint: Waypoint 2 (tag 251, 3 point(s)), starting point -1 |
| 8 | `Bora_Mace` | 8939 | Interactive | 1303.88,0.00,-605.37 | 381,0,0 | group/role: FG_AMETHYST / 0; waypoint: Waypoint 2 (tag 251, 3 point(s)), starting point -1 |
| 9 | `Bora_Mace` | 8940 | Interactive | 1260.97,0.00,-530.22 | 381,0,0 | label: BFGE_02; group/role: FG_AMETHYST / 0; waypoint: Waypoint 2 (tag 251, 3 point(s)), starting point -1 |
| 10 | `Bora_Mace` | 8941 | Interactive | 1389.47,0.00,-530.22 | 381,0,0 | group/role: FG_AMETHYST / 0; waypoint: Waypoint 2 (tag 251, 3 point(s)), starting point -1 |
