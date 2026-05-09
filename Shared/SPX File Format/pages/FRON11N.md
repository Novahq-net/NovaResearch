# Tachyon: The Fringe FRON11N.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON11N.SPX` |
| Sector | `QUAD_11` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 10 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 4 |
| Events | 11 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Independent_Merc_Gar` |
| Scripts | `ARENA.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `bfne_05`, `BFBE_04`, `bfne_01`, `bfne_03`, `bfne_02`, `bfne_04`, `bfne_06`, `bfne_08`, `bfne_07`, `bfne_09` |
| Aliases | `BC05_sistine_chapel`, `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1`, `bc05_2`, `bc05_3`, `bc05_5`, `bc05_4`, `Stocks01` |
| Groups | `FG_CAELUM`, `ARENA_CHALLENGER`, `FG_CANCER` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 25, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 44

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 25, op 1, value 8

**Action**

- Play dialog: ARENA.SCR, line/variant 50
- Play scene: unknown index 0, param 2

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 25, op 1, value 20

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 35
- Hide/remove HUD contact: contact/list 0, subtype 9, param 44
- Gate state/action: param 1, subtype 3, param 0
- Gate state/action: param 2, subtype 3, param 0
- Gate state/action: param 3, subtype 3, param 0

### Event 3

**Trigger**

- Group/spawn-list event: subject 216, op 0, value 0 (join 2)
- Group/spawn-list event: subject 27, op 0, value 0 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 185

### Event 4

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 185

**Action**

- Play dialog: ARENA.SCR, line/variant 19

### Event 5

**Trigger**

- Object event: subject Independent_Merc_Gar (object 1, id 674), op 3, value 20 (join 2)
- Object event: subject Independent_Merc_Gar (object 3, id 676), op 3, value 20 (join 2)

**Action**

- Play dialog: ARENA.SCR, line/variant 15

### Event 6

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 15

**Action**

- Play dialog: PLAYER.SCR, line/variant 187

### Event 7

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 100

**Action**

- Play dialog: ARENA.SCR, line/variant 20

### Event 8

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 20

**Action**

- Play dialog: ARENA.SCR, line/variant 51

### Event 9

**Trigger**

- Group/spawn-list event: subject 216, op 0, value 0
- Group/spawn-list event: subject 27, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 35
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 16, variable 446, subtype 0, value 1
- Set/add variable: variable group 16, variable 447, subtype 0, value 2
- Gate state/action: param 1, subtype 0, param 0
- Gate state/action: param 2, subtype 2, param 0
- Gate state/action: param 3, subtype 2, param 0
- Play dialog: ARENA.SCR, line/variant 52

### Event 10

**Trigger**

- Group/spawn-list event: subject 216, op 0, value 0
- Group/spawn-list event: subject 27, op 0, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 12, param 39

## Waypoints

### Waypoint 0

- Tag: `752`
- Members: `Independent_Merc_Gar (object 2, id 675, starts at point 0)`, `Independent_Merc_Gar (object 3, id 676, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1239.23, -613.41, 8797.17) | None |
| 1 | (486.64, -613.41, 6182.14) | None |

### Waypoint 1

- Tag: `751`
- Members: `Independent_Merc_Gar (object 0, id 673, starts at point 0)`, `Independent_Merc_Gar (object 1, id 674, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1471.83, -613.41, 8685.89) | None |
| 1 | (-462.66, -613.41, 6219.23) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Independent_Merc_Gar` | 673 | Interactive | -1534.97,-613.41,8748.62 | 228,0,0 | group/role: FG_CAELUM / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 1 (tag 751, 2 point(s)), starting point 0, arrival event value 49217536 |
| 1 | `Independent_Merc_Gar` | 674 | Interactive | -1479.51,-613.41,8774.99 | 228,0,0 | label: bfne_09; group/role: FG_CAELUM / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 1 (tag 751, 2 point(s)), starting point 0, arrival event value 49217536 |
| 2 | `Independent_Merc_Gar` | 675 | Interactive | 1248.58,-613.41,8868.89 | 289,0,0 | group/role: FG_CANCER / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 0 (tag 752, 2 point(s)), starting point 0, arrival event value 49283072 |
| 3 | `Independent_Merc_Gar` | 676 | Interactive | 1284.68,-613.41,8853.38 | 289,0,0 | label: bfne_05; group/role: FG_CANCER / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 0 (tag 752, 2 point(s)), starting point 0, arrival event value 49283072 |
