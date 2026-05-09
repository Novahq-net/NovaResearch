# Tachyon: The Fringe GALS03A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `GALS03A.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `(none)` |
| Region | 2 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 11 |
| Entities | 49 |
| Events | 24 |
| Waypoints | 11 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Science_Vessel`, `1: Medical_Frigate`, `2: GalSpan_Sing_Platform_Piece`, `3: Bora_Carrier`, `4: Bora_Dagger`, `5: Bora_Battleaxe`, `6: Drone_Worker`, `7: GalSpan_Shuttle_Medium`, `8: Bora_Cutlass`, `9: Bora_Warhammer`, `10: GalSpan_Archangel` |
| Scripts | `PLAYER.SCR`, `PROME.SCR` |
| Scenes | None |
| Labels | `BFGF_01`, `BFGE_01`, `explode` |
| Aliases | None |
| Groups | `FG_AGENOR`, `FG_ANTLIA`, `FG_ARA`, `FG_CERYON`, `FG_REBELLION`, `FG_BALLISTA`, `FG_INSURRECTION`, `FG_UNIT_DELTA`, `FG_UNIT_GAMMA`, `FG_UNIT_THETA`, `FG_PUNISHMENT`, `FG_JACKHAMMER`, `FG_GOLDRUSH`, `VINDICATOR`, `HEPH_MODULE` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 1, subtype 0, value 0
- Gate state/action: param 4, subtype 3, param 0
- Show/update HUD contact: contact/list 0, subtype 9, param 14
- Object spawn/action: Science_Vessel (object 47, id 394), subtype 3
- Group/spawn-list action: spawn list/group 255, subtype 1, param 348

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 10

**Action**

- Play dialog: PLAYER.SCR, line/variant 3
- Set runtime trigger variable: variable group 20, variable 1, subtype 1, value 0

### Event 2

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 3

**Action**

- Set runtime trigger variable: variable group 20, variable 1, subtype 0, value 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 20

**Action**

- Play dialog: PROME.SCR, line/variant 1
- Set runtime trigger variable: variable group 20, variable 1, subtype 1, value 0

### Event 4

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 1

**Action**

- Set runtime trigger variable: variable group 20, variable 1, subtype 0, value 0

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 30

**Action**

- Play dialog: PROME.SCR, line/variant 3
- Set runtime trigger variable: variable group 20, variable 1, subtype 1, value 0

### Event 6

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 3

**Action**

- Broadcast HUD contact action: contact/list 0, subtype 0, param 12
- Set/add variable: variable group 21, variable 22, subtype 0, value 1
- Gate state/action: param 4, subtype 2, param 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 14
- Mission objective/state: param 131073, subtype 0, param 0

### Event 7

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Object spawn/action: Bora_Carrier (object 43, id 221), subtype 3
- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0
- Object spawn/action: Medical_Frigate (object 45, id 392), subtype 4
- Object spawn/action: Science_Vessel (object 47, id 394), subtype 4

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 10

**Action**

- Group/spawn-list action: spawn list/group 101, subtype 1, param 221
- Group/spawn-list action: spawn list/group 102, subtype 1, param 221
- Group/spawn-list action: spawn list/group 125, subtype 1, param 221
- Group/spawn-list action: spawn list/group 95, subtype 2
- Group/spawn-list action: spawn list/group 96, subtype 2
- Group/spawn-list action: spawn list/group 97, subtype 2

### Event 9

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 20

**Action**

- Group/spawn-list action: spawn list/group 104, subtype 1, param 221
- Group/spawn-list action: spawn list/group 100, subtype 1, param 221
- Group/spawn-list action: spawn list/group 103, subtype 1, param 221
- Group/spawn-list action: spawn list/group 98, subtype 2

### Event 10

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Object spawn/action: Bora_Carrier (object 43, id 221), subtype 4
- Show/update HUD contact: contact/list 0, subtype 1, param 100
- Show/update HUD contact: contact/list 0, subtype 1, param 104

### Event 11

**Trigger**

- Object event: subject GalSpan_Sing_Platform_Piece (object 44, id 364), op 2, value 0

**Action**

- Set/add variable: variable group 14, variable 400, subtype 0, value 1
- Set/add variable: variable group 14, variable 401, subtype 0, value 1
- Broadcast mark/flash contact: contact/list 0, subtype 0, param 15
- Set/add variable: variable group 21, variable 30, subtype 0, value 1
- Play dialog: PROME.SCR, line/variant 8
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 21

### Event 12

**Trigger**

- Group/spawn-list event: subject 100, op 0, value 0
- Group/spawn-list event: subject 125, op 0, value 0
- Group/spawn-list event: subject 103, op 0, value 0
- Group/spawn-list event: subject 101, op 0, value 0
- Group/spawn-list event: subject 102, op 0, value 0
- Group/spawn-list event: subject 104, op 0, value 0 (join 1)
- Variable comparison: subject variable group 21, variable 30, op 1, value 1

**Action**

- Set/add variable: variable group 14, variable 401, subtype 0, value 2
- Set/add variable: variable group 14, variable 400, subtype 0, value 1
- Play dialog: PROME.SCR, line/variant 9
- Broadcast hide/remove contact: contact/list 0, subtype 0, param 15
- Show/update HUD contact: contact/list 0, subtype 12, param 20

### Event 13

**Trigger**

- Group/spawn-list event: subject 100, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 100

### Event 14

**Trigger**

- Group/spawn-list event: subject 104, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 104

### Event 15

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 9

**Action**

- Play dialog: PROME.SCR, line/variant 10

### Event 16

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 10

**Action**

- Play dialog: PROME.SCR, line/variant 15

### Event 17

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 15

**Action**

- Play scene: unknown index 0, param 0
- Object spawn/action: GalSpan_Sing_Platform_Piece (object 44, id 364), subtype 4
- Set runtime trigger variable: variable group 20, variable 31, subtype 0, value 0

### Event 18

**Trigger**

- Variable comparison: subject variable group 20, variable 31, op 1, value 10

**Action**

- Object spawn/action: GalSpan_Sing_Platform_Piece (object 48, id 472), subtype 3
- Set runtime trigger variable: variable group 20, variable 31, subtype 1, value 0
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 19

**Trigger**

- Object event: subject GalSpan_Sing_Platform_Piece (object 48, id 472), op 9, value 0

**Action**

- Object spawn/action: GalSpan_Sing_Platform_Piece (object 48, id 472), subtype 7
- Object spawn/action: GalSpan_Sing_Platform_Piece (object 48, id 472), subtype 21, param 10

### Event 20

**Trigger**

- Object event: subject GalSpan_Sing_Platform_Piece (object 44, id 364), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 104
- Hide/remove HUD contact: contact/list 0, subtype 1, param 100

### Event 21

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Object spawn/action: Drone_Worker (object 25, id 403), subtype 7
- Object spawn/action: Drone_Worker (object 27, id 405), subtype 7
- Object spawn/action: Drone_Worker (object 22, id 400), subtype 7
- Object spawn/action: Drone_Worker (object 29, id 444), subtype 7
- Object spawn/action: Drone_Worker (object 26, id 404), subtype 7
- Object spawn/action: Drone_Worker (object 28, id 406), subtype 7

### Event 22

**Trigger**

- Object event: subject GalSpan_Sing_Platform_Piece (object 48, id 472), op 2, value 0

**Action**

- Play dialog: PROME.SCR, line/variant 13

### Event 23

**Trigger**

- Runtime condition family: subject 0, op 0, value 0

**Action**

- Play dialog: PROME.SCR, line/variant 14

## Waypoints

### Waypoint 0

- Tag: `112`
- Members: `Drone_Worker (object 21, id 399, starts at point 1)`, `Drone_Worker (object 22, id 400, starts at point 0)`, `Drone_Worker (object 23, id 401, starts at point 1)`, `Drone_Worker (object 24, id 402, starts at point 1)`, `Drone_Worker (object 25, id 403, starts at point 0)`, `Drone_Worker (object 26, id 404, starts at point 3)`, `Drone_Worker (object 27, id 405, starts at point 0)`, `Drone_Worker (object 28, id 406, starts at point 3)`, `Drone_Worker (object 29, id 444, starts at point 3)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-249.17, 0.00, 3994.71) | None |
| 1 | (707.49, 0.00, 4066.16) | None |
| 2 | (1621.64, 0.00, 4006.62) | None |
| 3 | (2025.57, 0.00, 3184.90) | None |
| 4 | (1536.61, 0.00, 2768.09) | None |
| 5 | (622.45, 0.00, 3280.18) | on arrival redirect to Waypoint 0 (tag 112), point 0 |

### Waypoint 1

- Tag: `111`
- Members: `Science_Vessel (object 46, id 393, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2222.16, 0.00, 3666.87) | None |
| 1 | (1936.16, 0.00, 2489.18) | None |
| 2 | (1614.34, 0.00, 1617.76) | None |
| 3 | (754.56, 0.00, 857.49) | on arrival action 1, param -1 |

### Waypoint 2

- Tag: `110`
- Members: `GalSpan_Shuttle_Medium (object 19, id 397, starts at point 0)`, `GalSpan_Shuttle_Medium (object 20, id 398, starts at point 3)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (391.15, 0.00, 565.20) | None |
| 1 | (-901.23, 0.00, 914.37) | None |
| 2 | (-1164.80, 0.00, 1954.67) | None |
| 3 | (-691.99, -130.91, 2623.31) | None |
| 4 | (177.96, 0.00, 3044.10) | None |
| 5 | (781.75, 134.78, 2455.08) | None |
| 6 | (1064.16, 0.00, 1798.09) | None |

### Waypoint 3

- Tag: `109`
- Members: `GalSpan_Shuttle_Medium (object 17, id 395, starts at point 4)`, `GalSpan_Shuttle_Medium (object 18, id 396, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-527.62, 0.00, 3479.95) | None |
| 1 | (229.16, 0.00, 4327.80) | None |
| 2 | (361.92, 0.00, 5131.03) | None |
| 3 | (-660.39, 0.00, 5428.52) | None |
| 4 | (-2001.33, 0.00, 5131.03) | None |
| 5 | (-2877.60, 0.00, 4223.68) | None |
| 6 | (-2598.79, 0.00, 2959.34) | None |
| 7 | (-1616.31, 0.00, 2840.35) | on arrival redirect to Waypoint 3 (tag 109), point 0 |

### Waypoint 4

- Tag: `107`
- Members: `Medical_Frigate (object 45, id 392, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1407.00, 0.00, 2574.71) | None |
| 1 | (-532.28, 0.00, 2689.99) | None |
| 2 | (138.04, 0.00, 2186.03) | None |
| 3 | (1246.30, 101.98, 2274.85) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 5

- Tag: `106`
- Members: `Bora_Cutlass (object 34, id 126, starts at point 0)`, `Bora_Cutlass (object 35, id 127, starts at point 0)`, `Bora_Cutlass (object 36, id 125, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (53.62, 0.00, 2144.88) | None |
| 1 | (588.39, 0.00, 2633.68) | None |
| 2 | (1294.93, 0.00, 2618.15) | None |
| 3 | (1585.86, 0.00, 2928.58) | None |

### Waypoint 6

- Tag: `105`
- Members: `Bora_Battleaxe (object 37, id 122, starts at point 0)`, `Bora_Dagger (object 38, id 124, starts at point 0)`, `Bora_Dagger (object 39, id 123, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1711.34, 0.00, 2447.42) | None |
| 1 | (-1295.72, 0.00, 3037.22) | None |
| 2 | (-796.99, 0.00, 3161.39) | None |
| 3 | (-21.18, 0.00, 3239.00) | None |
| 4 | (505.27, 0.00, 3378.69) | None |

### Waypoint 7

- Tag: `104`
- Members: `Bora_Warhammer (object 11, id 343, starts at point 0)`, `Bora_Warhammer (object 12, id 344, starts at point 0)`, `Bora_Warhammer (object 13, id 345, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (164.45, 0.00, 1741.65) | None |
| 1 | (616.10, 0.00, 2245.65) | None |
| 2 | (1322.64, 0.00, 2850.97) | None |
| 3 | (1846.72, 0.00, 2981.67) | None |
| 4 | (1786.73, 0.00, 3647.69) | None |
| 5 | (1503.13, 0.00, 3947.09) | None |
| 6 | (897.75, 0.00, 3739.34) | None |
| 7 | (821.40, 0.00, 2877.80) | on arrival redirect to Waypoint 7 (tag 104), point 1 |

### Waypoint 8

- Tag: `103`
- Members: `Bora_Warhammer (object 8, id 340, starts at point 0)`, `Bora_Warhammer (object 9, id 341, starts at point 0)`, `Bora_Warhammer (object 10, id 342, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1004.79, 0.00, 2525.03) | None |
| 1 | (-409.08, 0.00, 3394.21) | None |
| 2 | (186.63, 0.00, 3921.93) | None |
| 3 | (1253.37, 0.00, 3875.36) | None |
| 4 | (1874.43, 0.00, 3668.56) | None |
| 5 | (1808.98, 0.00, 3118.64) | None |
| 6 | (969.09, 0.00, 3002.54) | None |
| 7 | (554.60, 0.00, 3509.69) | on arrival redirect to Waypoint 8 (tag 103), point 2 |

### Waypoint 9

- Tag: `102`
- Members: `Bora_Cutlass (object 14, id 116, starts at point 0)`, `Bora_Cutlass (object 15, id 118, starts at point 0)`, `Bora_Cutlass (object 16, id 117, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-76.59, 0.00, 2447.42) | None |
| 1 | (671.51, 0.00, 3145.87) | None |

### Waypoint 10

- Tag: `101`
- Members: `Bora_Battleaxe (object 40, id 121, starts at point 0)`, `Bora_Dagger (object 41, id 120, starts at point 0)`, `Bora_Dagger (object 42, id 119, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (228.19, 0.00, 1298.86) | None |
| 1 | (920.88, 0.00, 1733.45) | None |
| 2 | (1696.69, 0.00, 2323.25) | None |
| 3 | (1696.69, 0.00, 2804.41) | None |

## Spawn Lists

### Spawn List 0

- ID: `104`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | GalSpan_Sing_Platform_Piece (object 44, id 364) | None |

### Spawn List 1

- ID: `100`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | GalSpan_Sing_Platform_Piece (object 44, id 364) | None |

### Spawn List 2

- ID: `98`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 1 | spawn list 101 | None |

### Spawn List 3

- ID: `97`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 1 | Bora_Cutlass (object 36, id 125) | None |

### Spawn List 4

- ID: `96`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 1 | id 103 | None |

### Spawn List 5

- ID: `95`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 1 | spawn list 102 | None |

### Spawn List 6

- ID: `101`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 7

- ID: `102`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 8

- ID: `125`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `GalSpan_Archangel` | 166 | Interactive | 1108.94,79.00,3238.78 | 0,0,0 | label: BFGF_01; group/role: FG_AGENOR / 0 |
| 1 | `GalSpan_Archangel` | 167 | Interactive | 1110.14,79.00,3514.67 | 0,0,0 | group/role: FG_ANTLIA / 0 |
| 2 | `GalSpan_Archangel` | 168 | Interactive | 1044.31,79.00,3236.13 | 0,0,0 | group/role: FG_AGENOR / 0 |
| 3 | `GalSpan_Archangel` | 169 | Interactive | 1040.84,79.00,3507.00 | 0,0,0 | group/role: FG_ANTLIA / 0 |
| 4 | `GalSpan_Archangel` | 170 | Interactive | 1660.50,81.31,3214.49 | 0,0,0 | label: BFGF_01; group/role: FG_ARA / 0 |
| 5 | `GalSpan_Archangel` | 171 | Interactive | 1662.39,81.31,3507.94 | 0,0,0 | group/role: FG_CERYON / 0 |
| 6 | `GalSpan_Archangel` | 172 | Interactive | 1591.37,81.31,3216.85 | 0,0,0 | group/role: FG_ARA / 0 |
| 7 | `GalSpan_Archangel` | 173 | Interactive | 1581.80,81.31,3505.29 | 0,0,0 | label: BFGF_01; group/role: FG_CERYON / 0 |
| 8 | `Bora_Warhammer` | 340 | Interactive | -1103.18,0.00,2310.87 | 0,0,0 | group/role: FG_REBELLION / 0; waypoint: Waypoint 8 (tag 103, 8 point(s)), starting point 0, arrival event value 6750208 |
| 9 | `Bora_Warhammer` | 341 | Interactive | -965.82,0.00,2248.67 | 0,0,0 | label: BFGE_01; group/role: FG_REBELLION / 0; waypoint: Waypoint 8 (tag 103, 8 point(s)), starting point 0, arrival event value 6750208 |
| 10 | `Bora_Warhammer` | 342 | Interactive | -1120.35,0.00,2165.74 | 0,0,0 | group/role: FG_REBELLION / 0; waypoint: Waypoint 8 (tag 103, 8 point(s)), starting point 0, arrival event value 6750208 |
| 11 | `Bora_Warhammer` | 343 | Interactive | -153.80,0.00,1603.19 | 122,0,0 | group/role: FG_BALLISTA / 0; waypoint: Waypoint 7 (tag 104, 8 point(s)), starting point 0, arrival event value 6815744 |
| 12 | `Bora_Warhammer` | 344 | Interactive | -89.28,0.00,1486.32 | 122,0,0 | group/role: FG_BALLISTA / 0; waypoint: Waypoint 7 (tag 104, 8 point(s)), starting point 0, arrival event value 6815744 |
| 13 | `Bora_Warhammer` | 345 | Interactive | -182.48,0.00,1356.46 | 122,0,0 | label: BFGE_01; group/role: FG_BALLISTA / 0; waypoint: Waypoint 7 (tag 104, 8 point(s)), starting point 0, arrival event value 6815744 |
| 14 | `Bora_Cutlass` | 116 | Interactive | -125.36,0.00,2216.39 | 28,0,0 | group/role: FG_INSURRECTION / 0; waypoint: Waypoint 9 (tag 102, 2 point(s)), starting point 0, arrival event value 6684672 |
| 15 | `Bora_Cutlass` | 118 | Interactive | -254.46,0.00,2176.08 | 28,0,0 | label: BFGE_01; group/role: FG_INSURRECTION / 0; waypoint: Waypoint 9 (tag 102, 2 point(s)), starting point 0, arrival event value 6684672 |
| 16 | `Bora_Cutlass` | 117 | Interactive | -265.14,0.00,2321.89 | 28,0,0 | group/role: FG_INSURRECTION / 0; waypoint: Waypoint 9 (tag 102, 2 point(s)), starting point 0, arrival event value 6684672 |
| 17 | `GalSpan_Shuttle_Medium` | 395 | Interactive | -1712.96,0.00,5145.83 | 373,0,0 | waypoint: Waypoint 3 (tag 109, 8 point(s)), starting point 4, arrival event value 7143428 |
| 18 | `GalSpan_Shuttle_Medium` | 396 | Interactive | -624.27,0.00,3360.88 | 0,0,0 | waypoint: Waypoint 3 (tag 109, 8 point(s)), starting point -1 |
| 19 | `GalSpan_Shuttle_Medium` | 397 | Interactive | 734.29,0.00,482.18 | 405,0,0 | waypoint: Waypoint 2 (tag 110, 7 point(s)), starting point 0, arrival event value 7208960 |
| 20 | `GalSpan_Shuttle_Medium` | 398 | Interactive | -753.82,0.00,2254.12 | 0,0,0 | waypoint: Waypoint 2 (tag 110, 7 point(s)), starting point 3, arrival event value 7208963 |
| 21 | `Drone_Worker` | 399 | Interactive | 645.85,0.00,4209.66 | 220,0,0 | group/role: FG_UNIT_DELTA / 0; waypoint: Waypoint 0 (tag 112, 6 point(s)), starting point 1, arrival event value 7340033 |
| 22 | `Drone_Worker` | 400 | Interactive | -386.98,0.00,4119.65 | 181,0,0 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 0 (tag 112, 6 point(s)), starting point 0, arrival event value 7340032 |
| 23 | `Drone_Worker` | 401 | Interactive | 703.97,0.00,4215.65 | 220,0,0 | group/role: FG_UNIT_DELTA / 0; waypoint: Waypoint 0 (tag 112, 6 point(s)), starting point 1, arrival event value 7340033 |
| 24 | `Drone_Worker` | 402 | Interactive | 673.97,0.00,4173.15 | 220,0,0 | group/role: FG_UNIT_DELTA / 0; waypoint: Waypoint 0 (tag 112, 6 point(s)), starting point 1, arrival event value 7340033 |
| 25 | `Drone_Worker` | 403 | Interactive | -320.60,0.00,4119.65 | 181,0,0 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 0 (tag 112, 6 point(s)), starting point 0, arrival event value 7340032 |
| 26 | `Drone_Worker` | 404 | Interactive | 2045.83,0.00,3371.25 | 266,0,0 | group/role: FG_UNIT_THETA / 0; waypoint: Waypoint 0 (tag 112, 6 point(s)), starting point 3, arrival event value 7340035 |
| 27 | `Drone_Worker` | 405 | Interactive | -356.52,0.00,4080.76 | 181,0,0 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 0 (tag 112, 6 point(s)), starting point 0, arrival event value 7340032 |
| 28 | `Drone_Worker` | 406 | Interactive | 2028.20,0.00,3325.00 | 266,0,0 | group/role: FG_UNIT_THETA / 0; waypoint: Waypoint 0 (tag 112, 6 point(s)), starting point 3, arrival event value 7340035 |
| 29 | `Drone_Worker` | 444 | Interactive | 2070.29,0.00,3331.53 | 266,0,0 | group/role: FG_UNIT_THETA / 0; waypoint: Waypoint 0 (tag 112, 6 point(s)), starting point 3, arrival event value 7340035 |
| 30 | `GalSpan_Archangel` | 485 | Interactive | 1077.73,78.00,3516.08 | 0,0,0 | label: BFGF_01; group/role: FG_ANTLIA / 0 |
| 31 | `GalSpan_Archangel` | 486 | Interactive | 1626.50,78.00,3508.45 | 0,0,0 | group/role: FG_CERYON / 0 |
| 32 | `GalSpan_Archangel` | 494 | Interactive | 1076.48,77.00,3245.59 | 0,0,0 | group/role: FG_AGENOR / 0 |
| 33 | `GalSpan_Archangel` | 495 | Interactive | 1628.39,77.00,3222.16 | 0,0,0 | group/role: FG_ARA / 0 |
| 34 | `Bora_Cutlass` | 126 | Interactive | -264.00,-305.00,1930.03 | 117,0,0 | group/role: FG_PUNISHMENT / 0; waypoint: Waypoint 5 (tag 106, 4 point(s)), starting point 0, arrival event value 6946816 |
| 35 | `Bora_Cutlass` | 127 | Interactive | -274.98,-305.00,1742.46 | 132,0,0 | group/role: FG_PUNISHMENT / 0; waypoint: Waypoint 5 (tag 106, 4 point(s)), starting point 0, arrival event value 6946816 |
| 36 | `Bora_Cutlass` | 125 | Interactive | -100.60,-305.00,1830.63 | 117,0,0 | label: BFGE_01; group/role: FG_PUNISHMENT / 0; waypoint: Waypoint 5 (tag 106, 4 point(s)), starting point 0, arrival event value 6946816 |
| 37 | `Bora_Battleaxe` | 122 | Interactive | -1758.37,0.00,2048.54 | 508,0,0 | label: BFGE_01; group/role: FG_JACKHAMMER / 0; waypoint: Waypoint 6 (tag 105, 5 point(s)), starting point 0, arrival event value 6881280 |
| 38 | `Bora_Dagger` | 124 | Interactive | -1880.98,0.00,1935.05 | 508,0,0 | group/role: FG_JACKHAMMER / 0; waypoint: Waypoint 6 (tag 105, 5 point(s)), starting point 0, arrival event value 6881280 |
| 39 | `Bora_Dagger` | 123 | Interactive | -1901.61,0.00,2152.38 | 508,0,0 | group/role: FG_JACKHAMMER / 0; waypoint: Waypoint 6 (tag 105, 5 point(s)), starting point 0, arrival event value 6881280 |
| 40 | `Bora_Battleaxe` | 121 | Interactive | -64.44,0.00,1020.63 | 31,0,0 | label: BFGE_01; group/role: FG_GOLDRUSH / 0; waypoint: Waypoint 10 (tag 101, 4 point(s)), starting point 0, arrival event value 6619136 |
| 41 | `Bora_Dagger` | 120 | Interactive | -46.97,0.00,1231.63 | 31,0,0 | group/role: FG_GOLDRUSH / 0; waypoint: Waypoint 10 (tag 101, 4 point(s)), starting point 0, arrival event value 6619136 |
| 42 | `Bora_Dagger` | 119 | Interactive | 92.81,0.00,1126.13 | 31,0,0 | group/role: FG_GOLDRUSH / 0; waypoint: Waypoint 10 (tag 101, 4 point(s)), starting point 0, arrival event value 6619136 |
| 43 | `Bora_Carrier` | 221 | Interactive | -918.68,0.00,1579.76 | 127,0,0 | secondary groups: none, VINDICATOR |
| 44 | `GalSpan_Sing_Platform_Piece` | 364 | Interactive | 1358.66,0.00,3371.86 | 0,0,0 | secondary groups: none, HEPH_MODULE |
| 45 | `Medical_Frigate` | 392 | Interactive | -1962.48,0.00,2527.42 | 122,0,0 | waypoint: Waypoint 4 (tag 107, 4 point(s)), starting point -1 |
| 46 | `Science_Vessel` | 393 | Interactive | 2194.62,0.00,4026.18 | 253,0,0 | waypoint: Waypoint 1 (tag 111, 4 point(s)), starting point 0, arrival event value 7274496 |
| 47 | `Science_Vessel` | 394 | Interactive | 964.62,87.00,3396.87 | 1,0,0 | None |
| 48 | `GalSpan_Sing_Platform_Piece` | 472 | Interactive | 11384.19,0.00,39.85 | 0,0,0 | label: explode; secondary groups: none, HEPH_MODULE |
