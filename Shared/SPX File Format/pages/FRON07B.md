# Tachyon: The Fringe FRON07B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON07B.SPX` |
| Sector | `QUAD_07` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 6 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 16 |
| Events | 12 |
| Waypoints | 7 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Baronial_Shuttle`, `1: Hajod_Fighter_2`, `2: Onrald_Flare` |
| Scripts | `ALEX.SCR`, `HGARD.SCR`, `HAJOD.SCR` |
| Scenes | None |
| Labels | `BFGE_01`, `alexander`, `BFGF_01`, `baronhajod` |
| Aliases | `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1` |
| Groups | `FG_LIBRE`, `FG_TRAITE`, `FG_CONFIANCE`, `FG_SHREWD`, `FG_AMITIE`, `FG_VALEUR`, `ALEXANDER_ONRALD`, `FG_DISCIPLINE`, `FG_MONARCH`, `MANACLE` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 24, subtype 0, value 0
- Group/spawn-list action: spawn list/group 244, subtype 4, param 9
- Group/spawn-list action: spawn list/group 246, subtype 4, param 9
- Group/spawn-list action: spawn list/group 247, subtype 4, param 9
- Group/spawn-list action: spawn list/group 249, subtype 4, param 9
- Group/spawn-list action: spawn list/group 250, subtype 4, param 9

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Group/spawn-list action: spawn list/group 248, subtype 4, param 9
- Object spawn/action: id 896, subtype 8, param 9
- Show/update HUD contact: contact/list 0, subtype 9, param 25

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 24, op 1, value 5

**Action**

- Play dialog: ALEX.SCR, line/variant 0
- Set runtime trigger variable: variable group 20, variable 24, subtype 1, value 0
- Object spawn/action: Baronial_Shuttle (object 15, id 1202), subtype 1, param 1

### Event 3

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 0

**Action**

- Play dialog: HGARD.SCR, line/variant 0

### Event 4

**Trigger**

- Object event: subject Onrald_Flare (object 10, id 706), op 0, value 0 (join 1; flags 2)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Play dialog: HAJOD.SCR, line/variant 11

### Event 5

**Trigger**

- Object event: subject Onrald_Flare (object 10, id 706), op 4, value 80 (join 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Play dialog: HAJOD.SCR, line/variant 14

### Event 6

**Trigger**

- Object event: subject Onrald_Flare (object 10, id 706), op 6, value 0 (join 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Play scene: unknown index 0, param 1
- Play dialog: HAJOD.SCR, line/variant 16
- Hide/remove HUD contact: contact/list 0, subtype 9, param 25
- Set/add variable: variable group 21, variable 26, subtype 0, value 1

### Event 7

**Trigger**

- Object event: subject Onrald_Flare (object 10, id 706), op 2, value 0 (join 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1 (join 1)
- Runtime condition family: subject 0, op 0, value 0

**Action**

- Set/add variable: variable group 16, variable 411, subtype 0, value 1
- Set/add variable: variable group 16, variable 410, subtype 0, value 1
- Play dialog: HAJOD.SCR, line/variant 13
- Mark/flash contact: contact/list 0, subtype 8, param 25
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 38
- Hide/remove HUD contact: contact/list 0, subtype 9, param 26
- Hide/remove HUD contact: contact/list 0, subtype 9, param 25

### Event 8

**Trigger**

- Object event: subject Baronial_Shuttle (object 15, id 1202), op 2, value 0

**Action**

- Mark/flash contact: contact/list 0, subtype 8, param 26
- Set/add variable: variable group 21, variable 20, subtype 0, value 1
- Set/add variable: variable group 16, variable 411, subtype 0, value 1
- Set/add variable: variable group 16, variable 410, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 38
- Hide/remove HUD contact: contact/list 0, subtype 9, param 25

### Event 9

**Trigger**

- Object event: subject Baronial_Shuttle (object 15, id 1202), op 4, value 50

**Action**

- Play dialog: HAJOD.SCR, line/variant 15

### Event 10

**Trigger**

- Runtime condition family: subject 0, op 0, value 0

**Action**

- Object spawn/action: Baronial_Shuttle (object 15, id 1202), subtype 2, param 1
- Play dialog: HAJOD.SCR, line/variant 17
- Show/update HUD contact: contact/list 0, subtype 9, param 26
- Group/spawn-list action: spawn list/group 162, subtype 3, param 1
- Group/spawn-list action: spawn list/group 132, subtype 3, param 1
- Object spawn/action: Baronial_Shuttle (object 15, id 1202), subtype 14

### Event 11

**Trigger**

- Object event: subject Baronial_Shuttle (object 15, id 1202), op 7, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 37
- Set/add variable: variable group 16, variable 410, subtype 0, value 1
- Set/add variable: variable group 16, variable 411, subtype 0, value 2
- Hide/remove HUD contact: contact/list 0, subtype 9, param 26

## Waypoints

### Waypoint 0

- Tag: `4`
- Members: `Onrald_Flare (object 1, id 815, starts at point 0)`, `Onrald_Flare (object 2, id 816, starts at point 0)`, `Onrald_Flare (object 10, id 706, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-0.01, -586.36, 2886.55) | None |
| 1 | (256.18, -586.36, 2438.68) | None |
| 2 | (203.90, -586.36, 2002.16) | None |
| 3 | (-449.66, -586.36, 1917.12) | None |
| 4 | (-716.31, -586.36, 2489.71) | None |
| 5 | (-543.77, -586.36, 3323.08) | None |
| 6 | (203.90, -586.36, 3617.88) | None |
| 7 | (1003.85, -586.36, 3623.55) | None |
| 8 | (1453.50, -586.36, 3419.46) | None |
| 9 | (1578.98, -586.36, 2665.45) | None |
| 10 | (1103.19, -586.36, 2268.61) | None |
| 11 | (1469.18, -586.36, 1815.07) | None |
| 12 | (1814.26, -586.36, 2030.50) | None |
| 13 | (1877.00, -586.36, 3113.32) | on arrival redirect to Waypoint 0 (tag 4), point 0 |

### Waypoint 1

- Tag: `151`
- Members: `Baronial_Shuttle (object 15, id 1202, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (813.75, 0.00, -1117.10) | None |
| 1 | (813.75, 0.00, -862.54) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 2

- Tag: `12`
- Members: `Hajod_Fighter_2 (object 11, id 890, starts at point 0)`, `Hajod_Fighter_2 (object 12, id 891, starts at point 0)`, `Hajod_Fighter_2 (object 13, id 892, starts at point 0)`, `Hajod_Fighter_2 (object 14, id 893, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (620.69, 0.00, -1260.97) | None |
| 1 | (534.36, 0.00, -649.03) | None |

### Waypoint 3

- Tag: `11`
- Members: `Onrald_Flare (object 4, id 820, starts at point 0)`, `Onrald_Flare (object 5, id 821, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1309.35, -636.12, 1189.06) | None |
| 1 | (2034.91, -636.12, 268.19) | None |
| 2 | (877.99, -636.12, -199.30) | on arrival redirect to Waypoint 3 (tag 11), point 0 |

### Waypoint 4

- Tag: `10`
- Members: `Onrald_Flare (object 6, id 823, starts at point 0)`, `Onrald_Flare (object 7, id 824, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (798.80, 799.59, 238.41) | None |
| 1 | (754.40, 799.59, 958.28) | None |
| 2 | (-73.05, 799.59, 605.51) | on arrival redirect to Waypoint 4 (tag 10), point 0 |

### Waypoint 5

- Tag: `6`
- Members: `Onrald_Flare (object 0, id 809, starts at point 0)`, `Onrald_Flare (object 3, id 817, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-569.43, 611.24, 860.83) | None |
| 1 | (-911.71, 611.24, -61.01) | None |
| 2 | (194.55, 611.24, -143.74) | None |

### Waypoint 6

- Tag: `5`
- Members: `Onrald_Flare (object 8, id 825, starts at point 0)`, `Onrald_Flare (object 9, id 826, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (261.49, 0.00, -528.29) | None |
| 1 | (706.02, 0.00, -1807.10) | None |
| 2 | (1350.49, 0.00, -562.53) | on arrival redirect to Waypoint 6 (tag 5), point 0 |

## Spawn Lists

### Spawn List 0

- ID: `250`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 6 | Baronial_Shuttle (object 15, id 1202) | None |

### Spawn List 1

- ID: `249`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 8 | spawn list 250 | None |
| 2 | 6 | Baronial_Shuttle (object 15, id 1202) | None |

### Spawn List 2

- ID: `248`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 6 | Baronial_Shuttle (object 15, id 1202) | None |

### Spawn List 3

- ID: `247`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 6 | Baronial_Shuttle (object 15, id 1202) | None |

### Spawn List 4

- ID: `246`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 6 | Baronial_Shuttle (object 15, id 1202) | None |

### Spawn List 5

- ID: `244`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 6 | Baronial_Shuttle (object 15, id 1202) | None |

### Spawn List 6

- ID: `162`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 5 | spawn list 250 | None |
| 1 | 1 | spawn list 247 | None |

### Spawn List 7

- ID: `132`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 5 | spawn list 250 | None |
| 1 | 1 | spawn list 244 | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Onrald_Flare` | 809 | Interactive | -401.62,611.24,853.26 | 407,0,0 | group/role: FG_LIBRE / 0; waypoint: Waypoint 5 (tag 6, 3 point(s)), starting point 0, arrival event value 393216 |
| 1 | `Onrald_Flare` | 815 | Interactive | -239.71,0.00,3349.76 | 208,0,0 | group/role: FG_TRAITE / 0; waypoint: Waypoint 0 (tag 4, 14 point(s)), starting point 0, arrival event value 262144 |
| 2 | `Onrald_Flare` | 816 | Interactive | -135.06,0.00,3395.47 | 208,0,0 | label: BFGE_01; group/role: FG_TRAITE / 0; waypoint: Waypoint 0 (tag 4, 14 point(s)), starting point 0, arrival event value 262144 |
| 3 | `Onrald_Flare` | 817 | Interactive | -370.13,611.24,901.03 | 457,0,0 | group/role: FG_LIBRE / 0; waypoint: Waypoint 5 (tag 6, 3 point(s)), starting point 0, arrival event value 393216 |
| 4 | `Onrald_Flare` | 820 | Interactive | 1094.08,-636.12,1340.31 | 253,0,0 | group/role: FG_CONFIANCE / 0; waypoint: Waypoint 3 (tag 11, 3 point(s)), starting point 0, arrival event value 720896 |
| 5 | `Onrald_Flare` | 821 | Interactive | 1130.54,-636.12,1341.19 | 238,0,0 | group/role: FG_CONFIANCE / 0; waypoint: Waypoint 3 (tag 11, 3 point(s)), starting point 0, arrival event value 720896 |
| 6 | `Onrald_Flare` | 823 | Interactive | 796.65,799.59,81.21 | 0,0,0 | group/role: FG_SHREWD / 0; waypoint: Waypoint 4 (tag 10, 3 point(s)), starting point 0, arrival event value 655360 |
| 7 | `Onrald_Flare` | 824 | Interactive | 861.29,799.59,96.82 | 0,0,0 | label: BFGE_01; group/role: FG_SHREWD / 0; waypoint: Waypoint 4 (tag 10, 3 point(s)), starting point 0, arrival event value 655360 |
| 8 | `Onrald_Flare` | 825 | Interactive | 314.44,0.00,-305.21 | 316,0,0 | group/role: FG_AMITIE / 0; waypoint: Waypoint 6 (tag 5, 3 point(s)), starting point 0, arrival event value 327680 |
| 9 | `Onrald_Flare` | 826 | Interactive | 387.70,0.00,-305.21 | 316,0,0 | label: BFGE_01; group/role: FG_AMITIE / 0; waypoint: Waypoint 6 (tag 5, 3 point(s)), starting point 0, arrival event value 327680 |
| 10 | `Onrald_Flare` | 706 | Interactive | -192.28,0.00,3393.67 | 202,0,0 | label: alexander; group/role: FG_VALEUR / 0; secondary groups: none, ALEXANDER_ONRALD; waypoint: Waypoint 0 (tag 4, 14 point(s)), starting point 0, arrival event value 262144 |
| 11 | `Hajod_Fighter_2` | 890 | Interactive | 691.68,0.00,-1480.98 | 0,0,0 | label: BFGF_01; group/role: FG_DISCIPLINE / 0; alias: jumbo; waypoint: Waypoint 2 (tag 12, 2 point(s)), starting point 0, arrival event value 786432 |
| 12 | `Hajod_Fighter_2` | 891 | Interactive | 751.42,0.00,-1483.57 | 0,0,0 | group/role: FG_DISCIPLINE / 0; alias: jumbo_1; waypoint: Waypoint 2 (tag 12, 2 point(s)), starting point 0, arrival event value 786432 |
| 13 | `Hajod_Fighter_2` | 892 | Interactive | 694.13,0.00,-1551.54 | 0,0,0 | group/role: FG_MONARCH / 0; alias: egg; waypoint: Waypoint 2 (tag 12, 2 point(s)), starting point 0, arrival event value 786432 |
| 14 | `Hajod_Fighter_2` | 893 | Interactive | 750.15,0.00,-1548.52 | 0,0,0 | label: BFGF_01; group/role: FG_MONARCH / 0; alias: egg_1; waypoint: Waypoint 2 (tag 12, 2 point(s)), starting point 0, arrival event value 786432 |
| 15 | `Baronial_Shuttle` | 1202 | Interactive | 826.19,0.00,-1404.88 | 0,0,0 | label: baronhajod; alias: Hajod_1; secondary groups: none, MANACLE; waypoint: Waypoint 1 (tag 151, 2 point(s)), starting point 0, arrival event value 9895936 |
