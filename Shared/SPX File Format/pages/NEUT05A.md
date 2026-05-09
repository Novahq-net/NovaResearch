# Tachyon: The Fringe NEUT05A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT05A.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 4 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 12 |
| Events | 4 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Star_Patrol_Enforcer` |
| Scripts | `STP2.SCR` |
| Scenes | None |
| Labels | `aobul` |
| Aliases | `bagel`, `bagel_1`, `bagel_2`, `oside`, `oside_1`, `oside_2`, `Will_01`, `SHIP1_HYPER`, `ohshit`, `SHIP3_HYPER`, `SHIP2_HYPER` |
| Groups | `FG_LIGHTNING`, `FG_TYPHOON`, `FG_NOVA`, `FG_STORM` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Group/spawn-list event: subject 119, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 120, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 122, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 123, op 4, value 0 (flags 2)

**Action**

- Group/spawn-list action: spawn list/group 119, subtype 4, param 9
- Group/spawn-list action: spawn list/group 120, subtype 4, param 9
- Group/spawn-list action: spawn list/group 122, subtype 4, param 9
- Group/spawn-list action: spawn list/group 123, subtype 4, param 9
- Object spawn/action: id 858, subtype 8, param 9
- Play dialog: STP2.SCR, line/variant 0

### Event 1

**Trigger**

- Object event: subject Star_Patrol_Enforcer (object 6, id 329), op 4, value 90 (join 2)
- Object event: subject Star_Patrol_Enforcer (object 7, id 330), op 4, value 90 (join 2)
- Object event: subject Star_Patrol_Enforcer (object 8, id 331), op 4, value 90 (join 2)
- Object event: subject Star_Patrol_Enforcer (object 9, id 333), op 4, value 90 (join 2)
- Object event: subject Star_Patrol_Enforcer (object 10, id 334), op 4, value 90 (join 2)
- Object event: subject Star_Patrol_Enforcer (object 11, id 335), op 4, value 90 (join 2)

**Action**

- Group/spawn-list action: spawn list/group 119, subtype 0
- Group/spawn-list action: spawn list/group 123, subtype 0

### Event 2

**Trigger**

- Group/spawn-list event: subject 119, op 3, value 0

**Action**

- Group/spawn-list action: spawn list/group 119, subtype 4, param 9

### Event 3

**Trigger**

- Group/spawn-list event: subject 123, op 3, value 0

**Action**

- Group/spawn-list action: spawn list/group 123, subtype 4, param 9

## Waypoints

### Waypoint 0

- Tag: `8`
- Members: `Star_Patrol_Enforcer (object 3, id 219, starts at point 0)`, `Star_Patrol_Enforcer (object 4, id 220, starts at point 0)`, `Star_Patrol_Enforcer (object 5, id 221, starts at point 0)`, `Star_Patrol_Enforcer (object 6, id 329, starts at point 6)`, `Star_Patrol_Enforcer (object 7, id 330, starts at point 6)`, `Star_Patrol_Enforcer (object 8, id 331, starts at point 6)`, `Star_Patrol_Enforcer (object 9, id 333, starts at point 3)`, `Star_Patrol_Enforcer (object 10, id 334, starts at point 3)`, `Star_Patrol_Enforcer (object 11, id 335, starts at point 3)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (435.00, 100.00, 1270.00) | None |
| 1 | (1315.00, 80.00, 1270.00) | None |
| 2 | (1750.00, -450.00, 1270.00) | None |
| 3 | (1750.00, -450.00, 0.00) | None |
| 4 | (410.00, 0.00, -765.21) | None |
| 5 | (-875.00, -450.00, 0.00) | None |
| 6 | (-875.00, -450.00, 2550.00) | None |
| 7 | (470.00, 0.00, 2750.00) | None |
| 8 | (1750.00, -450.00, 2550.00) | None |
| 9 | (1750.00, -450.00, 1350.00) | None |
| 10 | (1315.00, 80.00, 1350.00) | on arrival redirect to Waypoint 1 (tag 7), point 0 |

### Waypoint 1

- Tag: `7`
- Members: `Star_Patrol_Enforcer (object 0, id 216, starts at point 0)`, `Star_Patrol_Enforcer (object 1, id 217, starts at point 0)`, `Star_Patrol_Enforcer (object 2, id 218, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (435.00, 100.00, 1360.00) | None |
| 1 | (435.00, 60.00, 2060.00) | None |
| 2 | (435.00, 0.00, 2750.00) | None |
| 3 | (435.00, -850.00, 2400.00) | None |
| 4 | (435.00, -1125.00, 1320.00) | None |
| 5 | (435.00, -850.00, 240.00) | None |
| 6 | (435.00, 0.00, -790.00) | None |
| 7 | (435.00, 60.00, 580.00) | on arrival redirect to Waypoint 0 (tag 8), point 0 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Star_Patrol_Enforcer` | 216 | Interactive | 435.00,-60.00,1370.00 | 128,128,0 | group/role: FG_LIGHTNING / 1; waypoint: Waypoint 1 (tag 7, 8 point(s)), starting point 0, arrival event value 458752 |
| 1 | `Star_Patrol_Enforcer` | 217 | Interactive | 435.00,-60.00,1360.00 | 128,128,0 | group/role: FG_LIGHTNING / 2; waypoint: Waypoint 1 (tag 7, 8 point(s)), starting point 0, arrival event value 458752 |
| 2 | `Star_Patrol_Enforcer` | 218 | Interactive | 435.00,-60.00,1350.00 | 128,128,0 | group/role: FG_LIGHTNING / 3; waypoint: Waypoint 1 (tag 7, 8 point(s)), starting point 0, arrival event value 458752 |
| 3 | `Star_Patrol_Enforcer` | 219 | Interactive | 435.00,-60.00,1280.00 | 128,128,0 | group/role: FG_TYPHOON / 1; waypoint: Waypoint 0 (tag 8, 11 point(s)), starting point 0, arrival event value 524288 |
| 4 | `Star_Patrol_Enforcer` | 220 | Interactive | 435.00,-60.00,1270.00 | 128,128,0 | group/role: FG_TYPHOON / 2; waypoint: Waypoint 0 (tag 8, 11 point(s)), starting point 0, arrival event value 524288 |
| 5 | `Star_Patrol_Enforcer` | 221 | Interactive | 435.00,-60.00,1260.00 | 128,128,0 | group/role: FG_TYPHOON / 3; waypoint: Waypoint 0 (tag 8, 11 point(s)), starting point 0, arrival event value 524288 |
| 6 | `Star_Patrol_Enforcer` | 329 | Interactive | -875.03,-450.00,1248.34 | 0,0,0 | group/role: FG_NOVA / 1; waypoint: Waypoint 0 (tag 8, 11 point(s)), starting point 6, arrival event value 524294 |
| 7 | `Star_Patrol_Enforcer` | 330 | Interactive | -895.03,-450.00,1221.17 | 0,0,0 | group/role: FG_NOVA / 2; waypoint: Waypoint 0 (tag 8, 11 point(s)), starting point 6, arrival event value 524294 |
| 8 | `Star_Patrol_Enforcer` | 331 | Interactive | -860.53,-450.00,1216.95 | 0,0,0 | group/role: FG_NOVA / 3; waypoint: Waypoint 0 (tag 8, 11 point(s)), starting point 6, arrival event value 524294 |
| 9 | `Star_Patrol_Enforcer` | 333 | Interactive | 1748.88,0.00,694.15 | 256,0,0 | group/role: FG_STORM / 1; waypoint: Waypoint 0 (tag 8, 11 point(s)), starting point 3, arrival event value 524291 |
| 10 | `Star_Patrol_Enforcer` | 334 | Interactive | 1772.00,0.00,740.23 | 256,0,0 | group/role: FG_STORM / 2; waypoint: Waypoint 0 (tag 8, 11 point(s)), starting point 3, arrival event value 524291 |
| 11 | `Star_Patrol_Enforcer` | 335 | Interactive | 1732.69,0.00,741.62 | 256,0,0 | group/role: FG_STORM / 3; waypoint: Waypoint 0 (tag 8, 11 point(s)), starting point 3, arrival event value 524291 |
