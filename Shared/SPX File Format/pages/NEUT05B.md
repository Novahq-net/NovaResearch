# Tachyon: The Fringe NEUT05B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT05B.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 4 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 3 |
| Events | 4 |
| Waypoints | 4 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Star_Patrol_Enforcer` |
| Scripts | `AOBUL.SCR` |
| Scenes | None |
| Labels | `aobul` |
| Aliases | `bagel`, `bagel_1`, `bagel_2`, `oside`, `oside_1`, `oside_2`, `Will_01`, `SHIP1_HYPER`, `ohshit`, `SHIP3_HYPER`, `SHIP2_HYPER` |
| Groups | `FG_QUAKE`, `COMMANDER_OBULO` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 8, variable 2, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 141, subtype 0

### Event 1

**Trigger**

- Group/spawn-list event: subject 141, op 2, value 9961472 (Waypoint 1 (tag 152), point 0)
- Variable comparison: subject variable group 8, variable 2, op 1, value 1

**Action**

- Play dialog: AOBUL.SCR, line/variant 4
- Object spawn/action: id 1160, subtype 12
- Play scene: unknown index 0, param 0

### Event 2

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 4

**Action**

- Group/spawn-list action: spawn list/group 141, subtype 8, param 10027008 (Waypoint 0 (tag 153), point 0)
- Group/spawn-list action: spawn list/group 141, subtype 2

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 8, variable 2, op 1, value 1

**Action**

- Disabled / no-op: param -1, subtype -1, param -1

## Waypoints

### Waypoint 0

- Tag: `153`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1425.41, 85.54, -87.93) | None |
| 1 | (1549.12, -272.78, 520.34) | None |
| 2 | (1526.16, -397.84, 1156.27) | None |
| 3 | (1239.43, -696.22, 1301.53) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 1

- Tag: `152`
- Members: `Star_Patrol_Enforcer (object 0, id 1199, starts at point 0)`, `Star_Patrol_Enforcer (object 2, id 1201, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (219.20, 131.16, 776.01) | None |
| 1 | (436.69, 131.16, 631.12) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 2

- Tag: `151`
- Members: `Star_Patrol_Enforcer (object 1, id 1200, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (58.44, 0.00, -832.61) | None |
| 1 | (412.51, 0.00, -1147.35) | None |
| 2 | (732.17, 0.00, -853.47) | None |
| 3 | (401.62, 0.00, -502.56) | on arrival redirect to Waypoint 2 (tag 151), point 0 |

### Waypoint 3

- Tag: `20`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (422.55, -809.08, -372.79) | None |
| 1 | (448.55, 14.56, -1195.54) | None |
| 2 | (-1080.31, 494.27, 27.93) | None |
| 3 | (-1080.65, 494.27, 345.44) | on arrival action 1, param -1 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Star_Patrol_Enforcer` | 1199 | Interactive | -45.91,126.75,921.95 | 185,0,0 | label: aobul; group/role: FG_QUAKE / 1; secondary groups: none, COMMANDER_OBULO; waypoint: Waypoint 1 (tag 152, 2 point(s)), starting point 0, arrival event value 9961472 |
| 1 | `Star_Patrol_Enforcer` | 1200 | Interactive | -290.28,126.75,994.89 | 199,0,0 | group/role: FG_QUAKE / 2; waypoint: Waypoint 2 (tag 151, 4 point(s)), starting point 0, arrival event value 9895936 |
| 2 | `Star_Patrol_Enforcer` | 1201 | Interactive | 65.62,126.75,1211.53 | 199,0,0 | group/role: FG_QUAKE / 3; waypoint: Waypoint 1 (tag 152, 2 point(s)), starting point 0, arrival event value 9961472 |
