# Tachyon: The Fringe NEUT05G.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT05G.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 4 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 1 |
| Events | 3 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Star_Patrol_Capital_Ship` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `aobul` |
| Aliases | `bagel`, `bagel_1`, `bagel_2`, `oside`, `oside_1`, `oside_2`, `Will_01`, `SHIP1_HYPER`, `ohshit`, `SHIP3_HYPER`, `SHIP2_HYPER` |
| Groups | None |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 450 (extra 2, 6; join 2; flags 2)
- Group/spawn-list event: subject 199, op 4, value 0 (flags 2)

**Action**

- Group/spawn-list action: spawn list/group 199, subtype 2

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 200 (extra 1, 6; flags 2)

**Action**

- Object spawn/action: Star_Patrol_Capital_Ship (object 0, id 1326), subtype 3

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 8, variable 4, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 188

## Waypoints

### Waypoint 0

- Tag: `402`
- Members: `Star_Patrol_Capital_Ship (object 0, id 1326, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (32.73, 571.82, 1600.59) | None |
| 1 | (-826.88, 587.27, -1697.81) | on arrival action 1, param -1 |

### Waypoint 1

- Tag: `401`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (427.43, -1290.90, 1922.99) | None |
| 1 | (351.53, -1012.85, 2592.45) | None |
| 2 | (456.62, -127.62, 2682.47) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Star_Patrol_Capital_Ship` | 1326 | Interactive | 41.49,556.36,3411.56 | 256,0,0 | waypoint: Waypoint 0 (tag 402, 2 point(s)), starting point 0, arrival event value 26345472 |
