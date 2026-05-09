# Tachyon: The Fringe EARTH04B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH04B.SPX` |
| Sector | `QUAD_04` |
| Backdrop | `(none)` |
| Region | 0 |
| Sector ID | 3 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 13 |
| Events | 11 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Minetender`, `1: AGT_Mako`, `2: CMI_Dart`, `3: Drone_Worker` |
| Scripts | `MNCP.SCR`, `AGTF.SCR` |
| Scenes | None |
| Labels | `AGT Fighter` |
| Aliases | `danc_blowfish4`, `danc_blowfish3`, `danc_blowfish2`, `danc_blowfish1`, `danc_blowfish5`, `Jerome50` |
| Groups | `FG_BORA7`, `CONT_027`, `FG_AGT_RIVAL5`, `FG_DRAGON`, `FG_AGT1`, `BURKHART` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 0, op 1, value 1

**Action**

- Object spawn/action: Generic_Minetender (object 12, id 1321), subtype 3
- Set runtime trigger variable: variable group 20, variable 7, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 2, param 1321
- Mission objective/state: param 3, subtype 0, param 0
- Object spawn/action: Generic_Minetender (object 12, id 1321), subtype 14

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 7, op 1, value 5

**Action**

- Play dialog: MNCP.SCR, line/variant 1

### Event 2

**Trigger**

- Object event: subject CMI_Dart (object 3, id 251), op 2, value 0

**Action**

- Play dialog: AGTF.SCR, line/variant 22

### Event 3

**Trigger**

- Object event: subject CMI_Dart (object 4, id 252), op 2, value 0

**Action**

- Play dialog: AGTF.SCR, line/variant 25

### Event 4

**Trigger**

- Global enemy/object-count event: subject 0, op 0, value 0 (join 1)
- Object event: subject Generic_Minetender (object 12, id 1321), op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 8, subtype 0, value 0

### Event 5

**Trigger**

- Global enemy/object-count event: subject 0, op 0, value 0 (join 1)
- Object event: subject Generic_Minetender (object 12, id 1321), op 2, value 0

**Action**

- Set/add variable: variable group 12, variable 1, subtype 0, value 1
- Set/add variable: variable group 12, variable 5, subtype 0, value 2
- Set/add variable: variable group 21, variable 1, subtype 0, value 1
- Set/add variable: variable group 0, variable 5, subtype 0, value 1001
- Hide/remove HUD contact: contact/list 0, subtype 2, param 1321
- Show/update HUD contact: contact/list 0, subtype 12, param 30
- Object spawn/action: Generic_Minetender (object 12, id 1321), subtype 15

### Event 6

**Trigger**

- Object event: subject Generic_Minetender (object 12, id 1321), op 2, value 0

**Action**

- Set/add variable: variable group 12, variable 1, subtype 0, value 1
- Set/add variable: variable group 12, variable 5, subtype 0, value 1
- Mark/flash contact: contact/list 0, subtype 2, param 1321
- Show/update HUD contact: contact/list 0, subtype 11, param 31

### Event 7

**Trigger**

- Object event: subject Generic_Minetender (object 12, id 1321), op 9, value 0

**Action**

- Group/spawn-list action: spawn list/group 14, subtype 0
- Group/spawn-list action: spawn list/group 32, subtype 0
- Show/update HUD contact: contact/list 0, subtype 1, param 32
- Show/update HUD contact: contact/list 0, subtype 1, param 14

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 8, op 1, value 2

**Action**

- Play dialog: MNCP.SCR, line/variant 2
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 9

**Trigger**

- Object event: subject Generic_Minetender (object 12, id 1321), op 2, value 0

**Action**

- Play dialog: AGTF.SCR, line/variant 6
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Hide/remove HUD contact: contact/list 0, subtype 1, param 32
- Hide/remove HUD contact: contact/list 0, subtype 1, param 14

### Event 10

**Trigger**

- Object arrival: Generic_Minetender (object 12, id 1321) reached Waypoint 1 (tag 1), point 2 (raw value 65538)
- Variable comparison: subject variable group 12, variable 5, op 1, value 2
- Variable comparison: subject variable group 20, variable 8, op 2, value 5

**Action**

- Group/spawn-list action: spawn list/group 25, subtype 1, param 1321
- Play dialog: MNCP.SCR, line/variant 11
- Object spawn/action: Generic_Minetender (object 12, id 1321), subtype 6

## Waypoints

### Waypoint 0

- Tag: `2`
- Members: `Drone_Worker (object 0, id 1298, starts at point 0)`, `Drone_Worker (object 1, id 1297, starts at point 0)`, `Drone_Worker (object 2, id 1296, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-116.79, 0.00, 600.41) | None |
| 1 | (-1478.00, -546.93, 790.08) | None |
| 2 | (-1481.09, -576.00, 841.69) | None |
| 3 | (-1502.54, -517.00, 861.52) | None |
| 4 | (-1564.69, -541.00, 822.52) | None |
| 5 | (-1562.07, -499.00, 733.63) | on arrival redirect to Waypoint 0 (tag 2), point 0 |

### Waypoint 1

- Tag: `1`
- Members: `Generic_Minetender (object 12, id 1321, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (522.22, 0.00, 1328.74) | None |
| 1 | (175.16, 0.00, 915.82) | None |
| 2 | (-161.55, 0.00, 708.75) | on arrival activate current object (raw param -1 ignored); listened by Event 10 for Generic_Minetender (object 12, id 1321) |

## Spawn Lists

### Spawn List 0

- ID: `0`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 1

- ID: `32`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Generic_Minetender (object 12, id 1321) | None |

### Spawn List 2

- ID: `14`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Generic_Minetender (object 12, id 1321) | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Drone_Worker` | 1298 | Interactive | -92.68,0.00,605.88 | 384,0,0 | group/role: FG_BORA7 / 0; secondary groups: CONT_027, none; waypoint: Waypoint 0 (tag 2, 6 point(s)), starting point 0, arrival event value 131072 |
| 1 | `Drone_Worker` | 1297 | Interactive | -92.61,0.00,601.62 | 384,0,0 | group/role: FG_BORA7 / 0; secondary groups: CONT_027, none; waypoint: Waypoint 0 (tag 2, 6 point(s)), starting point 0, arrival event value 131072 |
| 2 | `Drone_Worker` | 1296 | Interactive | -92.49,0.00,597.89 | 384,0,0 | group/role: FG_BORA7 / 0; secondary groups: CONT_027, none; waypoint: Waypoint 0 (tag 2, 6 point(s)), starting point 0, arrival event value 131072 |
| 3 | `CMI_Dart` | 251 | Interactive | 115.41,0.00,2077.74 | 151,0,0 | group/role: FG_AGT_RIVAL5 / 0 |
| 4 | `CMI_Dart` | 252 | Interactive | -0.64,0.00,2230.93 | 151,0,0 | group/role: FG_AGT_RIVAL5 / 0 |
| 5 | `CMI_Dart` | 253 | Interactive | -417.44,0.00,2132.14 | 151,0,0 | group/role: FG_DRAGON / 0 |
| 6 | `CMI_Dart` | 1017 | Interactive | -576.11,0.00,2235.54 | 152,0,0 | group/role: FG_DRAGON / 0 |
| 7 | `AGT_Mako` | 256 | Interactive | 1149.19,-55.32,2072.21 | 358,0,0 | group/role: FG_AGT1 / 0; alias: danc_blowfish4 |
| 8 | `AGT_Mako` | 255 | Interactive | 1238.04,-55.32,2134.36 | 357,0,0 | group/role: FG_AGT1 / 0; alias: danc_blowfish3 |
| 9 | `AGT_Mako` | 250 | Interactive | 1371.48,-55.32,2134.50 | 358,0,0 | group/role: FG_AGT1 / 0; alias: danc_blowfish2 |
| 10 | `AGT_Mako` | 249 | Interactive | 1379.90,-55.32,1997.64 | 358,0,0 | label: AGT Fighter; group/role: FG_AGT1 / 0; alias: danc_blowfish1 |
| 11 | `AGT_Mako` | 254 | Interactive | 1246.63,-55.32,1997.63 | 360,0,0 | group/role: FG_AGT1 / 0; alias: danc_blowfish5 |
| 12 | `Generic_Minetender` | 1321 | Interactive | 911.85,0.00,2062.17 | 299,0,0 | alias: Jerome50; secondary groups: none, BURKHART; waypoint: Waypoint 1 (tag 1, 3 point(s)), starting point 0, arrival event value 65536 |
