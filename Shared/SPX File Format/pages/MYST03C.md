# Tachyon: The Fringe MYST03C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST03C.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `(none)` |
| Region | 5 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 30 |
| Events | 15 |
| Waypoints | 9 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Science_Vessel`, `1: Cassitor_Assault_Drone` |
| Scripts | `MORLY.SCR`, `PLAYER.SCR`, `DRCAS.SCR` |
| Scenes | None |
| Labels | `BFNE_06` |
| Aliases | `Will_02` |
| Groups | `FG_STRAIN_PSI`, `FG_STRAIN_MU`, `FG_STRAIN_PI`, `FG_STRAIN_ETA`, `FG_STRAIN_LAMBDA`, `FG_STRAIN_ZETA`, `FG_STRAIN_IOTA`, `FG_STRAIN_CHI`, `FG_STRAIN_KAPPA`, `FG_STRAIN_RHO`, `FG_STRAIN_UPSILON`, `FG_STRAIN_XI`, `MORLEY`, `MICHELSON` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 2, param 93
- Show/update HUD contact: contact/list 0, subtype 2, param 105
- Set runtime trigger variable: variable group 20, variable 19, subtype 0, value 0
- Group/spawn-list action: spawn list/group 214, subtype 0
- Group/spawn-list action: spawn list/group 93, subtype 0
- Object spawn/action: Science_Vessel (object 29, id 105), subtype 14
- Object spawn/action: Science_Vessel (object 28, id 93), subtype 14
- Play dialog: MORLY.SCR, line/variant 0

### Event 1

**Trigger**

- Group/spawn-list event: subject 214, op 1, value 50 (join 2)
- Group/spawn-list event: subject 93, op 1, value 50 (join 2)

**Action**

- Group/spawn-list action: spawn list/group 89, subtype 0
- Group/spawn-list action: spawn list/group 88, subtype 0
- Group/spawn-list action: spawn list/group 92, subtype 0

### Event 2

**Trigger**

- Group/spawn-list event: subject 89, op 1, value 50 (join 2)
- Group/spawn-list event: subject 88, op 1, value 50 (join 2)

**Action**

- Group/spawn-list action: spawn list/group 211, subtype 0
- Group/spawn-list action: spawn list/group 205, subtype 0
- Group/spawn-list action: spawn list/group 207, subtype 0

### Event 3

**Trigger**

- Global enemy/object-count event: subject 0, op 0, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 61

### Event 4

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 61

**Action**

- Object spawn/action: Science_Vessel (object 29, id 105), subtype 4
- Object spawn/action: Science_Vessel (object 28, id 93), subtype 4
- Group/spawn-list action: spawn list/group 210, subtype 0
- Group/spawn-list action: spawn list/group 90, subtype 0
- Group/spawn-list action: spawn list/group 206, subtype 0
- Group/spawn-list action: spawn list/group 94, subtype 0

### Event 5

**Trigger**

- Object event: subject Science_Vessel (object 29, id 105), op 3, value 20 (join 2)
- Object event: subject Science_Vessel (object 28, id 93), op 3, value 20

**Action**

- Play dialog: MORLY.SCR, line/variant 1

### Event 6

**Trigger**

- Object event: subject Science_Vessel (object 29, id 105), op 2, value 0 (join 2)

**Action**

- Mark/flash contact: contact/list 0, subtype 2, param 105

### Event 7

**Trigger**

- Object event: subject Science_Vessel (object 28, id 93), op 2, value 0

**Action**

- Mark/flash contact: contact/list 0, subtype 2, param 93

### Event 8

**Trigger**

- Object event: subject Science_Vessel (object 29, id 105), op 8, value 0
- Object event: subject Science_Vessel (object 28, id 93), op 8, value 0

**Action**

- Set/add variable: variable group 21, variable 28, subtype 0, value 1

### Event 9

**Trigger**

- Object event: subject Science_Vessel (object 29, id 105), op 2, value 0 (join 2)
- Object event: subject Science_Vessel (object 28, id 93), op 2, value 0

**Action**

- Set/add variable: variable group 17, variable 410, subtype 0, value 1
- Set/add variable: variable group 17, variable 411, subtype 0, value 1
- Play dialog: DRCAS.SCR, line/variant 15
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 29

### Event 10

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 70

**Action**

- Play dialog: PLAYER.SCR, line/variant 125

### Event 11

**Trigger**

- Group/spawn-list event: subject 207, op 0, value 0
- Group/spawn-list event: subject 89, op 0, value 0
- Group/spawn-list event: subject 205, op 0, value 0
- Group/spawn-list event: subject 211, op 0, value 0
- Group/spawn-list event: subject 214, op 0, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 121

### Event 12

**Trigger**

- Variable comparison: subject variable group 21, variable 28, op 1, value 1
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Set/add variable: variable group 17, variable 410, subtype 0, value 1
- Set/add variable: variable group 17, variable 411, subtype 0, value 3
- Hide/remove HUD contact: contact/list 0, subtype 2, param 105
- Hide/remove HUD contact: contact/list 0, subtype 2, param 93
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 28

### Event 13

**Trigger**

- Variable comparison: subject variable group 21, variable 28, op 1, value 1
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Set/add variable: variable group 17, variable 410, subtype 0, value 1
- Set/add variable: variable group 17, variable 411, subtype 0, value 2
- Hide/remove HUD contact: contact/list 0, subtype 2, param 105
- Hide/remove HUD contact: contact/list 0, subtype 2, param 93
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 28

### Event 14

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 103

## Waypoints

### Waypoint 0

- Tag: `209`
- Members: `Cassitor_Assault_Drone (object 0, id 43, starts at point 0)`, `Cassitor_Assault_Drone (object 1, id 57, starts at point 0)`, `Cassitor_Assault_Drone (object 26, id 284, starts at point 0)`, `Cassitor_Assault_Drone (object 27, id 285, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1635.22, 0.00, -533.37) | None |
| 1 | (-1870.58, 0.00, -251.77) | on arrival redirect to Waypoint 5 (tag 203), point 0 |

### Waypoint 1

- Tag: `211`
- Members: `Cassitor_Assault_Drone (object 7, id 229, starts at point 0)`, `Cassitor_Assault_Drone (object 8, id 231, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2495.50, 0.00, -894.17) | None |
| 1 | (-2190.89, 0.00, -462.41) | on arrival redirect to Waypoint 8 (tag 205), point 0 |

### Waypoint 2

- Tag: `207`
- Members: `Cassitor_Assault_Drone (object 9, id 232, starts at point 0)`, `Cassitor_Assault_Drone (object 10, id 233, starts at point 0)`, `Cassitor_Assault_Drone (object 11, id 234, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1367.39, 0.00, -49.37) | None |
| 1 | (-1748.84, 0.00, 197.03) | on arrival redirect to Waypoint 3 (tag 206), point 0 |

### Waypoint 3

- Tag: `206`
- Members: `Cassitor_Assault_Drone (object 18, id 249, starts at point 0)`, `Cassitor_Assault_Drone (object 19, id 250, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2341.30, 0.00, 892.24) | None |
| 1 | (-2146.52, 0.00, 522.63) | on arrival redirect to Waypoint 0 (tag 209), point 0 |

### Waypoint 4

- Tag: `204`
- Members: `Cassitor_Assault_Drone (object 20, id 251, starts at point 0)`, `Cassitor_Assault_Drone (object 21, id 252, starts at point 0)`, `Cassitor_Assault_Drone (object 24, id 282, starts at point 0)`, `Cassitor_Assault_Drone (object 25, id 283, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2966.22, 0.00, 346.63) | None |
| 1 | (-2303.29, 0.00, 54.76) | on arrival redirect to Waypoint 1 (tag 211), point 0 |

### Waypoint 5

- Tag: `203`
- Members: `Cassitor_Assault_Drone (object 3, id 64, starts at point 0)`, `Cassitor_Assault_Drone (object 4, id 68, starts at point 0)`, `Cassitor_Assault_Drone (object 6, id 227, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-3128.54, 0.00, -14.17) | None |
| 1 | (-2474.05, 0.00, -48.25) | on arrival redirect to Waypoint 2 (tag 207), point 0 |

### Waypoint 6

- Tag: `212`
- Members: `Cassitor_Assault_Drone (object 2, id 62, starts at point 0)`, `Cassitor_Assault_Drone (object 5, id 172, starts at point 0)`, `Cassitor_Assault_Drone (object 22, id 280, starts at point 0)`, `Cassitor_Assault_Drone (object 23, id 281, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2998.69, 0.00, -498.17) | None |
| 1 | (-2552.31, 0.00, -295.77) | on arrival redirect to Waypoint 3 (tag 206), point 0 |

### Waypoint 7

- Tag: `210`
- Members: `Cassitor_Assault_Drone (object 12, id 236, starts at point 0)`, `Cassitor_Assault_Drone (object 13, id 237, starts at point 0)`, `Cassitor_Assault_Drone (object 14, id 238, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1976.08, 0.00, -858.97) | None |
| 1 | (-2041.01, 0.00, -322.17) | on arrival redirect to Waypoint 4 (tag 204), point 0 |

### Waypoint 8

- Tag: `205`
- Members: `Cassitor_Assault_Drone (object 15, id 242, starts at point 0)`, `Cassitor_Assault_Drone (object 16, id 243, starts at point 0)`, `Cassitor_Assault_Drone (object 17, id 244, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2803.90, 0.00, 654.64) | None |
| 1 | (-2269.02, 0.00, 200.31) | on arrival redirect to Waypoint 7 (tag 210), point 0 |

## Spawn Lists

### Spawn List 0

- ID: `93`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 9 | none | None |
| 1 | 0 | none | None |

### Spawn List 1

- ID: `214`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 9 | none | None |
| 1 | 0 | none | None |

### Spawn List 2

- ID: `92`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 3

- ID: `94`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 9 | none | None |

### Spawn List 4

- ID: `89`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Science_Vessel (object 28, id 93) | None |
| 1 | 6 | Science_Vessel (object 29, id 105) | None |

### Spawn List 5

- ID: `90`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | Science_Vessel (object 29, id 105) | None |
| 1 | 6 | Science_Vessel (object 28, id 93) | None |
| 2 | 0 | none | None |

### Spawn List 6

- ID: `88`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 7

- ID: `207`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 6 | Science_Vessel (object 29, id 105) | None |
| 2 | 6 | Science_Vessel (object 28, id 93) | None |

### Spawn List 8

- ID: `211`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 0 | none | None |

### Spawn List 9

- ID: `205`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 10

- ID: `210`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | Science_Vessel (object 29, id 105) | None |
| 1 | 6 | Science_Vessel (object 28, id 93) | None |
| 2 | 0 | none | None |

### Spawn List 11

- ID: `206`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | Science_Vessel (object 29, id 105) | None |
| 1 | 6 | Science_Vessel (object 28, id 93) | None |
| 2 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Cassitor_Assault_Drone` | 43 | Interactive | -1406.22,267.00,-706.65 | 459,0,0 | group/role: FG_STRAIN_PSI / 1; waypoint: Waypoint 0 (tag 209, 2 point(s)), starting point 0, arrival event value 13697024 |
| 1 | `Cassitor_Assault_Drone` | 57 | Interactive | -1318.20,262.00,-904.74 | 459,0,0 | group/role: FG_STRAIN_PSI / 4; waypoint: Waypoint 0 (tag 209, 2 point(s)), starting point 0, arrival event value 13697024 |
| 2 | `Cassitor_Assault_Drone` | 62 | Interactive | -3261.31,262.00,-854.98 | 100,0,0 | group/role: FG_STRAIN_MU / 3; waypoint: Waypoint 6 (tag 212, 2 point(s)), starting point 0, arrival event value 13893632 |
| 3 | `Cassitor_Assault_Drone` | 64 | Interactive | -3463.11,262.00,62.48 | 151,0,0 | group/role: FG_STRAIN_PI / 1; waypoint: Waypoint 5 (tag 203, 2 point(s)), starting point 0, arrival event value 13303808 |
| 4 | `Cassitor_Assault_Drone` | 68 | Interactive | -3417.68,262.00,-69.59 | 151,0,0 | group/role: FG_STRAIN_PI / 3; waypoint: Waypoint 5 (tag 203, 2 point(s)), starting point 0, arrival event value 13303808 |
| 5 | `Cassitor_Assault_Drone` | 172 | Interactive | -3215.45,185.00,-675.49 | 118,0,0 | group/role: FG_STRAIN_MU / 1; waypoint: Waypoint 6 (tag 212, 2 point(s)), starting point 0, arrival event value 13893632 |
| 6 | `Cassitor_Assault_Drone` | 227 | Interactive | -3312.26,225.53,3.49 | 149,0,0 | group/role: FG_STRAIN_PI / 0; waypoint: Waypoint 5 (tag 203, 2 point(s)), starting point 0, arrival event value 13303808 |
| 7 | `Cassitor_Assault_Drone` | 229 | Interactive | -2564.20,159.00,-1028.16 | 0,0,0 | group/role: FG_STRAIN_ETA / 0; waypoint: Waypoint 1 (tag 211, 2 point(s)), starting point 0, arrival event value 13828096 |
| 8 | `Cassitor_Assault_Drone` | 231 | Interactive | -2771.61,159.00,-1197.76 | 0,0,0 | group/role: FG_STRAIN_ETA / 0; waypoint: Waypoint 1 (tag 211, 2 point(s)), starting point 0, arrival event value 13828096 |
| 9 | `Cassitor_Assault_Drone` | 232 | Interactive | -1105.63,189.00,-306.90 | 435,0,0 | group/role: FG_STRAIN_LAMBDA / 0; waypoint: Waypoint 2 (tag 207, 2 point(s)), starting point 0, arrival event value 13565952 |
| 10 | `Cassitor_Assault_Drone` | 233 | Interactive | -1137.38,189.00,-181.05 | 435,0,0 | group/role: FG_STRAIN_LAMBDA / 0; waypoint: Waypoint 2 (tag 207, 2 point(s)), starting point 0, arrival event value 13565952 |
| 11 | `Cassitor_Assault_Drone` | 234 | Interactive | -998.58,189.00,-176.86 | 435,0,0 | group/role: FG_STRAIN_LAMBDA / 0; waypoint: Waypoint 2 (tag 207, 2 point(s)), starting point 0, arrival event value 13565952 |
| 12 | `Cassitor_Assault_Drone` | 236 | Interactive | -1939.56,145.00,-1053.87 | 0,0,0 | group/role: FG_STRAIN_ZETA / 0; waypoint: Waypoint 7 (tag 210, 2 point(s)), starting point 0, arrival event value 13762560 |
| 13 | `Cassitor_Assault_Drone` | 237 | Interactive | -1918.03,145.00,-1187.63 | 0,0,0 | group/role: FG_STRAIN_ZETA / 0; waypoint: Waypoint 7 (tag 210, 2 point(s)), starting point 0, arrival event value 13762560 |
| 14 | `Cassitor_Assault_Drone` | 238 | Interactive | -1800.54,225.53,-1009.13 | 0,0,0 | group/role: FG_STRAIN_ZETA / 0; waypoint: Waypoint 7 (tag 210, 2 point(s)), starting point 0, arrival event value 13762560 |
| 15 | `Cassitor_Assault_Drone` | 242 | Interactive | -2935.32,220.58,852.98 | 195,0,0 | group/role: FG_STRAIN_IOTA / 0; waypoint: Waypoint 8 (tag 205, 2 point(s)), starting point 0, arrival event value 13434880 |
| 16 | `Cassitor_Assault_Drone` | 243 | Interactive | -2869.70,220.58,861.88 | 195,0,0 | group/role: FG_STRAIN_IOTA / 0; waypoint: Waypoint 8 (tag 205, 2 point(s)), starting point 0, arrival event value 13434880 |
| 17 | `Cassitor_Assault_Drone` | 244 | Interactive | -2771.26,220.58,879.67 | 195,0,0 | group/role: FG_STRAIN_IOTA / 0; waypoint: Waypoint 8 (tag 205, 2 point(s)), starting point 0, arrival event value 13434880 |
| 18 | `Cassitor_Assault_Drone` | 249 | Interactive | -2426.73,220.58,1004.19 | 223,0,0 | group/role: FG_STRAIN_CHI / 0; waypoint: Waypoint 3 (tag 206, 2 point(s)), starting point 0, arrival event value 13500416 |
| 19 | `Cassitor_Assault_Drone` | 250 | Interactive | -2336.49,220.58,995.30 | 223,0,0 | group/role: FG_STRAIN_CHI / 0; waypoint: Waypoint 3 (tag 206, 2 point(s)), starting point 0, arrival event value 13500416 |
| 20 | `Cassitor_Assault_Drone` | 251 | Interactive | -3271.65,170.63,529.18 | 171,0,0 | group/role: FG_STRAIN_KAPPA / 0; waypoint: Waypoint 4 (tag 204, 2 point(s)), starting point 0, arrival event value 13369344 |
| 21 | `Cassitor_Assault_Drone` | 252 | Interactive | -3189.62,170.63,529.18 | 171,0,0 | group/role: FG_STRAIN_KAPPA / 0; waypoint: Waypoint 4 (tag 204, 2 point(s)), starting point 0, arrival event value 13369344 |
| 22 | `Cassitor_Assault_Drone` | 280 | Interactive | -3303.91,0.00,-326.42 | 75,0,0 | group/role: FG_STRAIN_RHO / 0; waypoint: Waypoint 6 (tag 212, 2 point(s)), starting point 0, arrival event value 13893632 |
| 23 | `Cassitor_Assault_Drone` | 281 | Interactive | -3251.27,0.00,-332.13 | 75,0,0 | group/role: FG_STRAIN_RHO / 0; waypoint: Waypoint 6 (tag 212, 2 point(s)), starting point 0, arrival event value 13893632 |
| 24 | `Cassitor_Assault_Drone` | 282 | Interactive | -3298.65,0.00,261.47 | 90,0,0 | group/role: FG_STRAIN_UPSILON / 0; waypoint: Waypoint 4 (tag 204, 2 point(s)), starting point 0, arrival event value 13369344 |
| 25 | `Cassitor_Assault_Drone` | 283 | Interactive | -3203.90,0.00,238.64 | 90,0,0 | group/role: FG_STRAIN_UPSILON / 0; waypoint: Waypoint 4 (tag 204, 2 point(s)), starting point 0, arrival event value 13369344 |
| 26 | `Cassitor_Assault_Drone` | 284 | Interactive | -1435.20,0.00,-309.30 | 439,0,0 | group/role: FG_STRAIN_XI / 0; waypoint: Waypoint 0 (tag 209, 2 point(s)), starting point 0, arrival event value 13697024 |
| 27 | `Cassitor_Assault_Drone` | 285 | Interactive | -1398.35,0.00,-315.01 | 439,0,0 | group/role: FG_STRAIN_XI / 0; waypoint: Waypoint 0 (tag 209, 2 point(s)), starting point 0, arrival event value 13697024 |
| 28 | `Science_Vessel` | 93 | Interactive | -2389.79,113.00,-410.57 | 257,0,0 | secondary groups: none, MORLEY |
| 29 | `Science_Vessel` | 105 | Interactive | -1991.04,128.00,63.97 | 257,0,0 | secondary groups: none, MICHELSON |
