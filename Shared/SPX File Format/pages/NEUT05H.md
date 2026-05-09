# Tachyon: The Fringe NEUT05H.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT05H.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 4 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 1 |
| Events | 4 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Star_Patrol_Capital_Ship` |
| Scripts | `ALPHA.SCR` |
| Scenes | None |
| Labels | `aobul` |
| Aliases | `bagel`, `bagel_1`, `bagel_2`, `oside`, `oside_1`, `oside_2`, `Will_01`, `SHIP1_HYPER`, `ohshit`, `SHIP3_HYPER`, `SHIP2_HYPER` |
| Groups | None |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Object event: subject Star_Patrol_Capital_Ship (object 0, id 1253), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Star_Patrol_Capital_Ship (object 0, id 1253), subtype 5

### Event 1

**Trigger**

- Object arrival: Star_Patrol_Capital_Ship (object 0, id 1253) reached Waypoint 0 (tag 451), point 0 (raw value 29556736)

**Action**

- Object spawn/action: Star_Patrol_Capital_Ship (object 0, id 1253), subtype 4

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 15, subtype 0, value 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 15, op 1, value 3

**Action**

- Set runtime trigger variable: variable group 20, variable 15, subtype 1, value 0
- Play dialog: ALPHA.SCR, line/variant 0

## Waypoints

### Waypoint 0

- Tag: `451`
- Members: `Star_Patrol_Capital_Ship (object 0, id 1253, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-742.67, 1400.05, 3263.38) | None; listened by Event 1 for Star_Patrol_Capital_Ship (object 0, id 1253) |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Star_Patrol_Capital_Ship` | 1253 | Interactive | -502.19,1253.27,1281.12 | 505,7,0 | waypoint: Waypoint 0 (tag 451, 1 point(s)), starting point 0, arrival event value 29556736 |
