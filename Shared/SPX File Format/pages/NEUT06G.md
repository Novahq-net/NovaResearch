# Tachyon: The Fringe NEUT06G.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT06G.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 5 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 7 |
| Events | 13 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Crate_6`, `1: Independent_Merc_Piranha`, `2: Independent_Merc_Dart` |
| Scripts | `PLAYER.SCR`, `WRECK.SCR`, `MERFR.SCR` |
| Scenes | None |
| Labels | `BFNE_02`, `bfbe_08`, `BFNE_01`, `bfne_09`, `bfbe_01`, `BLACK`, `repar` |
| Aliases | `Todd08`, `Todd09`, `Todd10`, `oside`, `oside_1`, `oside_2`, `bagel`, `bagel_1`, `bagel_2`, `kwB10_01`, `kwB10_02`, `Todd13`, `Todd12`, `Todd02`, `Todd03`, `Todd04`, `Todd05`, `Todd06`, `Todd07`, `will_01`, `kevin01`, `SHIP1_HYPER`, `SHIP2_HYPER`, `SHIP3_HYPER`, `ohshit` |
| Groups | `FG_MARBLE`, `FG_EMERALD`, `FG_AMETHYST` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Set runtime trigger variable: variable group 20, variable 16, subtype 0, value 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 21, op 1, value 0
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 16
- Object spawn/action: id 6264, subtype 14

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 6264; flags 2)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Object spawn/action: id 6264, subtype 15

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 6, value 2 (extra 1, 6264; flags 2)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Variable comparison: subject variable group 21, variable 21, op 1, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 16
- Set/add variable: variable group 21, variable 21, subtype 0, value 1
- Set/add variable: variable group 8, variable 4, subtype 0, value 0
- Play dialog: PLAYER.SCR, line/variant 108

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 16, op 1, value 17
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 199, subtype 1, param 4690

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 16, op 1, value 65
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 200, subtype 1, param 4690

### Event 6

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Set/add variable: variable group 13, variable 420, subtype 0, value 1
- Set/add variable: variable group 13, variable 421, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 33

### Event 7

**Trigger**

- Object event: subject Independent_Merc_Piranha (object 2, id 6223), op 2, value 0

**Action**

- Object spawn/action: Crate_6 (object 4, id 6265), subtype 1, param 6223
- Play dialog: PLAYER.SCR, line/variant 111

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 16, op 1, value 2

**Action**

- Play dialog: WRECK.SCR, line/variant 0

### Event 9

**Trigger**

- Variable comparison: subject variable group 20, variable 16, op 1, value 36

**Action**

- Play dialog: MERFR.SCR, line/variant 0
- Group/spawn-list action: spawn list/group 199, subtype 4, param 9

### Event 10

**Trigger**

- Group/spawn-list event: subject 200, op 0, value 0
- Group/spawn-list event: subject 199, op 0, value 0
- Group/spawn-list event: subject 143, op 0, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 112
- Object spawn/action: Crate_6 (object 4, id 6265), subtype 14

### Event 11

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 6265; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 113
- Set/add variable: variable group 0, variable 2, subtype 1, value 1250
- Set/add variable: variable group 13, variable 802, subtype 0, value 1
- Object spawn/action: Crate_6 (object 4, id 6265), subtype 15

### Event 12

**Trigger**

- Group/spawn-list event: subject 200, op 0, value 0 (join 2)
- Group/spawn-list event: subject 199, op 0, value 0 (join 2)

**Action**

- Group/spawn-list action: spawn list/group 143, subtype 1, param 4690

## Waypoints

### Waypoint 0

- Tag: `401`
- Members: `Independent_Merc_Dart (object 0, id 6220, starts at point 0)`, `Independent_Merc_Dart (object 1, id 6221, starts at point 0)`, `Independent_Merc_Piranha (object 2, id 6223, starts at point 0)`, `Independent_Merc_Piranha (object 3, id 6224, starts at point 0)`, `Independent_Merc_Dart (object 5, id 6225, starts at point 0)`, `Independent_Merc_Dart (object 6, id 6642, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-669.65, -67.44, -1171.18) | None |
| 1 | (-1663.64, -686.61, -440.12) | None |

## Spawn Lists

### Spawn List 0

- ID: `143`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | id 5649 | None |
| 1 | 6 | id 6264 | None |
| 2 | 0 | none | None |

### Spawn List 1

- ID: `199`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | id 5649 | None |
| 1 | 6 | id 6264 | None |
| 2 | 0 | none | None |

### Spawn List 2

- ID: `200`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | id 5649 | None |
| 1 | 6 | id 6264 | None |
| 2 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Independent_Merc_Dart` | 6220 | Interactive | 573.25,0.00,-2462.78 | 0,0,0 | group/role: FG_MARBLE / 1; alias: kwB10_01; waypoint: Waypoint 0 (tag 401, 2 point(s)), starting point 0, arrival event value 26279936 |
| 1 | `Independent_Merc_Dart` | 6221 | Interactive | 521.68,0.00,-2532.68 | 0,0,0 | label: bfbe_08; group/role: FG_MARBLE / 2; alias: kwB10_02; waypoint: Waypoint 0 (tag 401, 2 point(s)), starting point 0, arrival event value 26279936 |
| 2 | `Independent_Merc_Piranha` | 6223 | Interactive | 576.48,0.00,-2791.31 | 0,0,0 | group/role: FG_EMERALD / 1; waypoint: Waypoint 0 (tag 401, 2 point(s)), starting point 0, arrival event value 26279936 |
| 3 | `Independent_Merc_Piranha` | 6224 | Interactive | 512.01,0.00,-2861.21 | 0,0,0 | group/role: FG_EMERALD / 2; waypoint: Waypoint 0 (tag 401, 2 point(s)), starting point 0, arrival event value 26279936 |
| 4 | `Crate_6` | 6265 | Interactive | -1120.68,0.00,-875.89 | 114,121,57 | None |
| 5 | `Independent_Merc_Dart` | 6225 | Interactive | 638.25,0.00,-3156.52 | 0,0,0 | label: bfbe_01; group/role: FG_AMETHYST / 1; waypoint: Waypoint 0 (tag 401, 2 point(s)), starting point 0, arrival event value 26279936 |
| 6 | `Independent_Merc_Dart` | 6642 | Interactive | 586.21,0.00,-3230.63 | 0,0,0 | group/role: FG_AMETHYST / 2; waypoint: Waypoint 0 (tag 401, 2 point(s)), starting point 0, arrival event value 26279936 |
