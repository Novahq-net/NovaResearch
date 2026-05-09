# Tachyon: The Fringe FRON11K.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON11K.SPX` |
| Sector | `QUAD_11` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 10 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 5 |
| Events | 9 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Red_Pirate_Shrike` |
| Scripts | `ARENA.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `bfne_05`, `BFBE_04`, `bfne_01`, `bfne_03`, `bfne_02`, `bfne_04`, `bfne_06`, `bfne_08`, `bfne_07`, `bfne_09` |
| Aliases | `BC05_sistine_chapel`, `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1`, `bc05_2`, `bc05_3`, `bc05_5`, `bc05_4`, `Stocks01` |
| Groups | `FG_WEEVIL`, `ARENA_CHALLENGER`, `FG_WIGHT` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 22, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 44

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 22, op 1, value 5

**Action**

- Play dialog: ARENA.SCR, line/variant 42
- Play scene: unknown index 0, param 2

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 22, op 1, value 25

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 35
- Hide/remove HUD contact: contact/list 0, subtype 9, param 44
- Gate state/action: param 1, subtype 3, param 0
- Gate state/action: param 2, subtype 3, param 0
- Gate state/action: param 3, subtype 3, param 0

### Event 3

**Trigger**

- Group/spawn-list event: subject 261, op 0, value 0 (join 2)
- Group/spawn-list event: subject 239, op 0, value 0 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 187

### Event 4

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 187

**Action**

- Play dialog: ARENA.SCR, line/variant 14

### Event 5

**Trigger**

- Object event: subject Red_Pirate_Shrike (object 2, id 612), op 0, value 0 (flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 186

### Event 6

**Trigger**

- Object event: subject Red_Pirate_Shrike (object 2, id 612), op 2, value 0
- Group/spawn-list event: subject 261, op 0, value 0
- Group/spawn-list event: subject 239, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 35
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 16, variable 440, subtype 0, value 1
- Set/add variable: variable group 16, variable 441, subtype 0, value 2
- Gate state/action: param 1, subtype 0, param 0
- Gate state/action: param 2, subtype 2, param 0
- Gate state/action: param 3, subtype 2, param 0
- Play dialog: ARENA.SCR, line/variant 44

### Event 7

**Trigger**

- Object event: subject Red_Pirate_Shrike (object 2, id 612), op 2, value 0
- Group/spawn-list event: subject 261, op 0, value 0
- Group/spawn-list event: subject 239, op 0, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 12, param 39

### Event 8

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 44

**Action**

- Play dialog: ARENA.SCR, line/variant 30

## Waypoints

### Waypoint 0

- Tag: `603`
- Members: `Red_Pirate_Shrike (object 3, id 613, starts at point 0)`, `Red_Pirate_Shrike (object 4, id 614, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2779.94, -589.52, 7630.41) | None |
| 1 | (671.54, -589.52, 5639.68) | None |

### Waypoint 1

- Tag: `602`
- Members: `Red_Pirate_Shrike (object 2, id 612, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-352.79, -589.52, 10052.97) | None |
| 1 | (-358.97, -589.52, 6012.14) | None |

### Waypoint 2

- Tag: `601`
- Members: `Red_Pirate_Shrike (object 0, id 610, starts at point 0)`, `Red_Pirate_Shrike (object 1, id 611, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-3012.53, -589.52, 7827.39) | None |
| 1 | (-959.54, -589.52, 5803.71) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Red_Pirate_Shrike` | 610 | Interactive | -3114.33,-589.52,7866.75 | 186,0,0 | label: bfne_08; group/role: FG_WEEVIL / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 2 (tag 601, 2 point(s)), starting point 0, arrival event value 39387136 |
| 1 | `Red_Pirate_Shrike` | 611 | Interactive | -3070.62,-589.52,7915.23 | 186,0,0 | group/role: FG_WEEVIL / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 2 (tag 601, 2 point(s)), starting point 0, arrival event value 39387136 |
| 2 | `Red_Pirate_Shrike` | 612 | Interactive | -352.97,-589.52,10167.69 | 259,0,0 | label: bfne_07; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 1 (tag 602, 2 point(s)), starting point 0, arrival event value 39452672 |
| 3 | `Red_Pirate_Shrike` | 613 | Interactive | 2862.30,-589.52,7738.37 | 319,0,0 | group/role: FG_WIGHT / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 0 (tag 603, 2 point(s)), starting point 0, arrival event value 39518208 |
| 4 | `Red_Pirate_Shrike` | 614 | Interactive | 2906.53,-589.52,7690.22 | 319,0,0 | group/role: FG_WIGHT / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 0 (tag 603, 2 point(s)), starting point 0, arrival event value 39518208 |
