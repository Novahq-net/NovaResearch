# Tachyon: The Fringe FRON11L.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON11L.SPX` |
| Sector | `QUAD_11` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 10 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 6 |
| Events | 10 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Red_Pirate_Fighter_2` |
| Scripts | `ARENA.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `bfne_05`, `BFBE_04`, `bfne_01`, `bfne_03`, `bfne_02`, `bfne_04`, `bfne_06`, `bfne_08`, `bfne_07`, `bfne_09` |
| Aliases | `BC05_sistine_chapel`, `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1`, `bc05_2`, `bc05_3`, `bc05_5`, `bc05_4`, `Stocks01` |
| Groups | `FG_BANSHEE`, `ARENA_CHALLENGER`, `FG_BEETLE`, `FG_BOA` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 23, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 44

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 23, op 1, value 8

**Action**

- Play dialog: ARENA.SCR, line/variant 8
- Play scene: unknown index 0, param 2

### Event 2

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 8

**Action**

- Play dialog: PLAYER.SCR, line/variant 172

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 23, op 1, value 20

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 35
- Hide/remove HUD contact: contact/list 0, subtype 9, param 44
- Gate state/action: param 1, subtype 3, param 0
- Gate state/action: param 2, subtype 3, param 0
- Gate state/action: param 3, subtype 3, param 0

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 50

**Action**

- Play dialog: PLAYER.SCR, line/variant 190

### Event 5

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 190

**Action**

- Play dialog: ARENA.SCR, line/variant 21

### Event 6

**Trigger**

- Group/spawn-list event: subject 185, op 1, value 50 (join 2)
- Group/spawn-list event: subject 69, op 1, value 50 (join 2)

**Action**

- Play dialog: ARENA.SCR, line/variant 57

### Event 7

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 57

**Action**

- Play dialog: ARENA.SCR, line/variant 46

### Event 8

**Trigger**

- Group/spawn-list event: subject 185, op 0, value 0
- Group/spawn-list event: subject 183, op 0, value 0
- Group/spawn-list event: subject 69, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 35
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 16, variable 442, subtype 0, value 1
- Set/add variable: variable group 16, variable 443, subtype 0, value 2
- Gate state/action: param 1, subtype 0, param 0
- Gate state/action: param 2, subtype 2, param 0
- Gate state/action: param 3, subtype 2, param 0
- Play dialog: ARENA.SCR, line/variant 45

### Event 9

**Trigger**

- Group/spawn-list event: subject 185, op 0, value 0
- Group/spawn-list event: subject 183, op 0, value 0
- Group/spawn-list event: subject 69, op 0, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 12, param 39

## Waypoints

### Waypoint 0

- Tag: `653`
- Members: `Red_Pirate_Fighter_2 (object 4, id 634, starts at point 0)`, `Red_Pirate_Fighter_2 (object 5, id 635, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2795.59, -608.53, 7547.39) | None |
| 1 | (772.43, -608.53, 5657.77) | None |

### Waypoint 1

- Tag: `652`
- Members: `Red_Pirate_Fighter_2 (object 2, id 632, starts at point 0)`, `Red_Pirate_Fighter_2 (object 3, id 633, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-337.71, -608.53, 9824.51) | None |
| 1 | (-399.41, -608.53, 6157.32) | None |

### Waypoint 2

- Tag: `651`
- Members: `Red_Pirate_Fighter_2 (object 0, id 630, starts at point 0)`, `Red_Pirate_Fighter_2 (object 1, id 631, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2682.97, -608.53, 7579.97) | None |
| 1 | (-930.24, -608.53, 5798.94) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Red_Pirate_Fighter_2` | 630 | Interactive | -2797.05,-608.53,7636.23 | 186,0,0 | group/role: FG_BANSHEE / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 2 (tag 651, 2 point(s)), starting point 0, arrival event value 42663936 |
| 1 | `Red_Pirate_Fighter_2` | 631 | Interactive | -2756.41,-608.53,7688.98 | 186,0,0 | label: bfne_02; group/role: FG_BANSHEE / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 2 (tag 651, 2 point(s)), starting point 0, arrival event value 42663936 |
| 2 | `Red_Pirate_Fighter_2` | 632 | Interactive | -370.11,-608.53,9893.87 | 262,0,0 | group/role: FG_BEETLE / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 1 (tag 652, 2 point(s)), starting point 0, arrival event value 42729472 |
| 3 | `Red_Pirate_Fighter_2` | 633 | Interactive | -304.50,-608.53,9896.99 | 262,0,0 | label: bfne_04; group/role: FG_BEETLE / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 1 (tag 652, 2 point(s)), starting point 0, arrival event value 42729472 |
| 4 | `Red_Pirate_Fighter_2` | 634 | Interactive | 2856.40,-608.53,7642.90 | 326,0,0 | label: bfne_01; group/role: FG_BOA / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 0 (tag 653, 2 point(s)), starting point 0, arrival event value 42795008 |
| 5 | `Red_Pirate_Fighter_2` | 635 | Interactive | 2887.21,-608.53,7604.02 | 326,0,0 | group/role: FG_BOA / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 0 (tag 653, 2 point(s)), starting point 0, arrival event value 42795008 |
