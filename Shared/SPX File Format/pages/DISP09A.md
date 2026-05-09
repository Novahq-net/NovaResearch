# Tachyon: The Fringe DISP09A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP09A.SPX` |
| Sector | `QUAD_09` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 8 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 10 |
| Entities | 56 |
| Events | 23 |
| Waypoints | 6 |
| Child Sectors | 0 |
| Scripts | 7 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Sing_Pltfrm_Piece_Husk`, `1: Deliverance_BC10_Only`, `2: Zeus_GalSpan_Carrier`, `3: GalSpan_Singularity_Platform`, `4: Bora_Battleaxe`, `5: GalSpan_Orion`, `6: Bora_Shuttle_Medium`, `7: TNS_Inquirer`, `8: Bora_Claymore`, `9: Susan_Bradley_Waraxe` |
| Scripts | `HEPHA.SCR`, `G10BPA.SCR`, `DELIV.SCR`, `SUSAN.SCR`, `ATKIN.SCR`, `TNSB.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `anna`, `BFBF_07`, `news`, `JAKE`, `BFBE_07`, `zeus` |
| Aliases | `BC10_Waraxe`, `BC10_Claymore1`, `BC10_Claymore2`, `BC10_Claymore3`, `BC10_Claymore4`, `BC10_Mace4`, `BC10_Mace3`, `BC10_Mace2`, `BC10_Mace1`, `BC10_Warhammer1`, `BC10_Warhammer2`, `BC10_Warhammer3`, `BC10_Warhammer4`, `Stocks01` |
| Groups | `FG_LANCE`, `FG_SWORD`, `TNS_INQUIRER`, `FG_MUSCA`, `FG_ARIADNE`, `FG_PLUTUS`, `FG_CALLISTO`, `FG_NEPHELE`, `FG_MORNING_STAR`, `FG_TRIDENT`, `FG_LEPUS`, `FG_CRUX`, `FG_CRONUS`, `HEPH_MODULE`, `CONT_021`, `ZEUS`, `DELIVERANCE`, `CONT_024` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 2, op 1, value 2

**Action**

- Object spawn/action: Deliverance_BC10_Only (object 54, id 132), subtype 3
- Play dialog: HEPHA.SCR, line/variant 0
- Object spawn/action: Deliverance_BC10_Only (object 54, id 132), subtype 18
- Show/update HUD contact: contact/list 0, subtype 2, param 132
- Object spawn/action: Deliverance_BC10_Only (object 54, id 132), subtype 14

### Event 1

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 0

**Action**

- Play dialog: G10BPA.SCR, line/variant 4

### Event 2

**Trigger**

- Object arrival: Deliverance_BC10_Only (object 54, id 132) reached Waypoint 5 (tag 101), point 1 (raw value 6619137)

**Action**

- Play dialog: DELIV.SCR, line/variant 5

### Event 3

**Trigger**

- Sector/startup condition family: subject 2, op 0, value 5

**Action**

- Object spawn/action: Deliverance_BC10_Only (object 54, id 132), subtype 17

### Event 4

**Trigger**

- Object event: subject GalSpan_Singularity_Platform (object 50, id 1), op 4, value 40
- Sector/startup condition family: subject 2, op 0, value 5

**Action**

- Play dialog: HEPHA.SCR, line/variant 1

### Event 5

**Trigger**

- Object event: subject GalSpan_Singularity_Platform (object 50, id 1), op 4, value 100 (join 2)
- Object event: subject Deliverance_BC10_Only (object 54, id 132), op 14, value 56

**Action**

- Object spawn/action: Deliverance_BC10_Only (object 54, id 132), subtype 5
- Play dialog: HEPHA.SCR, line/variant 2
- Show/update HUD contact: contact/list 0, subtype 0, param 1
- Hide/remove HUD contact: contact/list 0, subtype 2, param 132
- Object spawn/action: Deliverance_BC10_Only (object 54, id 132), subtype 18
- Set/add variable: variable group 21, variable 3, subtype 0, value 2
- Object spawn/action: Deliverance_BC10_Only (object 54, id 132), subtype 15
- Object spawn/action: GalSpan_Singularity_Platform (object 50, id 1), subtype 14

### Event 6

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 2

**Action**

- Set runtime trigger variable: variable group 20, variable 17, subtype 0, value 0

### Event 7

**Trigger**

- Variable comparison: subject variable group 20, variable 17, op 1, value 15

**Action**

- Play dialog: DELIV.SCR, line/variant 7

### Event 8

**Trigger**

- Object arrival: Deliverance_BC10_Only (object 54, id 132) reached Waypoint 5 (tag 101), point 3 (raw value 6619139)

**Action**

- Object spawn/action: Zeus_GalSpan_Carrier (object 51, id 29), subtype 3
- Play dialog: SUSAN.SCR, line/variant 18
- Object spawn/action: Zeus_GalSpan_Carrier (object 51, id 29), subtype 18
- Set/add variable: variable group 21, variable 11, subtype 0, value 1

### Event 9

**Trigger**

- Sector/startup condition family: subject 3, op 0, value 18

**Action**

- Object spawn/action: Zeus_GalSpan_Carrier (object 51, id 29), subtype 17

### Event 10

**Trigger**

- Object event: subject Deliverance_BC10_Only (object 54, id 132), op 0, value 0 (extra 1, 29; flags 2)

**Action**

- Object spawn/action: Deliverance_BC10_Only (object 54, id 132), subtype 21, param 8
- Play dialog: DELIV.SCR, line/variant 9

### Event 11

**Trigger**

- Sector/startup condition family: subject 2, op 0, value 9

**Action**

- Play dialog: ATKIN.SCR, line/variant 1

### Event 12

**Trigger**

- Sector/startup condition family: subject 4, op 0, value 1

**Action**

- Object spawn/action: TNS_Inquirer (object 5, id 60), subtype 1, param 2
- Play dialog: TNSB.SCR, line/variant 0

### Event 13

**Trigger**

- Object event: subject GalSpan_Singularity_Platform (object 50, id 1), op 3, value 50
- Sector/startup condition family: subject 5, op 0, value 0

**Action**

- Play dialog: SUSAN.SCR, line/variant 22
- Group/spawn-list action: spawn list/group 176, subtype 0

### Event 14

**Trigger**

- Object event: subject GalSpan_Singularity_Platform (object 50, id 1), op 3, value 70
- Sector/startup condition family: subject 3, op 0, value 22

**Action**

- Play dialog: ATKIN.SCR, line/variant 3
- Group/spawn-list action: spawn list/group 226, subtype 0

### Event 15

**Trigger**

- Sector/startup condition family: subject 4, op 0, value 3

**Action**

- Play dialog: TNSB.SCR, line/variant 1
- Group/spawn-list action: spawn list/group 222, subtype 0

### Event 16

**Trigger**

- Object event: subject GalSpan_Singularity_Platform (object 50, id 1), op 3, value 90
- Sector/startup condition family: subject 5, op 0, value 1

**Action**

- Play dialog: SUSAN.SCR, line/variant 23

### Event 17

**Trigger**

- Object event: subject GalSpan_Singularity_Platform (object 50, id 1), op 2, value 0

**Action**

- Play scene: unknown index 0, param 0
- Object spawn/action: GalSpan_Singularity_Platform (object 50, id 1), subtype 21, param 25
- Play dialog: PLAYER.SCR, line/variant 34
- Object spawn/action: Zeus_GalSpan_Carrier (object 51, id 29), subtype 18
- Show/update HUD contact: contact/list 0, subtype 12, param 24
- Set/add variable: variable group 21, variable 16, subtype 0, value 1
- Set/add variable: variable group 21, variable 34, subtype 0, value 1
- Object spawn/action: Zeus_GalSpan_Carrier (object 51, id 29), subtype 8, param 4

### Event 18

**Trigger**

- Variable comparison: subject variable group 21, variable 16, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 230, subtype 4, param 4
- Group/spawn-list action: spawn list/group 224, subtype 4, param 4
- Group/spawn-list action: spawn list/group 275, subtype 4, param 4
- Group/spawn-list action: spawn list/group 276, subtype 4, param 4
- Group/spawn-list action: spawn list/group 158, subtype 4, param 4
- Group/spawn-list action: spawn list/group 222, subtype 4, param 4
- Group/spawn-list action: spawn list/group 226, subtype 4, param 4
- Group/spawn-list action: spawn list/group 176, subtype 4, param 4

### Event 19

**Trigger**

- Object event: subject GalSpan_Singularity_Platform (object 50, id 1), op 16, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 35
- Group/spawn-list action: spawn list/group 230, subtype 5, param 29
- Group/spawn-list action: spawn list/group 224, subtype 5, param 29
- Group/spawn-list action: spawn list/group 275, subtype 5, param 29
- Group/spawn-list action: spawn list/group 276, subtype 5, param 29
- Group/spawn-list action: spawn list/group 158, subtype 5, param 29
- Group/spawn-list action: spawn list/group 222, subtype 5, param 29
- Group/spawn-list action: spawn list/group 226, subtype 5, param 29

### Event 20

**Trigger**

- Variable comparison: subject variable group 21, variable 34, op 1, value 1
- Runtime condition family: subject 0, op 0, value 0

**Action**

- Play scene: unknown index 0, param 1
- Play dialog: TNSB.SCR, line/variant 3
- Set/add variable: variable group 18, variable 404, subtype 0, value 1
- Set/add variable: variable group 18, variable 405, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 21

**Trigger**

- Object event: subject Deliverance_BC10_Only (object 54, id 132), op 2, value 0
- Variable comparison: subject variable group 21, variable 3, op 3, value 2

**Action**

- Set/add variable: variable group 18, variable 404, subtype 0, value 0
- Set/add variable: variable group 18, variable 405, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Mark/flash contact: contact/list 0, subtype 2, param 132
- Show/update HUD contact: contact/list 0, subtype 11, param 25

### Event 22

**Trigger**

- Object event: subject GalSpan_Singularity_Platform (object 50, id 1), op 16, value 0

**Action**

- Object spawn/action: GalSpan_Sing_Pltfrm_Piece_Husk (object 55, id 133), subtype 0

## Waypoints

### Waypoint 0

- Tag: `106`
- Members: `GalSpan_Orion (object 44, id 142, starts at point 0)`, `GalSpan_Orion (object 45, id 143, starts at point 0)`, `GalSpan_Orion (object 46, id 146, starts at point 0)`, `GalSpan_Orion (object 47, id 147, starts at point 0)`, `GalSpan_Orion (object 48, id 150, starts at point 0)`, `GalSpan_Orion (object 49, id 151, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (3794.34, 0.00, 2290.53) | None |
| 1 | (3107.51, 0.00, 1753.36) | None |
| 2 | (1408.41, 0.00, 603.80) | None |

### Waypoint 1

- Tag: `105`
- Members: `GalSpan_Orion (object 14, id 3, starts at point 0)`, `GalSpan_Orion (object 15, id 4, starts at point 0)`, `GalSpan_Orion (object 16, id 15, starts at point 0)`, `GalSpan_Orion (object 17, id 16, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2278.78, 0.00, -1331.66) | None |
| 1 | (1699.25, 0.00, -1392.08) | None |
| 2 | (774.23, 0.00, -1476.67) | None |
| 3 | (-39.34, 0.00, -1452.50) | None |

### Waypoint 2

- Tag: `104`
- Members: `TNS_Inquirer (object 5, id 60, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1815.36, 0.00, -411.12) | on arrival activate current object (raw param -1 ignored) |
| 1 | (-363.45, 0.00, 1438.40) | None |
| 2 | (680.18, 0.00, 2552.26) | None |
| 3 | (1556.78, 0.00, 3137.71) | None |
| 4 | (2253.90, 0.00, 3293.51) | None |
| 5 | (2720.79, 198.00, 2935.53) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 3

- Tag: `103`
- Members: `GalSpan_Orion (object 12, id 11, starts at point 0)`, `GalSpan_Orion (object 13, id 13, starts at point 0)`, `GalSpan_Orion (object 18, id 126, starts at point 0)`, `GalSpan_Orion (object 19, id 8, starts at point 0)`, `GalSpan_Orion (object 20, id 9, starts at point 0)`, `GalSpan_Orion (object 21, id 10, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (612.47, 312.00, 1018.32) | None |
| 1 | (240.78, 251.00, 653.80) | None |
| 2 | (-101.07, 198.00, 296.73) | None |
| 3 | (-639.83, 108.00, -228.37) | None |

### Waypoint 4

- Tag: `102`
- Members: `GalSpan_Orion (object 22, id 19, starts at point 0)`, `GalSpan_Orion (object 23, id 20, starts at point 0)`, `GalSpan_Orion (object 24, id 21, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1868.67, 347.00, 1563.04) | None |
| 1 | (-1700.46, 296.00, 1109.93) | None |
| 2 | (-1492.40, 238.00, 592.79) | None |
| 3 | (-1254.78, 172.00, 121.91) | None |

### Waypoint 5

- Tag: `101`
- Members: `Deliverance_BC10_Only (object 54, id 132, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-644.53, 498.00, -1069.64) | None |
| 1 | (-43.35, 537.00, -544.72) | on arrival activate current object (raw param -1 ignored); listened by Event 2 for Deliverance_BC10_Only (object 54, id 132) |
| 2 | (997.90, 589.00, 481.47) | None |
| 3 | (2221.81, 616.00, 1681.47) | None; listened by Event 8 for Deliverance_BC10_Only (object 54, id 132) |
| 4 | (2938.47, 795.00, 2372.95) | on arrival activate current object (raw param -1 ignored) |

## Spawn Lists

### Spawn List 0

- ID: `124`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | Zeus_GalSpan_Carrier (object 51, id 29) | None |
| 1 | 0 | none | None |

### Spawn List 1

- ID: `56`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | GalSpan_Singularity_Platform (object 50, id 1) | None |

### Spawn List 2

- ID: `57`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 3

- ID: `230`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 4

- ID: `224`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Deliverance_BC10_Only (object 54, id 132) | None |

### Spawn List 5

- ID: `158`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 6

- ID: `47`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | GalSpan_Singularity_Platform (object 50, id 1) | None |

### Spawn List 7

- ID: `276`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Deliverance_BC10_Only (object 54, id 132) | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Susan_Bradley_Waraxe` | 23 | Interactive | -1734.09,0.00,-3022.96 | 61,0,0 | label: anna; group/role: FG_LANCE / 0; alias: BC10_Waraxe |
| 1 | `Bora_Claymore` | 42 | Interactive | -1986.00,0.00,-3163.47 | 80,0,0 | label: BFBF_07; group/role: FG_SWORD / 0; alias: BC10_Claymore1 |
| 2 | `Bora_Claymore` | 43 | Interactive | -1964.71,0.00,-3190.14 | 76,0,0 | group/role: FG_SWORD / 0; alias: BC10_Claymore2 |
| 3 | `Bora_Claymore` | 44 | Interactive | -1933.45,0.00,-3220.58 | 76,0,0 | group/role: FG_SWORD / 0; alias: BC10_Claymore3 |
| 4 | `Bora_Claymore` | 45 | Interactive | -1912.56,0.00,-3252.60 | 75,0,0 | group/role: FG_SWORD / 0; alias: BC10_Claymore4 |
| 5 | `TNS_Inquirer` | 60 | Interactive | -2741.20,0.00,-1194.02 | 0,0,0 | label: news; secondary groups: none, TNS_INQUIRER; waypoint: Waypoint 2 (tag 104, 6 point(s)), starting point 0, arrival event value 6815744 |
| 6 | `Bora_Shuttle_Medium` | 82 | Interactive | 3955.65,0.00,-23637.63 | 0,0,0 | label: JAKE |
| 7 | `Bora_Shuttle_Medium` | 83 | Interactive | 3882.21,85.27,-23477.30 | 0,0,0 | None |
| 8 | `Bora_Claymore` | 87 | Interactive | 3819.48,28.43,-23405.49 | 0,0,0 | None |
| 9 | `Bora_Claymore` | 88 | Interactive | 3895.42,43.19,-23586.31 | 0,0,0 | None |
| 10 | `Bora_Claymore` | 89 | Interactive | 3876.67,49.47,-23568.06 | 0,0,0 | None |
| 11 | `Bora_Claymore` | 90 | Interactive | 3873.66,4.07,-23370.86 | 0,0,0 | None |
| 12 | `GalSpan_Orion` | 11 | Interactive | 843.87,376.70,1426.56 | 316,0,0 | group/role: FG_MUSCA / 0; waypoint: Waypoint 3 (tag 103, 4 point(s)), starting point 0, arrival event value 6750208 |
| 13 | `GalSpan_Orion` | 13 | Interactive | 837.82,376.70,1339.13 | 311,0,0 | group/role: FG_MUSCA / 0; waypoint: Waypoint 3 (tag 103, 4 point(s)), starting point 0, arrival event value 6750208 |
| 14 | `GalSpan_Orion` | 3 | Interactive | 2863.18,320.00,-1093.73 | 385,0,0 | group/role: FG_ARIADNE / 0; waypoint: Waypoint 1 (tag 105, 4 point(s)), starting point 0, arrival event value 6881280 |
| 15 | `GalSpan_Orion` | 4 | Interactive | 2927.44,320.00,-1089.58 | 383,0,0 | group/role: FG_ARIADNE / 0; waypoint: Waypoint 1 (tag 105, 4 point(s)), starting point 0, arrival event value 6881280 |
| 16 | `GalSpan_Orion` | 15 | Interactive | 3031.51,384.00,-1358.42 | 375,0,0 | label: BFBE_07; group/role: FG_PLUTUS / 0; waypoint: Waypoint 1 (tag 105, 4 point(s)), starting point 0, arrival event value 6881280 |
| 17 | `GalSpan_Orion` | 16 | Interactive | 3079.38,384.00,-1380.67 | 375,0,0 | group/role: FG_PLUTUS / 0; waypoint: Waypoint 1 (tag 105, 4 point(s)), starting point 0, arrival event value 6881280 |
| 18 | `GalSpan_Orion` | 126 | Interactive | 791.72,0.00,1364.15 | 302,0,0 | group/role: FG_MUSCA / 0; waypoint: Waypoint 3 (tag 103, 4 point(s)), starting point 0, arrival event value 6750208 |
| 19 | `GalSpan_Orion` | 8 | Interactive | 830.73,384.00,1648.21 | 326,0,0 | group/role: FG_CALLISTO / 0; waypoint: Waypoint 3 (tag 103, 4 point(s)), starting point 0, arrival event value 6750208 |
| 20 | `GalSpan_Orion` | 9 | Interactive | 885.44,384.00,1611.14 | 325,0,0 | group/role: FG_CALLISTO / 0; waypoint: Waypoint 3 (tag 103, 4 point(s)), starting point 0, arrival event value 6750208 |
| 21 | `GalSpan_Orion` | 10 | Interactive | 960.67,384.00,1566.65 | 326,0,0 | label: BFBE_07; group/role: FG_CALLISTO / 0; waypoint: Waypoint 3 (tag 103, 4 point(s)), starting point 0, arrival event value 6750208 |
| 22 | `GalSpan_Orion` | 19 | Interactive | -1926.17,324.62,1986.81 | 309,0,0 | group/role: FG_NEPHELE / 0; waypoint: Waypoint 4 (tag 102, 4 point(s)), starting point 0, arrival event value 6684672 |
| 23 | `GalSpan_Orion` | 20 | Interactive | -1878.15,324.62,1955.69 | 309,0,0 | group/role: FG_NEPHELE / 0; waypoint: Waypoint 4 (tag 102, 4 point(s)), starting point 0, arrival event value 6684672 |
| 24 | `GalSpan_Orion` | 21 | Interactive | -1828.93,324.62,1926.02 | 300,0,0 | label: BFBE_07; group/role: FG_NEPHELE / 0; waypoint: Waypoint 4 (tag 102, 4 point(s)), starting point 0, arrival event value 6684672 |
| 25 | `Bora_Claymore` | 85 | Interactive | 3924.83,0.00,-23496.86 | 0,0,0 | None |
| 26 | `Bora_Claymore` | 86 | Interactive | 3866.87,85.27,-23679.81 | 0,0,0 | None |
| 27 | `Bora_Claymore` | 84 | Interactive | 3893.52,85.27,-23413.08 | 0,0,0 | None |
| 28 | `Bora_Claymore` | 78 | Interactive | 3874.56,4.07,-23627.78 | 0,0,0 | None |
| 29 | `Bora_Claymore` | 79 | Interactive | 3905.74,28.43,-23658.76 | 0,0,0 | None |
| 30 | `Bora_Claymore` | 80 | Interactive | 3819.32,28.43,-23548.75 | 0,0,0 | None |
| 31 | `Bora_Claymore` | 81 | Interactive | 3929.80,104.46,-23555.57 | 0,0,0 | None |
| 32 | `Bora_Battleaxe` | 76 | Interactive | 3866.50,28.43,-23415.91 | 0,0,0 | None |
| 33 | `Bora_Battleaxe` | 74 | Interactive | 3844.87,-29.22,-23436.92 | 0,0,0 | None |
| 34 | `Bora_Battleaxe` | 75 | Interactive | 3846.56,63.17,-23574.73 | 0,0,0 | None |
| 35 | `Bora_Battleaxe` | 77 | Interactive | 3877.75,104.46,-23705.46 | 0,0,0 | None |
| 36 | `Bora_Battleaxe` | 110 | Interactive | -1819.31,0.00,-3051.07 | 58,0,0 | label: BFBF_07; group/role: FG_MORNING_STAR / 0; alias: BC10_Mace4 |
| 37 | `Bora_Battleaxe` | 111 | Interactive | -1794.03,0.00,-3073.00 | 58,0,0 | group/role: FG_MORNING_STAR / 0; alias: BC10_Mace3 |
| 38 | `Bora_Battleaxe` | 112 | Interactive | -1770.43,0.00,-3091.28 | 58,0,0 | group/role: FG_MORNING_STAR / 0; alias: BC10_Mace2 |
| 39 | `Bora_Battleaxe` | 113 | Interactive | -1753.58,0.00,-3113.21 | 58,0,0 | group/role: FG_MORNING_STAR / 0; alias: BC10_Mace1 |
| 40 | `Bora_Battleaxe` | 38 | Interactive | -1898.70,0.00,-3111.16 | 70,0,0 | label: BFBF_07; group/role: FG_TRIDENT / 0; alias: BC10_Warhammer1 |
| 41 | `Bora_Battleaxe` | 39 | Interactive | -1877.99,0.00,-3135.62 | 69,0,0 | group/role: FG_TRIDENT / 0; alias: BC10_Warhammer2 |
| 42 | `Bora_Battleaxe` | 40 | Interactive | -1855.06,0.00,-3159.44 | 64,0,0 | group/role: FG_TRIDENT / 0; alias: BC10_Warhammer3 |
| 43 | `Bora_Battleaxe` | 41 | Interactive | -1828.07,0.00,-3182.74 | 70,0,0 | group/role: FG_TRIDENT / 0; alias: BC10_Warhammer4 |
| 44 | `GalSpan_Orion` | 142 | Interactive | 3673.50,0.00,2430.02 | 304,0,0 | group/role: FG_LEPUS / 0; waypoint: Waypoint 0 (tag 106, 3 point(s)), starting point 0, arrival event value 6946816 |
| 45 | `GalSpan_Orion` | 143 | Interactive | 3752.27,0.00,2422.90 | 304,0,0 | group/role: FG_LEPUS / 0; waypoint: Waypoint 0 (tag 106, 3 point(s)), starting point 0, arrival event value 6946816 |
| 46 | `GalSpan_Orion` | 146 | Interactive | 4200.89,0.00,2448.16 | 364,0,0 | group/role: FG_CRUX / 0; waypoint: Waypoint 0 (tag 106, 3 point(s)), starting point 0, arrival event value 6946816 |
| 47 | `GalSpan_Orion` | 147 | Interactive | 4286.23,0.00,2433.92 | 364,0,0 | group/role: FG_CRUX / 0; waypoint: Waypoint 0 (tag 106, 3 point(s)), starting point 0, arrival event value 6946816 |
| 48 | `GalSpan_Orion` | 150 | Interactive | 4048.69,0.00,2186.56 | 306,0,0 | group/role: FG_CRONUS / 0; waypoint: Waypoint 0 (tag 106, 3 point(s)), starting point 0, arrival event value 6946816 |
| 49 | `GalSpan_Orion` | 151 | Interactive | 4107.76,0.00,2150.98 | 306,0,0 | group/role: FG_CRONUS / 0; waypoint: Waypoint 0 (tag 106, 3 point(s)), starting point 0, arrival event value 6946816 |
| 50 | `GalSpan_Singularity_Platform` | 1 | Interactive | 1393.09,0.00,-314.92 | 88,0,0 | secondary groups: CONT_021, HEPH_MODULE |
| 51 | `Zeus_GalSpan_Carrier` | 29 | Interactive | 4453.26,443.00,2955.91 | 441,0,0 | label: zeus; secondary groups: none, ZEUS |
| 52 | `Bora_Shuttle_Medium` | 92 | Interactive | 3850.89,0.00,-23485.17 | 0,0,0 | None |
| 53 | `Bora_Shuttle_Medium` | 91 | Interactive | 3910.72,85.27,-23616.27 | 0,0,0 | None |
| 54 | `Deliverance_BC10_Only` | 132 | Interactive | -1083.83,504.46,-1438.09 | 73,506,0 | alias: Stocks01; secondary groups: CONT_024, DELIVERANCE; waypoint: Waypoint 5 (tag 101, 5 point(s)), starting point 0, arrival event value 6619136 |
| 55 | `GalSpan_Sing_Pltfrm_Piece_Husk` | 133 | Interactive | 1945.03,0.00,-48.93 | 85,0,0 | secondary groups: none, HEPH_MODULE |
