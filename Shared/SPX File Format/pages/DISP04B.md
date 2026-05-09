# Tachyon: The Fringe DISP04B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP04B.SPX` |
| Sector | `QUAD_04` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 3 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 7 |
| Events | 13 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Minelayer`, `1: Leoff_Coward_Destructable`, `2: Independent_Merc_Piranha` |
| Scripts | `CLEON.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFNE_01`, `CLEON`, `SPIKE` |
| Aliases | `Coward`, `spy_1`, `SPIKE` |
| Groups | `FG_OPAL`, `FG_EMERALD`, `FG_QUARTZ`, `FG_AMBER`, `LEON`, `COBALT_SPIKE` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 2, op 1, value 2

**Action**

- Object spawn/action: Generic_Minelayer (object 6, id 12), subtype 3
- Group/spawn-list action: spawn list/group 200, subtype 0
- Group/spawn-list action: spawn list/group 144, subtype 0
- Group/spawn-list action: spawn list/group 145, subtype 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 21, variable 2, op 1, value 2

**Action**

- Object spawn/action: Generic_Minelayer (object 6, id 12), subtype 3
- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Show/update HUD contact: contact/list 0, subtype 2, param 12
- Object spawn/action: Generic_Minelayer (object 6, id 12), subtype 14
- Mission objective/state: param 393219, subtype 0, param 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 2, op 1, value 2

**Action**

- Group/spawn-list action: spawn list/group 144, subtype 4, param 9
- Object spawn/action: Leoff_Coward_Destructable (object 4, id 25), subtype 8, param 9
- Group/spawn-list action: spawn list/group 200, subtype 4, param 9
- Group/spawn-list action: spawn list/group 145, subtype 4, param 9

### Event 3

**Trigger**

- Object event: subject Generic_Minelayer (object 6, id 12), op 2, value 0

**Action**

- Group/spawn-list action: spawn list/group 200, subtype 3, param 2
- Group/spawn-list action: spawn list/group 144, subtype 3, param 2
- Group/spawn-list action: spawn list/group 145, subtype 3, param 2
- Play dialog: CLEON.SCR, line/variant 1
- Set/add variable: variable group 21, variable 21, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 11, param 25

### Event 4

**Trigger**

- Object event: subject Generic_Minelayer (object 6, id 12), op 2, value 0 (join 1)
- Object event: subject Leoff_Coward_Destructable (object 4, id 25), op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 0, param 25

### Event 5

**Trigger**

- Object event: subject Leoff_Coward_Destructable (object 4, id 25), op 3, value 50

**Action**

- Play dialog: CLEON.SCR, line/variant 2

### Event 6

**Trigger**

- Object event: subject Leoff_Coward_Destructable (object 4, id 25), op 2, value 0
- Variable comparison: subject variable group 21, variable 2, op 1, value 3

**Action**

- Group/spawn-list action: spawn list/group 200, subtype 3, param 2
- Group/spawn-list action: spawn list/group 144, subtype 3, param 2
- Group/spawn-list action: spawn list/group 145, subtype 3, param 2

### Event 7

**Trigger**

- Object event: subject Leoff_Coward_Destructable (object 4, id 25), op 2, value 0 (join 2)
- Object event: subject Leoff_Coward_Destructable (object 4, id 25), op 6, value 0 (join 2)

**Action**

- Set/add variable: variable group 21, variable 22, subtype 0, value 1
- Play dialog: PLAYER.SCR, line/variant 101
- Mission objective/state: param 393223, subtype 0, param 0

### Event 8

**Trigger**

- Object event: subject Leoff_Coward_Destructable (object 4, id 25), op 4, value 50

**Action**

- Play dialog: PLAYER.SCR, line/variant 154

### Event 9

**Trigger**

- Object event: subject Generic_Minelayer (object 6, id 12), op 8, value 0
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Set/add variable: variable group 21, variable 2, subtype 0, value 3
- Mission objective/state: param 393223, subtype 0, param 0
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 24

### Event 10

**Trigger**

- Object event: subject Generic_Minelayer (object 6, id 12), op 8, value 0
- Variable comparison: subject variable group 21, variable 22, op 1, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Show/update HUD contact: contact/list 0, subtype 0, param 25

### Event 11

**Trigger**

- Group/spawn-list event: subject 135, op 0, value 0
- Group/spawn-list event: subject 200, op 0, value 0
- Object event: subject Generic_Minelayer (object 6, id 12), op 2, value 0
- Group/spawn-list event: subject 144, op 0, value 0
- Group/spawn-list event: subject 145, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Set runtime trigger variable: variable group 20, variable 5, subtype 0, value 0
- Mission objective/state: param 393223, subtype 0, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 25
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 12

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 101
- Variable comparison: subject variable group 20, variable 5, op 1, value 15

**Action**

- Play dialog: PLAYER.SCR, line/variant 102

## Waypoints

### Waypoint 0

- Tag: `152`
- Members: `Independent_Merc_Piranha (object 0, id 16, starts at point -1)`, `Independent_Merc_Piranha (object 1, id 18, starts at point -1)`, `Independent_Merc_Piranha (object 2, id 20, starts at point -1)`, `Independent_Merc_Piranha (object 3, id 21, starts at point -1)`, `Leoff_Coward_Destructable (object 4, id 25, starts at point -1)`, `Independent_Merc_Piranha (object 5, id 42, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1362.22, 0.00, 194.61) | None |

### Waypoint 1

- Tag: `151`
- Members: `Generic_Minelayer (object 6, id 12, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (88.65, 0.00, 1282.24) | None |
| 1 | (3320.33, 0.00, -1595.98) | on arrival action 1, param -1 |

## Spawn Lists

### Spawn List 0

- ID: `200`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Generic_Minelayer (object 6, id 12) | None |

### Spawn List 1

- ID: `144`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Generic_Minelayer (object 6, id 12) | None |

### Spawn List 2

- ID: `145`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Generic_Minelayer (object 6, id 12) | None |

### Spawn List 3

- ID: `135`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Independent_Merc_Piranha` | 16 | Interactive | 4406.10,0.00,-109.80 | 314,0,0 | group/role: FG_OPAL / 0; waypoint: Waypoint 0 (tag 152, 1 point(s)), starting point -1 |
| 1 | `Independent_Merc_Piranha` | 18 | Interactive | 8404.91,0.00,126.10 | 395,0,0 | group/role: FG_EMERALD / 0; waypoint: Waypoint 0 (tag 152, 1 point(s)), starting point -1 |
| 2 | `Independent_Merc_Piranha` | 20 | Interactive | 8402.23,0.00,167.91 | 395,0,0 | label: BFNE_01; group/role: FG_EMERALD / 0; waypoint: Waypoint 0 (tag 152, 1 point(s)), starting point -1 |
| 3 | `Independent_Merc_Piranha` | 21 | Interactive | 4727.60,0.00,310.39 | 0,0,0 | group/role: FG_QUARTZ / 0; waypoint: Waypoint 0 (tag 152, 1 point(s)), starting point -1 |
| 4 | `Leoff_Coward_Destructable` | 25 | Interactive | 4773.42,0.00,122.67 | 0,0,0 | label: CLEON; group/role: FG_AMBER / 0; alias: Coward; secondary groups: none, LEON; waypoint: Waypoint 0 (tag 152, 1 point(s)), starting point -1 |
| 5 | `Independent_Merc_Piranha` | 42 | Interactive | 8428.52,0.00,146.23 | 395,0,0 | group/role: FG_EMERALD / 0; waypoint: Waypoint 0 (tag 152, 1 point(s)), starting point -1 |
| 6 | `Generic_Minelayer` | 12 | Interactive | -402.95,0.00,1690.12 | 181,0,0 | label: SPIKE; alias: SPIKE; secondary groups: none, COBALT_SPIKE; waypoint: Waypoint 1 (tag 151, 2 point(s)), starting point -1 |
