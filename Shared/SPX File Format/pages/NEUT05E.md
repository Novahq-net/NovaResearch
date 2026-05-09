# Tachyon: The Fringe NEUT05E.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT05E.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 4 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 3 |
| Events | 2 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Star_Patrol_Enforcer`, `1: Shuttle_Medium` |
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

**Action**

- Set runtime trigger variable: variable group 20, variable 28, subtype 0, value 0
- Group/spawn-list action: spawn list/group 141, subtype 2

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 28, op 1, value 5

**Action**

- Set runtime trigger variable: variable group 20, variable 28, subtype 1, value 0
- Play dialog: AOBUL.SCR, line/variant 20

## Waypoints

### Waypoint 0

- Tag: `302`
- Members: `Star_Patrol_Enforcer (object 1, id 1268, starts at point 0)`, `Star_Patrol_Enforcer (object 2, id 1269, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1205.87, 226.12, 1152.07) | None |
| 1 | (1342.82, 202.56, 1750.03) | None |
| 2 | (715.47, 23.55, 2648.94) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Shuttle_Medium` | 1216 | Interactive | 255.80,236.63,1190.11 | 435,14,196 | None |
| 1 | `Star_Patrol_Enforcer` | 1268 | Interactive | 856.48,166.73,-191.26 | 0,0,85 | group/role: FG_QUAKE / 1; secondary groups: none, COMMANDER_OBULO; waypoint: Waypoint 0 (tag 302, 3 point(s)), starting point 0, arrival event value 19791872 |
| 2 | `Star_Patrol_Enforcer` | 1269 | Interactive | 794.90,136.41,-250.57 | 0,0,348 | group/role: FG_QUAKE / 2; waypoint: Waypoint 0 (tag 302, 3 point(s)), starting point 0, arrival event value 19791872 |
