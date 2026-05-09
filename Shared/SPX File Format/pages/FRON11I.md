# Tachyon: The Fringe FRON11I.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON11I.SPX` |
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
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Independent_Merc_Mako` |
| Scripts | `ARENA.SCR` |
| Scenes | None |
| Labels | `bfne_05`, `BFBE_04`, `bfne_01`, `bfne_03`, `bfne_02`, `bfne_04`, `bfne_06`, `bfne_08`, `bfne_07`, `bfne_09` |
| Aliases | `BC05_sistine_chapel`, `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1`, `bc05_2`, `bc05_3`, `bc05_5`, `bc05_4`, `Stocks01` |
| Groups | `FG_ALLIGATOR`, `ARENA_CHALLENGER`, `FG_DRAGON` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 20, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 44

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 20, op 1, value 8

**Action**

- Play dialog: ARENA.SCR, line/variant 41
- Play scene: unknown index 0, param 2

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 20, op 1, value 25

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 35
- Hide/remove HUD contact: contact/list 0, subtype 9, param 44
- Gate state/action: param 1, subtype 3, param 0
- Gate state/action: param 2, subtype 3, param 0
- Gate state/action: param 3, subtype 3, param 0

### Event 3

**Trigger**

- Group/spawn-list event: subject 139, op 0, value 0 (join 2)
- Group/spawn-list event: subject 32, op 0, value 0 (join 2)

**Action**

- Play dialog: ARENA.SCR, line/variant 22

### Event 4

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 22 (join 2)

**Action**

- Play dialog: ARENA.SCR, line/variant 18

### Event 5

**Trigger**

- Object event: subject Independent_Merc_Mako (object 0, id 506), op 2, value 0 (join 2)
- Object event: subject Independent_Merc_Mako (object 1, id 507), op 2, value 0 (join 2)
- Object event: subject Independent_Merc_Mako (object 2, id 508), op 2, value 0 (join 2)
- Object event: subject Independent_Merc_Mako (object 3, id 509), op 2, value 0 (join 2)
- Object event: subject Independent_Merc_Mako (object 4, id 510), op 2, value 0 (join 2)
- Object event: subject Independent_Merc_Mako (object 5, id 511), op 2, value 0
- Sector/startup condition family: subject 0, op 0, value 18

**Action**

- Play dialog: ARENA.SCR, line/variant 40

### Event 6

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 100 (extra 1, 507; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 100 (extra 1, 510; join 2; flags 3)

**Action**

- Play dialog: ARENA.SCR, line/variant 23

### Event 7

**Trigger**

- Group/spawn-list event: subject 139, op 0, value 0
- Group/spawn-list event: subject 32, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 35
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 16, variable 436, subtype 0, value 1
- Set/add variable: variable group 16, variable 437, subtype 0, value 2
- Gate state/action: param 1, subtype 0, param 0
- Gate state/action: param 2, subtype 2, param 0
- Gate state/action: param 3, subtype 2, param 0
- Play dialog: ARENA.SCR, line/variant 27

### Event 8

**Trigger**

- Group/spawn-list event: subject 139, op 0, value 0
- Group/spawn-list event: subject 32, op 0, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 12, param 39

### Event 9

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 41

**Action**

- Play dialog: ARENA.SCR, line/variant 39

### Event 10

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 40

**Action**

- Play dialog: ARENA.SCR, line/variant 58

## Waypoints

### Waypoint 0

- Tag: `502`
- Members: `Independent_Merc_Mako (object 3, id 509, starts at point 0)`, `Independent_Merc_Mako (object 4, id 510, starts at point 0)`, `Independent_Merc_Mako (object 5, id 511, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (548.87, -587.51, 8080.75) | None |
| 1 | (1663.26, -587.51, 6836.91) | None |
| 2 | (730.38, -587.51, 5534.54) | None |

### Waypoint 1

- Tag: `501`
- Members: `Independent_Merc_Mako (object 0, id 506, starts at point 0)`, `Independent_Merc_Mako (object 1, id 507, starts at point 0)`, `Independent_Merc_Mako (object 2, id 508, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-630.93, -587.51, 8154.55) | None |
| 1 | (-1710.92, -587.51, 6849.41) | None |
| 2 | (-653.62, -587.51, 5546.84) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Independent_Merc_Mako` | 506 | Interactive | -860.30,-587.51,9246.82 | 260,0,0 | label: bfne_02; group/role: FG_ALLIGATOR / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 1 (tag 501, 3 point(s)), starting point 0, arrival event value 32833536 |
| 1 | `Independent_Merc_Mako` | 507 | Interactive | -724.17,-587.51,9246.82 | 260,0,0 | group/role: FG_ALLIGATOR / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 1 (tag 501, 3 point(s)), starting point 0, arrival event value 32833536 |
| 2 | `Independent_Merc_Mako` | 508 | Interactive | -554.01,-587.51,9246.82 | 260,0,0 | group/role: FG_ALLIGATOR / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 1 (tag 501, 3 point(s)), starting point 0, arrival event value 32833536 |
| 3 | `Independent_Merc_Mako` | 509 | Interactive | 616.19,-587.51,9273.42 | 260,0,0 | group/role: FG_DRAGON / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 0 (tag 502, 3 point(s)), starting point 0, arrival event value 32899072 |
| 4 | `Independent_Merc_Mako` | 510 | Interactive | 706.95,-587.51,9261.12 | 260,0,0 | label: bfne_04; group/role: FG_DRAGON / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 0 (tag 502, 3 point(s)), starting point 0, arrival event value 32899072 |
| 5 | `Independent_Merc_Mako` | 511 | Interactive | 831.73,-587.51,9261.12 | 260,0,0 | group/role: FG_DRAGON / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 0 (tag 502, 3 point(s)), starting point 0, arrival event value 32899072 |
