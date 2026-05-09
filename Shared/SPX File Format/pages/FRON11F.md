# Tachyon: The Fringe FRON11F.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON11F.SPX` |
| Sector | `QUAD_11` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 10 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 6 |
| Events | 8 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Pirate_Mine_TRG`, `1: Baron_Malkar_Champion` |
| Scripts | `PLAYER.SCR`, `ARENA.SCR` |
| Scenes | None |
| Labels | `bfne_05`, `BFBE_04`, `bfne_01`, `bfne_03`, `bfne_02`, `bfne_04`, `bfne_06`, `bfne_08`, `bfne_07`, `bfne_09` |
| Aliases | `BC05_sistine_chapel`, `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1`, `bc05_2`, `bc05_3`, `bc05_5`, `bc05_4`, `Stocks01` |
| Groups | `CEZAR_COTTA`, `ARENA_CHALLENGER` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 10, subtype 0, value 0
- Play scene: unknown index 0, param 1

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 10, op 1, value 5

**Action**

- Play dialog: PLAYER.SCR, line/variant 122

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 10, op 1, value 20

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 35
- Gate state/action: param 1, subtype 3, param 0
- Gate state/action: param 2, subtype 3, param 0
- Gate state/action: param 3, subtype 3, param 0

### Event 3

**Trigger**

- Object event: subject Baron_Malkar_Champion (object 0, id 323), op 2, value 0 (join 2)
- Object event: subject Baron_Malkar_Champion (object 1, id 324), op 2, value 0 (join 2)

**Action**

- Play dialog: ARENA.SCR, line/variant 4

### Event 4

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 4

**Action**

- Play dialog: ARENA.SCR, line/variant 5

### Event 5

**Trigger**

- Object event: subject Baron_Malkar_Champion (object 0, id 323), op 2, value 0
- Object event: subject Baron_Malkar_Champion (object 1, id 324), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 35
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 16, variable 432, subtype 0, value 1
- Set/add variable: variable group 16, variable 433, subtype 0, value 2
- Gate state/action: param 1, subtype 0, param 0
- Gate state/action: param 2, subtype 2, param 0
- Gate state/action: param 3, subtype 2, param 0
- Play dialog: ARENA.SCR, line/variant 7

### Event 6

**Trigger**

- Object event: subject Baron_Malkar_Champion (object 0, id 323), op 2, value 0
- Object event: subject Baron_Malkar_Champion (object 1, id 324), op 2, value 0

**Action**

- Set/add variable: variable group 4, variable 15, subtype 1, value 1

### Event 7

**Trigger**

- Object event: subject Baron_Malkar_Champion (object 0, id 323), op 2, value 0
- Object event: subject Baron_Malkar_Champion (object 1, id 324), op 2, value 0

**Action**

- Object spawn/action: Pirate_Mine_TRG (object 2, id 469), subtype 8, param 4
- Object spawn/action: Pirate_Mine_TRG (object 3, id 470), subtype 8, param 4
- Object spawn/action: Pirate_Mine_TRG (object 4, id 471), subtype 8, param 4
- Object spawn/action: Pirate_Mine_TRG (object 5, id 472), subtype 8, param 4
- Show/update HUD contact: contact/list 0, subtype 12, param 37

## Waypoints

### Waypoint 0

- Tag: `352`
- Members: `Baron_Malkar_Champion (object 1, id 324, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (337.92, -191.32, 8510.03) | None |
| 1 | (1691.93, -441.50, 6805.56) | None |
| 2 | (826.24, -721.12, 5625.59) | None |

### Waypoint 1

- Tag: `351`
- Members: `Baron_Malkar_Champion (object 0, id 323, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-344.39, -824.13, 8493.72) | None |
| 1 | (-1739.64, -647.53, 6916.55) | None |
| 2 | (-937.69, -397.35, 5670.87) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Baron_Malkar_Champion` | 323 | Interactive | -89.34,-588.67,8766.32 | 257,0,0 | secondary groups: none, CEZAR_COTTA; waypoint: Waypoint 1 (tag 351, 3 point(s)), starting point 0, arrival event value 23003136 |
| 1 | `Baron_Malkar_Champion` | 324 | Interactive | 93.29,-588.67,8760.62 | 257,0,0 | label: bfne_05; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 0 (tag 352, 3 point(s)), starting point 0, arrival event value 23068672 |
| 2 | `Pirate_Mine_TRG` | 469 | Interactive | -159.44,-552.78,6485.36 | 337,0,0 | None |
| 3 | `Pirate_Mine_TRG` | 470 | Interactive | -329.32,-552.78,6968.02 | 447,0,0 | None |
| 4 | `Pirate_Mine_TRG` | 471 | Interactive | 139.75,-552.78,6760.67 | 445,0,0 | None |
| 5 | `Pirate_Mine_TRG` | 472 | Interactive | 316.95,-552.78,6291.25 | 209,0,0 | None |
