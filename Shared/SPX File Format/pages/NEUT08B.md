# Tachyon: The Fringe NEUT08B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT08B.SPX` |
| Sector | `QUAD_08` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 7 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 10 |
| Events | 5 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Light_Freighter`, `1: Star_Patrol_Enforcer` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `bfne_03` |
| Aliases | `Jerome26`, `Jerome25`, `Jerome24`, `Jerome22`, `Jerome21`, `Jerome20`, `kwI03_10` |
| Groups | `FG_BOLT`, `FG_MAGELLAN` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 20, op 0, value 2

**Action**

- Object spawn/action: Generic_Light_Freighter (object 4, id 11), subtype 3
- Object spawn/action: Generic_Light_Freighter (object 5, id 12), subtype 3
- Object spawn/action: Generic_Light_Freighter (object 6, id 13), subtype 3
- Object spawn/action: Generic_Light_Freighter (object 7, id 15), subtype 3
- Object spawn/action: Generic_Light_Freighter (object 8, id 16), subtype 3
- Object spawn/action: Generic_Light_Freighter (object 9, id 17), subtype 3

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Group/spawn-list event: subject 181, op 3, value 0
- Variable comparison: subject variable group 21, variable 18, op 1, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 7, param 181
- Object spawn/action: Generic_Light_Freighter (object 6, id 13), subtype 14

### Event 2

**Trigger**

- Group/spawn-list event: subject 181, op 2, value 9895936 (Waypoint 1 (tag 151), point 0) (join 2)
- Group/spawn-list event: subject 181, op 2, value 9961472 (Waypoint 0 (tag 152), point 0)
- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 18, op 1, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 171
- Hide/remove HUD contact: contact/list 0, subtype 7, param 181
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 13, variable 416, subtype 0, value 1
- Set/add variable: variable group 13, variable 417, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 12, param 33

### Event 3

**Trigger**

- Group/spawn-list event: subject 181, op 2, value 9895936 (Waypoint 1 (tag 151), point 0) (join 2)
- Group/spawn-list event: subject 181, op 2, value 9961472 (Waypoint 0 (tag 152), point 0)
- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 18, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 4

**Trigger**

- Group/spawn-list event: subject 181, op 2, value 9895936 (Waypoint 1 (tag 151), point 0) (join 2)
- Group/spawn-list event: subject 181, op 2, value 9961472 (Waypoint 0 (tag 152), point 0)
- Group/spawn-list event: subject 181, op 4, value 0 (flags 2)

**Action**

- Group/spawn-list action: spawn list/group 121, subtype 0

## Waypoints

### Waypoint 0

- Tag: `152`
- Members: `Generic_Light_Freighter (object 7, id 15, starts at point 0)`, `Generic_Light_Freighter (object 8, id 16, starts at point 0)`, `Generic_Light_Freighter (object 9, id 17, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1299.71, 0.00, 2497.43) | None |
| 1 | (410.23, -479.83, 870.82) | None |

### Waypoint 1

- Tag: `151`
- Members: `Generic_Light_Freighter (object 4, id 11, starts at point 0)`, `Generic_Light_Freighter (object 5, id 12, starts at point 0)`, `Generic_Light_Freighter (object 6, id 13, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (926.54, 0.00, 2456.97) | None |
| 1 | (262.81, -479.83, 942.33) | None |

## Spawn Lists

### Spawn List 0

- ID: `121`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 5 | id 181 | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Star_Patrol_Enforcer` | 64 | Interactive | 1804.38,0.00,3979.69 | 310,0,0 | group/role: FG_BOLT / 0 |
| 1 | `Star_Patrol_Enforcer` | 65 | Interactive | 1851.68,0.00,3965.06 | 310,0,0 | group/role: FG_BOLT / 0 |
| 2 | `Star_Patrol_Enforcer` | 66 | Interactive | 1896.69,0.00,3940.65 | 310,0,0 | group/role: FG_BOLT / 0 |
| 3 | `Star_Patrol_Enforcer` | 67 | Interactive | 1930.44,0.00,3916.25 | 310,0,0 | group/role: FG_BOLT / 0 |
| 4 | `Generic_Light_Freighter` | 11 | Interactive | 1650.77,0.00,3044.09 | 336,0,0 | group/role: FG_MAGELLAN / 0; alias: Jerome26; waypoint: Waypoint 1 (tag 151, 2 point(s)), starting point 0, arrival event value 9895936 |
| 5 | `Generic_Light_Freighter` | 12 | Interactive | 1478.64,0.00,2935.22 | 336,0,0 | group/role: FG_MAGELLAN / 0; alias: Jerome25; waypoint: Waypoint 1 (tag 151, 2 point(s)), starting point 0, arrival event value 9895936 |
| 6 | `Generic_Light_Freighter` | 13 | Interactive | 1335.19,0.00,2826.34 | 336,0,0 | group/role: FG_MAGELLAN / 0; alias: Jerome24; waypoint: Waypoint 1 (tag 151, 2 point(s)), starting point 0, arrival event value 9895936 |
| 7 | `Generic_Light_Freighter` | 15 | Interactive | 1865.94,0.00,2981.88 | 336,0,0 | group/role: FG_MAGELLAN / 0; alias: Jerome22; waypoint: Waypoint 0 (tag 152, 2 point(s)), starting point 0, arrival event value 9961472 |
| 8 | `Generic_Light_Freighter` | 16 | Interactive | 1706.03,0.00,2880.14 | 336,0,0 | group/role: FG_MAGELLAN / 0; alias: Jerome21; waypoint: Waypoint 0 (tag 152, 2 point(s)), starting point 0, arrival event value 9961472 |
| 9 | `Generic_Light_Freighter` | 17 | Interactive | 1545.89,0.00,2766.67 | 336,0,0 | group/role: FG_MAGELLAN / 0; alias: Jerome20; waypoint: Waypoint 0 (tag 152, 2 point(s)), starting point 0, arrival event value 9961472 |
