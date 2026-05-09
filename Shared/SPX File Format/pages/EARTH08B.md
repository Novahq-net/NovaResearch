# Tachyon: The Fringe EARTH08B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH08B.SPX` |
| Sector | `QUAD_08` |
| Backdrop | `(none)` |
| Region | 0 |
| Sector ID | 7 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 16 |
| Events | 21 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Training_Combat_Beacon`, `1: Drone_Worker` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | None |
| Aliases | None |
| Groups | `FG_ROOKIE`, `FG_VETERAN`, `FG_ACE`, `FG_ELITE`, `CONT_055`, `CONT_056`, `CONT_057`, `CONT_058` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 32
- Object spawn/action: Training_Combat_Beacon (object 8, id 97), subtype 14

### Event 1

**Trigger**

- Object event: subject Training_Combat_Beacon (object 8, id 97), op 2, value 0 (join 2)
- Object event: subject Training_Combat_Beacon (object 9, id 98), op 2, value 0 (join 2)
- Object event: subject Training_Combat_Beacon (object 10, id 99), op 2, value 0 (join 2)
- Object event: subject Training_Combat_Beacon (object 11, id 100), op 2, value 0 (join 2)

**Action**

- Object spawn/action: Training_Combat_Beacon (object 8, id 97), subtype 15
- Hide/remove HUD contact: contact/list 0, subtype 9, param 32

### Event 2

**Trigger**

- Object event: subject Training_Combat_Beacon (object 8, id 97), op 0, value 0 (flags 3)
- Variable comparison: subject variable group 21, variable 29, op 1, value 0

**Action**

- Object spawn/action: Training_Combat_Beacon (object 8, id 97), subtype 7
- Group/spawn-list action: spawn list/group 268, subtype 0
- Hide/remove HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 21, variable 29, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 9, param 25
- Show/update HUD contact: contact/list 0, subtype 9, param 22
- Show/update HUD contact: contact/list 0, subtype 9, param 23
- Show/update HUD contact: contact/list 0, subtype 1, param 268

### Event 3

**Trigger**

- Object event: subject Training_Combat_Beacon (object 9, id 98), op 0, value 0 (flags 3)
- Variable comparison: subject variable group 21, variable 29, op 1, value 0

**Action**

- Object spawn/action: Training_Combat_Beacon (object 9, id 98), subtype 7
- Group/spawn-list action: spawn list/group 269, subtype 0
- Hide/remove HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 21, variable 29, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 9, param 25
- Show/update HUD contact: contact/list 0, subtype 9, param 22
- Show/update HUD contact: contact/list 0, subtype 9, param 23
- Show/update HUD contact: contact/list 0, subtype 1, param 269

### Event 4

**Trigger**

- Object event: subject Training_Combat_Beacon (object 10, id 99), op 0, value 0 (flags 3)
- Variable comparison: subject variable group 21, variable 29, op 1, value 0

**Action**

- Object spawn/action: Training_Combat_Beacon (object 10, id 99), subtype 7
- Group/spawn-list action: spawn list/group 270, subtype 0
- Hide/remove HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 21, variable 29, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 9, param 25
- Show/update HUD contact: contact/list 0, subtype 9, param 22
- Show/update HUD contact: contact/list 0, subtype 9, param 23
- Show/update HUD contact: contact/list 0, subtype 1, param 270

### Event 5

**Trigger**

- Object event: subject Training_Combat_Beacon (object 11, id 100), op 0, value 0 (flags 3)
- Variable comparison: subject variable group 21, variable 29, op 1, value 0

**Action**

- Object spawn/action: Training_Combat_Beacon (object 11, id 100), subtype 7
- Group/spawn-list action: spawn list/group 271, subtype 0
- Hide/remove HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 21, variable 29, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 9, param 25
- Show/update HUD contact: contact/list 0, subtype 9, param 22
- Show/update HUD contact: contact/list 0, subtype 9, param 23
- Show/update HUD contact: contact/list 0, subtype 1, param 271

### Event 6

**Trigger**

- Group/spawn-list event: subject 268, op 0, value 0 (join 2)
- Group/spawn-list event: subject 269, op 0, value 0 (join 2)
- Group/spawn-list event: subject 270, op 0, value 0 (join 2)
- Group/spawn-list event: subject 271, op 0, value 0

**Action**

- Set/add variable: variable group 12, variable 202, subtype 0, value 1
- Set/add variable: variable group 12, variable 203, subtype 0, value 2

### Event 7

**Trigger**

- Group/spawn-list event: subject 268, op 0, value 0 (join 2)
- Group/spawn-list event: subject 270, op 0, value 0 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 128

### Event 8

**Trigger**

- Group/spawn-list event: subject 269, op 0, value 0 (join 2)
- Group/spawn-list event: subject 271, op 0, value 0 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 129

### Event 9

**Trigger**

- Group/spawn-list event: subject 268, op 1, value 30

**Action**

- Play dialog: PLAYER.SCR, line/variant 131

### Event 10

**Trigger**

- Group/spawn-list event: subject 269, op 1, value 60

**Action**

- Play dialog: PLAYER.SCR, line/variant 102

### Event 11

**Trigger**

- Group/spawn-list event: subject 270, op 1, value 30

**Action**

- Play dialog: PLAYER.SCR, line/variant 99

### Event 12

**Trigger**

- Group/spawn-list event: subject 271, op 1, value 70

**Action**

- Play dialog: PLAYER.SCR, line/variant 100

### Event 13

**Trigger**

- Group/spawn-list event: subject 268, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 268
- Set/add variable: variable group 21, variable 29, subtype 0, value 0
- Set/add variable: variable group 0, variable 2, subtype 1, value 25
- Hide/remove HUD contact: contact/list 0, subtype 9, param 23
- Hide/remove HUD contact: contact/list 0, subtype 9, param 22
- Hide/remove HUD contact: contact/list 0, subtype 9, param 25
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 14

**Trigger**

- Group/spawn-list event: subject 269, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 269
- Set/add variable: variable group 21, variable 29, subtype 0, value 0
- Set/add variable: variable group 0, variable 2, subtype 1, value 50
- Hide/remove HUD contact: contact/list 0, subtype 9, param 22
- Hide/remove HUD contact: contact/list 0, subtype 9, param 23
- Hide/remove HUD contact: contact/list 0, subtype 9, param 25
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 15

**Trigger**

- Group/spawn-list event: subject 270, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 270
- Set/add variable: variable group 21, variable 29, subtype 0, value 0
- Set/add variable: variable group 0, variable 2, subtype 1, value 75
- Hide/remove HUD contact: contact/list 0, subtype 9, param 22
- Hide/remove HUD contact: contact/list 0, subtype 9, param 23
- Hide/remove HUD contact: contact/list 0, subtype 9, param 25
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 16

**Trigger**

- Group/spawn-list event: subject 271, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 271
- Set/add variable: variable group 21, variable 29, subtype 0, value 0
- Set/add variable: variable group 0, variable 2, subtype 1, value 100
- Hide/remove HUD contact: contact/list 0, subtype 9, param 22
- Hide/remove HUD contact: contact/list 0, subtype 9, param 23
- Hide/remove HUD contact: contact/list 0, subtype 9, param 25
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 17

**Trigger**

- Object event: subject Training_Combat_Beacon (object 8, id 97), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 11, param 0

### Event 18

**Trigger**

- Object event: subject Training_Combat_Beacon (object 9, id 98), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 11, param 0

### Event 19

**Trigger**

- Object event: subject Training_Combat_Beacon (object 10, id 99), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 11, param 0

### Event 20

**Trigger**

- Object event: subject Training_Combat_Beacon (object 11, id 100), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 11, param 0

## Waypoints

### Waypoint 0

- Tag: `151`
- Members: `Drone_Worker (object 0, id 102, starts at point 0)`, `Drone_Worker (object 1, id 103, starts at point 0)`, `Drone_Worker (object 2, id 104, starts at point 0)`, `Drone_Worker (object 3, id 105, starts at point 0)`, `Drone_Worker (object 4, id 106, starts at point 0)`, `Drone_Worker (object 5, id 107, starts at point 0)`, `Drone_Worker (object 6, id 108, starts at point 0)`, `Drone_Worker (object 7, id 109, starts at point 0)`, `Drone_Worker (object 12, id 118, starts at point 0)`, `Drone_Worker (object 13, id 121, starts at point 0)`, `Drone_Worker (object 14, id 122, starts at point 0)`, `Drone_Worker (object 15, id 124, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1471.01, 0.00, -729.65) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Drone_Worker` | 102 | Interactive | -997.29,0.00,863.34 | 128,0,0 | group/role: FG_ROOKIE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 1 | `Drone_Worker` | 103 | Interactive | -1003.45,0.00,923.44 | 128,0,0 | group/role: FG_ROOKIE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 2 | `Drone_Worker` | 104 | Interactive | -918.55,0.00,1503.76 | 164,0,0 | group/role: FG_VETERAN / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 3 | `Drone_Worker` | 105 | Interactive | -893.92,0.00,1583.89 | 164,0,0 | group/role: FG_VETERAN / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 4 | `Drone_Worker` | 106 | Interactive | -617.60,0.00,2028.84 | 199,0,0 | group/role: FG_ACE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 5 | `Drone_Worker` | 107 | Interactive | -568.33,0.00,2068.91 | 199,0,0 | group/role: FG_ACE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 6 | `Drone_Worker` | 108 | Interactive | -149.40,0.00,2377.45 | 235,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 7 | `Drone_Worker` | 109 | Interactive | -93.97,0.00,2390.81 | 235,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 8 | `Training_Combat_Beacon` | 97 | Interactive | 1175.75,20.00,-346.14 | 43,0,7 | secondary groups: FG_ROOKIE, FG_ROOKIE |
| 9 | `Training_Combat_Beacon` | 98 | Interactive | 1251.30,41.16,-197.30 | 498,505,0 | secondary groups: FG_VETERAN, FG_VETERAN |
| 10 | `Training_Combat_Beacon` | 99 | Interactive | 1314.71,66.11,-24.13 | 192,0,0 | secondary groups: FG_ACE, FG_ACE |
| 11 | `Training_Combat_Beacon` | 100 | Interactive | 1380.95,83.64,121.17 | 114,0,505 | secondary groups: FG_ELITE, FG_ELITE |
| 12 | `Drone_Worker` | 118 | Interactive | -999.24,0.00,1027.96 | 149,0,0 | group/role: FG_ROOKIE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 13 | `Drone_Worker` | 121 | Interactive | -873.80,0.00,1645.56 | 192,0,0 | group/role: FG_VETERAN / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 14 | `Drone_Worker` | 122 | Interactive | -528.44,0.00,2101.07 | 228,0,0 | group/role: FG_ACE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 15 | `Drone_Worker` | 124 | Interactive | -30.83,0.00,2404.82 | 256,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
