# Tachyon: The Fringe NEUT06E.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT06E.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 5 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 5 |
| Entities | 12 |
| Events | 24 |
| Waypoints | 4 |
| Child Sectors | 0 |
| Scripts | 4 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Light_Freighter`, `1: Redship_Rory`, `2: Red_Pirate_Fighter_2`, `3: Red_Pirate_Shrike`, `4: Star_Patrol_Enforcer` |
| Scripts | `PLAYER.SCR`, `RRORY.SCR`, `AOBUL.SCR`, `GALLU.SCR` |
| Scenes | None |
| Labels | `BFNE_02`, `bfbe_08`, `BFNE_01`, `bfne_09`, `bfbe_01`, `BLACK`, `repar` |
| Aliases | `Todd08`, `Todd09`, `Todd10`, `oside`, `oside_1`, `oside_2`, `bagel`, `bagel_1`, `bagel_2`, `kwB10_01`, `kwB10_02`, `Todd13`, `Todd12`, `Todd02`, `Todd03`, `Todd04`, `Todd05`, `Todd06`, `Todd07`, `will_01`, `kevin01`, `SHIP1_HYPER`, `SHIP2_HYPER`, `SHIP3_HYPER`, `ohshit` |
| Groups | `FG_SLEET`, `FG_FAMINE`, `FG_ENVY`, `REDSHIP_RORY`, `FG_CONTEMPT`, `GALLURAN`, `CONT_041` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Gate state/action: param 4691, subtype 3, param 0
- Object spawn/action: id 5649, subtype 8, param 10

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Object spawn/action: Generic_Light_Freighter (object 11, id 6060), subtype 3
- Show/update HUD contact: contact/list 0, subtype 6, param 6060
- Set runtime trigger variable: variable group 20, variable 28, subtype 0, value 0
- Object spawn/action: Generic_Light_Freighter (object 11, id 6060), subtype 14

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 28, op 1, value 24

**Action**

- Set runtime trigger variable: variable group 20, variable 28, subtype 1, value 0
- Play dialog: PLAYER.SCR, line/variant 116

### Event 3

**Trigger**

- Object arrival: Generic_Light_Freighter (object 11, id 6060) reached Waypoint 3 (tag 301), point 0 (raw value 19726336)

**Action**

- Set runtime trigger variable: variable group 20, variable 28, subtype 0, value 0

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 28, op 1, value 38

**Action**

- Set runtime trigger variable: variable group 20, variable 28, subtype 1, value 0

### Event 5

**Trigger**

- Group/spawn-list event: subject 151, op 1, value 70

**Action**

- Show/update HUD contact: contact/list 0, subtype 1, param 242
- Set runtime trigger variable: variable group 20, variable 28, subtype 0, value 0
- Group/spawn-list action: spawn list/group 242, subtype 0

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 28, op 1, value 60

**Action**

- Group/spawn-list action: spawn list/group 152, subtype 0
- Show/update HUD contact: contact/list 0, subtype 1, param 152
- Show/update HUD contact: contact/list 0, subtype 9, param 46

### Event 7

**Trigger**

- Variable comparison: subject variable group 20, variable 28, op 1, value 64

**Action**

- Set runtime trigger variable: variable group 20, variable 28, subtype 1, value 0
- Play dialog: RRORY.SCR, line/variant 0

### Event 8

**Trigger**

- Variable comparison: subject variable group 21, variable 23, op 1, value 1
- Variable comparison: subject variable group 21, variable 24, op 1, value 1
- Group/spawn-list event: subject 242, op 0, value 0
- Group/spawn-list event: subject 151, op 0, value 0

**Action**

- Set/add variable: variable group 13, variable 422, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 12, param 33
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 9

**Trigger**

- Object arrival: Generic_Light_Freighter (object 11, id 6060) reached Waypoint 3 (tag 301), point 1 (raw value 19726337)
- Object event: subject Generic_Light_Freighter (object 11, id 6060), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 6, param 6060

### Event 10

**Trigger**

- Object event: subject Red_Pirate_Fighter_2 (object 6, id 6078), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 152

### Event 11

**Trigger**

- Group/spawn-list event: subject 151, op 0, value 0
- Group/spawn-list event: subject 152, op 0, value 0
- Group/spawn-list event: subject 242, op 0, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 23, subtype 0, value 0
- Set/add variable: variable group 13, variable 423, subtype 0, value 3

### Event 12

**Trigger**

- Group/spawn-list event: subject 151, op 0, value 0
- Object event: subject Red_Pirate_Fighter_2 (object 6, id 6078), op 2, value 0
- Object event: subject Redship_Rory (object 7, id 6077), op 6, value 0
- Group/spawn-list event: subject 242, op 0, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 23, subtype 0, value 0
- Play dialog: RRORY.SCR, line/variant 2
- Set/add variable: variable group 13, variable 423, subtype 0, value 2

### Event 13

**Trigger**

- Variable comparison: subject variable group 20, variable 23, op 1, value 12

**Action**

- Group/spawn-list action: spawn list/group 191, subtype 1, param 4690

### Event 14

**Trigger**

- Group/spawn-list event: subject 151, op 4, value 0 (join 2; flags 2)

**Action**

- Object spawn/action: Generic_Light_Freighter (object 11, id 6060), subtype 8, param 10
- Object spawn/action: Generic_Light_Freighter (object 11, id 6060), subtype 15
- Hide/remove HUD contact: contact/list 0, subtype 6, param 6060

### Event 15

**Trigger**

- Variable comparison: subject variable group 20, variable 23, op 1, value 20

**Action**

- Play dialog: AOBUL.SCR, line/variant 22

### Event 16

**Trigger**

- Object event: subject Generic_Light_Freighter (object 11, id 6060), op 0, value 0 (flags 2)

**Action**

- Play dialog: GALLU.SCR, line/variant 2

### Event 17

**Trigger**

- Variable comparison: subject variable group 20, variable 28, op 1, value 26

**Action**

- Group/spawn-list action: spawn list/group 151, subtype 0
- Play dialog: GALLU.SCR, line/variant 1

### Event 18

**Trigger**

- Object event: subject Redship_Rory (object 7, id 6077), op 2, value 0 (join 2)
- Object event: subject Redship_Rory (object 7, id 6077), op 6, value 0

**Action**

- Set/add variable: variable group 21, variable 23, subtype 0, value 1

### Event 19

**Trigger**

- Object event: subject Red_Pirate_Fighter_2 (object 6, id 6078), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 24, subtype 0, value 1

### Event 20

**Trigger**

- Object event: subject Redship_Rory (object 7, id 6077), op 6, value 0 (join 1)
- Object event: subject Red_Pirate_Fighter_2 (object 6, id 6078), op 2, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 168

### Event 21

**Trigger**

- Object event: subject Redship_Rory (object 7, id 6077), op 2, value 0 (join 2)
- Object event: subject Redship_Rory (object 7, id 6077), op 6, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 46

### Event 22

**Trigger**

- Sector/startup condition family: subject 3, op 0, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 1, param 151

### Event 23

**Trigger**

- Object event: subject Generic_Light_Freighter (object 11, id 6060), op 2, value 0
- Variable comparison: subject variable group 20, variable 28, op 3, value 25

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Set/add variable: variable group 13, variable 422, subtype 0, value 1
- Set/add variable: variable group 13, variable 423, subtype 0, value 1
- Set/add variable: variable group 20, variable 28, subtype 0, value 100
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 34

## Waypoints

### Waypoint 0

- Tag: `304`
- Members: `Star_Patrol_Enforcer (object 0, id 6148, starts at point 0)`, `Star_Patrol_Enforcer (object 1, id 6149, starts at point 0)`, `Star_Patrol_Enforcer (object 2, id 6150, starts at point 0)`, `Red_Pirate_Shrike (object 8, id 6652, starts at point 0)`, `Red_Pirate_Shrike (object 9, id 6653, starts at point 0)`, `Red_Pirate_Shrike (object 10, id 6674, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1212.96, 0.00, -1536.49) | None |
| 1 | (-1778.05, -683.67, -1035.47) | None |

### Waypoint 1

- Tag: `303`
- Members: `Red_Pirate_Fighter_2 (object 6, id 6078, starts at point 0)`, `Redship_Rory (object 7, id 6077, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (54.99, -161.95, -2201.37) | None |
| 1 | (-49.23, -275.52, -2440.71) | None |
| 2 | (-946.75, -375.37, -1954.57) | None |

### Waypoint 2

- Tag: `302`
- Members: `Red_Pirate_Shrike (object 3, id 6069, starts at point 0)`, `Red_Pirate_Shrike (object 4, id 6074, starts at point 0)`, `Red_Pirate_Shrike (object 5, id 6075, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (429.70, 723.18, -1238.81) | None |
| 1 | (-625.24, 424.08, -1675.01) | None |
| 2 | (-1478.36, -359.09, -1274.20) | None |

### Waypoint 3

- Tag: `301`
- Members: `Generic_Light_Freighter (object 11, id 6060, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1053.80, -500.66, -2086.59) | None; listened by Event 3 for Generic_Light_Freighter (object 11, id 6060) |
| 1 | (-1960.29, -1240.10, -701.58) | on arrival activate current object (raw param -1 ignored); listened by Event 9 for Generic_Light_Freighter (object 11, id 6060) |

## Spawn Lists

### Spawn List 0

- ID: `242`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 6 | id 5649 | None |
| 2 | 6 | Generic_Light_Freighter (object 11, id 6060) | None |

### Spawn List 1

- ID: `152`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | Generic_Light_Freighter (object 11, id 6060) | None |
| 1 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Star_Patrol_Enforcer` | 6148 | Interactive | 489.09,0.00,-2133.26 | 435,0,0 | group/role: FG_SLEET / 0; waypoint: Waypoint 0 (tag 304, 2 point(s)), starting point 0, arrival event value 19922944 |
| 1 | `Star_Patrol_Enforcer` | 6149 | Interactive | 509.58,0.00,-2265.20 | 428,0,0 | group/role: FG_SLEET / 0; waypoint: Waypoint 0 (tag 304, 2 point(s)), starting point 0, arrival event value 19922944 |
| 2 | `Star_Patrol_Enforcer` | 6150 | Interactive | 628.82,0.00,-2151.09 | 442,0,0 | group/role: FG_SLEET / 0; waypoint: Waypoint 0 (tag 304, 2 point(s)), starting point 0, arrival event value 19922944 |
| 3 | `Red_Pirate_Shrike` | 6069 | Interactive | 772.79,572.84,-1187.14 | 358,28,210 | group/role: FG_FAMINE / 1; waypoint: Waypoint 2 (tag 302, 3 point(s)), starting point 0, arrival event value 19791872 |
| 4 | `Red_Pirate_Shrike` | 6074 | Interactive | 797.61,586.73,-1152.79 | 358,28,210 | label: BFNE_02; group/role: FG_FAMINE / 2; waypoint: Waypoint 2 (tag 302, 3 point(s)), starting point 0, arrival event value 19791872 |
| 5 | `Red_Pirate_Shrike` | 6075 | Interactive | 797.15,545.53,-1203.22 | 358,28,210 | group/role: FG_FAMINE / 3; waypoint: Waypoint 2 (tag 302, 3 point(s)), starting point 0, arrival event value 19791872 |
| 6 | `Red_Pirate_Fighter_2` | 6078 | Interactive | 71.27,-162.64,-2027.47 | 256,0,0 | group/role: FG_ENVY / 2; waypoint: Waypoint 1 (tag 303, 3 point(s)), starting point 0, arrival event value 19857408 |
| 7 | `Redship_Rory` | 6077 | Interactive | 42.23,-180.26,-2049.69 | 259,0,0 | group/role: FG_ENVY / 1; secondary groups: none, REDSHIP_RORY; waypoint: Waypoint 1 (tag 303, 3 point(s)), starting point 0, arrival event value 19857408 |
| 8 | `Red_Pirate_Shrike` | 6652 | Interactive | -62.98,0.00,-1257.56 | 455,441,0 | label: bfne_09; group/role: FG_CONTEMPT / 1; waypoint: Waypoint 0 (tag 304, 2 point(s)), starting point 0, arrival event value 19922944 |
| 9 | `Red_Pirate_Shrike` | 6653 | Interactive | -55.32,0.00,-1315.38 | 476,427,0 | group/role: FG_CONTEMPT / 2; waypoint: Waypoint 0 (tag 304, 2 point(s)), starting point 0, arrival event value 19922944 |
| 10 | `Red_Pirate_Shrike` | 6674 | Interactive | -3.70,0.00,-1284.31 | 448,441,0 | group/role: FG_CONTEMPT / 3; waypoint: Waypoint 0 (tag 304, 2 point(s)), starting point 0, arrival event value 19922944 |
| 11 | `Generic_Light_Freighter` | 6060 | Interactive | -654.08,0.00,-2608.62 | 464,449,112 | alias: kevin01; secondary groups: CONT_041, GALLURAN; waypoint: Waypoint 3 (tag 301, 2 point(s)), starting point 0, arrival event value 19726336 |
