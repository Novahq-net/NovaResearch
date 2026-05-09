# Tachyon: The Fringe GALS05C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `GALS05C.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `(none)` |
| Region | 2 |
| Sector ID | 4 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 5 |
| Events | 6 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Wingman_Ramos`, `1: GalSpan_Pegasus` |
| Scripts | `LAKFR.SCR`, `LAKIT.SCR` |
| Scenes | None |
| Labels | `bfne_02`, `BFGE_04`, `bfne_03`, `bfgf_02`, `bfne_08`, `bfge_02` |
| Aliases | `wing_man` |
| Groups | `FG_CAELUM`, `LAKITA_CELENE` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Object spawn/action: GalSpan_Pegasus (object 0, id 24), subtype 8, param 1
- Object spawn/action: GalSpan_Pegasus (object 1, id 25), subtype 8, param 1
- Set runtime trigger variable: variable group 20, variable 6, subtype 0, value 0

### Event 1

**Trigger**

- Object event: subject Wingman_Ramos (object 2, id 41), op 15, value 0

**Action**

- Object spawn/action: Wingman_Ramos (object 2, id 41), subtype 8

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 6, op 1, value 5

**Action**

- Play dialog: LAKFR.SCR, line/variant 0

### Event 3

**Trigger**

- Object event: subject Wingman_Ramos (object 2, id 41), op 0, value 0 (flags 2)

**Action**

- Play dialog: LAKIT.SCR, line/variant 1

### Event 4

**Trigger**

- Object event: subject GalSpan_Pegasus (object 0, id 24), op 0, value 0 (join 2; flags 2)
- Object event: subject GalSpan_Pegasus (object 1, id 25), op 0, value 0 (join 2; flags 2)
- Variable comparison: subject variable group 20, variable 6, op 1, value 20 (join 2)

**Action**

- Object spawn/action: GalSpan_Pegasus (object 1, id 25), subtype 2, param 1
- Object spawn/action: GalSpan_Pegasus (object 0, id 24), subtype 2, param 1
- Set runtime trigger variable: variable group 20, variable 6, subtype 1, value 0

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 21, op 1, value 1 (join 1)
- Variable comparison: subject variable group 21, variable 29, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 216, subtype 1, param 1
- Object spawn/action: Wingman_Ramos (object 2, id 41), subtype 1, param 2

## Waypoints

### Waypoint 0

- Tag: `202`
- Members: `GalSpan_Pegasus (object 3, id 108, starts at point 0)`, `GalSpan_Pegasus (object 4, id 109, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-482.22, 0.00, 89.71) | None |
| 1 | (39.74, 0.00, 89.71) | None |

### Waypoint 1

- Tag: `203`
- Members: `Wingman_Ramos (object 2, id 41, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (699.02, 0.00, 331.59) | None |
| 1 | (474.14, 0.00, 278.41) | None |
| 2 | (254.15, 0.00, 314.19) | None |
| 3 | (-51.00, 0.00, 306.24) | None |
| 4 | (-345.50, 0.00, 282.39) | None |
| 5 | (-551.30, 0.00, 190.96) | on arrival play dialog/script or enter gate, param 1 |

### Waypoint 2

- Tag: `201`
- Members: `GalSpan_Pegasus (object 0, id 24, starts at point 0)`, `GalSpan_Pegasus (object 1, id 25, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-224.62, 0.00, 747.15) | None |
| 1 | (-532.85, 0.00, 574.48) | None |
| 2 | (-645.87, 0.00, 286.71) | None |
| 3 | (-394.14, 0.00, 165.84) | None |
| 4 | (-142.42, 0.00, 269.44) | None |
| 5 | (6.56, 0.00, 424.84) | on arrival redirect to Waypoint 2 (tag 201), point 0 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `GalSpan_Pegasus` | 24 | Interactive | -105.21,0.00,864.92 | 326,0,0 | group/role: FG_CAELUM / 0; waypoint: Waypoint 2 (tag 201, 6 point(s)), starting point 0, arrival event value 13172736 |
| 1 | `GalSpan_Pegasus` | 25 | Interactive | -69.15,0.00,825.97 | 327,0,0 | label: BFGE_04; group/role: FG_CAELUM / 0; waypoint: Waypoint 2 (tag 201, 6 point(s)), starting point 0, arrival event value 13172736 |
| 2 | `Wingman_Ramos` | 41 | Interactive | 725.63,0.00,84.85 | 385,0,0 | alias: wing_man; secondary groups: none, LAKITA_CELENE; waypoint: Waypoint 1 (tag 203, 6 point(s)), starting point 0, arrival event value 13303808 |
| 3 | `GalSpan_Pegasus` | 108 | Interactive | -668.94,0.00,-39.12 | 0,0,0 | group/role: FG_CAELUM / 0; waypoint: Waypoint 0 (tag 202, 2 point(s)), starting point 0, arrival event value 13238272 |
| 4 | `GalSpan_Pegasus` | 109 | Interactive | -673.18,0.00,-85.13 | 0,0,0 | group/role: FG_CAELUM / 0; waypoint: Waypoint 0 (tag 202, 2 point(s)), starting point 0, arrival event value 13238272 |
