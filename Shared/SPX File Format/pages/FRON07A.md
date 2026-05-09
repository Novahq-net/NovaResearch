# Tachyon: The Fringe FRON07A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON07A.SPX` |
| Sector | `QUAD_07` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 6 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 5 |
| Events | 13 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Drone_Attack`, `1: Laser_Core` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFGE_01`, `alexander`, `BFGF_01`, `baronhajod` |
| Aliases | `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1` |
| Groups | `ARMAGEDDON_LASER_CORE`, `FG_DEGAS`, `FG_SHAKESPEARE` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Group/spawn-list action: spawn list/group 220, subtype 6
- Group/spawn-list action: spawn list/group 217, subtype 6

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Group/spawn-list action: spawn list/group 220, subtype 4, param 2
- Group/spawn-list action: spawn list/group 217, subtype 4, param 2
- Play scene: unknown index 0, param 0
- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0
- Set/add variable: variable group 21, variable 20, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 9, param 12

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 5

**Action**

- Play dialog: PLAYER.SCR, line/variant 47
- Set runtime trigger variable: variable group 20, variable 0, subtype 1, value 0

### Event 3

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 47

**Action**

- Group/spawn-list action: spawn list/group 220, subtype 2
- Group/spawn-list action: spawn list/group 217, subtype 2

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 300 (extra 1, 1151; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 300 (extra 1, 1159; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 300 (extra 1, 683; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 300 (extra 1, 681; join 2; flags 2)

**Action**

- Set/add variable: variable group 21, variable 21, subtype 0, value 1

### Event 5

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 1
- Sector/startup condition family: subject 0, op 0, value 47

**Action**

- Play dialog: PLAYER.SCR, line/variant 51

### Event 6

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 1146; flags 2)

**Action**

- Set/add variable: variable group 16, variable 400, subtype 0, value 1
- Set/add variable: variable group 16, variable 401, subtype 0, value 2
- Hide/remove HUD contact: contact/list 0, subtype 9, param 12
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 37
- Play dialog: PLAYER.SCR, line/variant 53
- Set/add variable: variable group 38, variable 4, subtype 0, value 1

### Event 7

**Trigger**

- Object event: subject Laser_Core (object 0, id 1146), op 2, value 0

**Action**

- Set/add variable: variable group 16, variable 400, subtype 0, value 0
- Set/add variable: variable group 16, variable 401, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 12
- Play dialog: PLAYER.SCR, line/variant 52
- Show/update HUD contact: contact/list 0, subtype 11, param 38

### Event 8

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 47

**Action**

- Group/spawn-list action: spawn list/group 220, subtype 2
- Group/spawn-list action: spawn list/group 217, subtype 2

### Event 9

**Trigger**

- Object event: subject Drone_Attack (object 1, id 1151), op 4, value 100

**Action**

- Object spawn/action: Drone_Attack (object 1, id 1151), subtype 7

### Event 10

**Trigger**

- Object event: subject Drone_Attack (object 4, id 1159), op 4, value 100

**Action**

- Object spawn/action: Drone_Attack (object 4, id 1159), subtype 7

### Event 11

**Trigger**

- Object event: subject Drone_Attack (object 2, id 681), op 4, value 100

**Action**

- Object spawn/action: Drone_Attack (object 2, id 681), subtype 7

### Event 12

**Trigger**

- Object event: subject Drone_Attack (object 3, id 683), op 4, value 100

**Action**

- Object spawn/action: Drone_Attack (object 3, id 683), subtype 7

## Waypoints

### Waypoint 0

- Tag: `1`
- Members: `Drone_Attack (object 1, id 1151, starts at point 4)`, `Drone_Attack (object 2, id 681, starts at point 4)`, `Drone_Attack (object 3, id 683, starts at point 6)`, `Drone_Attack (object 4, id 1159, starts at point 6)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (403.61, 0.00, -102.69) | None |
| 1 | (1513.02, -223.83, 227.38) | None |
| 2 | (834.88, -27.27, 1542.52) | None |
| 3 | (1688.26, 216.36, 2159.28) | None |
| 4 | (308.51, -196.00, 1904.97) | None |
| 5 | (-341.56, -65.45, 2481.94) | None |
| 6 | (-906.63, -61.44, 2134.46) | None |
| 7 | (367.59, 88.17, 1283.78) | None |
| 8 | (-966.04, 61.44, 511.47) | None |
| 9 | (-454.27, 0.00, 4.53) | on arrival redirect to waypoint tag 3, point 0 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Laser_Core` | 1146 | Interactive | 510.16,125.50,1620.45 | 454,0,0 | secondary groups: none, ARMAGEDDON_LASER_CORE |
| 1 | `Drone_Attack` | 1151 | Interactive | 1532.48,0.00,2110.93 | 0,0,0 | group/role: FG_DEGAS / 0; waypoint: Waypoint 0 (tag 1, 10 point(s)), starting point 4, arrival event value 65540 |
| 2 | `Drone_Attack` | 681 | Interactive | 1536.48,0.00,2152.36 | 0,0,0 | group/role: FG_DEGAS / 0; waypoint: Waypoint 0 (tag 1, 10 point(s)), starting point 4, arrival event value 65540 |
| 3 | `Drone_Attack` | 683 | Interactive | -400.56,0.00,2440.33 | 384,0,0 | group/role: FG_SHAKESPEARE / 0; waypoint: Waypoint 0 (tag 1, 10 point(s)), starting point 6, arrival event value 65542 |
| 4 | `Drone_Attack` | 1159 | Interactive | -373.86,0.00,2423.76 | 384,0,0 | group/role: FG_SHAKESPEARE / 0; waypoint: Waypoint 0 (tag 1, 10 point(s)), starting point 6, arrival event value 65542 |
