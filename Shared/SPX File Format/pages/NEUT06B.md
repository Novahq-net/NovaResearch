# Tachyon: The Fringe NEUT06B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT06B.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 5 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 15 |
| Events | 17 |
| Waypoints | 5 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Star_Patrol_Capital_Ship`, `1: Tycho_Brahe`, `2: Crate_5_Special_Placehold`, `3: Star_Patrol_Enforcer` |
| Scripts | `PLAYER.SCR`, `REPAR.SCR`, `STP2.SCR` |
| Scenes | None |
| Labels | `BFNE_02`, `bfbe_08`, `BFNE_01`, `bfne_09`, `bfbe_01`, `BLACK`, `repar` |
| Aliases | `Todd08`, `Todd09`, `Todd10`, `oside`, `oside_1`, `oside_2`, `bagel`, `bagel_1`, `bagel_2`, `kwB10_01`, `kwB10_02`, `Todd13`, `Todd12`, `Todd02`, `Todd03`, `Todd04`, `Todd05`, `Todd06`, `Todd07`, `will_01`, `kevin01`, `SHIP1_HYPER`, `SHIP2_HYPER`, `SHIP3_HYPER`, `ohshit` |
| Groups | `FG_SLEET`, `FG_TORNADO`, `FG_HAIL`, `FG_NOVA`, `TYCHO_BRAHE`, `CONT_004` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 8, variable 2, op 1, value 1

**Action**

- Set runtime trigger variable: variable group 20, variable 19, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 38

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Gate state/action: param 4691, subtype 3, param 0

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 4

**Action**

- Play dialog: PLAYER.SCR, line/variant 29
- Set runtime trigger variable: variable group 20, variable 19, subtype 1, value 0

### Event 3

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 29

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 21
- Hide/remove HUD contact: contact/list 0, subtype 9, param 38
- Object spawn/action: Crate_5_Special_Placehold (object 12, id 6851), subtype 14

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 6, value 1 (extra 1, 5476; flags 2)
- Variable comparison: subject variable group 8, variable 2, op 1, value 1

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Set/add variable: variable group 8, variable 2, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 25
- Object spawn/action: Crate_5_Special_Placehold (object 12, id 6851), subtype 15
- Object spawn/action: Crate_5_Special_Placehold (object 12, id 6851), subtype 19

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 5, value 0 (extra 1, 5476; flags 2)
- Variable comparison: subject variable group 8, variable 2, op 1, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Object spawn/action: Tycho_Brahe (object 13, id 5476), subtype 5
- Show/update HUD contact: contact/list 0, subtype 9, param 37

### Event 6

**Trigger**

- Object arrival: Tycho_Brahe (object 13, id 5476) reached Waypoint 4 (tag 151), point 3 (raw value 9895939)

**Action**

- Set/add variable: variable group 21, variable 27, subtype 0, value 1
- Set runtime trigger variable: variable group 20, variable 19, subtype 0, value 0

### Event 7

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 18

**Action**

- Play dialog: REPAR.SCR, line/variant 2
- Set/add variable: variable group 13, variable 402, subtype 0, value 1
- Set/add variable: variable group 13, variable 403, subtype 0, value 2
- Object spawn/action: Tycho_Brahe (object 13, id 5476), subtype 5

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 24

**Action**

- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 33
- Hide/remove HUD contact: contact/list 0, subtype 9, param 37

### Event 9

**Trigger**

- Object event: subject Tycho_Brahe (object 13, id 5476), op 0, value 0 (flags 3)
- Sector/startup condition family: subject 0, op 0, value 29

**Action**

- Play dialog: REPAR.SCR, line/variant 3
- Object spawn/action: Tycho_Brahe (object 13, id 5476), subtype 8, param 9

### Event 10

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 3
- Variable comparison: subject variable group 21, variable 27, op 1, value 0

**Action**

- Set/add variable: variable group 13, variable 402, subtype 0, value 0
- Set/add variable: variable group 13, variable 403, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 34
- Object spawn/action: Tycho_Brahe (object 13, id 5476), subtype 4
- Set runtime trigger variable: variable group 20, variable 26, subtype 0, value 0

### Event 11

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 3
- Variable comparison: subject variable group 21, variable 27, op 1, value 1

**Action**

- Object spawn/action: Tycho_Brahe (object 13, id 5476), subtype 4

### Event 12

**Trigger**

- Variable comparison: subject variable group 20, variable 26, op 1, value 4

**Action**

- Group/spawn-list action: spawn list/group 191, subtype 1, param 4690

### Event 13

**Trigger**

- Variable comparison: subject variable group 20, variable 26, op 1, value 8

**Action**

- Group/spawn-list action: spawn list/group 256, subtype 1, param 4690

### Event 14

**Trigger**

- Variable comparison: subject variable group 20, variable 26, op 1, value 12

**Action**

- Group/spawn-list action: spawn list/group 163, subtype 1, param 4690
- Object spawn/action: Star_Patrol_Capital_Ship (object 14, id 6801), subtype 3

### Event 15

**Trigger**

- Variable comparison: subject variable group 20, variable 26, op 1, value 16

**Action**

- Group/spawn-list action: spawn list/group 120, subtype 1, param 4690

### Event 16

**Trigger**

- Variable comparison: subject variable group 20, variable 26, op 1, value 10

**Action**

- Play dialog: STP2.SCR, line/variant 0

## Waypoints

### Waypoint 0

- Tag: `158`
- Members: `Star_Patrol_Enforcer (object 9, id 6811, starts at point 0)`, `Star_Patrol_Enforcer (object 10, id 6812, starts at point 0)`, `Star_Patrol_Enforcer (object 11, id 6813, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-121.20, -224.79, -1677.21) | None |

### Waypoint 1

- Tag: `157`
- Members: `Star_Patrol_Enforcer (object 6, id 6808, starts at point 0)`, `Star_Patrol_Enforcer (object 7, id 6809, starts at point 0)`, `Star_Patrol_Enforcer (object 8, id 6810, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-247.05, -122.31, -1838.82) | None |

### Waypoint 2

- Tag: `156`
- Members: `Star_Patrol_Enforcer (object 3, id 6805, starts at point 0)`, `Star_Patrol_Enforcer (object 4, id 6806, starts at point 0)`, `Star_Patrol_Enforcer (object 5, id 6807, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-184.44, 46.28, -341.89) | None |

### Waypoint 3

- Tag: `155`
- Members: `Star_Patrol_Enforcer (object 0, id 6802, starts at point 0)`, `Star_Patrol_Enforcer (object 1, id 6803, starts at point 0)`, `Star_Patrol_Enforcer (object 2, id 6804, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-215.48, -390.08, -1037.37) | None |

### Waypoint 4

- Tag: `151`
- Members: `Tycho_Brahe (object 13, id 5476, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1496.71, -37.74, 138.07) | None |
| 1 | (-1592.74, -37.61, 138.25) | None |
| 2 | (-1874.93, -37.24, 137.08) | None |
| 3 | (-2164.53, -27.77, 141.81) | on arrival activate current object (raw param -1 ignored); listened by Event 6 for Tycho_Brahe (object 13, id 5476) |
| 4 | (-2785.28, -26.36, 180.89) | on arrival activate current object (raw param -1 ignored) |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Star_Patrol_Enforcer` | 6802 | Interactive | 306.78,0.00,-2168.52 | 0,0,0 | group/role: FG_SLEET / 1; waypoint: Waypoint 3 (tag 155, 1 point(s)), starting point 0, arrival event value 10158080 |
| 1 | `Star_Patrol_Enforcer` | 6803 | Interactive | 196.35,0.00,-2272.77 | 0,0,0 | group/role: FG_SLEET / 2; waypoint: Waypoint 3 (tag 155, 1 point(s)), starting point 0, arrival event value 10158080 |
| 2 | `Star_Patrol_Enforcer` | 6804 | Interactive | 382.64,0.00,-2312.08 | 0,0,0 | group/role: FG_SLEET / 3; waypoint: Waypoint 3 (tag 155, 1 point(s)), starting point 0, arrival event value 10158080 |
| 3 | `Star_Patrol_Enforcer` | 6805 | Interactive | 301.46,0.00,-2546.21 | 0,0,0 | group/role: FG_TORNADO / 1; waypoint: Waypoint 2 (tag 156, 1 point(s)), starting point 0, arrival event value 10223616 |
| 4 | `Star_Patrol_Enforcer` | 6806 | Interactive | 196.48,0.00,-2688.21 | 0,0,0 | group/role: FG_TORNADO / 2; waypoint: Waypoint 2 (tag 156, 1 point(s)), starting point 0, arrival event value 10223616 |
| 5 | `Star_Patrol_Enforcer` | 6807 | Interactive | 412.94,0.00,-2678.82 | 0,0,0 | group/role: FG_TORNADO / 3; waypoint: Waypoint 2 (tag 156, 1 point(s)), starting point 0, arrival event value 10223616 |
| 6 | `Star_Patrol_Enforcer` | 6808 | Interactive | 321.89,0.00,-2887.09 | 0,0,0 | group/role: FG_HAIL / 1; waypoint: Waypoint 1 (tag 157, 1 point(s)), starting point 0, arrival event value 10289152 |
| 7 | `Star_Patrol_Enforcer` | 6809 | Interactive | 185.55,0.00,-3029.24 | 0,0,0 | group/role: FG_HAIL / 2; waypoint: Waypoint 1 (tag 157, 1 point(s)), starting point 0, arrival event value 10289152 |
| 8 | `Star_Patrol_Enforcer` | 6810 | Interactive | 418.90,0.00,-3017.87 | 0,0,0 | group/role: FG_HAIL / 3; waypoint: Waypoint 1 (tag 157, 1 point(s)), starting point 0, arrival event value 10289152 |
| 9 | `Star_Patrol_Enforcer` | 6811 | Interactive | 345.49,0.00,-3198.40 | 0,0,0 | group/role: FG_NOVA / 1; waypoint: Waypoint 0 (tag 158, 1 point(s)), starting point 0, arrival event value 10354688 |
| 10 | `Star_Patrol_Enforcer` | 6812 | Interactive | 192.10,0.00,-3333.44 | 0,0,0 | group/role: FG_NOVA / 2; waypoint: Waypoint 0 (tag 158, 1 point(s)), starting point 0, arrival event value 10354688 |
| 11 | `Star_Patrol_Enforcer` | 6813 | Interactive | 450.37,0.00,-3334.86 | 0,0,0 | group/role: FG_NOVA / 3; waypoint: Waypoint 0 (tag 158, 1 point(s)), starting point 0, arrival event value 10354688 |
| 12 | `Crate_5_Special_Placehold` | 6851 | Interactive | -1135.20,10.73,138.38 | 0,0,0 | None |
| 13 | `Tycho_Brahe` | 5476 | Interactive | -1144.73,-35.59,137.60 | 384,0,0 | label: repar; secondary groups: CONT_004, TYCHO_BRAHE; waypoint: Waypoint 4 (tag 151, 5 point(s)), starting point 0, arrival event value 9895936 |
| 14 | `Star_Patrol_Capital_Ship` | 6801 | Interactive | -848.94,-234.71,-1610.32 | 21,0,0 | None |
