# Tachyon: The Fringe FRON05B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON05B.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 4 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 6 |
| Entities | 84 |
| Events | 19 |
| Waypoints | 10 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Cruiser`, `1: Bora_Claymore`, `2: Bora_Cutlass`, `3: Ripstar`, `4: Void_Pirate_Fighter`, `5: Asteroid_2` |
| Scripts | `PLAYER.SCR`, `CEPHS.SCR`, `VOIDP.SCR` |
| Scenes | None |
| Labels | `BFGF_05`, `Ripstar`, `BFGE_05`, `Cephius` |
| Aliases | `Kimodo 4`, `Python 2`, `Python 1`, `Python 4`, `Kimodo 3`, `Kimodo 1`, `Kimodo 2`, `Python 3`, `Jerome13`, `Cephius` |
| Groups | `FG_GALSPAN4`, `FG_KOMODO`, `FG_PYTHON`, `FG_UNIT_GAMMA`, `FG_FAITH`, `FG_SWORD`, `FG_REBELLION`, `FG_TRIDENT`, `FG_BALLISTA`, `FG_CATAPULT`, `FG_HONOR`, `CEPHIUS` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 2, subtype 0, value 0
- Object spawn/action: id 891, subtype 14
- Show/update HUD contact: contact/list 0, subtype 9, param 42
- Play dialog: PLAYER.SCR, line/variant 74
- Set/add variable: variable group 21, variable 5, subtype 0, value 2
- Mission objective/state: param 262148, subtype 0, param 0
- Set/add variable: variable group 21, variable 12, subtype 0, value 0

### Event 1

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 74
- Variable comparison: subject variable group 21, variable 2, op 1, value 2
- Group/spawn-list event: subject 228, op 3, value 0

**Action**

- Play dialog: CEPHS.SCR, line/variant 6

### Event 2

**Trigger**

- Variable comparison: subject variable group 21, variable 2, op 1, value 2

**Action**

- Object spawn/action: GalSpan_Cruiser (object 83, id 1016), subtype 3

### Event 3

**Trigger**

- Variable comparison: subject variable group 21, variable 31, op 1, value 1

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Show/update HUD contact: contact/list 0, subtype 9, param 42

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 5

**Action**

- Set/add variable: variable group 21, variable 2, subtype 0, value 2
- Object spawn/action: id 819, subtype 8, param 1
- Play dialog: CEPHS.SCR, line/variant 6

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 250 (extra 1, 891; flags 2)

**Action**

- Play scene: unknown index 0, param 1
- Set runtime trigger variable: variable group 20, variable 12, subtype 0, value 0
- Set runtime trigger variable: variable group 20, variable 11, subtype 0, value 0
- Set runtime trigger variable: variable group 20, variable 10, subtype 0, value 0

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 10, op 1, value 16

**Action**

- Set/add variable: variable group 21, variable 23, subtype 0, value 1
- Play dialog: PLAYER.SCR, line/variant 77
- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Show/update HUD contact: contact/list 0, subtype 2, param 1016
- Object spawn/action: GalSpan_Cruiser (object 83, id 1016), subtype 14

### Event 7

**Trigger**

- Variable comparison: subject variable group 20, variable 11, op 1, value 30
- Variable comparison: subject variable group 21, variable 23, op 0, value 1

**Action**

- Object spawn/action: id 891, subtype 7
- Set/add variable: variable group 21, variable 32, subtype 0, value 1

### Event 8

**Trigger**

- Runtime condition family: subject 0, op 0, value 0

**Action**

- Group/spawn-list action: spawn list/group 262, subtype 7
- Group/spawn-list action: spawn list/group 28, subtype 7

### Event 9

**Trigger**

- Variable comparison: subject variable group 21, variable 32, op 0, value 1

**Action**

- Group/spawn-list action: spawn list/group 255, subtype 0

### Event 10

**Trigger**

- Variable comparison: subject variable group 20, variable 12, op 1, value 60

**Action**

- Object spawn/action: id 819, subtype 6
- Set runtime trigger variable: variable group 20, variable 12, subtype 1, value 0

### Event 11

**Trigger**

- Variable comparison: subject variable group 20, variable 12, op 1, value 5

**Action**

- Play dialog: PLAYER.SCR, line/variant 76
- Hide/remove HUD contact: contact/list 0, subtype 10, param 0

### Event 12

**Trigger**

- Group/spawn-list event: subject 255, op 2, value 10551297 (Waypoint 2 (tag 161), point 1)
- Object arrival: GalSpan_Cruiser (object 83, id 1016) reached Waypoint 8 (tag 3), point 2 (raw value 196610)
- Variable comparison: subject variable group 21, variable 12, op 1, value 0

**Action**

- Set/add variable: variable group 21, variable 25, subtype 0, value 1
- Set runtime trigger variable: variable group 20, variable 10, subtype 1, value 0
- Set runtime trigger variable: variable group 20, variable 11, subtype 1, value 0

### Event 13

**Trigger**

- Variable comparison: subject variable group 21, variable 25, op 1, value 1
- Variable comparison: subject variable group 21, variable 12, op 1, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Object spawn/action: GalSpan_Cruiser (object 83, id 1016), subtype 13, param 196611
- Object spawn/action: GalSpan_Cruiser (object 83, id 1016), subtype 5
- Play dialog: CEPHS.SCR, line/variant 9
- Show/update HUD contact: contact/list 0, subtype 2, param 1016
- Group/spawn-list action: spawn list/group 229, subtype 3, param 1
- Group/spawn-list action: spawn list/group 228, subtype 3, param 1

### Event 14

**Trigger**

- Object event: subject GalSpan_Cruiser (object 83, id 1016), op 8, value 0

**Action**

- Set/add variable: variable group 21, variable 21, subtype 0, value 2
- Set/add variable: variable group 21, variable 2, subtype 0, value 3

### Event 15

**Trigger**

- Object event: subject GalSpan_Cruiser (object 83, id 1016), op 2, value 0 (join 2)
- Object event: subject GalSpan_Cruiser (object 83, id 1016), op 6, value 0 (join 2)

**Action**

- Set/add variable: variable group 16, variable 409, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 38
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Mission objective/state: param 262144, subtype 0, param 0
- Set/add variable: variable group 21, variable 12, subtype 0, value 1

### Event 16

**Trigger**

- Object event: subject GalSpan_Cruiser (object 83, id 1016), op 8, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Set/add variable: variable group 21, variable 2, subtype 0, value 3
- Show/update HUD contact: contact/list 0, subtype 12, param 37
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 16, variable 409, subtype 0, value 2
- Set/add variable: variable group 16, variable 408, subtype 0, value 1

### Event 17

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 9

**Action**

- Play dialog: CEPHS.SCR, line/variant 10

### Event 18

**Trigger**

- Group/spawn-list event: subject 262, op 1, value 30
- Object event: subject Void_Pirate_Fighter (object 2, id 432), op 15, value 0

**Action**

- Play dialog: VOIDP.SCR, line/variant 3

## Waypoints

### Waypoint 0

- Tag: `171`
- Members: `Bora_Cutlass (object 63, id 979, starts at point -1)`, `Bora_Cutlass (object 64, id 980, starts at point -1)`, `Bora_Cutlass (object 65, id 981, starts at point -1)`, `Bora_Cutlass (object 66, id 1030, starts at point -1)`, `Bora_Cutlass (object 67, id 1031, starts at point -1)`, `Bora_Cutlass (object 68, id 1032, starts at point -1)`, `Bora_Claymore (object 74, id 975, starts at point -1)`, `Bora_Claymore (object 75, id 976, starts at point -1)`, `Bora_Claymore (object 76, id 977, starts at point -1)`, `Bora_Claymore (object 78, id 1025, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-513.77, 229.09, -103.06) | None |
| 1 | (-3811.26, 229.09, 617.68) | on arrival action 4, param -1 |

### Waypoint 1

- Tag: `170`
- Members: `Bora_Claymore (object 69, id 1010, starts at point -1)`, `Bora_Claymore (object 70, id 1008, starts at point -1)`, `Bora_Claymore (object 71, id 971, starts at point -1)`, `Bora_Claymore (object 72, id 972, starts at point -1)`, `Bora_Claymore (object 73, id 974, starts at point -1)`, `Bora_Claymore (object 77, id 1023, starts at point -1)`, `Bora_Claymore (object 79, id 1037, starts at point -1)`, `Bora_Claymore (object 80, id 1038, starts at point -1)`, `Bora_Claymore (object 81, id 1043, starts at point -1)`, `Bora_Claymore (object 82, id 1044, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2597.03, 0.00, 3159.85) | None |
| 1 | (-3535.78, 0.00, 3170.37) | None |
| 2 | (-3726.94, 0.00, 179.46) | None |
| 3 | (2275.72, 0.00, -567.02) | None |
| 4 | (2268.38, 0.00, 3434.41) | on arrival redirect to Waypoint 1 (tag 170), point 0 |

### Waypoint 2

- Tag: `161`
- Members: `Ripstar (object 10, id 892, starts at point -1)`, `Ripstar (object 11, id 893, starts at point -1)`, `Ripstar (object 12, id 894, starts at point -1)`, `Ripstar (object 13, id 895, starts at point -1)`, `Ripstar (object 14, id 896, starts at point -1)`, `Ripstar (object 15, id 897, starts at point -1)`, `Ripstar (object 16, id 898, starts at point -1)`, `Ripstar (object 17, id 899, starts at point -1)`, `Ripstar (object 18, id 900, starts at point -1)`, `Ripstar (object 19, id 901, starts at point -1)`, `Ripstar (object 20, id 902, starts at point -1)`, `Ripstar (object 21, id 903, starts at point -1)`, `Ripstar (object 22, id 904, starts at point -1)`, `Ripstar (object 23, id 905, starts at point -1)`, `Ripstar (object 24, id 906, starts at point -1)`, `Ripstar (object 25, id 907, starts at point -1)`, `Ripstar (object 26, id 908, starts at point -1)`, `Ripstar (object 27, id 909, starts at point -1)`, `Ripstar (object 28, id 910, starts at point -1)`, `Ripstar (object 29, id 911, starts at point -1)`, `Ripstar (object 30, id 912, starts at point -1)`, `Ripstar (object 31, id 913, starts at point -1)`, `Ripstar (object 32, id 914, starts at point -1)`, `Ripstar (object 33, id 915, starts at point -1)`, `Ripstar (object 34, id 916, starts at point -1)`, `Ripstar (object 35, id 917, starts at point -1)`, `Ripstar (object 36, id 918, starts at point -1)`, `Ripstar (object 37, id 919, starts at point -1)`, `Ripstar (object 38, id 920, starts at point -1)`, `Ripstar (object 39, id 921, starts at point -1)`, `Ripstar (object 40, id 922, starts at point -1)`, `Ripstar (object 41, id 923, starts at point -1)`, `Ripstar (object 42, id 924, starts at point -1)`, `Ripstar (object 43, id 925, starts at point -1)`, `Ripstar (object 44, id 926, starts at point -1)`, `Ripstar (object 45, id 927, starts at point -1)`, `Ripstar (object 46, id 928, starts at point -1)`, `Ripstar (object 47, id 929, starts at point -1)`, `Ripstar (object 48, id 930, starts at point -1)`, `Ripstar (object 49, id 931, starts at point -1)`, `Ripstar (object 50, id 932, starts at point -1)`, `Ripstar (object 51, id 933, starts at point -1)`, `Ripstar (object 52, id 934, starts at point -1)`, `Ripstar (object 53, id 935, starts at point -1)`, `Ripstar (object 54, id 936, starts at point -1)`, `Ripstar (object 55, id 937, starts at point -1)`, `Ripstar (object 56, id 938, starts at point -1)`, `Ripstar (object 57, id 939, starts at point -1)`, `Ripstar (object 58, id 940, starts at point -1)`, `Ripstar (object 59, id 941, starts at point -1)`, `Ripstar (object 60, id 942, starts at point -1)`, `Ripstar (object 61, id 943, starts at point -1)`, `Ripstar (object 62, id 944, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2381.30, 870.94, 1276.12) | None |
| 1 | (-3461.55, 1703.35, 1445.07) | on arrival action 4, param -1 |

### Waypoint 3

- Tag: `1`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1484.33, 1959.69, 5268.18) | None |
| 1 | (-2125.03, 1959.69, 5264.18) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 4

- Tag: `160`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-3066.59, 0.00, -1749.93) | on arrival play dialog/script or enter gate, param 1 |
| 1 | (-2525.44, 0.00, -1089.22) | None |
| 2 | (-1701.28, 0.00, -673.93) | None |
| 3 | (-1698.15, 0.00, 70.65) | None |

### Waypoint 5

- Tag: `159`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2677.44, -456.29, 2015.42) | None |
| 1 | (-3267.48, -456.29, 1422.18) | None |
| 2 | (-3266.14, -456.29, 788.04) | None |
| 3 | (201.38, -456.29, 154.54) | None |
| 4 | (482.63, -456.29, 2432.64) | None |
| 5 | (-98.90, -456.29, 2692.27) | on arrival redirect to Waypoint 5 (tag 159), point 0 |

### Waypoint 6

- Tag: `5`
- Members: `Void_Pirate_Fighter (object 2, id 432, starts at point -1)`, `Void_Pirate_Fighter (object 3, id 433, starts at point -1)`, `Void_Pirate_Fighter (object 4, id 434, starts at point -1)`, `Void_Pirate_Fighter (object 5, id 435, starts at point -1)`, `Void_Pirate_Fighter (object 6, id 436, starts at point -1)`, `Void_Pirate_Fighter (object 7, id 437, starts at point -1)`, `Void_Pirate_Fighter (object 8, id 438, starts at point -1)`, `Void_Pirate_Fighter (object 9, id 439, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-3232.35, 794.40, -1571.29) | None |
| 1 | (-2744.23, 362.90, -413.60) | None |
| 2 | (-1361.83, 362.90, -219.81) | None |

### Waypoint 7

- Tag: `4`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-4558.79, 1214.13, -2206.01) | None |
| 1 | (-2520.37, 1214.13, -637.93) | None |
| 2 | (-2508.12, 1223.35, 2411.48) | on arrival activate current object (raw param -1 ignored) |
| 3 | (-4432.42, 1223.35, 2413.08) | None |
| 4 | (-5056.92, 1223.35, 1818.68) | None |

### Waypoint 8

- Tag: `3`
- Members: `GalSpan_Cruiser (object 83, id 1016, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-4770.65, 1685.00, -1651.08) | None |
| 1 | (-3510.18, 1685.00, -717.74) | None |
| 2 | (-3509.58, 1685.01, 1060.50) | on arrival activate current object (raw param -1 ignored); listened by Event 12 for GalSpan_Cruiser (object 83, id 1016) |
| 3 | (-4141.82, 1685.67, 1058.17) | None |
| 4 | (-4937.12, 1682.16, 325.63) | on arrival action 1, param -1 |

### Waypoint 9

- Tag: `2`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-5344.75, 1459.50, -1453.17) | None |
| 1 | (-3995.49, 1453.25, -421.82) | None |
| 2 | (-4000.79, 1454.22, 3031.27) | on arrival activate current object (raw param -1 ignored) |
| 3 | (-5962.71, 1447.65, 3036.75) | None |
| 4 | (-6823.58, 1450.13, 2324.69) | None |

## Spawn Lists

### Spawn List 0

- ID: `28`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | GalSpan_Cruiser (object 83, id 1016) | None |

### Spawn List 1

- ID: `228`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 2

- ID: `229`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 3

- ID: `106`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | GalSpan_Cruiser (object 83, id 1016) | None |
| 1 | 9 | none | None |

### Spawn List 4

- ID: `104`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | GalSpan_Cruiser (object 83, id 1016) | None |
| 1 | 9 | none | None |

### Spawn List 5

- ID: `262`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 6

- ID: `100`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 9 | none | None |

### Spawn List 7

- ID: `57`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 4 | GalSpan_Cruiser (object 83, id 1016) | None |
| 1 | 9 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Asteroid_2` | 110 | Object | -4176.22,163.69,3096.24 | 494,431,85 | Scale/Radius: 4.00 |
| 1 | `Asteroid_2` | 253 | Object | -5297.17,817.93,1346.39 | 397,131,104 | Scale/Radius: 1.00 |
| 2 | `Void_Pirate_Fighter` | 432 | Interactive | -3189.31,0.00,-2833.80 | 319,1,1 | label: BFGF_05; group/role: FG_KOMODO / 0; alias: Kimodo 4; waypoint: Waypoint 6 (tag 5, 3 point(s)), starting point -1 |
| 3 | `Void_Pirate_Fighter` | 433 | Interactive | -3036.74,0.00,-2879.95 | 319,1,1 | group/role: FG_PYTHON / 0; alias: Python 2; waypoint: Waypoint 6 (tag 5, 3 point(s)), starting point -1 |
| 4 | `Void_Pirate_Fighter` | 434 | Interactive | -3061.14,0.00,-2878.70 | 319,1,1 | label: BFGF_05; group/role: FG_PYTHON / 0; alias: Python 1; waypoint: Waypoint 6 (tag 5, 3 point(s)), starting point -1 |
| 5 | `Void_Pirate_Fighter` | 435 | Interactive | -3028.61,0.00,-2847.72 | 319,1,1 | group/role: FG_PYTHON / 0; alias: Python 4; waypoint: Waypoint 6 (tag 5, 3 point(s)), starting point -1 |
| 6 | `Void_Pirate_Fighter` | 436 | Interactive | -3231.72,0.00,-2850.96 | 319,1,1 | group/role: FG_KOMODO / 0; alias: Kimodo 3; waypoint: Waypoint 6 (tag 5, 3 point(s)), starting point -1 |
| 7 | `Void_Pirate_Fighter` | 437 | Interactive | -3210.22,0.00,-2874.67 | 319,1,1 | group/role: FG_KOMODO / 0; alias: Kimodo 1; waypoint: Waypoint 6 (tag 5, 3 point(s)), starting point -1 |
| 8 | `Void_Pirate_Fighter` | 438 | Interactive | -3189.31,0.00,-2879.08 | 319,1,1 | label: BFGF_05; group/role: FG_KOMODO / 0; alias: Kimodo 2; waypoint: Waypoint 6 (tag 5, 3 point(s)), starting point -1 |
| 9 | `Void_Pirate_Fighter` | 439 | Interactive | -3066.38,0.00,-2855.31 | 319,1,1 | label: BFGF_05; group/role: FG_PYTHON / 0; alias: Python 3; waypoint: Waypoint 6 (tag 5, 3 point(s)), starting point -1 |
| 10 | `Ripstar` | 892 | Interactive | -2360.74,851.40,1267.43 | 0,0,70 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 11 | `Ripstar` | 893 | Interactive | -2349.32,842.11,1275.60 | 0,0,496 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 12 | `Ripstar` | 894 | Interactive | -2362.00,851.63,1283.53 | 0,0,70 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 13 | `Ripstar` | 895 | Interactive | -2356.34,848.67,1282.54 | 0,0,492 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 14 | `Ripstar` | 896 | Interactive | -2365.78,857.14,1278.58 | 0,0,217 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 15 | `Ripstar` | 897 | Interactive | -2372.96,862.69,1276.59 | 0,0,79 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 16 | `Ripstar` | 898 | Interactive | -2365.78,857.14,1271.63 | 0,0,217 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 17 | `Ripstar` | 899 | Interactive | -2368.20,858.26,1265.68 | 0,0,0 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 18 | `Ripstar` | 900 | Interactive | -2374.13,863.87,1266.68 | 0,0,167 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 19 | `Ripstar` | 901 | Interactive | -2374.13,863.87,1271.63 | 0,0,167 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 20 | `Ripstar` | 902 | Interactive | -2370.34,861.44,1280.56 | 0,0,0 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 21 | `Ripstar` | 903 | Interactive | -2371.01,860.05,1287.50 | 0,0,100 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 22 | `Ripstar` | 904 | Interactive | -2350.52,843.52,1274.11 | 0,0,148 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 23 | `Ripstar` | 905 | Interactive | -2350.98,843.52,1266.68 | 0,0,148 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 24 | `Ripstar` | 906 | Interactive | -2350.98,843.52,1262.71 | 0,0,148 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 25 | `Ripstar` | 907 | Interactive | -2368.20,858.26,1262.71 | 0,0,0 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 26 | `Ripstar` | 908 | Interactive | -2367.66,856.18,1262.71 | 0,0,36 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 27 | `Ripstar` | 909 | Interactive | -2361.42,852.05,1265.68 | 0,0,70 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 28 | `Ripstar` | 910 | Interactive | -2363.72,853.15,1272.63 | 0,0,135 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 29 | `Ripstar` | 911 | Interactive | -2366.13,855.35,1281.55 | 0,0,437 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 30 | `Ripstar` | 912 | Interactive | -2357.88,849.73,1286.51 | 0,0,70 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 31 | `Ripstar` | 913 | Interactive | -2365.78,857.14,1288.49 | 0,0,217 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 32 | `Ripstar` | 914 | Interactive | -2353.51,845.75,1292.46 | 0,0,53 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 33 | `Ripstar` | 915 | Interactive | -2355.83,848.33,1276.10 | 0,0,334 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 34 | `Ripstar` | 916 | Interactive | -2371.54,860.97,1271.14 | 0,0,363 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 35 | `Ripstar` | 917 | Interactive | -2352.49,844.72,1266.68 | 0,0,334 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 36 | `Ripstar` | 918 | Interactive | -2353.95,846.20,1275.60 | 0,0,148 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 37 | `Ripstar` | 919 | Interactive | -2368.20,858.26,1282.54 | 0,0,0 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 38 | `Ripstar` | 920 | Interactive | -2370.55,860.05,1281.55 | 0,0,100 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 39 | `Ripstar` | 921 | Interactive | -2350.52,843.52,1274.11 | 0,0,148 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 40 | `Ripstar` | 922 | Interactive | -2370.55,860.05,1271.14 | 0,0,100 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 41 | `Ripstar` | 923 | Interactive | -2355.83,848.33,1272.13 | 0,0,334 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 42 | `Ripstar` | 924 | Interactive | -2355.83,848.33,1286.51 | 0,0,334 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 43 | `Ripstar` | 925 | Interactive | -2353.49,846.20,1286.51 | 0,0,148 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 44 | `Ripstar` | 926 | Interactive | -2353.95,846.20,1283.53 | 0,0,148 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 45 | `Ripstar` | 927 | Interactive | -2365.57,854.84,1266.68 | 0,0,28 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 46 | `Ripstar` | 928 | Interactive | -2359.39,850.51,1272.13 | 0,0,36 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 47 | `Ripstar` | 929 | Interactive | -2348.80,841.55,1277.09 | 0,0,496 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 48 | `Ripstar` | 930 | Interactive | -2350.98,843.52,1288.49 | 0,0,148 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 49 | `Ripstar` | 931 | Interactive | -2367.87,857.44,1279.57 | 0,0,404 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 50 | `Ripstar` | 932 | Interactive | -2370.34,861.44,1277.09 | 0,0,0 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 51 | `Ripstar` | 933 | Interactive | -2371.01,860.05,1274.11 | 0,0,100 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 52 | `Ripstar` | 934 | Interactive | -2370.55,860.05,1268.66 | 0,0,100 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 53 | `Ripstar` | 935 | Interactive | -2350.98,843.52,1266.68 | 0,0,148 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 54 | `Ripstar` | 936 | Interactive | -2352.49,844.72,1269.65 | 0,0,334 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 55 | `Ripstar` | 937 | Interactive | -2366.13,855.35,1280.06 | 0,0,437 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 56 | `Ripstar` | 938 | Interactive | -2364.94,854.15,1279.07 | 0,0,238 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 57 | `Ripstar` | 939 | Interactive | -2372.96,862.69,1288.99 | 0,0,79 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 58 | `Ripstar` | 940 | Interactive | -2372.96,862.69,1277.58 | 0,0,79 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 59 | `Ripstar` | 941 | Interactive | -2370.55,860.05,1275.60 | 0,0,100 | label: Ripstar; group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 60 | `Ripstar` | 942 | Interactive | -2369.22,858.76,1271.63 | 0,0,433 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 61 | `Ripstar` | 943 | Interactive | -2360.63,851.40,1271.63 | 0,0,404 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 62 | `Ripstar` | 944 | Interactive | -2360.63,851.40,1272.63 | 0,0,404 | group/role: FG_UNIT_GAMMA / 0; waypoint: Waypoint 2 (tag 161, 2 point(s)), starting point -1 |
| 63 | `Bora_Cutlass` | 979 | Interactive | 239.90,-70.91,290.76 | 0,0,0 | group/role: FG_FAITH / 0; waypoint: Waypoint 0 (tag 171, 2 point(s)), starting point -1 |
| 64 | `Bora_Cutlass` | 980 | Interactive | 255.52,-70.91,290.68 | 0,0,0 | label: BFGE_05; group/role: FG_FAITH / 0; waypoint: Waypoint 0 (tag 171, 2 point(s)), starting point -1 |
| 65 | `Bora_Cutlass` | 981 | Interactive | 271.91,-70.91,290.43 | 0,0,0 | group/role: FG_FAITH / 0; waypoint: Waypoint 0 (tag 171, 2 point(s)), starting point -1 |
| 66 | `Bora_Cutlass` | 1030 | Interactive | 303.34,-70.91,-757.49 | 0,0,0 | group/role: FG_SWORD / 0; waypoint: Waypoint 0 (tag 171, 2 point(s)), starting point -1 |
| 67 | `Bora_Cutlass` | 1031 | Interactive | 288.71,-70.91,-757.49 | 0,0,0 | label: BFGE_05; group/role: FG_SWORD / 0; waypoint: Waypoint 0 (tag 171, 2 point(s)), starting point -1 |
| 68 | `Bora_Cutlass` | 1032 | Interactive | 274.07,-70.91,-757.49 | 0,0,0 | group/role: FG_SWORD / 0; waypoint: Waypoint 0 (tag 171, 2 point(s)), starting point -1 |
| 69 | `Bora_Claymore` | 1010 | Interactive | -1442.30,0.00,3259.83 | 0,0,0 | label: BFGE_05; group/role: FG_REBELLION / 0; waypoint: Waypoint 1 (tag 170, 5 point(s)), starting point -1 |
| 70 | `Bora_Claymore` | 1008 | Interactive | -1404.80,0.00,3300.50 | 0,0,0 | group/role: FG_REBELLION / 0; waypoint: Waypoint 1 (tag 170, 5 point(s)), starting point -1 |
| 71 | `Bora_Claymore` | 971 | Interactive | -1766.82,0.00,3210.37 | 0,0,0 | group/role: FG_TRIDENT / 0; waypoint: Waypoint 1 (tag 170, 5 point(s)), starting point -1 |
| 72 | `Bora_Claymore` | 972 | Interactive | -2064.98,0.00,3122.07 | 0,0,0 | group/role: FG_BALLISTA / 0; waypoint: Waypoint 1 (tag 170, 5 point(s)), starting point -1 |
| 73 | `Bora_Claymore` | 974 | Interactive | -2027.33,0.00,3076.53 | 0,0,0 | label: BFGE_05; group/role: FG_BALLISTA / 0; waypoint: Waypoint 1 (tag 170, 5 point(s)), starting point -1 |
| 74 | `Bora_Claymore` | 975 | Interactive | 291.94,-70.91,350.23 | 0,0,0 | group/role: FG_CATAPULT / 0; waypoint: Waypoint 0 (tag 171, 2 point(s)), starting point -1 |
| 75 | `Bora_Claymore` | 976 | Interactive | 316.94,-70.91,349.99 | 0,0,0 | label: BFGE_05; group/role: FG_CATAPULT / 0; waypoint: Waypoint 0 (tag 171, 2 point(s)), starting point -1 |
| 76 | `Bora_Claymore` | 977 | Interactive | 291.57,-70.91,391.52 | 0,0,0 | group/role: FG_CATAPULT / 0; waypoint: Waypoint 0 (tag 171, 2 point(s)), starting point -1 |
| 77 | `Bora_Claymore` | 1023 | Interactive | -1726.97,0.00,3181.50 | 0,0,0 | group/role: FG_TRIDENT / 0; waypoint: Waypoint 1 (tag 170, 5 point(s)), starting point -1 |
| 78 | `Bora_Claymore` | 1025 | Interactive | 316.43,-70.91,391.53 | 0,0,0 | group/role: FG_CATAPULT / 0; waypoint: Waypoint 0 (tag 171, 2 point(s)), starting point -1 |
| 79 | `Bora_Claymore` | 1037 | Interactive | -2201.87,0.00,3083.35 | 0,0,0 | group/role: FG_HONOR / 0; waypoint: Waypoint 1 (tag 170, 5 point(s)), starting point -1 |
| 80 | `Bora_Claymore` | 1038 | Interactive | -2237.72,0.00,3038.00 | 0,0,0 | label: BFGE_05; group/role: FG_HONOR / 0; waypoint: Waypoint 1 (tag 170, 5 point(s)), starting point -1 |
| 81 | `Bora_Claymore` | 1043 | Interactive | -2326.15,0.00,3121.58 | 0,0,0 | group/role: FG_HONOR / 0; waypoint: Waypoint 1 (tag 170, 5 point(s)), starting point -1 |
| 82 | `Bora_Claymore` | 1044 | Interactive | -2291.09,0.00,3075.96 | 0,0,0 | label: BFGE_05; group/role: FG_HONOR / 0; waypoint: Waypoint 1 (tag 170, 5 point(s)), starting point -1 |
| 83 | `GalSpan_Cruiser` | 1016 | Interactive | -5550.88,1647.60,-2555.32 | 64,0,0 | label: Cephius; alias: Cephius; secondary groups: none, CEPHIUS; waypoint: Waypoint 8 (tag 3, 5 point(s)), starting point -1 |
