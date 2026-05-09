# Tachyon: The Fringe FRON09B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON09B.SPX` |
| Sector | `QUAD_09` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 8 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 12 |
| Events | 2 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Hajod_Fighter_1` |
| Scripts | `HMSLA.SCR` |
| Scenes | None |
| Labels | `BFNE_04`, `BFNE_02`, `BFNE_07` |
| Aliases | None |
| Groups | `FG_DESPOT`, `FG_DISCIPLINE` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 2; flags 2)

**Action**

- Play scene: unknown index 0, param 0

### Event 1

**Trigger**

- Object event: subject 2, op 0, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 86, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 132, op 4, value 0 (join 2; flags 2)

**Action**

- Play dialog: HMSLA.SCR, line/variant 4
- Object spawn/action: id 2, subtype 8, param 1
- Group/spawn-list action: spawn list/group 86, subtype 4, param 1
- Group/spawn-list action: spawn list/group 132, subtype 4, param 1
- Group/spawn-list action: spawn list/group 86, subtype 7
- Group/spawn-list action: spawn list/group 132, subtype 7

## Waypoints

### Waypoint 0

- Tag: `1`
- Members: `Hajod_Fighter_1 (object 0, id 122, starts at point -1)`, `Hajod_Fighter_1 (object 1, id 123, starts at point -1)`, `Hajod_Fighter_1 (object 2, id 124, starts at point -1)`, `Hajod_Fighter_1 (object 3, id 125, starts at point -1)`, `Hajod_Fighter_1 (object 4, id 126, starts at point -1)`, `Hajod_Fighter_1 (object 5, id 127, starts at point -1)`, `Hajod_Fighter_1 (object 6, id 128, starts at point -1)`, `Hajod_Fighter_1 (object 7, id 129, starts at point -1)`, `Hajod_Fighter_1 (object 8, id 130, starts at point -1)`, `Hajod_Fighter_1 (object 9, id 131, starts at point -1)`, `Hajod_Fighter_1 (object 10, id 132, starts at point -1)`, `Hajod_Fighter_1 (object 11, id 133, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-3075.77, -186.94, -927.42) | None |
| 1 | (-3062.99, -186.94, -10.93) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hajod_Fighter_1` | 122 | Interactive | -3463.42,-330.58,-668.91 | 118,506,0 | group/role: FG_DESPOT / 0; waypoint: Waypoint 0 (tag 1, 2 point(s)), starting point -1 |
| 1 | `Hajod_Fighter_1` | 123 | Interactive | -3462.68,-330.58,-680.26 | 118,506,0 | group/role: FG_DESPOT / 0; waypoint: Waypoint 0 (tag 1, 2 point(s)), starting point -1 |
| 2 | `Hajod_Fighter_1` | 124 | Interactive | -3464.61,-330.58,-656.99 | 118,506,0 | group/role: FG_DESPOT / 0; waypoint: Waypoint 0 (tag 1, 2 point(s)), starting point -1 |
| 3 | `Hajod_Fighter_1` | 125 | Interactive | -3465.57,-330.58,-645.32 | 118,506,0 | group/role: FG_DESPOT / 0; waypoint: Waypoint 0 (tag 1, 2 point(s)), starting point -1 |
| 4 | `Hajod_Fighter_1` | 126 | Interactive | -3804.51,-267.74,-1117.03 | 118,506,0 | group/role: FG_DESPOT / 0; waypoint: Waypoint 0 (tag 1, 2 point(s)), starting point -1 |
| 5 | `Hajod_Fighter_1` | 127 | Interactive | -3800.36,-267.74,-1144.70 | 118,506,0 | group/role: FG_DESPOT / 0; waypoint: Waypoint 0 (tag 1, 2 point(s)), starting point -1 |
| 6 | `Hajod_Fighter_1` | 128 | Interactive | -3806.40,-267.74,-1103.13 | 118,506,0 | group/role: FG_DESPOT / 0; waypoint: Waypoint 0 (tag 1, 2 point(s)), starting point -1 |
| 7 | `Hajod_Fighter_1` | 129 | Interactive | -3802.57,-267.74,-1130.70 | 118,506,0 | group/role: FG_DESPOT / 0; waypoint: Waypoint 0 (tag 1, 2 point(s)), starting point -1 |
| 8 | `Hajod_Fighter_1` | 130 | Interactive | -2877.41,0.00,-1205.39 | 0,0,0 | group/role: FG_DISCIPLINE / 0; waypoint: Waypoint 0 (tag 1, 2 point(s)), starting point -1 |
| 9 | `Hajod_Fighter_1` | 131 | Interactive | -2857.10,0.00,-1207.18 | 0,0,0 | group/role: FG_DISCIPLINE / 0; waypoint: Waypoint 0 (tag 1, 2 point(s)), starting point -1 |
| 10 | `Hajod_Fighter_1` | 132 | Interactive | -2835.15,0.00,-1207.18 | 0,0,0 | group/role: FG_DISCIPLINE / 0; waypoint: Waypoint 0 (tag 1, 2 point(s)), starting point -1 |
| 11 | `Hajod_Fighter_1` | 133 | Interactive | -2807.16,0.00,-1207.18 | 0,0,0 | group/role: FG_DISCIPLINE / 0; waypoint: Waypoint 0 (tag 1, 2 point(s)), starting point -1 |
