# Tachyon: The Fringe FRON11B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON11B.SPX` |
| Sector | `QUAD_11` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 10 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 9 |
| Events | 21 |
| Waypoints | 4 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Luxury_Liner`, `1: Skav_Pirate_Manta`, `2: Red_Pirate_Shrike` |
| Scripts | `PLAYER.SCR`, `ARENA.SCR` |
| Scenes | None |
| Labels | `bfne_05`, `BFBE_04`, `bfne_01`, `bfne_03`, `bfne_02`, `bfne_04`, `bfne_06`, `bfne_08`, `bfne_07`, `bfne_09` |
| Aliases | `BC05_sistine_chapel`, `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1`, `bc05_2`, `bc05_3`, `bc05_5`, `bc05_4`, `Stocks01` |
| Groups | `FG_DRAGON`, `FG_WASP`, `FG_GALSPAN5`, `KILIMANJARO`, `CONT_033` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Gate state/action: param 1, subtype 3, param 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 21, variable 24, op 1, value 1

**Action**

- Gate state/action: param 1, subtype 2, param 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 24, subtype 0, value 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 24, op 1, value 7

**Action**

- Play dialog: PLAYER.SCR, line/variant 11

### Event 4

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 11

**Action**

- Play dialog: ARENA.SCR, line/variant 38

### Event 5

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 38

**Action**

- Group/spawn-list action: spawn list/group 32, subtype 7
- Group/spawn-list action: spawn list/group 32, subtype 4
- Play dialog: ARENA.SCR, line/variant 34

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 24, op 1, value 30
- Sector/startup condition family: subject 1, op 0, value 38

**Action**

- Group/spawn-list action: spawn list/group 76, subtype 7
- Group/spawn-list action: spawn list/group 76, subtype 4, param 5

### Event 7

**Trigger**

- Group/spawn-list event: subject 76, op 0, value 0

**Action**

- Group/spawn-list action: spawn list/group 32, subtype 8, param 262145 (Waypoint 3 (tag 4), point 1)
- Play dialog: ARENA.SCR, line/variant 30

### Event 8

**Trigger**

- Group/spawn-list event: subject 32, op 2, value 262145 (Waypoint 3 (tag 4), point 1)

**Action**

- Group/spawn-list action: spawn list/group 32, subtype 6

### Event 9

**Trigger**

- Group/spawn-list event: subject 32, op 0, value 0

**Action**

- Group/spawn-list action: spawn list/group 76, subtype 8, param 327681 (Waypoint 2 (tag 5), point 1)
- Play dialog: ARENA.SCR, line/variant 30

### Event 10

**Trigger**

- Group/spawn-list event: subject 76, op 2, value 327681 (Waypoint 2 (tag 5), point 1)

**Action**

- Group/spawn-list action: spawn list/group 76, subtype 6

### Event 11

**Trigger**

- Group/spawn-list event: subject 76, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 32, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 144, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 145, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 146, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 147, op 4, value 0 (join 2; flags 2)
- Object event: subject Luxury_Liner (object 8, id 145), op 0, value 0 (join 2; flags 2)

**Action**

- Group/spawn-list action: spawn list/group 144, subtype 4, param 3
- Group/spawn-list action: spawn list/group 145, subtype 4, param 3
- Group/spawn-list action: spawn list/group 146, subtype 4, param 3
- Group/spawn-list action: spawn list/group 147, subtype 4, param 3

### Event 12

**Trigger**

- Object event: subject Luxury_Liner (object 8, id 145), op 4, value 50

**Action**

- Object spawn/action: Luxury_Liner (object 8, id 145), subtype 4

### Event 13

**Trigger**

- Group/spawn-list event: subject 76, op 1, value 20

**Action**

- Play dialog: ARENA.SCR, line/variant 35

### Event 14

**Trigger**

- Group/spawn-list event: subject 76, op 1, value 40

**Action**

- Play dialog: ARENA.SCR, line/variant 57

### Event 15

**Trigger**

- Group/spawn-list event: subject 76, op 1, value 60

**Action**

- Play dialog: ARENA.SCR, line/variant 61

### Event 16

**Trigger**

- Group/spawn-list event: subject 32, op 1, value 20

**Action**

- Play dialog: ARENA.SCR, line/variant 56

### Event 17

**Trigger**

- Group/spawn-list event: subject 32, op 1, value 40

**Action**

- Play dialog: ARENA.SCR, line/variant 37

### Event 18

**Trigger**

- Group/spawn-list event: subject 32, op 1, value 60

**Action**

- Play dialog: ARENA.SCR, line/variant 58

### Event 19

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 30

**Action**

- Play dialog: ARENA.SCR, line/variant 32

### Event 20

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 32

**Action**

- Play dialog: ARENA.SCR, line/variant 33

## Waypoints

### Waypoint 0

- Tag: `7`
- Members: `Luxury_Liner (object 8, id 145, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-53.92, 1700.00, 7460.99) | on arrival action 1, param -1 |

### Waypoint 1

- Tag: `6`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (4210.09, -620.00, 6657.80) | None |
| 1 | (-15.91, -620.00, 11019.18) | None |
| 2 | (-4462.52, -620.00, 6672.76) | None |
| 3 | (-32.52, -620.00, 2125.74) | None |

### Waypoint 2

- Tag: `5`
- Members: `Skav_Pirate_Manta (object 3, id 123, starts at point 0)`, `Skav_Pirate_Manta (object 4, id 124, starts at point 0)`, `Skav_Pirate_Manta (object 5, id 125, starts at point 0)`, `Skav_Pirate_Manta (object 6, id 729, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-154.37, -620.00, 7112.05) | None |
| 1 | (-155.37, -586.35, 8277.55) | None |
| 2 | (-155.49, -586.35, 8336.76) | on arrival activate current object (raw param -1 ignored) |
| 3 | (-155.07, -586.35, 8364.94) | None |

### Waypoint 3

- Tag: `4`
- Members: `Red_Pirate_Shrike (object 0, id 117, starts at point 0)`, `Red_Pirate_Shrike (object 1, id 118, starts at point 0)`, `Red_Pirate_Shrike (object 2, id 119, starts at point 0)`, `Red_Pirate_Shrike (object 7, id 731, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-131.23, -620.00, 6353.38) | None |
| 1 | (-129.24, -584.50, 4817.04) | None |
| 2 | (-129.24, -584.50, 4752.00) | on arrival activate current object (raw param -1 ignored) |

## Spawn Lists

### Spawn List 0

- ID: `76`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 1 | spawn list 32 | None |
| 1 | 0 | none | None |

### Spawn List 1

- ID: `32`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 1 | spawn list 76 | None |
| 1 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Red_Pirate_Shrike` | 117 | Interactive | -129.34,-584.50,4828.45 | 0,0,0 | group/role: FG_DRAGON / 1; waypoint: Waypoint 3 (tag 4, 3 point(s)), starting point 0, arrival event value 262144 |
| 1 | `Red_Pirate_Shrike` | 118 | Interactive | -101.04,-584.50,4789.48 | 0,0,0 | group/role: FG_DRAGON / 2; waypoint: Waypoint 3 (tag 4, 3 point(s)), starting point 0, arrival event value 262144 |
| 2 | `Red_Pirate_Shrike` | 119 | Interactive | -155.11,-584.50,4789.48 | 0,0,0 | group/role: FG_DRAGON / 3; waypoint: Waypoint 3 (tag 4, 3 point(s)), starting point 0, arrival event value 262144 |
| 3 | `Skav_Pirate_Manta` | 123 | Interactive | -155.46,-586.35,8280.85 | 256,0,0 | group/role: FG_WASP / 1; waypoint: Waypoint 2 (tag 5, 4 point(s)), starting point 0, arrival event value 327680 |
| 4 | `Skav_Pirate_Manta` | 124 | Interactive | -194.68,-586.35,8317.10 | 256,0,0 | group/role: FG_WASP / 2; waypoint: Waypoint 2 (tag 5, 4 point(s)), starting point 0, arrival event value 327680 |
| 5 | `Skav_Pirate_Manta` | 125 | Interactive | -104.68,-586.35,8315.59 | 256,0,0 | group/role: FG_WASP / 3; waypoint: Waypoint 2 (tag 5, 4 point(s)), starting point 0, arrival event value 327680 |
| 6 | `Skav_Pirate_Manta` | 729 | Interactive | -155.07,-586.35,8367.92 | 256,0,0 | group/role: FG_WASP / 1; waypoint: Waypoint 2 (tag 5, 4 point(s)), starting point 0, arrival event value 327680 |
| 7 | `Red_Pirate_Shrike` | 731 | Interactive | -128.77,-584.50,4785.65 | 0,0,0 | group/role: FG_DRAGON / 1; waypoint: Waypoint 3 (tag 4, 3 point(s)), starting point 0, arrival event value 262144 |
| 8 | `Luxury_Liner` | 145 | Interactive | -49.61,1700.00,6678.33 | 0,0,448 | group/role: FG_GALSPAN5 / 1; secondary groups: CONT_033, KILIMANJARO; waypoint: Waypoint 0 (tag 7, 1 point(s)), starting point 0, arrival event value 458752 |
