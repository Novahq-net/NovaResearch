# Tachyon: The Fringe DISP02D.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP02D.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 9 |
| Events | 24 |
| Waypoints | 4 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Minelayer`, `1: Leoff_Coward_Destructable`, `2: Independent_Merc_Piranha` |
| Scripts | `SPIKE.SCR`, `CLEON.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFGE_03`, `BFGF_03`, `MERC_17`, `BFNE_01`, `CLEON`, `Patrol1`, `Patrol2`, `SPIKE`, `Redemption` |
| Aliases | `BC10_Claymore1`, `BC10_Claymore2`, `BC10_Claymore3`, `BC10_Claymore4`, `Coward`, `BC10_Waraxe`, `BC10_Mace1`, `BC10_Mace2`, `BC10_Mace3`, `BC10_Mace4`, `BC10_Warhammer1`, `BC10_Warhammer2`, `BC10_Warhammer3`, `BC10_Warhammer4`, `SPIKE`, `Stocks01` |
| Groups | `FG_DIAMOND`, `FG_EMERALD`, `FG_BLOODSTONE`, `LEON`, `FG_AMBER`, `COBALT_SPIKE` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 13, subtype 0, value 0
- Set/add variable: variable group 21, variable 20, subtype 0, value 1

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 13, op 1, value 12

**Action**

- Play dialog: SPIKE.SCR, line/variant 0
- Object spawn/action: Generic_Minelayer (object 8, id 572), subtype 14

### Event 2

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 0

**Action**

- Play dialog: CLEON.SCR, line/variant 0

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 1, param 169
- Show/update HUD contact: contact/list 0, subtype 2, param 572
- Object spawn/action: Leoff_Coward_Destructable (object 7, id 1677), subtype 0
- Group/spawn-list action: spawn list/group 169, subtype 4, param 9
- Set runtime trigger variable: variable group 20, variable 14, subtype 0, value 0
- Set/add variable: variable group 21, variable 34, subtype 0, value 1
- Object spawn/action: Leoff_Coward_Destructable (object 7, id 1677), subtype 8, param 9
- Object spawn/action: Leoff_Coward_Destructable (object 7, id 1677), subtype 2, param 2

### Event 4

**Trigger**

- Group/spawn-list event: subject 169, op 0, value 0
- Variable comparison: subject variable group 0, variable 0, op 0, value 1

**Action**

- Set runtime trigger variable: variable group 20, variable 19, subtype 0, value 0
- Play dialog: PLAYER.SCR, line/variant 103

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 20

**Action**

- Object spawn/action: Generic_Minelayer (object 8, id 572), subtype 5
- Object spawn/action: Generic_Minelayer (object 8, id 572), subtype 13, param 16449536
- Hide/remove HUD contact: contact/list 0, subtype 2, param 572
- Show/update HUD contact: contact/list 0, subtype 6, param 572

### Event 6

**Trigger**

- Object arrival: Generic_Minelayer (object 8, id 572) reached Waypoint 3 (tag 251), point 1 (raw value 16449537)

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Mission objective/state: param 393223, subtype 0, param 0
- Set/add variable: variable group 21, variable 2, subtype 0, value 1

### Event 7

**Trigger**

- Variable comparison: subject variable group 21, variable 34, op 1, value 1
- Object event: subject Generic_Minelayer (object 8, id 572), op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 11, param 25
- Mission objective/state: param 393223, subtype 0, param 0
- Set/add variable: variable group 21, variable 22, subtype 0, value 1

### Event 8

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Group/spawn-list action: spawn list/group 127, subtype 0
- Group/spawn-list action: spawn list/group 200, subtype 0
- Group/spawn-list action: spawn list/group 144, subtype 0
- Group/spawn-list action: spawn list/group 145, subtype 0
- Show/update HUD contact: contact/list 0, subtype 2, param 572

### Event 9

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Group/spawn-list action: spawn list/group 169, subtype 4, param 9
- Group/spawn-list action: spawn list/group 200, subtype 4, param 9
- Group/spawn-list action: spawn list/group 144, subtype 4, param 9
- Group/spawn-list action: spawn list/group 145, subtype 4, param 9
- Group/spawn-list action: spawn list/group 127, subtype 4, param 9

### Event 10

**Trigger**

- Object event: subject Generic_Minelayer (object 8, id 572), op 2, value 0
- Variable comparison: subject variable group 0, variable 0, op 0, value 2

**Action**

- Play dialog: CLEON.SCR, line/variant 1
- Show/update HUD contact: contact/list 0, subtype 1, param 127

### Event 11

**Trigger**

- Object event: subject Generic_Minelayer (object 8, id 572), op 2, value 0

**Action**

- Group/spawn-list action: spawn list/group 200, subtype 3, param 2
- Group/spawn-list action: spawn list/group 144, subtype 3, param 2
- Group/spawn-list action: spawn list/group 145, subtype 3, param 2

### Event 12

**Trigger**

- Variable comparison: subject variable group 0, variable 0, op 0, value 2
- Object event: subject Generic_Minelayer (object 8, id 572), op 2, value 0
- Group/spawn-list event: subject 169, op 0, value 0

**Action**

- Group/spawn-list action: spawn list/group 127, subtype 3, param 2

### Event 13

**Trigger**

- Object event: subject Leoff_Coward_Destructable (object 7, id 1677), op 3, value 70 (join 2)

**Action**

- Play dialog: CLEON.SCR, line/variant 2

### Event 14

**Trigger**

- Object event: subject Leoff_Coward_Destructable (object 3, id 448), op 4, value 50 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 153

### Event 15

**Trigger**

- Object event: subject Leoff_Coward_Destructable (object 3, id 448), op 2, value 0 (join 2)
- Object event: subject Leoff_Coward_Destructable (object 7, id 1677), op 2, value 0 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 101
- Set/add variable: variable group 21, variable 21, subtype 0, value 1

### Event 16

**Trigger**

- Group/spawn-list event: subject 169, op 0, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 2
- Group/spawn-list event: subject 127, op 0, value 0
- Sector/startup condition family: subject 2, op 0, value 101 (join 1)
- Object event: subject Generic_Minelayer (object 8, id 572), op 2, value 0 (join 1)

**Action**

- Set/add variable: variable group 18, variable 412, subtype 0, value 1
- Set/add variable: variable group 18, variable 413, subtype 0, value 2
- Set runtime trigger variable: variable group 20, variable 6, subtype 0, value 0
- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Group/spawn-list action: spawn list/group 200, subtype 3, param 2
- Group/spawn-list action: spawn list/group 144, subtype 3, param 2
- Group/spawn-list action: spawn list/group 145, subtype 3, param 2

### Event 17

**Trigger**

- Variable comparison: subject variable group 0, variable 0, op 1, value 2
- Group/spawn-list event: subject 127, op 0, value 0
- Sector/startup condition family: subject 2, op 0, value 101 (join 1)
- Object event: subject Generic_Minelayer (object 8, id 572), op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 12, param 24
- Mission objective/state: param 393216, subtype 0, param 0

### Event 18

**Trigger**

- Variable comparison: subject variable group 20, variable 6, op 1, value 15

**Action**

- Object spawn/action: Generic_Minelayer (object 8, id 572), subtype 13, param 16646145
- Play dialog: PLAYER.SCR, line/variant 103
- Object spawn/action: Generic_Minelayer (object 8, id 572), subtype 5

### Event 19

**Trigger**

- Variable comparison: subject variable group 0, variable 0, op 1, value 2
- Group/spawn-list event: subject 127, op 0, value 0
- Object event: subject Generic_Minelayer (object 8, id 572), op 2, value 0
- Sector/startup condition family: subject 2, op 0, value 101

**Action**

- Set/add variable: variable group 18, variable 412, subtype 0, value 1
- Set/add variable: variable group 18, variable 413, subtype 0, value 3
- Mission objective/state: param 393216, subtype 0, param 0
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 20

**Trigger**

- Object event: subject Generic_Minelayer (object 8, id 572), op 2, value 0
- Group/spawn-list event: subject 127, op 0, value 0
- Group/spawn-list event: subject 169, op 0, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 102

### Event 21

**Trigger**

- Object event: subject Generic_Minelayer (object 8, id 572), op 8, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Set/add variable: variable group 21, variable 2, subtype 0, value 4

### Event 22

**Trigger**

- Group/spawn-list event: subject 169, op 1, value 30

**Action**

- Play dialog: PLAYER.SCR, line/variant 151

### Event 23

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 100

**Action**

- Play dialog: PLAYER.SCR, line/variant 150

## Waypoints

### Waypoint 0

- Tag: `254`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-439.07, 0.00, 621.43) | on arrival action 1, param -1 |

### Waypoint 1

- Tag: `253`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (3076.34, 0.00, -4107.41) | on arrival play dialog/script or enter gate, param 2 |

### Waypoint 2

- Tag: `252`
- Members: `Independent_Merc_Piranha (object 0, id 355, starts at point -1)`, `Independent_Merc_Piranha (object 1, id 444, starts at point -1)`, `Independent_Merc_Piranha (object 2, id 445, starts at point -1)`, `Leoff_Coward_Destructable (object 3, id 448, starts at point -1)`, `Independent_Merc_Piranha (object 4, id 1633, starts at point -1)`, `Independent_Merc_Piranha (object 5, id 1640, starts at point -1)`, `Independent_Merc_Piranha (object 6, id 1641, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1395.23, 0.00, -685.62) | None |
| 1 | (584.71, 0.00, -381.57) | None |

### Waypoint 3

- Tag: `251`
- Members: `Generic_Minelayer (object 8, id 572, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-75.65, 0.00, -1267.82) | None |
| 1 | (253.62, 0.00, -2023.74) | on arrival action 1, param -1; listened by Event 6 for Generic_Minelayer (object 8, id 572) |

## Spawn Lists

### Spawn List 0

- ID: `200`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | id 433 | None |

### Spawn List 1

- ID: `169`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 2

- ID: `135`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 9 | none | None |

### Spawn List 3

- ID: `127`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Independent_Merc_Piranha` | 355 | Interactive | 2572.09,43.00,-185.43 | 0,0,0 | group/role: FG_DIAMOND / 3; waypoint: Waypoint 2 (tag 252, 2 point(s)), starting point -1 |
| 1 | `Independent_Merc_Piranha` | 444 | Interactive | 2297.17,0.00,-2080.17 | 0,0,0 | label: BFNE_01; group/role: FG_EMERALD / 0; waypoint: Waypoint 2 (tag 252, 2 point(s)), starting point -1 |
| 2 | `Independent_Merc_Piranha` | 445 | Interactive | 2258.61,0.00,-2150.19 | 0,0,0 | group/role: FG_EMERALD / 0; waypoint: Waypoint 2 (tag 252, 2 point(s)), starting point -1 |
| 3 | `Leoff_Coward_Destructable` | 448 | Interactive | 1937.53,0.00,-3967.55 | 0,0,0 | label: CLEON; group/role: FG_BLOODSTONE / 0; alias: Coward; secondary groups: none, LEON; waypoint: Waypoint 2 (tag 252, 2 point(s)), starting point -1 |
| 4 | `Independent_Merc_Piranha` | 1633 | Interactive | 2574.10,43.00,-223.61 | 0,0,0 | label: BFNE_01; group/role: FG_DIAMOND / 3; waypoint: Waypoint 2 (tag 252, 2 point(s)), starting point -1 |
| 5 | `Independent_Merc_Piranha` | 1640 | Interactive | 2584.89,43.00,-129.76 | 0,0,0 | label: BFNE_01; group/role: FG_DIAMOND / 3; waypoint: Waypoint 2 (tag 252, 2 point(s)), starting point -1 |
| 6 | `Independent_Merc_Piranha` | 1641 | Interactive | 2618.76,43.00,-167.76 | 0,0,0 | group/role: FG_DIAMOND / 3; waypoint: Waypoint 2 (tag 252, 2 point(s)), starting point -1 |
| 7 | `Leoff_Coward_Destructable` | 1677 | Interactive | 6867.42,0.00,-1731.26 | 0,0,0 | group/role: FG_AMBER / 0; alias: Coward; secondary groups: none, LEON |
| 8 | `Generic_Minelayer` | 572 | Interactive | -117.20,0.00,-165.46 | 256,0,0 | label: SPIKE; alias: SPIKE; secondary groups: none, COBALT_SPIKE; waypoint: Waypoint 3 (tag 251, 2 point(s)), starting point -1 |
