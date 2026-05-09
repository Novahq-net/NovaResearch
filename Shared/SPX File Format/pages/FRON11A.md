# Tachyon: The Fringe FRON11A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON11A.SPX` |
| Sector | `QUAD_11` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 10 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 11 |
| Events | 12 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Baronial_Shuttle`, `1: Hajod_Fighter_1`, `2: Hajod_Fighter_2` |
| Scripts | `HAJOD.SCR` |
| Scenes | None |
| Labels | `bfne_05`, `BFBE_04`, `bfne_01`, `bfne_03`, `bfne_02`, `bfne_04`, `bfne_06`, `bfne_08`, `bfne_07`, `bfne_09` |
| Aliases | `BC05_sistine_chapel`, `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1`, `bc05_2`, `bc05_3`, `bc05_5`, `bc05_4`, `Stocks01` |
| Groups | `FG_DISCIPLINE`, `FG_MONARCH`, `FG_PUNISHER`, `FG_DESPOT`, `MANACLE` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 1200 (extra 1, 396; flags 2)

**Action**

- Play dialog: HAJOD.SCR, line/variant 5
- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0
- Play scene: unknown index 0, param 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 40

**Action**

- Group/spawn-list action: spawn list/group 132, subtype 1, param 2

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 45

**Action**

- Group/spawn-list action: spawn list/group 132, subtype 3, param 3

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 50

**Action**

- Group/spawn-list action: spawn list/group 162, subtype 1, param 2

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 55

**Action**

- Group/spawn-list action: spawn list/group 162, subtype 3, param 3

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 60

**Action**

- Group/spawn-list action: spawn list/group 131, subtype 1, param 2

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 65

**Action**

- Group/spawn-list action: spawn list/group 131, subtype 3, param 3

### Event 7

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 60

**Action**

- Mission objective/state: param 262150, subtype 0, param 0
- Show/update HUD contact: contact/list 0, subtype 6, param 396
- Hide/remove HUD contact: contact/list 0, subtype 9, param 24

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 90

**Action**

- Object spawn/action: Baronial_Shuttle (object 10, id 396), subtype 2, param 3
- Set runtime trigger variable: variable group 20, variable 0, subtype 1, value 0
- Group/spawn-list action: spawn list/group 87, subtype 3, param 2
- Group/spawn-list action: spawn list/group 86, subtype 3, param 2

### Event 9

**Trigger**

- Object event: subject Baronial_Shuttle (object 10, id 396), op 2, value 0

**Action**

- Set/add variable: variable group 16, variable 410, subtype 0, value 1
- Set/add variable: variable group 16, variable 411, subtype 0, value 1
- Broadcast mark/flash contact: contact/list 0, subtype 0, param 26

### Event 10

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 24
- Object spawn/action: Baronial_Shuttle (object 10, id 396), subtype 14

### Event 11

**Trigger**

- Object event: subject Baronial_Shuttle (object 10, id 396), op 7, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 6, param 396

## Waypoints

### Waypoint 0

- Tag: `3`
- Members: `Hajod_Fighter_1 (object 7, id 51, starts at point 0)`, `Hajod_Fighter_1 (object 8, id 52, starts at point 0)`, `Hajod_Fighter_1 (object 9, id 53, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1083.16, -550.44, 3901.99) | None |
| 1 | (1951.61, -550.44, 3061.04) | None |
| 2 | (1059.76, -550.44, 2369.94) | None |

### Waypoint 1

- Tag: `2`
- Members: `Hajod_Fighter_1 (object 4, id 48, starts at point 0)`, `Hajod_Fighter_1 (object 5, id 49, starts at point 0)`, `Hajod_Fighter_1 (object 6, id 50, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (367.33, -550.44, 3907.57) | None |
| 1 | (-465.19, -550.44, 3171.26) | None |
| 2 | (387.35, -550.44, 2398.18) | on arrival redirect to Waypoint 1 (tag 2), point 0 |

### Waypoint 2

- Tag: `1`
- Members: `Hajod_Fighter_2 (object 0, id 55, starts at point 0)`, `Hajod_Fighter_2 (object 1, id 56, starts at point 0)`, `Hajod_Fighter_2 (object 2, id 57, starts at point 0)`, `Hajod_Fighter_2 (object 3, id 58, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (8.30, 0.00, 1370.56) | None |
| 1 | (315.49, 0.00, 1871.83) | None |
| 2 | (855.13, 0.00, 1761.55) | None |
| 3 | (996.27, 0.00, 1440.74) | None |
| 4 | (1079.29, 0.00, 1089.86) | on arrival play dialog/script or enter gate, param 3 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hajod_Fighter_2` | 55 | Interactive | -40.46,0.00,1007.44 | 0,0,0 | group/role: FG_DISCIPLINE / 0; alias: jumbo; waypoint: Waypoint 2 (tag 1, 5 point(s)), starting point 0, arrival event value 65536 |
| 1 | `Hajod_Fighter_2` | 56 | Interactive | 44.42,0.00,1007.44 | 0,0,0 | group/role: FG_DISCIPLINE / 0; alias: jumbo_1; waypoint: Waypoint 2 (tag 1, 5 point(s)), starting point 0, arrival event value 65536 |
| 2 | `Hajod_Fighter_2` | 57 | Interactive | -48.94,0.00,874.19 | 0,0,0 | group/role: FG_MONARCH / 0; alias: egg; waypoint: Waypoint 2 (tag 1, 5 point(s)), starting point 0, arrival event value 65536 |
| 3 | `Hajod_Fighter_2` | 58 | Interactive | 38.15,0.00,863.94 | 0,0,0 | group/role: FG_MONARCH / 0; alias: egg_1; waypoint: Waypoint 2 (tag 1, 5 point(s)), starting point 0, arrival event value 65536 |
| 4 | `Hajod_Fighter_1` | 48 | Interactive | 626.83,-550.44,3324.62 | 0,0,0 | group/role: FG_PUNISHER / 0; waypoint: Waypoint 1 (tag 2, 3 point(s)), starting point 0, arrival event value 131072 |
| 5 | `Hajod_Fighter_1` | 49 | Interactive | 620.58,-550.44,3000.95 | 0,0,0 | group/role: FG_PUNISHER / 0; waypoint: Waypoint 1 (tag 2, 3 point(s)), starting point 0, arrival event value 131072 |
| 6 | `Hajod_Fighter_1` | 50 | Interactive | 415.68,-550.44,3181.40 | 0,0,0 | group/role: FG_PUNISHER / 0; waypoint: Waypoint 1 (tag 2, 3 point(s)), starting point 0, arrival event value 131072 |
| 7 | `Hajod_Fighter_1` | 51 | Interactive | 880.00,-550.44,3331.55 | 0,0,0 | group/role: FG_DESPOT / 0; waypoint: Waypoint 0 (tag 3, 3 point(s)), starting point 0, arrival event value 196608 |
| 8 | `Hajod_Fighter_1` | 52 | Interactive | 877.84,-550.44,2986.25 | 0,0,0 | group/role: FG_DESPOT / 0; waypoint: Waypoint 0 (tag 3, 3 point(s)), starting point 0, arrival event value 196608 |
| 9 | `Hajod_Fighter_1` | 53 | Interactive | 1057.79,-550.44,3183.02 | 0,0,0 | group/role: FG_DESPOT / 0; waypoint: Waypoint 0 (tag 3, 3 point(s)), starting point 0, arrival event value 196608 |
| 10 | `Baronial_Shuttle` | 396 | Interactive | 756.17,-551.42,3177.22 | 0,0,0 | alias: Hajod_1; secondary groups: none, MANACLE |
