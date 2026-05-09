# Tachyon: The Fringe BORA03A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `BORA03A.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `(none)` |
| Region | 3 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 6 |
| Entities | 17 |
| Events | 25 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 4 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Frigate`, `1: Bora_Battleaxe`, `2: GalSpan_Orion`, `3: Skav_Pirate_Manta`, `4: GalSpan_Poseidon`, `5: Bora_Cutlass` |
| Scripts | `ORPHS.SCR`, `PLAYER.SCR`, `B04SK.SCR`, `CHAAS.SCR` |
| Scenes | None |
| Labels | `CHAAS`, `ORPHS` |
| Aliases | `frank01`, `frank02`, `frank03`, `frank04` |
| Groups | `FG_CLAW`, `FG_LYNX`, `FG_MANTIS`, `FG_WASP`, `FG_LIGHTNING`, `ORPHEUS` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 2
- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Group/spawn-list action: spawn list/group 30, subtype 1, param 5

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Gate state/action: param 7, subtype 3, param 0
- Set runtime trigger variable: variable group 20, variable 9, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 15

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 20

**Action**

- Group/spawn-list action: spawn list/group 74, subtype 1, param 6

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 21

**Action**

- Group/spawn-list action: spawn list/group 119, subtype 1, param 6
- Group/spawn-list action: spawn list/group 76, subtype 1, param 6
- Hide/remove HUD contact: contact/list 0, subtype 9, param 11

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 24

**Action**

- Group/spawn-list action: spawn list/group 44, subtype 1, param 6
- Gate state/action: param 6, subtype 3, param 0

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 24

**Action**

- Object spawn/action: GalSpan_Frigate (object 16, id 1299), subtype 3
- Play dialog: ORPHS.SCR, line/variant 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 15
- Show/update HUD contact: contact/list 0, subtype 1, param 119
- Show/update HUD contact: contact/list 0, subtype 1, param 44

### Event 6

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 0

**Action**

- Group/spawn-list action: spawn list/group 30, subtype 2
- Play dialog: ORPHS.SCR, line/variant 2

### Event 7

**Trigger**

- Group/spawn-list event: subject 119, op 0, value 0
- Group/spawn-list event: subject 44, op 0, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 11
- Hide/remove HUD contact: contact/list 0, subtype 1, param 44
- Hide/remove HUD contact: contact/list 0, subtype 1, param 119
- Play dialog: PLAYER.SCR, line/variant 19

### Event 8

**Trigger**

- Object event: subject GalSpan_Frigate (object 16, id 1299), op 14, value 21

**Action**

- Play dialog: B04SK.SCR, line/variant 2

### Event 9

**Trigger**

- Group/spawn-list event: subject 44, op 0, value 0
- Group/spawn-list event: subject 119, op 0, value 0
- Sector/startup condition family: subject 2, op 0, value 2

**Action**

- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 15, variable 402, subtype 0, value 1
- Set/add variable: variable group 15, variable 403, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 12, param 19
- Hide/remove HUD contact: contact/list 0, subtype 9, param 11

### Event 10

**Trigger**

- Variable comparison: subject variable group 15, variable 402, op 1, value 1
- Variable comparison: subject variable group 15, variable 403, op 1, value 2

**Action**

- Play scene: unknown index 0, param 0
- Play dialog: PLAYER.SCR, line/variant 20
- Object spawn/action: GalSpan_Frigate (object 16, id 1299), subtype 8, param 1
- Set/add variable: variable group 38, variable 3, subtype 0, value 1

### Event 11

**Trigger**

- Object event: subject GalSpan_Frigate (object 16, id 1299), op 8, value 0 (join 2)
- Object event: subject GalSpan_Frigate (object 16, id 1299), op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 15, variable 402, subtype 0, value 0
- Set/add variable: variable group 15, variable 403, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 10, param 0

### Event 12

**Trigger**

- Variable comparison: subject variable group 15, variable 402, op 0, value 0
- Variable comparison: subject variable group 15, variable 403, op 0, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 11, param 20
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 13

**Trigger**

- Group/spawn-list event: subject 74, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 76, op 4, value 0 (flags 2)
- Variable comparison: subject variable group 21, variable 20, op 1, value 0

**Action**

- Play dialog: CHAAS.SCR, line/variant 11
- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 14

**Trigger**

- Group/spawn-list event: subject 76, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 74, op 4, value 0 (flags 2)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Play dialog: CHAAS.SCR, line/variant 11

### Event 15

**Trigger**

- Object event: subject GalSpan_Frigate (object 16, id 1299), op 0, value 0 (extra 4, 0; flags 3)

**Action**

- Play dialog: ORPHS.SCR, line/variant 3

### Event 16

**Trigger**

- Object event: subject Bora_Cutlass (object 0, id 413), op 4, value 10

**Action**

- Play dialog: CHAAS.SCR, line/variant 10

### Event 17

**Trigger**

- Object event: subject Bora_Cutlass (object 0, id 413), op 4, value 40

**Action**

- Play dialog: CHAAS.SCR, line/variant 9

### Event 18

**Trigger**

- Object event: subject GalSpan_Frigate (object 16, id 1299), op 4, value 10

**Action**

- Play dialog: ORPHS.SCR, line/variant 3

### Event 19

**Trigger**

- Group/spawn-list event: subject 30, op 1, value 30

**Action**

- Play dialog: CHAAS.SCR, line/variant 7

### Event 20

**Trigger**

- Group/spawn-list event: subject 30, op 1, value 50

**Action**

- Play dialog: CHAAS.SCR, line/variant 8

### Event 21

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 0
- Object event: subject GalSpan_Frigate (object 16, id 1299), op 4, value 10

**Action**

- Play dialog: ORPHS.SCR, line/variant 2

### Event 22

**Trigger**

- Object event: subject GalSpan_Frigate (object 16, id 1299), op 4, value 90

**Action**

- Play dialog: B04SK.SCR, line/variant 1

### Event 23

**Trigger**

- Object event: subject GalSpan_Orion (object 12, id 497), op 4, value 10
- Object event: subject GalSpan_Poseidon (object 2, id 493), op 4, value 10
- Object event: subject GalSpan_Orion (object 11, id 496), op 4, value 80

**Action**

- Object spawn/action: GalSpan_Orion (object 12, id 497), subtype 7
- Object spawn/action: GalSpan_Poseidon (object 2, id 493), subtype 7
- Object spawn/action: GalSpan_Orion (object 11, id 496), subtype 7

### Event 24

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 2
- Object arrival: GalSpan_Frigate (object 16, id 1299) reached Waypoint 1 (tag 102), point 1 (raw value 6684673)

**Action**

- Object spawn/action: id 449, subtype 5

## Waypoints

### Waypoint 0

- Tag: `105`
- Members: `GalSpan_Poseidon (object 1, id 492, starts at point 0)`, `GalSpan_Poseidon (object 2, id 493, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1966.60, 0.00, 3139.02) | on arrival play dialog/script or enter gate, param 6 |

### Waypoint 1

- Tag: `102`
- Members: `GalSpan_Frigate (object 16, id 1299, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (991.21, 0.00, 4636.67) | None |
| 1 | (1500.82, 0.00, 3297.02) | on arrival activate current object (raw param -1 ignored); listened by Event 24 for GalSpan_Frigate (object 16, id 1299) |
| 2 | (2396.70, 0.00, 911.01) | None |
| 3 | (2999.32, 0.00, -629.45) | None |
| 4 | (3739.60, 0.00, -2541.98) | on arrival action 1, param -1 |

### Waypoint 2

- Tag: `101`
- Members: `Bora_Cutlass (object 0, id 413, starts at point 0)`, `Bora_Battleaxe (object 13, id 414, starts at point 0)`, `Bora_Battleaxe (object 14, id 417, starts at point 0)`, `Bora_Battleaxe (object 15, id 544, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1946.41, 0.00, 1945.31) | None |
| 1 | (1672.33, 0.00, 2846.97) | on arrival activate current object (raw param -1 ignored) |

## Spawn Lists

### Spawn List 0

- ID: `76`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 1 | spawn list 119 | None |
| 1 | 1 | spawn list 44 | None |
| 2 | 4 | GalSpan_Frigate (object 16, id 1299) | None |

### Spawn List 1

- ID: `74`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 1 | spawn list 119 | None |
| 1 | 4 | GalSpan_Frigate (object 16, id 1299) | None |

### Spawn List 2

- ID: `30`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 1 | spawn list 119 | None |
| 1 | 1 | spawn list 44 | None |
| 2 | 6 | GalSpan_Frigate (object 16, id 1299) | None |

### Spawn List 3

- ID: `44`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 4

- ID: `119`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Bora_Cutlass` | 413 | Interactive | -2145.27,0.00,1985.93 | 156,0,0 | label: CHAAS; group/role: FG_CLAW / 1; alias: frank01; waypoint: Waypoint 2 (tag 101, 2 point(s)), starting point 0, arrival event value 6619136 |
| 1 | `GalSpan_Poseidon` | 492 | Interactive | 2739.95,0.00,4539.02 | 0,0,0 | group/role: FG_LYNX / 1; waypoint: Waypoint 0 (tag 105, 1 point(s)), starting point 0, arrival event value 6881280 |
| 2 | `GalSpan_Poseidon` | 493 | Interactive | 2867.05,0.00,4541.83 | 0,0,0 | group/role: FG_LYNX / 2; waypoint: Waypoint 0 (tag 105, 1 point(s)), starting point 0, arrival event value 6881280 |
| 3 | `Skav_Pirate_Manta` | 427 | Interactive | 3060.55,0.00,3999.61 | 0,0,0 | group/role: FG_MANTIS / 1 |
| 4 | `Skav_Pirate_Manta` | 428 | Interactive | 3166.84,0.00,3990.62 | 0,0,0 | group/role: FG_MANTIS / 2 |
| 5 | `Skav_Pirate_Manta` | 429 | Interactive | 3046.68,0.00,3869.06 | 0,0,0 | group/role: FG_MANTIS / 3 |
| 6 | `Skav_Pirate_Manta` | 430 | Interactive | 3140.17,0.00,3873.93 | 0,0,0 | group/role: FG_MANTIS / 4 |
| 7 | `Skav_Pirate_Manta` | 431 | Interactive | 3256.84,0.00,3994.05 | 0,0,0 | group/role: FG_WASP / 1 |
| 8 | `Skav_Pirate_Manta` | 541 | Interactive | 3375.60,0.00,3988.14 | 0,0,0 | group/role: FG_WASP / 2 |
| 9 | `Skav_Pirate_Manta` | 542 | Interactive | 3273.12,0.00,3853.37 | 0,0,0 | group/role: FG_WASP / 3 |
| 10 | `Skav_Pirate_Manta` | 543 | Interactive | 3373.49,0.00,3854.51 | 0,0,0 | group/role: FG_WASP / 4 |
| 11 | `GalSpan_Orion` | 496 | Interactive | 3020.63,0.00,4537.32 | 0,0,0 | group/role: FG_LIGHTNING / 1 |
| 12 | `GalSpan_Orion` | 497 | Interactive | 3124.93,0.00,4537.23 | 0,0,0 | group/role: FG_LIGHTNING / 2 |
| 13 | `Bora_Battleaxe` | 414 | Interactive | -2179.06,0.00,2031.34 | 156,0,0 | group/role: FG_CLAW / 2; alias: frank02; waypoint: Waypoint 2 (tag 101, 2 point(s)), starting point 0, arrival event value 6619136 |
| 14 | `Bora_Battleaxe` | 417 | Interactive | -2211.55,0.00,1971.24 | 156,0,0 | group/role: FG_CLAW / 3; alias: frank03; waypoint: Waypoint 2 (tag 101, 2 point(s)), starting point 0, arrival event value 6619136 |
| 15 | `Bora_Battleaxe` | 544 | Interactive | -2258.33,0.00,2027.12 | 156,0,0 | group/role: FG_CLAW / 4; alias: frank04; waypoint: Waypoint 2 (tag 101, 2 point(s)), starting point 0, arrival event value 6619136 |
| 16 | `GalSpan_Frigate` | 1299 | Interactive | 822.29,6.35,4997.52 | 220,0,0 | label: ORPHS; secondary groups: none, ORPHEUS; waypoint: Waypoint 1 (tag 102, 5 point(s)), starting point 0, arrival event value 6684672 |
