# Tachyon: The Fringe GALS06A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `GALS06A.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `(none)` |
| Region | 2 |
| Sector ID | 5 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 9 |
| Events | 16 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Lt_Freighter`, `1: GalSpan_Pegasus`, `2: Bora_Cutlass`, `3: Bora_Battleaxe` |
| Scripts | `PLAYER.SCR`, `BJAMR.SCR` |
| Scenes | None |
| Labels | None |
| Aliases | `wing_man` |
| Groups | `FG_RESOLVE`, `CONT_053`, `FG_PROWESS`, `FG_CLAW`, `FG_CETUS` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Gate state/action: param 2, subtype 3, param 0
- Object spawn/action: id 11, subtype 5
- Set runtime trigger variable: variable group 20, variable 15, subtype 0, value 0
- Group/spawn-list action: spawn list/group 179, subtype 2

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 1, param 180

### Event 2

**Trigger**

- Object arrival: 11 reached Waypoint 2 (tag 101), point 1 (raw value 6619137)

**Action**

- Object spawn/action: id 11, subtype 2, param 1

### Event 3

**Trigger**

- Group/spawn-list event: subject 180, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 180

### Event 4

**Trigger**

- Group/spawn-list event: subject 179, op 0, value 0
- Variable comparison: subject variable group 21, variable 33, op 1, value 1

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 179

### Event 5

**Trigger**

- Group/spawn-list event: subject 180, op 0, value 0
- Group/spawn-list event: subject 179, op 0, value 0
- Group/spawn-list event: subject 30, op 0, value 0
- Global enemy/object-count event: subject 0, op 0, value 0
- Variable comparison: subject variable group 21, variable 33, op 1, value 1

**Action**

- Set/add variable: variable group 14, variable 402, subtype 0, value 1
- Set/add variable: variable group 14, variable 403, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Play dialog: PLAYER.SCR, line/variant 16
- Show/update HUD contact: contact/list 0, subtype 12, param 20

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 15, op 1, value 4

**Action**

- Play dialog: PLAYER.SCR, line/variant 13

### Event 7

**Trigger**

- Group/spawn-list event: subject 180, op 1, value 50

**Action**

- Play dialog: BJAMR.SCR, line/variant 2

### Event 8

**Trigger**

- Group/spawn-list event: subject 179, op 0, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 15

### Event 9

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 800 (extra 1, 8; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 800 (extra 1, 9; join 2; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 14

### Event 10

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 14

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 17

### Event 11

**Trigger**

- Object event: subject Bora_Battleaxe (object 0, id 8), op 10, value 0 (join 2)
- Object event: subject Bora_Battleaxe (object 1, id 9), op 10, value 0 (join 2)

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 17
- Set/add variable: variable group 21, variable 33, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 1, param 179

### Event 12

**Trigger**

- Group/spawn-list event: subject 180, op 0, value 0 (join 2)
- Group/spawn-list event: subject 179, op 0, value 0 (join 2)

**Action**

- Group/spawn-list action: spawn list/group 30, subtype 1, param 1
- Show/update HUD contact: contact/list 0, subtype 1, param 30

### Event 13

**Trigger**

- Group/spawn-list event: subject 30, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 30

### Event 14

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 13

**Action**

- Object spawn/action: GalSpan_Lt_Freighter (object 8, id 48), subtype 8, param 10
- Object spawn/action: id 43, subtype 8, param 10

### Event 15

**Trigger**

- Group/spawn-list event: subject 180, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 179, op 4, value 0 (join 2; flags 2)

**Action**

- Group/spawn-list action: spawn list/group 221, subtype 1, param 1

## Waypoints

### Waypoint 0

- Tag: `103`
- Members: `Bora_Battleaxe (object 0, id 8, starts at point 0)`, `Bora_Battleaxe (object 1, id 9, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (286.59, 0.00, -376.78) | None |
| 1 | (-81.94, -66.12, 221.40) | None |

### Waypoint 1

- Tag: `102`
- Members: `Bora_Cutlass (object 2, id 4, starts at point 0)`, `Bora_Cutlass (object 3, id 5, starts at point 0)`, `Bora_Cutlass (object 4, id 106, starts at point 0)`, `Bora_Cutlass (object 5, id 107, starts at point 0)`, `GalSpan_Pegasus (object 6, id 123, starts at point 0)`, `GalSpan_Pegasus (object 7, id 124, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-380.41, -103.31, 485.54) | None |

### Waypoint 2

- Tag: `101`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-578.01, -272.83, 971.99) | None |
| 1 | (-885.07, -160.56, 875.85) | None; listened by Event 2 for id 11 |

## Spawn Lists

### Spawn List 0

- ID: `221`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 5 | spawn list 179 | None |

### Spawn List 1

- ID: `179`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | id 44 | None |
| 1 | 6 | id 11 | None |
| 2 | 6 | GalSpan_Lt_Freighter (object 8, id 48) | None |
| 3 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Bora_Battleaxe` | 8 | Interactive | 599.58,41.77,-801.13 | 414,7,134 | group/role: FG_RESOLVE / 1; secondary groups: CONT_053, none; waypoint: Waypoint 0 (tag 103, 2 point(s)), starting point 0, arrival event value 6750208 |
| 1 | `Bora_Battleaxe` | 9 | Interactive | 607.65,-5.78,-869.12 | 407,14,464 | group/role: FG_RESOLVE / 2; secondary groups: CONT_053, none; waypoint: Waypoint 0 (tag 103, 2 point(s)), starting point 0, arrival event value 6750208 |
| 2 | `Bora_Cutlass` | 4 | Interactive | 17.56,-229.22,-10.18 | 9,28,486 | group/role: FG_PROWESS / 1; waypoint: Waypoint 1 (tag 102, 1 point(s)), starting point 0, arrival event value 6684672 |
| 3 | `Bora_Cutlass` | 5 | Interactive | -15.60,-213.60,-45.79 | 9,28,127 | group/role: FG_PROWESS / 2; waypoint: Waypoint 1 (tag 102, 1 point(s)), starting point 0, arrival event value 6684672 |
| 4 | `Bora_Cutlass` | 106 | Interactive | -1456.77,0.00,1070.64 | 171,0,0 | group/role: FG_CLAW / 1; waypoint: Waypoint 1 (tag 102, 1 point(s)), starting point 0, arrival event value 6684672 |
| 5 | `Bora_Cutlass` | 107 | Interactive | -1465.15,0.00,1166.31 | 178,0,0 | group/role: FG_CLAW / 2; waypoint: Waypoint 1 (tag 102, 1 point(s)), starting point 0, arrival event value 6684672 |
| 6 | `GalSpan_Pegasus` | 123 | Interactive | -1159.54,0.00,687.51 | 0,0,0 | group/role: FG_CETUS / 1; waypoint: Waypoint 1 (tag 102, 1 point(s)), starting point 0, arrival event value 6684672 |
| 7 | `GalSpan_Pegasus` | 124 | Interactive | -1081.80,0.00,620.07 | 0,0,0 | group/role: FG_CETUS / 2; waypoint: Waypoint 1 (tag 102, 1 point(s)), starting point 0, arrival event value 6684672 |
| 8 | `GalSpan_Lt_Freighter` | 48 | Interactive | 77.84,0.00,440.50 | 164,114,0 | None |
