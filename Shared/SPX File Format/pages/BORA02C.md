# Tachyon: The Fringe BORA02C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `BORA02C.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `(none)` |
| Region | 3 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 7 |
| Events | 14 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Navigational_Bouy`, `1: Void_Pirate_Fighter` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `chaas`, `bfbf_01`, `BFBE_05`, `BFGE_05`, `BFBF_05` |
| Aliases | `frank01`, `frank02`, `frank03`, `frank04`, `stocks06` |
| Groups | `FG_ALLIGATOR`, `CONT_034`, `BLANK` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 0, value 0
- Set runtime trigger variable: variable group 20, variable 19, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 24
- Object spawn/action: Navigational_Bouy (object 6, id 357), subtype 14

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 30

**Action**

- Play dialog: PLAYER.SCR, line/variant 37
- Mission objective/state: param 196610, subtype 0, param 0
- Object spawn/action: Navigational_Bouy (object 6, id 357), subtype 15
- Hide/remove HUD contact: contact/list 0, subtype 10, param 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 20, op 0, value 1

**Action**

- Group/spawn-list action: spawn list/group 139, subtype 0
- Mission objective/state: param 196608, subtype 0, param 0
- Set runtime trigger variable: variable group 20, variable 20, subtype 0, value 0

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 3500 (extra 1, 14; flags 2)

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Play dialog: PLAYER.SCR, line/variant 39
- Show/update HUD contact: contact/list 0, subtype 1, param 139
- Group/spawn-list action: spawn list/group 139, subtype 2
- Set/add variable: variable group 21, variable 24, subtype 0, value 1

### Event 4

**Trigger**

- Group/spawn-list event: subject 139, op 0, value 0

**Action**

- Mission objective/state: param 196608, subtype 0, param 0
- Set/add variable: variable group 15, variable 408, subtype 0, value 1
- Set/add variable: variable group 15, variable 409, subtype 0, value 2
- Play dialog: PLAYER.SCR, line/variant 43
- Show/update HUD contact: contact/list 0, subtype 12, param 19
- Set/add variable: variable group 21, variable 24, subtype 0, value 2

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 20, op 1, value 300

**Action**

- Group/spawn-list action: spawn list/group 139, subtype 3, param 6
- Mark/flash contact: contact/list 0, subtype 8, param 16
- Set/add variable: variable group 15, variable 409, subtype 0, value 1

### Event 6

**Trigger**

- Group/spawn-list event: subject 139, op 4, value 0 (flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 48

### Event 7

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 40

**Action**

- Play dialog: PLAYER.SCR, line/variant 156

### Event 8

**Trigger**

- Group/spawn-list event: subject 139, op 1, value 40

**Action**

- Play dialog: PLAYER.SCR, line/variant 161

### Event 9

**Trigger**

- Group/spawn-list event: subject 139, op 1, value 60

**Action**

- Play dialog: PLAYER.SCR, line/variant 157

### Event 10

**Trigger**

- Group/spawn-list event: subject 139, op 1, value 80

**Action**

- Play dialog: PLAYER.SCR, line/variant 41

### Event 11

**Trigger**

- Group/spawn-list event: subject 139, op 1, value 100

**Action**

- Play dialog: PLAYER.SCR, line/variant 83

### Event 12

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 83

**Action**

- Play dialog: PLAYER.SCR, line/variant 169

### Event 13

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 4)

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 16

## Waypoints

### Waypoint 0

- Tag: `201`
- Members: `Void_Pirate_Fighter (object 0, id 14, starts at point -1)`, `Void_Pirate_Fighter (object 1, id 15, starts at point -1)`, `Void_Pirate_Fighter (object 2, id 16, starts at point -1)`, `Void_Pirate_Fighter (object 3, id 17, starts at point -1)`, `Void_Pirate_Fighter (object 4, id 271, starts at point -1)`, `Void_Pirate_Fighter (object 5, id 272, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (4253.60, 230.08, -166.26) | None |
| 1 | (633.37, 230.08, -3007.31) | None |

## Spawn Lists

### Spawn List 0

- ID: `139`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | id 18 | None |
| 1 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Void_Pirate_Fighter` | 14 | Interactive | 4804.84,20.18,97.89 | 0,0,0 | group/role: FG_ALLIGATOR / 0; secondary groups: CONT_034, none; waypoint: Waypoint 0 (tag 201, 2 point(s)), starting point -1 |
| 1 | `Void_Pirate_Fighter` | 15 | Interactive | 4850.16,20.18,108.81 | 0,0,0 | group/role: FG_ALLIGATOR / 0; waypoint: Waypoint 0 (tag 201, 2 point(s)), starting point -1 |
| 2 | `Void_Pirate_Fighter` | 16 | Interactive | 4885.42,20.18,141.58 | 0,0,0 | group/role: FG_ALLIGATOR / 0; secondary groups: CONT_034, none; waypoint: Waypoint 0 (tag 201, 2 point(s)), starting point -1 |
| 3 | `Void_Pirate_Fighter` | 17 | Interactive | 4935.79,20.18,174.35 | 0,0,0 | group/role: FG_ALLIGATOR / 0; secondary groups: CONT_034, none; waypoint: Waypoint 0 (tag 201, 2 point(s)), starting point -1 |
| 4 | `Void_Pirate_Fighter` | 271 | Interactive | 4776.59,20.18,93.59 | 0,0,0 | group/role: FG_ALLIGATOR / 0; secondary groups: CONT_034, none; waypoint: Waypoint 0 (tag 201, 2 point(s)), starting point -1 |
| 5 | `Void_Pirate_Fighter` | 272 | Interactive | 4741.38,20.18,80.87 | 0,0,0 | group/role: FG_ALLIGATOR / 0; secondary groups: CONT_034, none; waypoint: Waypoint 0 (tag 201, 2 point(s)), starting point -1 |
| 6 | `Navigational_Bouy` | 357 | Interactive | 3140.84,0.00,-2189.79 | 0,0,0 | secondary groups: none, BLANK |
