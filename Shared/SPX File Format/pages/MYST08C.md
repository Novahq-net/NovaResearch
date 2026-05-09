# Tachyon: The Fringe MYST08C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST08C.SPX` |
| Sector | `QUAD_08` |
| Backdrop | `(none)` |
| Region | 5 |
| Sector ID | 7 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 12 |
| Events | 17 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Luxury_Liner`, `1: Demon_Pirate_Fighter` |
| Scripts | `SIGHT.SCR`, `DEMNP.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `OPAL` |
| Aliases | `stocks02` |
| Groups | `FG_SPECTER`, `FG_PHANTASM`, `FG_SHADOW`, `FG_POLTERGEIST`, `FG_SPOOK`, `THE_SIGHTSEER` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 20, op 1, value 2

**Action**

- Set runtime trigger variable: variable group 20, variable 31, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 31, op 0, value 5
- Variable comparison: subject variable group 21, variable 20, op 1, value 2

**Action**

- Object spawn/action: Luxury_Liner (object 11, id 2119), subtype 3
- Show/update HUD contact: contact/list 0, subtype 2, param 2119
- Play dialog: SIGHT.SCR, line/variant 3
- Object spawn/action: Luxury_Liner (object 11, id 2119), subtype 14

### Event 2

**Trigger**

- Object event: subject Luxury_Liner (object 11, id 2119), op 9, value 0
- Variable comparison: subject variable group 21, variable 20, op 1, value 2

**Action**

- Set runtime trigger variable: variable group 20, variable 28, subtype 0, value 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 28, op 1, value 7
- Variable comparison: subject variable group 21, variable 20, op 1, value 2

**Action**

- Group/spawn-list action: spawn list/group 155, subtype 0
- Group/spawn-list action: spawn list/group 82, subtype 0
- Play dialog: DEMNP.SCR, line/variant 0

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 28, op 1, value 90
- Variable comparison: subject variable group 21, variable 20, op 1, value 2

**Action**

- Group/spawn-list action: spawn list/group 154, subtype 0
- Group/spawn-list action: spawn list/group 79, subtype 0
- Play dialog: PLAYER.SCR, line/variant 162

### Event 5

**Trigger**

- Object arrival: Luxury_Liner (object 11, id 2119) reached Waypoint 1 (tag 201), point 2 (raw value 13172738)

**Action**

- Play dialog: SIGHT.SCR, line/variant 6

### Event 6

**Trigger**

- Object event: subject Luxury_Liner (object 11, id 2119), op 8, value 0

**Action**

- Group/spawn-list action: spawn list/group 80, subtype 0
- Set/add variable: variable group 21, variable 20, subtype 0, value 3
- Mission objective/state: param 327686, subtype 0, param 0
- Hide/remove HUD contact: contact/list 0, subtype 2, param 2119
- Play dialog: PLAYER.SCR, line/variant 98

### Event 7

**Trigger**

- Object event: subject Luxury_Liner (object 11, id 2119), op 2, value 0 (join 2)
- Object event: subject Luxury_Liner (object 11, id 2119), op 6, value 0 (join 2)

**Action**

- Set/add variable: variable group 17, variable 408, subtype 0, value 1
- Set/add variable: variable group 17, variable 409, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 29
- Mark/flash contact: contact/list 0, subtype 2, param 2119

### Event 8

**Trigger**

- Object event: subject Demon_Pirate_Fighter (object 2, id 4051), op 2, value 0 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 89

### Event 9

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 30 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 93

### Event 10

**Trigger**

- Object event: subject Luxury_Liner (object 11, id 2119), op 3, value 60

**Action**

- Play dialog: PLAYER.SCR, line/variant 122

### Event 11

**Trigger**

- Object event: subject Demon_Pirate_Fighter (object 2, id 4051), op 4, value 70

**Action**

- Object spawn/action: Demon_Pirate_Fighter (object 2, id 4051), subtype 7
- Play dialog: PLAYER.SCR, line/variant 150

### Event 12

**Trigger**

- Object event: subject Demon_Pirate_Fighter (object 1, id 4058), op 4, value 100 (join 2)
- Object event: subject Demon_Pirate_Fighter (object 4, id 4056), op 4, value 100 (join 2)
- Object event: subject Demon_Pirate_Fighter (object 0, id 4053), op 4, value 100 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 137

### Event 13

**Trigger**

- Object event: subject Demon_Pirate_Fighter (object 6, id 4074), op 4, value 70

**Action**

- Object spawn/action: Demon_Pirate_Fighter (object 6, id 4074), subtype 7

### Event 14

**Trigger**

- Object event: subject Demon_Pirate_Fighter (object 9, id 4081), op 4, value 90

**Action**

- Object spawn/action: Demon_Pirate_Fighter (object 9, id 4081), subtype 7

### Event 15

**Trigger**

- Object event: subject Demon_Pirate_Fighter (object 4, id 4056), op 4, value 80

**Action**

- Object spawn/action: Demon_Pirate_Fighter (object 4, id 4056), subtype 7

### Event 16

**Trigger**

- Global enemy/object-count event: subject 0, op 0, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 149

## Waypoints

### Waypoint 0

- Tag: `202`
- Members: `Demon_Pirate_Fighter (object 6, id 4074, starts at point 0)`, `Demon_Pirate_Fighter (object 7, id 4075, starts at point 0)`, `Demon_Pirate_Fighter (object 8, id 4076, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1733.11, 0.00, 1575.25) | None |
| 1 | (-1575.55, 0.00, 930.70) | None |
| 2 | (-1238.94, 0.00, 550.19) | None |

### Waypoint 1

- Tag: `201`
- Members: `Luxury_Liner (object 11, id 2119, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1044.14, -238.84, 847.04) | None |
| 1 | (-590.29, -238.84, 366.35) | None |
| 2 | (69.51, -238.84, -418.97) | None; listened by Event 5 for Luxury_Liner (object 11, id 2119) |
| 3 | (446.65, -238.84, -864.87) | None |
| 4 | (796.22, -238.84, -1284.48) | on arrival action 1, param -1 |

## Spawn Lists

### Spawn List 0

- ID: `80`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 1

- ID: `79`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 2

- ID: `82`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 6 | Luxury_Liner (object 11, id 2119) | None |

### Spawn List 3

- ID: `155`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Luxury_Liner (object 11, id 2119) | None |

### Spawn List 4

- ID: `154`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Luxury_Liner (object 11, id 2119) | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Demon_Pirate_Fighter` | 4053 | Interactive | -712.98,-238.84,-170.69 | 0,0,0 | group/role: FG_SPECTER / 0 |
| 1 | `Demon_Pirate_Fighter` | 4058 | Interactive | -752.22,-238.84,-169.69 | 0,0,0 | group/role: FG_PHANTASM / 0 |
| 2 | `Demon_Pirate_Fighter` | 4051 | Interactive | -1292.58,-238.84,-53.98 | 0,0,0 | group/role: FG_SHADOW / 0 |
| 3 | `Demon_Pirate_Fighter` | 4052 | Interactive | -1236.46,-238.84,-74.27 | 0,0,0 | group/role: FG_POLTERGEIST / 0 |
| 4 | `Demon_Pirate_Fighter` | 4056 | Interactive | -1269.28,-238.84,-114.28 | 0,0,0 | group/role: FG_POLTERGEIST / 0 |
| 5 | `Demon_Pirate_Fighter` | 4072 | Interactive | -724.01,-238.84,-211.19 | 0,0,0 | group/role: FG_PHANTASM / 0 |
| 6 | `Demon_Pirate_Fighter` | 4074 | Interactive | -2055.11,0.00,2039.84 | 208,0,0 | group/role: FG_SPOOK / 0; waypoint: Waypoint 0 (tag 202, 3 point(s)), starting point 0, arrival event value 13238272 |
| 7 | `Demon_Pirate_Fighter` | 4075 | Interactive | -2024.64,0.00,2052.23 | 208,0,0 | group/role: FG_SPOOK / 0; waypoint: Waypoint 0 (tag 202, 3 point(s)), starting point 0, arrival event value 13238272 |
| 8 | `Demon_Pirate_Fighter` | 4076 | Interactive | -1990.37,0.00,2052.23 | 208,0,0 | group/role: FG_SPOOK / 0; waypoint: Waypoint 0 (tag 202, 3 point(s)), starting point 0, arrival event value 13238272 |
| 9 | `Demon_Pirate_Fighter` | 4081 | Interactive | -1324.81,0.00,-107.66 | 0,0,0 | group/role: FG_SHADOW / 0 |
| 10 | `Demon_Pirate_Fighter` | 4082 | Interactive | -765.71,0.00,-217.20 | 0,0,0 | group/role: FG_SPECTER / 0 |
| 11 | `Luxury_Liner` | 2119 | Interactive | -1341.53,-238.84,1148.46 | 198,0,0 | alias: stocks02; secondary groups: none, THE_SIGHTSEER; waypoint: Waypoint 1 (tag 201, 5 point(s)), starting point 0, arrival event value 13172736 |
