# Tachyon: The Fringe EARTH02A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH02A.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `(none)` |
| Region | 0 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 6 |
| Entities | 20 |
| Events | 31 |
| Waypoints | 4 |
| Child Sectors | 0 |
| Scripts | 6 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Minetender`, `1: GalSpan_Heavy_Freighter`, `2: Luxury_Liner`, `3: Generic_Light_Freighter`, `4: AGT_Mako`, `5: CMI_Dart` |
| Scripts | `MNCP.SCR`, `MRVS.SCR`, `3MRV.SCR`, `ARIV.SCR`, `AGTF.SCR`, `CAPA.SCR` |
| Scenes | None |
| Labels | `bfnf_03`, `ariv`, `AGT FIGHTER`, `CAPB`, `CAPA`, `ofrt` |
| Aliases | `danc_blowfish1`, `danc_blowfish2`, `danc_blowfish5`, `danc_blowfish3`, `danc_blowfish4`, `Jerome50` |
| Groups | `FG_AGT_RIVAL1`, `FG_AGT_RIVAL3`, `FG_AGT_RIVAL2`, `FG_AGT_RIVAL4`, `FG_GALSPAN4`, `FG_AGT1`, `CONT_009`, `KILIMANJARO`, `CONT_033`, `CONT_012`, `BURKHART` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0
- Play scene: unknown index 0, param 0
- Show/update HUD contact: contact/list 0, subtype 6, param 1465
- Object spawn/action: Generic_Minetender (object 19, id 1465), subtype 14

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 18

**Action**

- Play dialog: MNCP.SCR, line/variant 3
- Object spawn/action: Generic_Minetender (object 19, id 1465), subtype 5

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 30

**Action**

- Group/spawn-list action: spawn list/group 10, subtype 1, param 2
- Play dialog: MRVS.SCR, line/variant 8
- Show/update HUD contact: contact/list 0, subtype 2, param 1465
- Hide/remove HUD contact: contact/list 0, subtype 6, param 1465

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 50

**Action**

- Group/spawn-list action: spawn list/group 12, subtype 1, param 1

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 60

**Action**

- Group/spawn-list action: spawn list/group 11, subtype 1, param 2
- Play dialog: MRVS.SCR, line/variant 1

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 60

**Action**

- Group/spawn-list action: spawn list/group 0, subtype 1, param 1309
- Play dialog: 3MRV.SCR, line/variant 27

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 80

**Action**

- Group/spawn-list action: spawn list/group 13, subtype 1, param 2

### Event 7

**Trigger**

- Global enemy/object-count event: subject 0, op 0, value 0

**Action**

- Object spawn/action: AGT_Mako (object 11, id 270), subtype 2, param 2
- Object spawn/action: AGT_Mako (object 12, id 271), subtype 2, param 2
- Object spawn/action: AGT_Mako (object 14, id 580), subtype 2, param 2
- Object spawn/action: AGT_Mako (object 15, id 581), subtype 2, param 2
- Object spawn/action: AGT_Mako (object 13, id 582), subtype 2, param 2

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 5

**Action**

- Play dialog: MRVS.SCR, line/variant 6

### Event 9

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 12

**Action**

- Play dialog: MRVS.SCR, line/variant 13

### Event 10

**Trigger**

- Object event: subject Generic_Minetender (object 19, id 1465), op 3, value 90

**Action**

- Play dialog: ARIV.SCR, line/variant 3

### Event 11

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 55

**Action**

- Play dialog: MRVS.SCR, line/variant 0

### Event 12

**Trigger**

- Object event: subject Generic_Minetender (object 19, id 1465), op 4, value 50

**Action**

- Play dialog: MNCP.SCR, line/variant 5

### Event 13

**Trigger**

- Object event: subject Generic_Minetender (object 19, id 1465), op 4, value 100

**Action**

- Play dialog: MNCP.SCR, line/variant 6

### Event 14

**Trigger**

- Object event: subject Generic_Minetender (object 19, id 1465), op 3, value 50

**Action**

- Play dialog: MNCP.SCR, line/variant 7

### Event 15

**Trigger**

- Object event: subject Generic_Minetender (object 19, id 1465), op 2, value 0

**Action**

- Play dialog: MRVS.SCR, line/variant 4

### Event 16

**Trigger**

- Object event: subject CMI_Dart (object 0, id 264), op 4, value 100

**Action**

- Play dialog: ARIV.SCR, line/variant 6

### Event 17

**Trigger**

- Object event: subject Generic_Minetender (object 19, id 1465), op 8, value 0
- Global enemy/object-count event: subject 0, op 0, value 0 (join 1)
- Variable comparison: subject variable group 20, variable 30, op 1, value 1

**Action**

- Play dialog: AGTF.SCR, line/variant 0

### Event 18

**Trigger**

- Object event: subject Generic_Minetender (object 19, id 1465), op 2, value 0

**Action**

- Set/add variable: variable group 12, variable 1, subtype 0, value 1
- Set/add variable: variable group 12, variable 5, subtype 0, value 1
- Mark/flash contact: contact/list 0, subtype 2, param 1465
- Mission objective/state: param 2, subtype 0, param 0
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 31

### Event 19

**Trigger**

- Object event: subject CMI_Dart (object 4, id 589), op 2, value 0

**Action**

- Play dialog: AGTF.SCR, line/variant 8

### Event 20

**Trigger**

- Object event: subject CMI_Dart (object 5, id 268), op 2, value 0

**Action**

- Play dialog: AGTF.SCR, line/variant 9

### Event 21

**Trigger**

- Object event: subject Generic_Minetender (object 19, id 1465), op 8, value 0

**Action**

- Set/add variable: variable group 21, variable 0, subtype 0, value 1

### Event 22

**Trigger**

- Variable comparison: subject variable group 0, variable 5, op 1, value 1001
- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)

**Action**

- Set runtime trigger variable: variable group 20, variable 31, subtype 0, value 0
- Object spawn/action: GalSpan_Heavy_Freighter (object 18, id 1424), subtype 0
- Object spawn/action: Generic_Light_Freighter (object 16, id 811), subtype 0

### Event 23

**Trigger**

- Variable comparison: subject variable group 20, variable 31, op 1, value 8

**Action**

- Group/spawn-list action: spawn list/group 36, subtype 0

### Event 24

**Trigger**

- Variable comparison: subject variable group 20, variable 31, op 1, value 34

**Action**

- Object spawn/action: Generic_Light_Freighter (object 16, id 811), subtype 5
- Play dialog: 3MRV.SCR, line/variant 1

### Event 25

**Trigger**

- Variable comparison: subject variable group 20, variable 31, op 1, value 15

**Action**

- Object spawn/action: Luxury_Liner (object 17, id 864), subtype 3

### Event 26

**Trigger**

- Object arrival: Generic_Minetender (object 19, id 1465) reached Waypoint 3 (tag 1), point 0 (raw value 65536)

**Action**

- Play dialog: MNCP.SCR, line/variant 10

### Event 27

**Trigger**

- Object event: subject Generic_Minetender (object 19, id 1465), op 8, value 0 (join 1)
- Global enemy/object-count event: subject 0, op 0, value 0

**Action**

- Play dialog: AGTF.SCR, line/variant 1
- Set/add variable: variable group 20, variable 30, subtype 0, value 1

### Event 28

**Trigger**

- Variable comparison: subject variable group 20, variable 31, op 1, value 16

**Action**

- Play dialog: CAPA.SCR, line/variant 0

### Event 29

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 25

**Action**

- Set/add variable: variable group 12, variable 5, subtype 0, value 0

### Event 30

**Trigger**

- Object event: subject Generic_Minetender (object 19, id 1465), op 8, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 2, param 1465
- Mission objective/state: param 3, subtype 0, param 0

## Waypoints

### Waypoint 0

- Tag: `11`
- Members: `Luxury_Liner (object 17, id 864, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-168.05, 0.00, 522.38) | None |
| 1 | (-170.80, -304.00, -446.46) | None |
| 2 | (-2456.20, -517.00, -449.90) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 1

- Tag: `10`
- Members: `Generic_Light_Freighter (object 16, id 811, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-271.06, 100.00, -1702.96) | None |
| 1 | (-271.20, -100.00, -1238.34) | None |
| 2 | (-36.19, -200.00, -1239.19) | on arrival action 1, param -1 |

### Waypoint 2

- Tag: `9`
- Members: `AGT_Mako (object 8, id 780, starts at point 0)`, `AGT_Mako (object 9, id 782, starts at point 0)`, `AGT_Mako (object 10, id 781, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (981.21, -294.27, -1311.39) | None |
| 1 | (816.16, -294.27, -865.72) | None |
| 2 | (496.75, -126.27, -573.86) | None |
| 3 | (76.56, 0.00, -443.39) | None |
| 4 | (-779.69, 0.00, -445.75) | on arrival redirect to Waypoint 2 (tag 9), point 3 |

### Waypoint 3

- Tag: `1`
- Members: `GalSpan_Heavy_Freighter (object 18, id 1424, starts at point 0)`, `Generic_Minetender (object 19, id 1465, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-983.37, 86.00, -1513.57) | None; listened by Event 26 for Generic_Minetender (object 19, id 1465) |
| 1 | (-635.07, 0.00, 500.78) | None |
| 2 | (-386.26, 0.00, 1266.33) | on arrival action 1, param -1 |

## Spawn Lists

### Spawn List 0

- ID: `10`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Generic_Minetender (object 19, id 1465) | None |

### Spawn List 1

- ID: `11`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Generic_Minetender (object 19, id 1465) | None |

### Spawn List 2

- ID: `12`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Generic_Minetender (object 19, id 1465) | None |

### Spawn List 3

- ID: `13`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | Generic_Minetender (object 19, id 1465) | None |

### Spawn List 4

- ID: `0`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 5

- ID: `36`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `CMI_Dart` | 264 | Interactive | -1242.16,0.00,297.96 | 255,0,0 | label: ariv; group/role: FG_AGT_RIVAL1 / 0 |
| 1 | `CMI_Dart` | 1471 | Interactive | -1359.90,0.00,298.82 | 255,0,0 | label: ariv; group/role: FG_AGT_RIVAL1 / 0 |
| 2 | `CMI_Dart` | 588 | Interactive | -799.55,0.00,167.55 | 255,0,0 | group/role: FG_AGT_RIVAL3 / 2 |
| 3 | `CMI_Dart` | 584 | Interactive | -545.86,0.00,213.23 | 292,0,0 | group/role: FG_AGT_RIVAL2 / 0 |
| 4 | `CMI_Dart` | 589 | Interactive | -921.62,0.00,41.67 | 255,0,0 | group/role: FG_AGT_RIVAL3 / 0 |
| 5 | `CMI_Dart` | 268 | Interactive | -528.91,0.00,416.84 | 292,0,0 | group/role: FG_AGT_RIVAL2 / 1 |
| 6 | `CMI_Dart` | 272 | Interactive | -194.43,0.00,334.40 | 304,0,0 | group/role: FG_AGT_RIVAL4 / 0 |
| 7 | `CMI_Dart` | 273 | Interactive | -128.54,0.00,231.30 | 304,0,0 | group/role: FG_AGT_RIVAL4 / 0 |
| 8 | `AGT_Mako` | 780 | Interactive | 980.04,-294.27,-1461.17 | 0,0,0 | group/role: FG_GALSPAN4 / 0; waypoint: Waypoint 2 (tag 9, 5 point(s)), starting point 0, arrival event value 589824 |
| 9 | `AGT_Mako` | 782 | Interactive | 1002.90,-294.27,-1513.88 | 0,0,0 | group/role: FG_GALSPAN4 / 0; waypoint: Waypoint 2 (tag 9, 5 point(s)), starting point 0, arrival event value 589824 |
| 10 | `AGT_Mako` | 781 | Interactive | 954.22,-294.27,-1509.68 | 0,0,0 | group/role: FG_GALSPAN4 / 0; waypoint: Waypoint 2 (tag 9, 5 point(s)), starting point 0, arrival event value 589824 |
| 11 | `AGT_Mako` | 270 | Interactive | -193.99,0.00,-1421.15 | 0,0,0 | label: AGT FIGHTER; group/role: FG_AGT1 / 0; alias: danc_blowfish1 |
| 12 | `AGT_Mako` | 271 | Interactive | -70.76,0.00,-1608.79 | 0,0,0 | group/role: FG_AGT1 / 0; alias: danc_blowfish2 |
| 13 | `AGT_Mako` | 582 | Interactive | -63.41,0.00,-1801.08 | 0,0,0 | group/role: FG_AGT1 / 0; alias: danc_blowfish5 |
| 14 | `AGT_Mako` | 580 | Interactive | -319.01,0.00,-1609.48 | 0,0,0 | group/role: FG_AGT1 / 0; alias: danc_blowfish3 |
| 15 | `AGT_Mako` | 581 | Interactive | -319.01,0.00,-1803.36 | 0,0,0 | group/role: FG_AGT1 / 0; alias: danc_blowfish4 |
| 16 | `Generic_Light_Freighter` | 811 | Interactive | -272.52,100.00,-1898.89 | 0,0,0 | label: CAPB; secondary groups: CONT_009, none; waypoint: Waypoint 1 (tag 10, 3 point(s)), starting point 0, arrival event value 655360 |
| 17 | `Luxury_Liner` | 864 | Interactive | -176.82,0.00,1100.74 | 256,0,0 | label: CAPA; secondary groups: CONT_033, KILIMANJARO; waypoint: Waypoint 0 (tag 11, 3 point(s)), starting point 0, arrival event value 720896 |
| 18 | `GalSpan_Heavy_Freighter` | 1424 | Interactive | -2045.90,77.36,-2252.32 | 0,0,0 | secondary groups: CONT_012, none; waypoint: Waypoint 3 (tag 1, 3 point(s)), starting point 0, arrival event value 65536 |
| 19 | `Generic_Minetender` | 1465 | Interactive | -982.69,84.15,-2152.79 | 0,0,0 | alias: Jerome50; secondary groups: none, BURKHART; waypoint: Waypoint 3 (tag 1, 3 point(s)), starting point 0, arrival event value 65536 |
