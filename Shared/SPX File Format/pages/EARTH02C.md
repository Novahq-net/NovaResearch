# Tachyon: The Fringe EARTH02C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH02C.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `(none)` |
| Region | 0 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 6 |
| Events | 1 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 0 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Star_Patrol_Capital_Ship`, `1: Generic_Light_Freighter`, `2: Independent_Merc_Mako` |
| Scripts | None |
| Scenes | None |
| Labels | `bfnf_03`, `ariv`, `AGT FIGHTER`, `CAPB`, `CAPA`, `ofrt` |
| Aliases | `danc_blowfish1`, `danc_blowfish2`, `danc_blowfish5`, `danc_blowfish3`, `danc_blowfish4`, `Jerome50` |
| Groups | `FG_AGT_RIVAL5`, `CONT_018`, `CONT_001`, `THUNDER`, `CONT_025` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Object event: subject Star_Patrol_Capital_Ship (object 5, id 1447), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Star_Patrol_Capital_Ship (object 5, id 1447), subtype 12

## Waypoints

### Waypoint 0

- Tag: `201`
- Members: `Star_Patrol_Capital_Ship (object 5, id 1447, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2057.78, 344.13, -1293.17) | None |
| 1 | (-2060.60, 333.77, -145.16) | on arrival action 1, param -1 |

### Waypoint 1

- Tag: `17`
- Members: `Generic_Light_Freighter (object 3, id 1346, starts at point 1)`, `Generic_Light_Freighter (object 4, id 1355, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-227.71, 0.00, -215.62) | None |
| 1 | (170.38, 200.00, 191.61) | on arrival action 1, param -1 |

### Waypoint 2

- Tag: `16`
- Members: `Independent_Merc_Mako (object 0, id 1339, starts at point 0)`, `Independent_Merc_Mako (object 1, id 1340, starts at point 0)`, `Independent_Merc_Mako (object 2, id 1341, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1244.52, 600.00, -2256.72) | None |
| 1 | (-1806.37, 600.00, -2220.19) | None |
| 2 | (-1806.37, 600.00, -3091.75) | None |
| 3 | (-1244.52, 600.00, -3086.53) | on arrival redirect to Waypoint 2 (tag 16), point 0 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Independent_Merc_Mako` | 1339 | Interactive | -1240.37,600.00,-3028.27 | 0,0,0 | label: bfnf_03; group/role: FG_AGT_RIVAL5 / 1; waypoint: Waypoint 2 (tag 16, 4 point(s)), starting point 0, arrival event value 1048576 |
| 1 | `Independent_Merc_Mako` | 1340 | Interactive | -1221.34,600.00,-3050.48 | 0,0,0 | group/role: FG_AGT_RIVAL5 / 2; waypoint: Waypoint 2 (tag 16, 4 point(s)), starting point 0, arrival event value 1048576 |
| 2 | `Independent_Merc_Mako` | 1341 | Interactive | -1256.81,600.00,-3062.97 | 0,0,0 | group/role: FG_AGT_RIVAL5 / 0; waypoint: Waypoint 2 (tag 16, 4 point(s)), starting point 0, arrival event value 1048576 |
| 3 | `Generic_Light_Freighter` | 1346 | Interactive | -417.60,0.00,-412.39 | 64,0,0 | label: bfnf_03; secondary groups: CONT_018, none; waypoint: Waypoint 1 (tag 17, 2 point(s)), starting point 1, arrival event value 1114113 |
| 4 | `Generic_Light_Freighter` | 1355 | Interactive | -400.98,0.00,-586.35 | 64,0,0 | label: bfnf_03; group/role: none / 2; secondary groups: CONT_001, none; waypoint: Waypoint 1 (tag 17, 2 point(s)), starting point 0, arrival event value 1114112 |
| 5 | `Star_Patrol_Capital_Ship` | 1447 | Interactive | -2043.49,351.13,-2039.99 | 0,0,0 | label: bfnf_03; group/role: none / 1; secondary groups: CONT_025, THUNDER; waypoint: Waypoint 0 (tag 201, 2 point(s)), starting point 0, arrival event value 13172736 |
