# Tachyon: The Fringe FRON11H.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON11H.SPX` |
| Sector | `QUAD_11` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 10 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 6 |
| Events | 11 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Independent_Merc_Dart` |
| Scripts | `ARENA.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `bfne_05`, `BFBE_04`, `bfne_01`, `bfne_03`, `bfne_02`, `bfne_04`, `bfne_06`, `bfne_08`, `bfne_07`, `bfne_09` |
| Aliases | `BC05_sistine_chapel`, `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1`, `bc05_2`, `bc05_3`, `bc05_5`, `bc05_4`, `Stocks01` |
| Groups | `FG_ACE`, `ARENA_CHALLENGER`, `FG_ADDER` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 19, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 44

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 8

**Action**

- Play dialog: ARENA.SCR, line/variant 38
- Play scene: unknown index 0, param 2

### Event 2

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 38

**Action**

- Play dialog: ARENA.SCR, line/variant 37

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 25

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 35
- Hide/remove HUD contact: contact/list 0, subtype 9, param 44
- Gate state/action: param 1, subtype 3, param 0
- Gate state/action: param 2, subtype 3, param 0
- Gate state/action: param 3, subtype 3, param 0

### Event 4

**Trigger**

- Object event: subject Independent_Merc_Dart (object 0, id 487), op 0, value 0 (join 2; flags 2)
- Object event: subject Independent_Merc_Dart (object 3, id 490), op 0, value 0 (join 2; flags 3)

**Action**

- Play dialog: ARENA.SCR, line/variant 17

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 30 (flags 1)

**Action**

- Play dialog: PLAYER.SCR, line/variant 167

### Event 6

**Trigger**

- Group/spawn-list event: subject 270, op 0, value 0 (join 2)
- Group/spawn-list event: subject 67, op 0, value 0 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 163

### Event 7

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 163

**Action**

- Play dialog: ARENA.SCR, line/variant 16

### Event 8

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 100 (extra 1, 488; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 100 (extra 1, 492; join 2; flags 3)

**Action**

- Play dialog: ARENA.SCR, line/variant 23

### Event 9

**Trigger**

- Group/spawn-list event: subject 270, op 0, value 0
- Group/spawn-list event: subject 67, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 35
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 16, variable 434, subtype 0, value 1
- Set/add variable: variable group 16, variable 435, subtype 0, value 2
- Gate state/action: param 1, subtype 0, param 0
- Gate state/action: param 2, subtype 2, param 0
- Gate state/action: param 3, subtype 2, param 0
- Play dialog: ARENA.SCR, line/variant 28

### Event 10

**Trigger**

- Group/spawn-list event: subject 270, op 0, value 0
- Group/spawn-list event: subject 67, op 0, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 12, param 39

## Waypoints

### Waypoint 0

- Tag: `452`
- Members: `Independent_Merc_Dart (object 3, id 490, starts at point 0)`, `Independent_Merc_Dart (object 4, id 491, starts at point 0)`, `Independent_Merc_Dart (object 5, id 492, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (516.58, -586.76, 8279.77) | None |
| 1 | (1710.32, -586.76, 6949.64) | None |
| 2 | (838.95, -586.76, 5740.96) | None |

### Waypoint 1

- Tag: `451`
- Members: `Independent_Merc_Dart (object 0, id 487, starts at point 0)`, `Independent_Merc_Dart (object 1, id 488, starts at point 0)`, `Independent_Merc_Dart (object 2, id 489, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-738.97, -586.76, 8206.18) | None |
| 1 | (-1776.09, -586.76, 7030.22) | None |
| 2 | (-823.80, -586.76, 5869.74) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Independent_Merc_Dart` | 487 | Interactive | -741.27,-586.76,9441.89 | 254,0,0 | group/role: FG_ACE / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 1 (tag 451, 3 point(s)), starting point 0, arrival event value 29556736 |
| 1 | `Independent_Merc_Dart` | 488 | Interactive | -671.71,-586.76,9441.89 | 254,0,0 | group/role: FG_ACE / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 1 (tag 451, 3 point(s)), starting point 0, arrival event value 29556736 |
| 2 | `Independent_Merc_Dart` | 489 | Interactive | -594.42,-586.76,9425.13 | 255,0,0 | label: bfne_01; group/role: FG_ACE / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 1 (tag 451, 3 point(s)), starting point 0, arrival event value 29556736 |
| 3 | `Independent_Merc_Dart` | 490 | Interactive | 711.79,-586.76,9458.65 | 255,0,0 | label: bfne_03; group/role: FG_ADDER / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 0 (tag 452, 3 point(s)), starting point 0, arrival event value 29622272 |
| 4 | `Independent_Merc_Dart` | 491 | Interactive | 765.90,-586.76,9458.65 | 254,0,0 | group/role: FG_ADDER / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 0 (tag 452, 3 point(s)), starting point 0, arrival event value 29622272 |
| 5 | `Independent_Merc_Dart` | 492 | Interactive | 835.46,-586.76,9458.65 | 254,0,0 | group/role: FG_ADDER / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 0 (tag 452, 3 point(s)), starting point 0, arrival event value 29622272 |
