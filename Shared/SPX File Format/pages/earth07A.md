# Tachyon: The Fringe earth07A.spx

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `earth07A.spx` |
| Sector | `QUAD_07` |
| Backdrop | `(none)` |
| Region | 0 |
| Sector ID | 6 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | not present in this file header |
| BWBaseSectorRace | not present in this file header |
| Object Types | 9 |
| Entities | 47 |
| Events | 16 |
| Waypoints | 16 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GALSPAN_DESTROYER`, `1: Sol_Patrol`, `2: GALSPAN_CARRIER`, `3: BORA_CRUISER`, `4: BORA_CARRIER`, `5: RIPPER`, `6: CLAW`, `7: MANTA`, `8: DART` |
| Scripts | `PLAYER.SCR`, `DILL.SCR` |
| Scenes | None |
| Labels | None |
| Aliases | `fred1`, `fred2`, `fred3` |
| Groups | None |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 9, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 43

**Action**

- Group/spawn-list action: spawn list/group 76, subtype 1, param 335 (Waypoint 0 (tag 0), point 335 (point out of range))

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 48

**Action**

- Group/spawn-list action: spawn list/group 77, subtype 1, param 335 (Waypoint 0 (tag 0), point 335 (point out of range))

### Event 3

**Trigger**

- Group/spawn-list event: subject 76, op 0, value 0 (Waypoint 0 (tag 0), point 0)
- Group/spawn-list event: subject 77, op 0, value 0 (Waypoint 0 (tag 0), point 0)

**Action**

- Set/add variable: variable group 12, variable 9, subtype 0, value 1
- Set/add variable: variable group 12, variable 10, subtype 0, value 2
- Set runtime trigger variable: variable group 20, variable 10, subtype 0, value 0

### Event 4

**Trigger**

- Object event: subject GALSPAN_CARRIER (object 34, id 527), op 2, value 0

**Action**

- Set/add variable: variable group 12, variable 9, subtype 0, value 0
- Set/add variable: variable group 12, variable 10, subtype 0, value 1
- Set runtime trigger variable: variable group 20, variable 10, subtype 0, value 0

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 10, op 1, value 55

**Action**

- Object spawn/action: BORA_CRUISER (object 33, id 417), subtype 4
- Object spawn/action: BORA_CARRIER (object 32, id 335), subtype 4

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 10, op 1, value 65

**Action**

- Object spawn/action: GALSPAN_DESTROYER (object 46, id 608), subtype 4
- Object spawn/action: GALSPAN_CARRIER (object 34, id 527), subtype 4

### Event 7

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 15

**Action**

- Object spawn/action: GALSPAN_DESTROYER (object 46, id 608), subtype 3

### Event 8

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 2, param 527

### Event 9

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 60

**Action**

- Show/update HUD contact: contact/list 0, subtype 1, param 76
- Show/update HUD contact: contact/list 0, subtype 1, param 77

### Event 10

**Trigger**

- Variable comparison: subject variable group 20, variable 10, op 1, value 100

**Action**

- Group/spawn-list action: spawn list/group 87, subtype 0
- Group/spawn-list action: spawn list/group 88, subtype 0

### Event 11

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 4

**Action**

- Play dialog: PLAYER.SCR, line/variant 55

### Event 12

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 55

**Action**

- Play dialog: DILL.SCR, line/variant 45

### Event 13

**Trigger**

- Variable comparison: subject variable group 20, variable 10, op 1, value 5

**Action**

- Play dialog: DILL.SCR, line/variant 46
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 14

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 20

**Action**

- Group/spawn-list action: spawn list/group 68, subtype 1, param 527 (Waypoint 0 (tag 0), point 527 (point out of range))

### Event 15

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 20

**Action**

- Group/spawn-list action: spawn list/group 69, subtype 1, param 527 (Waypoint 0 (tag 0), point 527 (point out of range))

## Waypoints

### Waypoint 0

- Tag: `0`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2042.64, 0.00, -24.04) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 1

- Tag: `0`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2417.39, 0.00, 18.26) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 2

- Tag: `0`
- Members: `GALSPAN_DESTROYER (object 46, id 608, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2013.47, 0.00, -1729.96) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 3

- Tag: `0`
- Members: `CLAW (object 43, id 565, starts at point 0)`, `CLAW (object 44, id 566, starts at point 0)`, `CLAW (object 45, id 567, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (247.70, 0.00, -2082.14) | None |
| 1 | (-12.27, 0.00, -477.96) | None |
| 2 | (1177.31, 0.00, -290.63) | on arrival redirect to waypoint tag 19, point 1 |

### Waypoint 4

- Tag: `0`
- Members: `Sol_Patrol (object 35, id 555, starts at point 0)`, `Sol_Patrol (object 36, id 556, starts at point 0)`, `Sol_Patrol (object 37, id 557, starts at point 0)`, `Sol_Patrol (object 38, id 558, starts at point 0)`, `Sol_Patrol (object 39, id 561, starts at point 0)`, `Sol_Patrol (object 40, id 562, starts at point 0)`, `Sol_Patrol (object 41, id 563, starts at point 0)`, `Sol_Patrol (object 42, id 564, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-53.19, 0.00, 6475.66) | None |
| 1 | (35.71, 0.00, 73.57) | None |

### Waypoint 5

- Tag: `0`
- Members: `RIPPER (object 25, id 220, starts at point 0)`, `RIPPER (object 26, id 221, starts at point 0)`, `RIPPER (object 27, id 223, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1099.88, 2.00, 136.18) | None |
| 1 | (-886.83, 0.00, -558.40) | on arrival redirect to waypoint tag 15, point 0 |

### Waypoint 6

- Tag: `0`
- Members: `BORA_CRUISER (object 33, id 417, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1911.72, -165.00, -1939.83) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 7

- Tag: `0`
- Members: `RIPPER (object 22, id 216, starts at point 0)`, `RIPPER (object 23, id 217, starts at point 0)`, `RIPPER (object 24, id 219, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1366.50, 2.00, -248.23) | None |
| 1 | (-920.06, 72.00, 213.35) | on arrival redirect to waypoint tag 14, point 0 |

### Waypoint 8

- Tag: `0`
- Members: `CLAW (object 16, id 204, starts at point 0)`, `CLAW (object 17, id 205, starts at point 0)`, `CLAW (object 18, id 206, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-430.99, 72.00, -292.59) | None |
| 1 | (-1006.09, 0.00, 21.27) | on arrival redirect to waypoint tag 13, point 0 |

### Waypoint 9

- Tag: `0`
- Members: `CLAW (object 19, id 208, starts at point 0)`, `CLAW (object 20, id 209, starts at point 0)`, `CLAW (object 21, id 210, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-391.31, 72.00, 81.26) | None |
| 1 | (-818.81, 0.00, -387.89) | on arrival redirect to waypoint tag 12, point 0 |

### Waypoint 10

- Tag: `0`
- Members: `MANTA (object 12, id 181, starts at point 0)`, `MANTA (object 13, id 182, starts at point 0)`, `MANTA (object 14, id 183, starts at point 0)`, `MANTA (object 15, id 184, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (634.57, -140.00, 285.05) | None |
| 1 | (3076.64, 397.00, -98.16) | None |

### Waypoint 11

- Tag: `0`
- Members: `DART (object 6, id 173, starts at point 0)`, `DART (object 7, id 174, starts at point 0)`, `DART (object 8, id 175, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (292.46, -145.00, 228.15) | None |
| 1 | (1337.71, 377.00, -331.06) | None |

### Waypoint 12

- Tag: `0`
- Members: `MANTA (object 28, id 255, starts at point 0)`, `MANTA (object 29, id 256, starts at point 0)`, `MANTA (object 30, id 257, starts at point 0)`, `MANTA (object 31, id 258, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (660.97, -150.00, -609.37) | None |
| 1 | (3280.70, -463.00, -284.06) | None |

### Waypoint 13

- Tag: `0`
- Members: `DART (object 3, id 169, starts at point 0)`, `DART (object 4, id 170, starts at point 0)`, `DART (object 5, id 171, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (565.15, -145.00, -619.49) | None |
| 1 | (1324.87, 72.00, -422.40) | on arrival redirect to waypoint tag 8, point 0 |

### Waypoint 14

- Tag: `0`
- Members: `DART (object 9, id 177, starts at point 0)`, `DART (object 10, id 178, starts at point 0)`, `DART (object 11, id 179, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (326.71, -160.00, -328.96) | None |
| 1 | (1303.18, 0.00, -33.74) | on arrival redirect to waypoint tag 7, point 0 |

### Waypoint 15

- Tag: `0`
- Members: `DART (object 0, id 165, starts at point 0)`, `DART (object 1, id 166, starts at point 0)`, `DART (object 2, id 167, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (368.26, -160.00, -1.96) | None |
| 1 | (2062.51, 35.00, -223.01) | None |

## Spawn Lists

### Spawn List 0

- ID: `77`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | GALSPAN_CARRIER (object 34, id 527) | None |

### Spawn List 1

- ID: `76`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | GALSPAN_CARRIER (object 34, id 527) | None |

### Spawn List 2

- ID: `87`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 3

- ID: `88`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 4

- ID: `64`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 5

- ID: `65`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 6

- ID: `74`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 7

- ID: `75`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 8

- ID: `66`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 9

- ID: `67`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 10

- ID: `68`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 11

- ID: `69`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 12

- ID: `72`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `DART` | 165 | Interactive | -123.40,-160.00,274.94 | 128,0,0 | group/role: unknown index 64 / 0; secondary groups: unknown index 0, none; waypoint: Waypoint 15 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 1 | `DART` | 166 | Interactive | -258.80,-160.00,588.68 | 128,0,0 | group/role: unknown index 64 / 1; secondary groups: unknown index 0, none; waypoint: Waypoint 15 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 2 | `DART` | 167 | Interactive | -256.40,-160.00,13.70 | 128,0,0 | group/role: unknown index 64 / 2; secondary groups: unknown index 0, none; waypoint: Waypoint 15 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 3 | `DART` | 169 | Interactive | -2224.51,-160.00,-526.19 | 114,0,0 | group/role: unknown index 74 / 0; secondary groups: unknown index 0, none; waypoint: Waypoint 13 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 4 | `DART` | 170 | Interactive | -2414.05,-160.00,-272.03 | 114,0,0 | group/role: unknown index 74 / 1; secondary groups: unknown index 0, none; waypoint: Waypoint 13 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 5 | `DART` | 171 | Interactive | -2438.90,-160.00,-797.02 | 114,0,0 | group/role: unknown index 74 / 2; secondary groups: unknown index 0, none; waypoint: Waypoint 13 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 6 | `DART` | 173 | Interactive | -2307.13,-160.00,656.94 | 142,0,0 | group/role: unknown index 75 / 0; secondary groups: unknown index 0, none; waypoint: Waypoint 11 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 7 | `DART` | 174 | Interactive | -2516.60,-160.00,998.59 | 142,0,0 | group/role: unknown index 75 / 1; secondary groups: unknown index 0, none; waypoint: Waypoint 11 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 8 | `DART` | 175 | Interactive | -2466.45,-160.00,396.11 | 142,0,0 | group/role: unknown index 75 / 2; secondary groups: unknown index 0, none; waypoint: Waypoint 11 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 9 | `DART` | 177 | Interactive | -186.75,-160.00,-496.28 | 128,0,0 | group/role: unknown index 65 / 0; secondary groups: unknown index 0, none; waypoint: Waypoint 14 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 10 | `DART` | 178 | Interactive | -301.30,-160.00,-232.96 | 128,0,0 | group/role: unknown index 65 / 1; secondary groups: unknown index 0, none; waypoint: Waypoint 14 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 11 | `DART` | 179 | Interactive | -311.07,-160.00,-776.27 | 128,0,0 | group/role: unknown index 65 / 2; secondary groups: unknown index 0, none; waypoint: Waypoint 14 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 12 | `MANTA` | 181 | Interactive | -2781.95,-160.00,813.50 | 146,0,0 | group/role: unknown index 77 / 0; secondary groups: unknown index 0, none; waypoint: Waypoint 10 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 13 | `MANTA` | 182 | Interactive | -2911.49,-160.00,962.68 | 146,0,0 | group/role: unknown index 77 / 1; secondary groups: unknown index 0, none; waypoint: Waypoint 10 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 14 | `MANTA` | 183 | Interactive | -2901.27,-160.00,693.49 | 146,0,0 | group/role: unknown index 77 / 2; secondary groups: unknown index 0, none; waypoint: Waypoint 10 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 15 | `MANTA` | 184 | Interactive | -3010.88,-160.00,822.67 | 146,0,0 | group/role: unknown index 77 / 3; secondary groups: unknown index 0, none; waypoint: Waypoint 10 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 16 | `CLAW` | 204 | Interactive | 174.55,72.00,-524.65 | 384,0,0 | group/role: unknown index 67 / 0; secondary groups: unknown index 0, none; waypoint: Waypoint 8 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 17 | `CLAW` | 205 | Interactive | 369.33,72.00,-770.49 | 384,0,0 | group/role: unknown index 67 / 1; secondary groups: unknown index 0, none; waypoint: Waypoint 8 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 18 | `CLAW` | 206 | Interactive | 344.25,72.00,-270.47 | 384,0,0 | group/role: unknown index 67 / 2; secondary groups: unknown index 0, none; waypoint: Waypoint 8 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 19 | `CLAW` | 208 | Interactive | 202.78,72.00,275.96 | 384,0,0 | group/role: unknown index 66 / 0; secondary groups: unknown index 0, none; waypoint: Waypoint 9 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 20 | `CLAW` | 209 | Interactive | 404.55,72.00,-52.22 | 384,0,0 | group/role: unknown index 66 / 1; secondary groups: unknown index 0, none; waypoint: Waypoint 9 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 21 | `CLAW` | 210 | Interactive | 349.40,72.00,617.80 | 384,0,0 | group/role: unknown index 66 / 2; secondary groups: unknown index 0, none; waypoint: Waypoint 9 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 22 | `RIPPER` | 216 | Interactive | 3014.48,2.00,-919.57 | 384,0,0 | group/role: unknown index 68 / 0; secondary groups: unknown index 0, none; waypoint: Waypoint 7 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 23 | `RIPPER` | 217 | Interactive | 2899.10,2.00,-1105.39 | 384,0,0 | group/role: unknown index 68 / 1; secondary groups: unknown index 0, none; waypoint: Waypoint 7 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 24 | `RIPPER` | 219 | Interactive | 3053.56,2.00,-1309.57 | 384,0,0 | group/role: unknown index 68 / 3; secondary groups: unknown index 0, none; waypoint: Waypoint 7 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 25 | `RIPPER` | 220 | Interactive | 2800.47,2.00,1302.73 | 384,0,0 | group/role: unknown index 69 / 0; secondary groups: unknown index 0, none; waypoint: Waypoint 5 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 26 | `RIPPER` | 221 | Interactive | 2690.01,2.00,1091.08 | 384,0,0 | group/role: unknown index 69 / 1; secondary groups: unknown index 0, none; waypoint: Waypoint 5 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 27 | `RIPPER` | 223 | Interactive | 2839.63,2.00,876.90 | 384,0,0 | group/role: unknown index 69 / 3; secondary groups: unknown index 0, none; waypoint: Waypoint 5 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 28 | `MANTA` | 255 | Interactive | -2852.85,-160.00,-901.13 | 128,0,0 | group/role: unknown index 76 / 0; secondary groups: unknown index 0, none; waypoint: Waypoint 12 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 29 | `MANTA` | 256 | Interactive | -2990.81,-160.00,-790.38 | 128,0,0 | group/role: unknown index 76 / 1; secondary groups: unknown index 0, none; waypoint: Waypoint 12 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 30 | `MANTA` | 257 | Interactive | -2980.81,-160.00,-1019.85 | 128,0,0 | group/role: unknown index 76 / 2; secondary groups: unknown index 0, none; waypoint: Waypoint 12 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 31 | `MANTA` | 258 | Interactive | -4849.49,-160.00,-883.13 | 128,0,0 | group/role: unknown index 76 / 3; secondary groups: unknown index 0, none; waypoint: Waypoint 12 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 32 | `BORA_CARRIER` | 335 | Interactive | -3702.75,-160.00,9.37 | 128,0,0 | group/role: unknown index 78 / 0; secondary groups: unknown index 0, none |
| 33 | `BORA_CRUISER` | 417 | Interactive | -2769.23,-155.00,-1959.47 | 128,0,0 | group/role: unknown index 83 / 0; secondary groups: unknown index 0, none; waypoint: Waypoint 6 (tag 0, 1 point(s)), starting point 0, arrival event value 0 |
| 34 | `GALSPAN_CARRIER` | 527 | Interactive | 3404.74,0.00,-28.78 | 384,0,0 | group/role: unknown index 86 / 0; secondary groups: unknown index 0, unknown index 164 |
| 35 | `Sol_Patrol` | 555 | Interactive | -541.99,0.00,7457.40 | 256,0,0 | group/role: unknown index 87 / 0; secondary groups: unknown index 0, none; waypoint: Waypoint 4 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 36 | `Sol_Patrol` | 556 | Interactive | -132.45,0.00,7457.40 | 256,0,0 | group/role: unknown index 87 / 1; secondary groups: unknown index 0, none; waypoint: Waypoint 4 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 37 | `Sol_Patrol` | 557 | Interactive | 208.83,0.00,7457.40 | 256,0,0 | group/role: unknown index 87 / 2; secondary groups: unknown index 0, none; waypoint: Waypoint 4 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 38 | `Sol_Patrol` | 558 | Interactive | 584.25,0.00,7383.02 | 256,0,0 | group/role: unknown index 87 / 3; secondary groups: unknown index 0, none; waypoint: Waypoint 4 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 39 | `Sol_Patrol` | 561 | Interactive | -678.51,0.00,8052.44 | 256,0,0 | group/role: unknown index 88 / 0; secondary groups: unknown index 0, none; waypoint: Waypoint 4 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 40 | `Sol_Patrol` | 562 | Interactive | -303.09,0.00,8015.25 | 256,0,0 | group/role: unknown index 88 / 1; secondary groups: unknown index 0, none; waypoint: Waypoint 4 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 41 | `Sol_Patrol` | 563 | Interactive | 72.32,0.00,7978.06 | 256,0,0 | group/role: unknown index 88 / 2; secondary groups: unknown index 0, none; waypoint: Waypoint 4 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 42 | `Sol_Patrol` | 564 | Interactive | 447.73,0.00,7903.68 | 256,0,0 | group/role: unknown index 88 / 3; secondary groups: unknown index 0, none; waypoint: Waypoint 4 (tag 0, 2 point(s)), starting point 0, arrival event value 0 |
| 43 | `CLAW` | 565 | Interactive | 478.90,0.00,-2844.94 | 0,0,0 | group/role: unknown index 72 / 0; alias: fred1; secondary groups: unknown index 0, none; waypoint: Waypoint 3 (tag 0, 3 point(s)), starting point 0, arrival event value 0 |
| 44 | `CLAW` | 566 | Interactive | 337.64,0.00,-3113.99 | 0,0,0 | group/role: unknown index 72 / 1; alias: fred2; secondary groups: unknown index 0, none; waypoint: Waypoint 3 (tag 0, 3 point(s)), starting point 0, arrival event value 0 |
| 45 | `CLAW` | 567 | Interactive | 639.76,0.00,-3115.99 | 0,0,0 | group/role: unknown index 72 / 2; alias: fred3; secondary groups: unknown index 0, none; waypoint: Waypoint 3 (tag 0, 3 point(s)), starting point 0, arrival event value 0 |
| 46 | `GALSPAN_DESTROYER` | 608 | Interactive | 2650.95,0.00,-1748.99 | 384,0,0 | group/role: unknown index 73 / 3; secondary groups: unknown index 0, none; waypoint: Waypoint 2 (tag 0, 1 point(s)), starting point 0, arrival event value 0 |
