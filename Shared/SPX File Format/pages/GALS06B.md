# Tachyon: The Fringe GALS06B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `GALS06B.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `(none)` |
| Region | 2 |
| Sector ID | 5 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 17 |
| Events | 27 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Drone_Attack`, `1: Drone_Contest`, `2: Wingman_Ramos` |
| Scripts | `TRISH.SCR`, `PLAYER.SCR`, `LAKIT.SCR` |
| Scenes | None |
| Labels | None |
| Aliases | `wing_man` |
| Groups | `LAKITA_CELENE`, `FG_CHAMAELEON`, `FG_EUDOXUS`, `FG_EURYDICE`, `FG_EURYALE`, `FG_ETATUS`, `FG_CHARA`, `FG_CENTAURS`, `FG_CHEIRON` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0
- Object spawn/action: Wingman_Ramos (object 0, id 15), subtype 8
- Gate state/action: param 2, subtype 3, param 0
- Play dialog: TRISH.SCR, line/variant 3
- Show/update HUD contact: contact/list 0, subtype 9, param 24

### Event 1

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 3 (join 1)
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Object spawn/action: Wingman_Ramos (object 0, id 15), subtype 5
- Show/update HUD contact: contact/list 0, subtype 1, param 203
- Hide/remove HUD contact: contact/list 0, subtype 9, param 24
- Show/update HUD contact: contact/list 0, subtype 9, param 25
- Group/spawn-list action: spawn list/group 203, subtype 0

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 25

**Action**

- Group/spawn-list action: spawn list/group 201, subtype 1, param 43
- Set runtime trigger variable: variable group 20, variable 0, subtype 1, value 0

### Event 3

**Trigger**

- Group/spawn-list event: subject 203, op 0, value 0 (join 1)
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 284, subtype 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 25
- Hide/remove HUD contact: contact/list 0, subtype 1, param 203
- Show/update HUD contact: contact/list 0, subtype 1, param 284

### Event 4

**Trigger**

- Group/spawn-list event: subject 284, op 0, value 0 (join 1)
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 285, subtype 0
- Show/update HUD contact: contact/list 0, subtype 1, param 285
- Hide/remove HUD contact: contact/list 0, subtype 1, param 284

### Event 5

**Trigger**

- Group/spawn-list event: subject 285, op 0, value 0 (join 1)
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 204, subtype 0
- Show/update HUD contact: contact/list 0, subtype 1, param 204
- Hide/remove HUD contact: contact/list 0, subtype 1, param 285

### Event 6

**Trigger**

- Group/spawn-list event: subject 204, op 0, value 0 (join 1)
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Set/add variable: variable group 21, variable 21, subtype 0, value 1
- Mission objective/state: param 131072, subtype 0, param 0
- Hide/remove HUD contact: contact/list 0, subtype 1, param 204
- Show/update HUD contact: contact/list 0, subtype 9, param 26

### Event 7

**Trigger**

- Group/spawn-list event: subject 201, op 0, value 0

**Action**

- Group/spawn-list action: spawn list/group 282, subtype 0

### Event 8

**Trigger**

- Group/spawn-list event: subject 282, op 0, value 0

**Action**

- Group/spawn-list action: spawn list/group 283, subtype 0
- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0

### Event 9

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 50

**Action**

- Object spawn/action: Drone_Contest (object 16, id 63), subtype 7

### Event 10

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 60

**Action**

- Object spawn/action: Drone_Contest (object 1, id 64), subtype 7

### Event 11

**Trigger**

- Group/spawn-list event: subject 283, op 0, value 0

**Action**

- Group/spawn-list action: spawn list/group 202, subtype 0
- Play dialog: PLAYER.SCR, line/variant 19

### Event 12

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 95

**Action**

- Object spawn/action: Drone_Attack (object 10, id 65), subtype 7

### Event 13

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 145

**Action**

- Object spawn/action: Drone_Attack (object 11, id 66), subtype 7

### Event 14

**Trigger**

- Object event: subject Wingman_Ramos (object 0, id 15), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 22, subtype 0, value 1
- Set/add variable: variable group 21, variable 25, subtype 0, value 1

### Event 15

**Trigger**

- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 10, param 0
- Set/add variable: variable group 14, variable 0, subtype 0, value 1
- Set/add variable: variable group 14, variable 405, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 11, param 21
- Hide/remove HUD contact: contact/list 0, subtype 9, param 24

### Event 16

**Trigger**

- Object event: subject Wingman_Ramos (object 0, id 15), op 0, value 0 (flags 2)

**Action**

- Play dialog: LAKIT.SCR, line/variant 1

### Event 17

**Trigger**

- Object event: subject Drone_Contest (object 8, id 61), op 2, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 122

### Event 18

**Trigger**

- Variable comparison: subject variable group 21, variable 24, op 1, value 1

**Action**

- Object spawn/action: Drone_Contest (object 8, id 61), subtype 19
- Object spawn/action: Drone_Contest (object 2, id 55), subtype 19
- Object spawn/action: Drone_Contest (object 3, id 56), subtype 19
- Object spawn/action: Drone_Contest (object 4, id 57), subtype 19
- Object spawn/action: Drone_Contest (object 5, id 58), subtype 19
- Object spawn/action: Drone_Contest (object 6, id 59), subtype 19
- Object spawn/action: Drone_Contest (object 7, id 60), subtype 19
- Object spawn/action: Drone_Contest (object 9, id 62), subtype 19

### Event 19

**Trigger**

- Variable comparison: subject variable group 21, variable 24, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Hide/remove HUD contact: contact/list 0, subtype 1, param 285
- Hide/remove HUD contact: contact/list 0, subtype 1, param 203
- Hide/remove HUD contact: contact/list 0, subtype 1, param 204
- Hide/remove HUD contact: contact/list 0, subtype 1, param 284

### Event 20

**Trigger**

- Variable comparison: subject variable group 21, variable 25, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 285, subtype 0
- Group/spawn-list action: spawn list/group 203, subtype 0
- Group/spawn-list action: spawn list/group 204, subtype 0
- Group/spawn-list action: spawn list/group 284, subtype 0
- Set/add variable: variable group 21, variable 24, subtype 0, value 1

### Event 21

**Trigger**

- Group/spawn-list event: subject 204, op 0, value 0

**Action**

- Group/spawn-list action: spawn list/group 201, subtype 0
- Group/spawn-list action: spawn list/group 283, subtype 0
- Group/spawn-list action: spawn list/group 202, subtype 0
- Group/spawn-list action: spawn list/group 282, subtype 0
- Set/add variable: variable group 21, variable 25, subtype 0, value 1

### Event 22

**Trigger**

- Variable comparison: subject variable group 21, variable 25, op 1, value 1

**Action**

- Object spawn/action: Drone_Contest (object 13, id 51), subtype 7
- Object spawn/action: Drone_Contest (object 12, id 52), subtype 7
- Object spawn/action: Drone_Contest (object 14, id 53), subtype 7
- Object spawn/action: Drone_Contest (object 15, id 54), subtype 7
- Object spawn/action: Drone_Attack (object 10, id 65), subtype 7
- Object spawn/action: Drone_Contest (object 16, id 63), subtype 7
- Object spawn/action: Drone_Contest (object 1, id 64), subtype 7
- Object spawn/action: Drone_Attack (object 11, id 66), subtype 7

### Event 23

**Trigger**

- Variable comparison: subject variable group 21, variable 25, op 1, value 1

**Action**

- Set runtime trigger variable: variable group 20, variable 12, subtype 0, value 0

### Event 24

**Trigger**

- Variable comparison: subject variable group 20, variable 12, op 1, value 15

**Action**

- Object spawn/action: Wingman_Ramos (object 0, id 15), subtype 2, param 1

### Event 25

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 170

**Action**

- Object spawn/action: Wingman_Ramos (object 0, id 15), subtype 2, param 1
- Set runtime trigger variable: variable group 20, variable 0, subtype 1, value 0

### Event 26

**Trigger**

- Object event: subject Wingman_Ramos (object 0, id 15), op 6, value 0

**Action**

- Set/add variable: variable group 21, variable 29, subtype 0, value 1

## Waypoints

### Waypoint 0

- Tag: `153`
- Members: `Wingman_Ramos (object 0, id 15, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-931.38, 0.00, 1029.97) | None |
| 1 | (-712.03, 0.00, 1091.40) | None |
| 2 | (-572.44, 0.00, 946.19) | None |
| 3 | (-567.45, 0.00, 594.32) | None |
| 4 | (-766.86, 0.00, 410.01) | None |
| 5 | (-911.44, 0.00, 616.67) | on arrival redirect to Waypoint 0 (tag 153), point 0 |

### Waypoint 1

- Tag: `152`
- Members: `Drone_Contest (object 2, id 55, starts at point 0)`, `Drone_Contest (object 3, id 56, starts at point 0)`, `Drone_Contest (object 4, id 57, starts at point 0)`, `Drone_Contest (object 5, id 58, starts at point 0)`, `Drone_Contest (object 6, id 59, starts at point 0)`, `Drone_Contest (object 7, id 60, starts at point 0)`, `Drone_Contest (object 8, id 61, starts at point 0)`, `Drone_Contest (object 9, id 62, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-40.86, 203.72, 557.74) | None |
| 1 | (-211.09, 147.05, 448.24) | None |
| 2 | (-197.47, 147.05, 260.96) | None |
| 3 | (-357.00, 147.05, 300.06) | None |
| 4 | (-456.70, 147.05, 110.16) | None |
| 5 | (-391.89, 147.05, -51.81) | None |
| 6 | (-227.38, 147.05, -96.49) | None |
| 7 | (-127.68, 147.05, 37.55) | None |

### Waypoint 2

- Tag: `151`
- Members: `Drone_Contest (object 1, id 64, starts at point 0)`, `Drone_Attack (object 10, id 65, starts at point 0)`, `Drone_Attack (object 11, id 66, starts at point 0)`, `Drone_Contest (object 12, id 52, starts at point 0)`, `Drone_Contest (object 13, id 51, starts at point 0)`, `Drone_Contest (object 14, id 53, starts at point 0)`, `Drone_Contest (object 15, id 54, starts at point 0)`, `Drone_Contest (object 16, id 63, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-172.77, 251.20, 1069.67) | None |
| 1 | (-377.16, 251.20, 1052.91) | None |
| 2 | (-482.71, 251.20, 873.46) | None |
| 3 | (-692.08, 251.20, 792.77) | None |
| 4 | (-841.64, 251.20, 867.88) | None |
| 5 | (-983.90, 251.20, 778.51) | None |
| 6 | (-976.24, 251.20, 555.11) | None |
| 7 | (-841.64, 251.20, 499.26) | None |
| 8 | (-707.04, 251.20, 610.96) | None |

## Spawn Lists

### Spawn List 0

- ID: `202`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Wingman_Ramos (object 0, id 15) | None |

### Spawn List 1

- ID: `201`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Wingman_Ramos (object 0, id 15) | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Wingman_Ramos` | 15 | Interactive | -807.83,-122.00,965.80 | 122,0,0 | alias: wing_man; secondary groups: none, LAKITA_CELENE; waypoint: Waypoint 0 (tag 153, 6 point(s)), starting point 0, arrival event value 10027008 |
| 1 | `Drone_Contest` | 64 | Interactive | 77.36,0.00,1305.35 | 370,0,0 | group/role: FG_CHAMAELEON / 0; waypoint: Waypoint 2 (tag 151, 9 point(s)), starting point 0, arrival event value 9895936 |
| 2 | `Drone_Contest` | 55 | Interactive | 307.03,185.95,899.03 | 397,0,0 | group/role: FG_EUDOXUS / 2; waypoint: Waypoint 1 (tag 152, 8 point(s)), starting point 0, arrival event value 9961472 |
| 3 | `Drone_Contest` | 56 | Interactive | 374.53,185.95,907.44 | 397,0,0 | group/role: FG_EUDOXUS / 3; waypoint: Waypoint 1 (tag 152, 8 point(s)), starting point 0, arrival event value 9961472 |
| 4 | `Drone_Contest` | 57 | Interactive | -65.14,0.00,624.73 | 397,0,0 | group/role: FG_EURYDICE / 0; waypoint: Waypoint 1 (tag 152, 8 point(s)), starting point 0, arrival event value 9961472 |
| 5 | `Drone_Contest` | 58 | Interactive | -140.14,0.00,616.33 | 397,0,0 | group/role: FG_EURYDICE / 0; waypoint: Waypoint 1 (tag 152, 8 point(s)), starting point 0, arrival event value 9961472 |
| 6 | `Drone_Contest` | 59 | Interactive | 39.86,0.00,540.71 | 361,0,0 | group/role: FG_EURYALE / 2; waypoint: Waypoint 1 (tag 152, 8 point(s)), starting point 0, arrival event value 9961472 |
| 7 | `Drone_Contest` | 60 | Interactive | 92.36,0.00,481.89 | 361,0,0 | group/role: FG_ETATUS / 4; waypoint: Waypoint 1 (tag 152, 8 point(s)), starting point 0, arrival event value 9961472 |
| 8 | `Drone_Contest` | 61 | Interactive | -5.14,0.00,490.29 | 361,0,0 | group/role: FG_EURYALE / 1; waypoint: Waypoint 1 (tag 152, 8 point(s)), starting point 0, arrival event value 9961472 |
| 9 | `Drone_Contest` | 62 | Interactive | 32.36,0.00,448.28 | 361,0,0 | group/role: FG_ETATUS / 3; waypoint: Waypoint 1 (tag 152, 8 point(s)), starting point 0, arrival event value 9961472 |
| 10 | `Drone_Attack` | 65 | Interactive | -42.64,0.00,1347.36 | 370,0,0 | group/role: FG_CHARA / 0; waypoint: Waypoint 2 (tag 151, 9 point(s)), starting point 0, arrival event value 9895936 |
| 11 | `Drone_Attack` | 66 | Interactive | 17.36,0.00,1389.37 | 370,0,0 | group/role: FG_CHARA / 0; waypoint: Waypoint 2 (tag 151, 9 point(s)), starting point 0, arrival event value 9895936 |
| 12 | `Drone_Contest` | 52 | Interactive | -87.64,0.00,1137.29 | 356,0,0 | group/role: FG_CENTAURS / 0; waypoint: Waypoint 2 (tag 151, 9 point(s)), starting point 0, arrival event value 9895936 |
| 13 | `Drone_Contest` | 51 | Interactive | -72.64,0.00,1212.92 | 356,0,0 | group/role: FG_CENTAURS / 0; waypoint: Waypoint 2 (tag 151, 9 point(s)), starting point 0, arrival event value 9895936 |
| 14 | `Drone_Contest` | 53 | Interactive | -147.64,0.00,1212.92 | 356,0,0 | group/role: FG_CHEIRON / 0; waypoint: Waypoint 2 (tag 151, 9 point(s)), starting point 0, arrival event value 9895936 |
| 15 | `Drone_Contest` | 54 | Interactive | -155.14,0.00,1137.29 | 356,0,0 | group/role: FG_CHEIRON / 0; waypoint: Waypoint 2 (tag 151, 9 point(s)), starting point 0, arrival event value 9895936 |
| 16 | `Drone_Contest` | 63 | Interactive | 17.36,0.00,1271.74 | 370,0,0 | group/role: FG_CHAMAELEON / 0; waypoint: Waypoint 2 (tag 151, 9 point(s)), starting point 0, arrival event value 9895936 |
