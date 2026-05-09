# Tachyon: The Fringe FRON12E.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON12E.SPX` |
| Sector | `QUAD_12` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 11 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 19 |
| Events | 18 |
| Waypoints | 5 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Crate_5_Special_Placehold`, `1: Red_Pirate_Fighter_2`, `2: Red_Pirate_Shrike` |
| Scripts | `PRSPH.SCR`, `BLODC.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFNF_01`, `BFGE_01`, `BFNE_02` |
| Aliases | `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1`, `Stocks01` |
| Groups | `FG_PLAGUE`, `FG_ENVY`, `FG_GLUTTONY`, `FG_CONTEMPT`, `FG_DISDAIN` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Object spawn/action: id 1333, subtype 6
- Object spawn/action: id 1333, subtype 18
- Show/update HUD contact: contact/list 0, subtype 9, param 19
- Play dialog: PRSPH.SCR, line/variant 9

### Event 1

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 9

**Action**

- Play dialog: BLODC.SCR, line/variant 0
- Show/update HUD contact: contact/list 0, subtype 1, param 152
- Hide/remove HUD contact: contact/list 0, subtype 9, param 19
- Group/spawn-list action: spawn list/group 152, subtype 4, param 9

### Event 2

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 125

### Event 3

**Trigger**

- Group/spawn-list event: subject 152, op 0, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 19
- Set/add variable: variable group 21, variable 28, subtype 0, value 1
- Object spawn/action: Crate_5_Special_Placehold (object 18, id 1466), subtype 14

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 8, value 0 (extra 1, 1333; flags 3)
- Variable comparison: subject variable group 21, variable 28, op 1, value 1

**Action**

- Object spawn/action: Crate_5_Special_Placehold (object 18, id 1466), subtype 15
- Gate state/action: param 1, subtype 3, param 0
- Gate state/action: param 2, subtype 3, param 0
- Gate state/action: param 3, subtype 3, param 0

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1333; flags 2)

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 19
- Show/update HUD contact: contact/list 0, subtype 9, param 45

### Event 6

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 5, value 0 (extra 1, 1333; flags 3)
- Variable comparison: subject variable group 21, variable 28, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 242, subtype 0
- Group/spawn-list action: spawn list/group 193, subtype 0
- Play dialog: PRSPH.SCR, line/variant 11
- Show/update HUD contact: contact/list 0, subtype 2, param 1333
- Hide/remove HUD contact: contact/list 0, subtype 9, param 45
- Set runtime trigger variable: variable group 20, variable 19, subtype 0, value 0

### Event 7

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 30

**Action**

- Group/spawn-list action: spawn list/group 65, subtype 0
- Group/spawn-list action: spawn list/group 168, subtype 0

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 65 (join 1)
- Object event: subject 1333, op 2, value 0

**Action**

- Play dialog: PRSPH.SCR, line/variant 12

### Event 9

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 150 (join 1)
- Object event: subject 1333, op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 7, subtype 0, value 1
- Play dialog: PRSPH.SCR, line/variant 13

### Event 10

**Trigger**

- Object arrival: 1333 reached waypoint tag 51, point 2 (raw value 3342338)
- Variable comparison: subject variable group 16, variable 427, op 1, value 1

**Action**

- Gate state/action: param 1, subtype 2, param 0
- Gate state/action: param 2, subtype 2, param 0
- Gate state/action: param 3, subtype 2, param 0

### Event 11

**Trigger**

- Object event: subject 1333, op 8, value 0

**Action**

- Set/add variable: variable group 16, variable 800, subtype 0, value 1
- Set/add variable: variable group 21, variable 29, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 2, param 1333
- Mission objective/state: param 262154, subtype 0, param 0

### Event 12

**Trigger**

- Object event: subject 1333, op 2, value 0

**Action**

- Set/add variable: variable group 16, variable 426, subtype 0, value 1
- Set/add variable: variable group 16, variable 427, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Mark/flash contact: contact/list 0, subtype 2, param 1333
- Play dialog: PLAYER.SCR, line/variant 129
- Show/update HUD contact: contact/list 0, subtype 11, param 38

### Event 13

**Trigger**

- Object event: subject Red_Pirate_Fighter_2 (object 8, id 1347), op 4, value 50

**Action**

- Object spawn/action: Red_Pirate_Fighter_2 (object 8, id 1347), subtype 7

### Event 14

**Trigger**

- Object event: subject Red_Pirate_Fighter_2 (object 9, id 1421), op 4, value 50

**Action**

- Object spawn/action: Red_Pirate_Fighter_2 (object 9, id 1421), subtype 7

### Event 15

**Trigger**

- Object event: subject Red_Pirate_Shrike (object 12, id 1417), op 4, value 30

**Action**

- Object spawn/action: Red_Pirate_Shrike (object 12, id 1417), subtype 7

### Event 16

**Trigger**

- Object event: subject Red_Pirate_Shrike (object 1, id 1343), op 4, value 30

**Action**

- Object spawn/action: Red_Pirate_Shrike (object 1, id 1343), subtype 7

### Event 17

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 12

**Action**

- Play dialog: PLAYER.SCR, line/variant 175

## Waypoints

### Waypoint 0

- Tag: `306`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1995.49, 0.00, -1971.14) | None |
| 1 | (-2239.58, 0.00, -1394.46) | None |
| 2 | (-2422.76, 0.00, -965.93) | None |
| 3 | (-2659.80, 0.00, -516.91) | None |

### Waypoint 1

- Tag: `305`
- Members: `Red_Pirate_Shrike (object 12, id 1417, starts at point 0)`, `Red_Pirate_Shrike (object 13, id 1419, starts at point 0)`, `Red_Pirate_Shrike (object 14, id 1435, starts at point 0)`, `Red_Pirate_Shrike (object 17, id 1462, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1799.40, 0.00, -1397.41) | None |
| 1 | (-2083.24, 0.00, -901.98) | None |
| 2 | (-2440.25, 0.00, -522.10) | None |

### Waypoint 2

- Tag: `304`
- Members: `Red_Pirate_Shrike (object 2, id 1334, starts at point 0)`, `Red_Pirate_Shrike (object 3, id 1335, starts at point 0)`, `Red_Pirate_Shrike (object 4, id 1336, starts at point 0)`, `Red_Pirate_Shrike (object 5, id 1337, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2572.65, 237.72, 369.68) | None |
| 1 | (-3318.91, 215.10, 198.39) | None |
| 2 | (-3528.80, 159.44, -307.53) | None |
| 3 | (-3055.90, 249.37, -590.47) | None |
| 4 | (-2497.30, 291.32, -328.57) | None |
| 5 | (-1889.12, 298.31, 60.06) | on arrival redirect to Waypoint 2 (tag 304), point 0 |

### Waypoint 3

- Tag: `302`
- Members: `Red_Pirate_Fighter_2 (object 6, id 1344, starts at point 0)`, `Red_Pirate_Fighter_2 (object 7, id 1345, starts at point 0)`, `Red_Pirate_Fighter_2 (object 8, id 1347, starts at point 0)`, `Red_Pirate_Fighter_2 (object 16, id 1461, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2457.89, 104.00, -1980.72) | None |
| 1 | (-2643.04, 104.00, -1491.93) | None |
| 2 | (-2747.79, 104.00, -1048.31) | None |
| 3 | (-2854.54, 104.00, -553.48) | None |

### Waypoint 4

- Tag: `301`
- Members: `Red_Pirate_Shrike (object 0, id 1342, starts at point 0)`, `Red_Pirate_Shrike (object 1, id 1343, starts at point 0)`, `Red_Pirate_Shrike (object 15, id 1436, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1374.87, 104.00, -1574.06) | None |
| 1 | (-1647.67, 104.00, -1135.45) | None |
| 2 | (-1971.05, 104.00, -690.60) | None |
| 3 | (-2287.85, 104.00, -361.48) | None |

## Spawn Lists

### Spawn List 0

- ID: `152`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 6 | id 1333 | None |

### Spawn List 1

- ID: `168`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 2

- ID: `242`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | id 1333 | None |

### Spawn List 3

- ID: `193`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | id 1333 | None |

### Spawn List 4

- ID: `65`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Red_Pirate_Shrike` | 1342 | Interactive | -1163.69,102.00,-1774.66 | 404,0,0 | label: BFNF_01; group/role: FG_PLAGUE / 0; waypoint: Waypoint 4 (tag 301, 4 point(s)), starting point 0, arrival event value 19726336 |
| 1 | `Red_Pirate_Shrike` | 1343 | Interactive | -1197.38,102.00,-1896.42 | 404,0,0 | group/role: FG_PLAGUE / 0; waypoint: Waypoint 4 (tag 301, 4 point(s)), starting point 0, arrival event value 19726336 |
| 2 | `Red_Pirate_Shrike` | 1334 | Interactive | -2261.53,224.74,465.83 | 385,0,0 | label: BFNF_01; group/role: FG_ENVY / 0; waypoint: Waypoint 2 (tag 304, 6 point(s)), starting point 0, arrival event value 19922944 |
| 3 | `Red_Pirate_Shrike` | 1335 | Interactive | -2182.92,224.74,380.60 | 385,0,0 | group/role: FG_ENVY / 0; waypoint: Waypoint 2 (tag 304, 6 point(s)), starting point 0, arrival event value 19922944 |
| 4 | `Red_Pirate_Shrike` | 1336 | Interactive | -2138.00,224.74,465.83 | 385,0,0 | group/role: FG_ENVY / 0; waypoint: Waypoint 2 (tag 304, 6 point(s)), starting point 0, arrival event value 19922944 |
| 5 | `Red_Pirate_Shrike` | 1337 | Interactive | -2059.39,224.74,380.59 | 385,0,0 | label: BFNF_01; group/role: FG_ENVY / 0; waypoint: Waypoint 2 (tag 304, 6 point(s)), starting point 0, arrival event value 19922944 |
| 6 | `Red_Pirate_Fighter_2` | 1344 | Interactive | -2367.70,102.00,-2229.31 | 459,0,0 | label: BFNF_01; group/role: FG_GLUTTONY / 0; waypoint: Waypoint 3 (tag 302, 4 point(s)), starting point 0, arrival event value 19791872 |
| 7 | `Red_Pirate_Fighter_2` | 1345 | Interactive | -2244.16,102.00,-2241.49 | 459,0,0 | label: BFNF_01; group/role: FG_GLUTTONY / 0; waypoint: Waypoint 3 (tag 302, 4 point(s)), starting point 0, arrival event value 19791872 |
| 8 | `Red_Pirate_Fighter_2` | 1347 | Interactive | -2300.31,102.00,-2338.90 | 459,0,0 | group/role: FG_GLUTTONY / 0; waypoint: Waypoint 3 (tag 302, 4 point(s)), starting point 0, arrival event value 19791872 |
| 9 | `Red_Pirate_Fighter_2` | 1421 | Interactive | -2001.76,0.00,-2263.10 | 492,0,0 | label: BFNF_01; group/role: FG_CONTEMPT / 0 |
| 10 | `Red_Pirate_Fighter_2` | 1422 | Interactive | -1938.28,0.00,-2232.50 | 492,0,0 | group/role: FG_CONTEMPT / 0 |
| 11 | `Red_Pirate_Fighter_2` | 1424 | Interactive | -1938.28,0.00,-2301.33 | 492,0,0 | group/role: FG_CONTEMPT / 0 |
| 12 | `Red_Pirate_Shrike` | 1417 | Interactive | -1759.18,0.00,-1612.21 | 427,0,0 | label: BFNF_01; group/role: FG_DISDAIN / 0; waypoint: Waypoint 1 (tag 305, 3 point(s)), starting point 0, arrival event value 19988480 |
| 13 | `Red_Pirate_Shrike` | 1419 | Interactive | -1674.54,0.00,-1642.81 | 427,0,0 | group/role: FG_DISDAIN / 0; waypoint: Waypoint 1 (tag 305, 3 point(s)), starting point 0, arrival event value 19988480 |
| 14 | `Red_Pirate_Shrike` | 1435 | Interactive | -1712.68,0.00,-1667.83 | 432,0,0 | group/role: FG_DISDAIN / 0; waypoint: Waypoint 1 (tag 305, 3 point(s)), starting point 0, arrival event value 19988480 |
| 15 | `Red_Pirate_Shrike` | 1436 | Interactive | -1170.06,0.00,-1844.55 | 405,0,0 | group/role: FG_PLAGUE / 0; waypoint: Waypoint 4 (tag 301, 4 point(s)), starting point 0, arrival event value 19726336 |
| 16 | `Red_Pirate_Fighter_2` | 1461 | Interactive | -2197.30,0.00,-2351.05 | 447,0,0 | group/role: FG_GLUTTONY / 0; waypoint: Waypoint 3 (tag 302, 4 point(s)), starting point 0, arrival event value 19791872 |
| 17 | `Red_Pirate_Shrike` | 1462 | Interactive | -1649.55,0.00,-1709.29 | 420,0,0 | group/role: FG_DISDAIN / 0; waypoint: Waypoint 1 (tag 305, 3 point(s)), starting point 0, arrival event value 19988480 |
| 18 | `Crate_5_Special_Placehold` | 1466 | Interactive | -2631.36,148.00,-106.90 | 0,0,0 | None |
