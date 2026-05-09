# Tachyon: The Fringe FRON12B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON12B.SPX` |
| Sector | `QUAD_12` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 11 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 34 |
| Events | 10 |
| Waypoints | 11 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Baronial_Shuttle`, `1: Hajod_Fighter_2`, `2: Red_Pirate_Fighter_2`, `3: Red_Pirate_Shrike` |
| Scripts | `RRORY.SCR`, `PRSPH.SCR`, `HAJOD.SCR` |
| Scenes | None |
| Labels | `BFNF_01`, `BFGE_01`, `BFNE_02` |
| Aliases | `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1`, `Stocks01` |
| Groups | `FG_PRIDE`, `FG_HORROR`, `FG_PLAGUE`, `FG_SLOTH`, `FG_GREED`, `FG_WAR`, `FG_LUST`, `FG_RAGE`, `FG_PESTILENCE`, `FG_DEATH`, `FG_DISCIPLINE`, `FG_MONARCH`, `MANACLE` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Object event: subject Baronial_Shuttle (object 33, id 1385), op 15, value 0

**Action**

- Play dialog: RRORY.SCR, line/variant 7
- Group/spawn-list action: spawn list/group 63, subtype 4, param 4
- Object spawn/action: id 1366, subtype 8, param 4
- Set runtime trigger variable: variable group 20, variable 2, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 6, param 1385
- Object spawn/action: Baronial_Shuttle (object 33, id 1385), subtype 14

### Event 1

**Trigger**

- Group/spawn-list event: subject 132, op 3, value 0 (join 2)
- Group/spawn-list event: subject 162, op 3, value 0 (join 2)
- Group/spawn-list event: subject 131, op 3, value 0 (join 2)

**Action**

- Group/spawn-list action: spawn list/group 61, subtype 4, param 4
- Group/spawn-list action: spawn list/group 62, subtype 4, param 4
- Group/spawn-list action: spawn list/group 136, subtype 4, param 4
- Group/spawn-list action: spawn list/group 137, subtype 4, param 4
- Group/spawn-list action: spawn list/group 65, subtype 4, param 4
- Group/spawn-list action: spawn list/group 66, subtype 4, param 4
- Group/spawn-list action: spawn list/group 64, subtype 4, param 4
- Group/spawn-list action: spawn list/group 60, subtype 4, param 4

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 10

**Action**

- Group/spawn-list action: spawn list/group 132, subtype 3, param 3
- Group/spawn-list action: spawn list/group 162, subtype 3, param 3
- Set runtime trigger variable: variable group 20, variable 2, subtype 1, value 0

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 1600 (extra 1, 1333; flags 2)

**Action**

- Play dialog: PRSPH.SCR, line/variant 1

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 900 (extra 1, 1333; flags 2)

**Action**

- Play dialog: PRSPH.SCR, line/variant 5

### Event 5

**Trigger**

- Object event: subject Baronial_Shuttle (object 33, id 1385), op 15, value 0
- Variable comparison: subject variable group 21, variable 26, op 1, value 1

**Action**

- Object spawn/action: Baronial_Shuttle (object 33, id 1385), subtype 16

### Event 6

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 26, op 1, value 1

**Action**

- Play dialog: HAJOD.SCR, line/variant 18
- Object spawn/action: id 1333, subtype 18

### Event 7

**Trigger**

- Variable comparison: subject variable group 21, variable 26, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 61, subtype 4, param 9
- Group/spawn-list action: spawn list/group 62, subtype 4, param 9
- Group/spawn-list action: spawn list/group 136, subtype 4, param 9
- Group/spawn-list action: spawn list/group 137, subtype 4, param 9
- Group/spawn-list action: spawn list/group 65, subtype 4, param 9
- Group/spawn-list action: spawn list/group 66, subtype 4, param 9
- Group/spawn-list action: spawn list/group 64, subtype 4, param 9
- Object spawn/action: id 1366, subtype 8, param 9

### Event 8

**Trigger**

- Object event: subject Baronial_Shuttle (object 33, id 1385), op 7, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 6, param 1385

### Event 9

**Trigger**

- Object arrival: Baronial_Shuttle (object 33, id 1385) reached Waypoint 0 (tag 15), point 4 (raw value 983044)

**Action**

- Object spawn/action: Baronial_Shuttle (object 33, id 1385), subtype 2, param 3

## Waypoints

### Waypoint 0

- Tag: `15`
- Members: `Hajod_Fighter_2 (object 29, id 1118, starts at point 0)`, `Hajod_Fighter_2 (object 30, id 1119, starts at point 0)`, `Hajod_Fighter_2 (object 31, id 1120, starts at point 0)`, `Hajod_Fighter_2 (object 32, id 1121, starts at point 0)`, `Baronial_Shuttle (object 33, id 1385, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (104.67, 0.00, -50.87) | None |
| 1 | (695.89, 0.00, 965.66) | None |
| 2 | (1444.28, 0.00, 1655.93) | None |
| 3 | (2413.94, 0.00, 2064.25) | None |
| 4 | (3375.06, 0.00, 2138.18) | on arrival play dialog/script or enter gate, param 3; listened by Event 9 for Baronial_Shuttle (object 33, id 1385) |

### Waypoint 1

- Tag: `14`
- Members: `Red_Pirate_Fighter_2 (object 24, id 1073, starts at point 0)`, `Red_Pirate_Fighter_2 (object 25, id 1074, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (529.40, 0.00, 857.32) | on arrival redirect to Waypoint 2 (tag 13), point 0 |
| 1 | (1068.30, 0.00, 2212.81) | None |
| 2 | (2282.54, 0.00, 3061.49) | None |
| 3 | (3510.02, 0.00, 2911.80) | None |

### Waypoint 2

- Tag: `13`
- Members: `Red_Pirate_Fighter_2 (object 15, id 1069, starts at point 0)`, `Red_Pirate_Fighter_2 (object 17, id 1071, starts at point 0)`, `Red_Pirate_Fighter_2 (object 18, id 1072, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1437.91, 0.00, -122.32) | None |
| 1 | (2938.95, 0.00, -1085.39) | None |
| 2 | (4726.59, 0.00, -654.23) | None |
| 3 | (5205.08, 0.00, 1593.74) | on arrival redirect to Waypoint 1 (tag 14), point 3 |

### Waypoint 3

- Tag: `12`
- Members: `Red_Pirate_Fighter_2 (object 4, id 1049, starts at point 0)`, `Red_Pirate_Fighter_2 (object 5, id 1050, starts at point 0)`, `Red_Pirate_Fighter_2 (object 6, id 1051, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (5288.81, 0.00, -882.47) | None |
| 1 | (5952.41, 0.00, 2499.27) | None |
| 2 | (7705.65, 0.00, 3516.25) | None |
| 3 | (6401.71, 0.00, -2020.64) | None |
| 4 | (3511.83, 0.00, -2292.32) | on arrival redirect to Waypoint 3 (tag 12), point 0 |

### Waypoint 4

- Tag: `10`
- Members: `Red_Pirate_Fighter_2 (object 7, id 1053, starts at point 0)`, `Red_Pirate_Fighter_2 (object 8, id 1054, starts at point 0)`, `Red_Pirate_Fighter_2 (object 9, id 1052, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2272.95, 0.00, 4535.09) | None |
| 1 | (3532.26, 0.00, 6626.02) | None |
| 2 | (5027.69, 0.00, 4408.37) | on arrival redirect to Waypoint 4 (tag 10), point 0 |

### Waypoint 5

- Tag: `9`
- Members: `Red_Pirate_Shrike (object 0, id 1055, starts at point 0)`, `Red_Pirate_Shrike (object 1, id 1056, starts at point 0)`, `Red_Pirate_Fighter_2 (object 16, id 1070, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2992.57, 0.00, 3703.11) | None |
| 1 | (-1602.09, 0.00, 5730.68) | None |
| 2 | (452.07, 0.00, 4440.77) | on arrival redirect to Waypoint 5 (tag 9), point 0 |

### Waypoint 6

- Tag: `7`
- Members: `Red_Pirate_Shrike (object 2, id 1063, starts at point 0)`, `Red_Pirate_Fighter_2 (object 21, id 1061, starts at point 0)`, `Red_Pirate_Fighter_2 (object 22, id 1062, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (52.76, 0.00, 223.58) | None |
| 1 | (1664.46, 0.00, -843.40) | None |
| 2 | (475.60, 0.00, -2329.78) | None |
| 3 | (-570.67, 0.00, -1214.99) | on arrival redirect to Waypoint 7 (tag 6), point 0 |

### Waypoint 7

- Tag: `6`
- Members: `Red_Pirate_Fighter_2 (object 19, id 1060, starts at point 0)`, `Red_Pirate_Fighter_2 (object 20, id 1059, starts at point 0)`, `Red_Pirate_Shrike (object 23, id 1065, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-816.86, 0.00, -685.14) | None |
| 1 | (-1740.04, 0.00, -908.10) | None |
| 2 | (-970.72, 0.00, -2022.89) | None |
| 3 | (875.65, 0.00, -685.14) | on arrival redirect to Waypoint 6 (tag 7), point 0 |

### Waypoint 8

- Tag: `5`
- Members: `Red_Pirate_Shrike (object 3, id 1064, starts at point 0)`, `Red_Pirate_Fighter_2 (object 10, id 1057, starts at point 0)`, `Red_Pirate_Fighter_2 (object 11, id 1058, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2326.47, 0.00, 1677.71) | None |
| 1 | (-3674.95, 0.00, 1322.79) | None |
| 2 | (-3505.12, 0.00, -1208.22) | None |
| 3 | (-1573.26, 0.00, -167.91) | on arrival redirect to Waypoint 8 (tag 5), point 0 |

### Waypoint 9

- Tag: `4`
- Members: `Red_Pirate_Fighter_2 (object 26, id 1009, starts at point 0)`, `Red_Pirate_Fighter_2 (object 27, id 1010, starts at point 0)`, `Red_Pirate_Fighter_2 (object 28, id 1011, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (4337.95, 0.00, 41.84) | None |
| 1 | (4289.37, 0.00, 2228.92) | None |
| 2 | (3290.86, 0.00, 3715.07) | None |
| 3 | (201.48, 0.00, 3142.70) | on arrival redirect to Waypoint 10 (tag 3), point 0 |

### Waypoint 10

- Tag: `3`
- Members: `Red_Pirate_Fighter_2 (object 12, id 1006, starts at point 0)`, `Red_Pirate_Fighter_2 (object 13, id 1007, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1521.39, 0.00, 2682.82) | None |
| 1 | (-1869.71, 0.00, 1084.50) | None |
| 2 | (54.95, 0.00, 786.28) | None |
| 3 | (2131.96, 0.00, 2483.81) | on arrival redirect to Waypoint 9 (tag 4), point 2 |

## Spawn Lists

### Spawn List 0

- ID: `66`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | id 1333 | None |

### Spawn List 1

- ID: `60`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | id 1333 | None |

### Spawn List 2

- ID: `64`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | id 1333 | None |

### Spawn List 3

- ID: `63`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | id 1333 | None |

### Spawn List 4

- ID: `138`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | id 1333 | None |

### Spawn List 5

- ID: `162`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | id 1333 | None |

### Spawn List 6

- ID: `137`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | id 1333 | None |

### Spawn List 7

- ID: `136`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | id 1333 | None |

### Spawn List 8

- ID: `62`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | id 1333 | None |
| 1 | 0 | none | None |

### Spawn List 9

- ID: `132`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | id 1333 | None |

### Spawn List 10

- ID: `61`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | id 1333 | None |
| 1 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Red_Pirate_Shrike` | 1055 | Interactive | -3251.29,0.00,3342.38 | 0,0,0 | group/role: FG_PRIDE / 0; waypoint: Waypoint 5 (tag 9, 3 point(s)), starting point 0, arrival event value 589824 |
| 1 | `Red_Pirate_Shrike` | 1056 | Interactive | -3129.85,0.00,3374.97 | 0,0,0 | group/role: FG_PRIDE / 0; waypoint: Waypoint 5 (tag 9, 3 point(s)), starting point 0, arrival event value 589824 |
| 2 | `Red_Pirate_Shrike` | 1063 | Interactive | -237.97,0.00,362.81 | 122,0,0 | group/role: FG_HORROR / 0; waypoint: Waypoint 6 (tag 7, 4 point(s)), starting point 0, arrival event value 458752 |
| 3 | `Red_Pirate_Shrike` | 1064 | Interactive | -2733.33,0.00,2205.04 | 122,0,0 | group/role: FG_PLAGUE / 0; waypoint: Waypoint 8 (tag 5, 4 point(s)), starting point 0, arrival event value 327680 |
| 4 | `Red_Pirate_Fighter_2` | 1049 | Interactive | 5052.39,0.00,-1520.01 | 0,0,0 | group/role: FG_SLOTH / 0; waypoint: Waypoint 3 (tag 12, 5 point(s)), starting point 0, arrival event value 786432 |
| 5 | `Red_Pirate_Fighter_2` | 1050 | Interactive | 5308.83,0.00,-1352.63 | 0,0,0 | group/role: FG_SLOTH / 0; waypoint: Waypoint 3 (tag 12, 5 point(s)), starting point 0, arrival event value 786432 |
| 6 | `Red_Pirate_Fighter_2` | 1051 | Interactive | 5371.21,0.00,-1720.88 | 0,0,0 | group/role: FG_SLOTH / 0; waypoint: Waypoint 3 (tag 12, 5 point(s)), starting point 0, arrival event value 786432 |
| 7 | `Red_Pirate_Fighter_2` | 1053 | Interactive | 2169.36,0.00,3851.28 | 0,0,0 | label: BFGE_01; group/role: FG_GREED / 0; waypoint: Waypoint 4 (tag 10, 3 point(s)), starting point 0, arrival event value 655360 |
| 8 | `Red_Pirate_Fighter_2` | 1054 | Interactive | 2398.74,0.00,3965.34 | 0,0,0 | group/role: FG_GREED / 0; waypoint: Waypoint 4 (tag 10, 3 point(s)), starting point 0, arrival event value 655360 |
| 9 | `Red_Pirate_Fighter_2` | 1052 | Interactive | 1966.96,0.00,4128.28 | 0,0,0 | group/role: FG_GREED / 0; waypoint: Waypoint 4 (tag 10, 3 point(s)), starting point 0, arrival event value 655360 |
| 10 | `Red_Pirate_Fighter_2` | 1057 | Interactive | -2669.35,0.00,2317.63 | 214,0,0 | group/role: FG_PLAGUE / 0; waypoint: Waypoint 8 (tag 5, 4 point(s)), starting point 0, arrival event value 327680 |
| 11 | `Red_Pirate_Fighter_2` | 1058 | Interactive | -2588.39,0.00,2170.99 | 213,0,0 | label: BFGE_01; group/role: FG_PLAGUE / 0; waypoint: Waypoint 8 (tag 5, 4 point(s)), starting point 0, arrival event value 327680 |
| 12 | `Red_Pirate_Fighter_2` | 1006 | Interactive | -1263.52,0.00,3016.40 | 294,0,0 | group/role: FG_WAR / 0; waypoint: Waypoint 10 (tag 3, 4 point(s)), starting point 0, arrival event value 196608 |
| 13 | `Red_Pirate_Fighter_2` | 1007 | Interactive | -1436.91,0.00,3108.00 | 295,0,0 | group/role: FG_WAR / 0; waypoint: Waypoint 10 (tag 3, 4 point(s)), starting point 0, arrival event value 196608 |
| 14 | `Red_Pirate_Fighter_2` | 1068 | Interactive | 3545.56,0.00,2592.47 | 190,0,0 | group/role: FG_LUST / 0 |
| 15 | `Red_Pirate_Fighter_2` | 1069 | Interactive | 1219.74,0.00,109.40 | 191,0,0 | group/role: FG_RAGE / 0; waypoint: Waypoint 2 (tag 13, 4 point(s)), starting point 0, arrival event value 851968 |
| 16 | `Red_Pirate_Fighter_2` | 1070 | Interactive | -2942.05,0.00,3407.72 | 191,0,0 | group/role: FG_PRIDE / 0; waypoint: Waypoint 5 (tag 9, 3 point(s)), starting point 0, arrival event value 589824 |
| 17 | `Red_Pirate_Fighter_2` | 1071 | Interactive | 1299.05,0.00,226.40 | 70,0,0 | group/role: FG_RAGE / 0; waypoint: Waypoint 2 (tag 13, 4 point(s)), starting point 0, arrival event value 851968 |
| 18 | `Red_Pirate_Fighter_2` | 1072 | Interactive | 1368.35,0.00,82.95 | 70,0,0 | group/role: FG_RAGE / 0; waypoint: Waypoint 2 (tag 13, 4 point(s)), starting point 0, arrival event value 851968 |
| 19 | `Red_Pirate_Fighter_2` | 1060 | Interactive | -1005.53,0.00,-1090.17 | 43,0,0 | group/role: FG_PESTILENCE / 0; waypoint: Waypoint 7 (tag 6, 4 point(s)), starting point 0, arrival event value 393216 |
| 20 | `Red_Pirate_Fighter_2` | 1059 | Interactive | -1085.89,0.00,-960.79 | 43,0,0 | group/role: FG_PESTILENCE / 0; waypoint: Waypoint 7 (tag 6, 4 point(s)), starting point 0, arrival event value 393216 |
| 21 | `Red_Pirate_Fighter_2` | 1061 | Interactive | -352.97,0.00,144.80 | 132,0,0 | group/role: FG_HORROR / 0; waypoint: Waypoint 6 (tag 7, 4 point(s)), starting point 0, arrival event value 458752 |
| 22 | `Red_Pirate_Fighter_2` | 1062 | Interactive | -194.49,0.00,168.73 | 132,0,0 | group/role: FG_HORROR / 0; waypoint: Waypoint 6 (tag 7, 4 point(s)), starting point 0, arrival event value 458752 |
| 23 | `Red_Pirate_Shrike` | 1065 | Interactive | -1111.42,0.00,-1094.35 | 122,0,0 | group/role: FG_PESTILENCE / 0; waypoint: Waypoint 7 (tag 6, 4 point(s)), starting point 0, arrival event value 393216 |
| 24 | `Red_Pirate_Fighter_2` | 1073 | Interactive | 3668.91,0.00,2555.03 | 0,0,0 | label: BFGE_01; group/role: FG_LUST / 0; waypoint: Waypoint 1 (tag 14, 4 point(s)), starting point 0, arrival event value 917504 |
| 25 | `Red_Pirate_Fighter_2` | 1074 | Interactive | 3645.41,0.00,2713.79 | 0,0,0 | group/role: FG_LUST / 0; waypoint: Waypoint 1 (tag 14, 4 point(s)), starting point 0, arrival event value 917504 |
| 26 | `Red_Pirate_Fighter_2` | 1009 | Interactive | 4263.57,0.00,-342.29 | 0,0,0 | group/role: FG_DEATH / 0; waypoint: Waypoint 9 (tag 4, 4 point(s)), starting point 0, arrival event value 262144 |
| 27 | `Red_Pirate_Fighter_2` | 1010 | Interactive | 4491.03,0.00,-521.29 | 0,0,0 | label: BFGE_01; group/role: FG_DEATH / 0; waypoint: Waypoint 9 (tag 4, 4 point(s)), starting point 0, arrival event value 262144 |
| 28 | `Red_Pirate_Fighter_2` | 1011 | Interactive | 4276.34,0.00,-518.21 | 0,0,0 | group/role: FG_DEATH / 0; waypoint: Waypoint 9 (tag 4, 4 point(s)), starting point 0, arrival event value 262144 |
| 29 | `Hajod_Fighter_2` | 1118 | Interactive | -43.95,0.00,-467.61 | 0,0,0 | group/role: FG_DISCIPLINE / 0; alias: jumbo; waypoint: Waypoint 0 (tag 15, 5 point(s)), starting point 0, arrival event value 983040 |
| 30 | `Hajod_Fighter_2` | 1119 | Interactive | 12.20,0.00,-466.03 | 0,0,0 | group/role: FG_DISCIPLINE / 0; alias: jumbo_1; waypoint: Waypoint 0 (tag 15, 5 point(s)), starting point 0, arrival event value 983040 |
| 31 | `Hajod_Fighter_2` | 1120 | Interactive | -50.48,0.00,-563.80 | 0,0,0 | group/role: FG_MONARCH / 0; alias: egg; waypoint: Waypoint 0 (tag 15, 5 point(s)), starting point 0, arrival event value 983040 |
| 32 | `Hajod_Fighter_2` | 1121 | Interactive | 14.81,0.00,-563.80 | 0,0,0 | group/role: FG_MONARCH / 0; alias: egg_1; waypoint: Waypoint 0 (tag 15, 5 point(s)), starting point 0, arrival event value 983040 |
| 33 | `Baronial_Shuttle` | 1385 | Interactive | 73.33,0.00,-404.50 | 0,0,0 | alias: Hajod_1; secondary groups: none, MANACLE; waypoint: Waypoint 0 (tag 15, 5 point(s)), starting point 0, arrival event value 983040 |
