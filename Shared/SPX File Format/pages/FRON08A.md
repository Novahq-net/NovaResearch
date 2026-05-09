# Tachyon: The Fringe FRON08A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON08A.SPX` |
| Sector | `QUAD_08` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 7 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 7 |
| Events | 20 |
| Waypoints | 6 |
| Child Sectors | 0 |
| Scripts | 4 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Malkar_Sistine_Chapel`, `1: Hajod_Fighter_2`, `2: Baronial_Shuttle`, `3: Hajod_Fighter_1` |
| Scripts | `PLAYER.SCR`, `HSLAV.SCR`, `PODDS.SCR`, `PODPN.SCR` |
| Scenes | None |
| Labels | `bfne_03`, `bfne_01`, `HSLAV`, `BFGE_01`, `CHAPEL` |
| Aliases | `Jerome01`, `Jerome02`, `Jerome03`, `Jerome04`, `Jerome05`, `Jerome06`, `bc05_2`, `bc05_1`, `bc05_4`, `bc05_5`, `BC05_Sistine_Chapel` |
| Groups | `FG_DESPOT`, `OPPRESSOR`, `OBEDIENCE`, `FG_PUNISHER`, `SISTINE_CHAPEL` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 13
- Show/update HUD contact: contact/list 0, subtype 9, param 14
- Object spawn/action: id 996, subtype 8, param 4
- Play scene: unknown index 0, param 0
- Play dialog: PLAYER.SCR, line/variant 58

### Event 1

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 58

**Action**

- Set runtime trigger variable: variable group 20, variable 20, subtype 0, value 0

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 20, op 1, value 2

**Action**

- Play dialog: PLAYER.SCR, line/variant 60

### Event 3

**Trigger**

- Object event: subject Baronial_Shuttle (object 2, id 1029), op 6, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 13
- Object spawn/action: Baronial_Shuttle (object 2, id 1029), subtype 8, param 4

### Event 4

**Trigger**

- Object event: subject Baronial_Shuttle (object 3, id 1030), op 6, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 14
- Object spawn/action: Baronial_Shuttle (object 3, id 1030), subtype 8, param 4

### Event 5

**Trigger**

- Object event: subject Baronial_Shuttle (object 2, id 1029), op 6, value 0
- Object event: subject Baronial_Shuttle (object 3, id 1030), op 6, value 0

**Action**

- Group/spawn-list action: spawn list/group 87, subtype 0
- Group/spawn-list action: spawn list/group 86, subtype 0

### Event 6

**Trigger**

- Object event: subject Baronial_Shuttle (object 2, id 1029), op 6, value 0
- Object event: subject Baronial_Shuttle (object 3, id 1030), op 6, value 0
- Variable comparison: subject variable group 21, variable 21, op 1, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 21
- Show/update HUD contact: contact/list 0, subtype 9, param 20
- Play dialog: HSLAV.SCR, line/variant 2

### Event 7

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 100 (extra 1, 1096; flags 3)
- Object event: subject Baronial_Shuttle (object 2, id 1029), op 6, value 0
- Object event: subject Baronial_Shuttle (object 3, id 1030), op 6, value 0
- Variable comparison: subject variable group 21, variable 21, op 1, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 184
- Show/update HUD contact: contact/list 0, subtype 9, param 15
- Set/add variable: variable group 21, variable 20, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 20
- Hide/remove HUD contact: contact/list 0, subtype 9, param 21

### Event 8

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Variable comparison: subject variable group 21, variable 21, op 1, value 0

**Action**

- Object spawn/action: Malkar_Sistine_Chapel (object 6, id 1096), subtype 13, param 720896

### Event 9

**Trigger**

- Object event: subject Malkar_Sistine_Chapel (object 6, id 1096), op 8, value 0

**Action**

- Set/add variable: variable group 21, variable 2, subtype 0, value 1

### Event 10

**Trigger**

- Object event: subject Baronial_Shuttle (object 2, id 1029), op 0, value 0 (join 2; flags 2)
- Object event: subject Baronial_Shuttle (object 3, id 1030), op 0, value 0 (flags 2)

**Action**

- Play dialog: HSLAV.SCR, line/variant 1

### Event 11

**Trigger**

- Object event: subject Hajod_Fighter_2 (object 5, id 754), op 4, value 100

**Action**

- Play dialog: PODDS.SCR, line/variant 1

### Event 12

**Trigger**

- Group/spawn-list event: subject 87, op 1, value 30

**Action**

- Play dialog: PODPN.SCR, line/variant 1

### Event 13

**Trigger**

- Object event: subject Malkar_Sistine_Chapel (object 6, id 1096), op 2, value 0 (join 2)

**Action**

- Set/add variable: variable group 16, variable 404, subtype 0, value 0
- Set/add variable: variable group 16, variable 405, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 15
- Play dialog: PLAYER.SCR, line/variant 68
- Set/add variable: variable group 21, variable 21, subtype 0, value 1
- Set/add variable: variable group 21, variable 20, subtype 0, value 0

### Event 14

**Trigger**

- Object event: subject Baronial_Shuttle (object 2, id 1029), op 2, value 0 (join 2)
- Object event: subject Baronial_Shuttle (object 3, id 1030), op 2, value 0 (join 2)

**Action**

- Set/add variable: variable group 16, variable 404, subtype 0, value 1
- Set/add variable: variable group 16, variable 405, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 15
- Set/add variable: variable group 21, variable 21, subtype 0, value 1
- Set/add variable: variable group 21, variable 20, subtype 0, value 0

### Event 15

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 37
- Show/update HUD contact: contact/list 0, subtype 11, param 38
- Object spawn/action: Malkar_Sistine_Chapel (object 6, id 1096), subtype 13, param 65536
- Set runtime trigger variable: variable group 20, variable 19, subtype 1, value 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 13
- Hide/remove HUD contact: contact/list 0, subtype 9, param 14
- Hide/remove HUD contact: contact/list 0, subtype 9, param 20
- Hide/remove HUD contact: contact/list 0, subtype 9, param 21

### Event 16

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 1
- Variable comparison: subject variable group 21, variable 0, op 1, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 17

**Trigger**

- Variable comparison: subject variable group 21, variable 24, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 86, subtype 3, param 1
- Group/spawn-list action: spawn list/group 87, subtype 3, param 1

### Event 18

**Trigger**

- Object event: subject Malkar_Sistine_Chapel (object 6, id 1096), op 8, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 15
- Mission objective/state: param 262144, subtype 0, param 0

### Event 19

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 60

**Action**

- Object spawn/action: id 996, subtype 8, param 2

## Waypoints

### Waypoint 0

- Tag: `11`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1240.97, 494.94, 600.78) | None |
| 1 | (-1474.56, 494.94, 691.08) | on arrival action 1, param -1 |

### Waypoint 1

- Tag: `12`
- Members: `Baronial_Shuttle (object 3, id 1030, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1183.80, 570.31, -324.68) | None |
| 1 | (-1280.22, 571.75, -765.08) | None |
| 2 | (-732.23, 557.17, -1659.31) | None |
| 3 | (-3.63, 568.83, -2433.14) | None |
| 4 | (964.18, 549.55, -2173.24) | None |
| 5 | (1602.88, 567.06, -1570.63) | None |
| 6 | (2190.48, 569.75, 19.30) | None |
| 7 | (1492.89, 571.54, 822.17) | None |
| 8 | (-256.98, 581.06, 999.27) | on arrival redirect to Waypoint 1 (tag 12), point 0 |

### Waypoint 2

- Tag: `9`
- Members: `Baronial_Shuttle (object 2, id 1029, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-955.41, 403.09, -377.74) | None |
| 1 | (-735.44, 446.02, -1205.58) | None |
| 2 | (-249.02, 418.48, -1857.30) | None |
| 3 | (341.36, 423.31, -1970.66) | None |
| 4 | (1084.43, 424.79, -1751.58) | None |
| 5 | (1601.10, 437.50, -906.71) | None |
| 6 | (1810.65, 430.17, 13.92) | None |
| 7 | (1250.55, 367.04, 725.30) | None |
| 8 | (-238.23, 358.89, 798.87) | on arrival redirect to Waypoint 2 (tag 9), point 0 |

### Waypoint 3

- Tag: `3`
- Members: `Hajod_Fighter_2 (object 4, id 755, starts at point 0)`, `Hajod_Fighter_2 (object 5, id 754, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (341.66, 421.50, -2280.59) | None |
| 1 | (-644.96, 417.12, -1670.08) | None |
| 2 | (-1268.10, 473.27, 485.36) | None |
| 3 | (1082.93, 444.49, 690.36) | None |
| 4 | (-773.51, 445.29, 721.11) | None |
| 5 | (-1544.59, 445.29, 747.50) | None |
| 6 | (-1391.63, 448.26, 12.43) | on arrival redirect to Waypoint 3 (tag 3), point 4 |

### Waypoint 4

- Tag: `2`
- Members: `Hajod_Fighter_1 (object 0, id 751, starts at point 0)`, `Hajod_Fighter_1 (object 1, id 750, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1109.85, 436.28, 660.80) | None |
| 1 | (-1212.25, 471.37, 376.85) | None |
| 2 | (-581.72, 465.36, -2007.45) | None |
| 3 | (1284.26, 411.09, -1796.59) | None |
| 4 | (1667.23, 399.16, 585.72) | None |
| 5 | (-587.16, 404.63, 795.41) | None |
| 6 | (-1571.01, 404.63, 644.62) | None |
| 7 | (-1348.52, 404.63, -146.98) | on arrival redirect to Waypoint 4 (tag 2), point 5 |

### Waypoint 5

- Tag: `1`
- Members: `Malkar_Sistine_Chapel (object 6, id 1096, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1184.03, 504.35, -686.59) | None |
| 1 | (-587.65, 516.60, -1630.33) | None |
| 2 | (21.07, 509.82, -2230.46) | None |
| 3 | (879.95, 509.06, -2009.06) | None |
| 4 | (1473.31, 500.78, -1489.51) | None |
| 5 | (2006.48, 499.12, 40.33) | None |
| 6 | (1352.74, 500.21, 764.49) | None |
| 7 | (-249.83, 504.13, 890.15) | on arrival redirect to Waypoint 5 (tag 1), point 0 |

## Spawn Lists

### Spawn List 0

- ID: `86`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | Baronial_Shuttle (object 2, id 1029) | None |
| 1 | 6 | Baronial_Shuttle (object 3, id 1030) | None |
| 2 | 6 | Malkar_Sistine_Chapel (object 6, id 1096) | None |
| 3 | 6 | id 996 | None |
| 4 | 0 | none | None |

### Spawn List 1

- ID: `87`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | Baronial_Shuttle (object 2, id 1029) | None |
| 1 | 6 | Baronial_Shuttle (object 3, id 1030) | None |
| 2 | 6 | Malkar_Sistine_Chapel (object 6, id 1096) | None |
| 3 | 6 | id 996 | None |
| 4 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hajod_Fighter_1` | 751 | Interactive | 894.77,26.81,335.50 | 64,0,0 | group/role: FG_DESPOT / 1; alias: bc05_2; waypoint: Waypoint 4 (tag 2, 8 point(s)), starting point 0, arrival event value 131072 |
| 1 | `Hajod_Fighter_1` | 750 | Interactive | 851.61,26.81,369.69 | 64,0,0 | group/role: FG_DESPOT / 0; alias: bc05_1; waypoint: Waypoint 4 (tag 2, 8 point(s)), starting point 0, arrival event value 131072 |
| 2 | `Baronial_Shuttle` | 1029 | Interactive | -1069.48,389.62,369.88 | 282,0,0 | label: HSLAV; secondary groups: none, OPPRESSOR; waypoint: Waypoint 2 (tag 9, 9 point(s)), starting point 0, arrival event value 589824 |
| 3 | `Baronial_Shuttle` | 1030 | Interactive | -905.29,573.33,-104.14 | 282,0,0 | secondary groups: none, OBEDIENCE; waypoint: Waypoint 1 (tag 12, 9 point(s)), starting point 0, arrival event value 786432 |
| 4 | `Hajod_Fighter_2` | 755 | Interactive | 62.61,36.20,-1559.63 | 317,0,0 | group/role: FG_PUNISHER / 0; alias: bc05_4; waypoint: Waypoint 3 (tag 3, 7 point(s)), starting point 0, arrival event value 196608 |
| 5 | `Hajod_Fighter_2` | 754 | Interactive | 87.90,36.20,-1583.11 | 317,0,0 | group/role: FG_PUNISHER / 1; alias: bc05_5; waypoint: Waypoint 3 (tag 3, 7 point(s)), starting point 0, arrival event value 196608 |
| 6 | `Malkar_Sistine_Chapel` | 1096 | Interactive | -960.16,499.93,105.90 | 282,0,0 | label: CHAPEL; alias: BC05_Sistine_Chapel; secondary groups: none, SISTINE_CHAPEL; waypoint: Waypoint 5 (tag 1, 8 point(s)), starting point 0, arrival event value 65536 |
