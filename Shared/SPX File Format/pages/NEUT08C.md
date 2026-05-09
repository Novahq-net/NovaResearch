# Tachyon: The Fringe NEUT08C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT08C.SPX` |
| Sector | `QUAD_08` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 7 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 5 |
| Events | 8 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Lt_Freighter`, `1: Luxury_Liner`, `2: Bora_Dagger`, `3: Shuttle_Medium` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `bfne_03` |
| Aliases | `Jerome26`, `Jerome25`, `Jerome24`, `Jerome22`, `Jerome21`, `Jerome20`, `kwI03_10` |
| Groups | `FG_GRACE`, `HESPERIDES`, `CONT_044` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 20, op 1, value 0

**Action**

- Gate state/action: param 9, subtype 3, param 0
- Set runtime trigger variable: variable group 20, variable 19, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 4
- Variable comparison: subject variable group 13, variable 413, op 1, value 0

**Action**

- Object spawn/action: GalSpan_Lt_Freighter (object 4, id 31), subtype 3
- Show/update HUD contact: contact/list 0, subtype 6, param 31
- Set runtime trigger variable: variable group 20, variable 19, subtype 1, value 0
- Play dialog: PLAYER.SCR, line/variant 79
- Object spawn/action: GalSpan_Lt_Freighter (object 4, id 31), subtype 14

### Event 2

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 79 (join 2)
- Object event: subject GalSpan_Lt_Freighter (object 4, id 31), op 0, value 0 (extra 5, 171; flags 2)

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 6, param 31
- Show/update HUD contact: contact/list 0, subtype 1, param 171
- Show/update HUD contact: contact/list 0, subtype 2, param 31
- Group/spawn-list action: spawn list/group 171, subtype 4, param 9

### Event 3

**Trigger**

- Group/spawn-list event: subject 171, op 0, value 0
- Variable comparison: subject variable group 21, variable 20, op 1, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 171
- Play dialog: PLAYER.SCR, line/variant 80
- Object spawn/action: GalSpan_Lt_Freighter (object 4, id 31), subtype 5
- Show/update HUD contact: contact/list 0, subtype 6, param 31
- Hide/remove HUD contact: contact/list 0, subtype 2, param 31

### Event 4

**Trigger**

- Object arrival: GalSpan_Lt_Freighter (object 4, id 31) reached Waypoint 2 (tag 201), point 1 (raw value 13172737)

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 6, param 31
- Set/add variable: variable group 13, variable 412, subtype 0, value 1
- Set/add variable: variable group 13, variable 413, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 33
- Play dialog: PLAYER.SCR, line/variant 81
- Object spawn/action: GalSpan_Lt_Freighter (object 4, id 31), subtype 15

### Event 5

**Trigger**

- Object event: subject GalSpan_Lt_Freighter (object 4, id 31), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Set/add variable: variable group 21, variable 26, subtype 0, value 1

### Event 6

**Trigger**

- Variable comparison: subject variable group 21, variable 26, op 1, value 1

**Action**

- Set/add variable: variable group 13, variable 412, subtype 0, value 1
- Set/add variable: variable group 13, variable 413, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Mark/flash contact: contact/list 0, subtype 6, param 31
- Show/update HUD contact: contact/list 0, subtype 11, param 34
- Set/add variable: variable group 21, variable 20, subtype 0, value 1

### Event 7

**Trigger**

- Object arrival: Luxury_Liner (object 3, id 35) reached Waypoint 1 (tag 202), point 1 (raw value 13238273)

**Action**

- Object spawn/action: Luxury_Liner (object 3, id 35), subtype 4

## Waypoints

### Waypoint 0

- Tag: `203`
- Members: `Bora_Dagger (object 1, id 53, starts at point 0)`, `Bora_Dagger (object 2, id 54, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-59.11, 148.76, 2390.73) | None |

### Waypoint 1

- Tag: `202`
- Members: `Luxury_Liner (object 3, id 35, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1434.00, -391.77, 1845.35) | None |
| 1 | (2732.41, 0.00, 3093.92) | None; listened by Event 7 for Luxury_Liner (object 3, id 35) |

### Waypoint 2

- Tag: `201`
- Members: `GalSpan_Lt_Freighter (object 4, id 31, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (131.22, 195.04, 2595.97) | on arrival activate current object (raw param -1 ignored) |
| 1 | (-269.75, 172.99, 1989.72) | on arrival activate current object (raw param -1 ignored); listened by Event 4 for GalSpan_Lt_Freighter (object 4, id 31) |

## Spawn Lists

### Spawn List 0

- ID: `171`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | GalSpan_Lt_Freighter (object 4, id 31) | None |
| 1 | 6 | Luxury_Liner (object 3, id 35) | None |
| 2 | 6 | id 30 | None |
| 3 | 6 | Shuttle_Medium (object 0, id 38) | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Shuttle_Medium` | 38 | Interactive | -27.34,-545.41,1183.56 | 164,0,0 | None |
| 1 | `Bora_Dagger` | 53 | Interactive | -729.58,0.00,2040.06 | 50,0,0 | label: bfne_03; group/role: FG_GRACE / 1; waypoint: Waypoint 0 (tag 203, 1 point(s)), starting point 0, arrival event value 13303808 |
| 2 | `Bora_Dagger` | 54 | Interactive | -703.71,50.33,1957.97 | 57,0,156 | group/role: FG_GRACE / 2; waypoint: Waypoint 0 (tag 203, 1 point(s)), starting point 0, arrival event value 13303808 |
| 3 | `Luxury_Liner` | 35 | Interactive | 305.22,-522.36,1225.60 | 92,0,0 | waypoint: Waypoint 1 (tag 202, 2 point(s)), starting point 0, arrival event value 13238272 |
| 4 | `GalSpan_Lt_Freighter` | 31 | Interactive | 229.34,199.73,2743.04 | 299,0,100 | alias: kwI03_10; secondary groups: CONT_044, HESPERIDES; waypoint: Waypoint 2 (tag 201, 2 point(s)), starting point 0, arrival event value 13172736 |
