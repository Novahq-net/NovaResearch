# Tachyon: The Fringe EARTH03E.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH03E.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `(none)` |
| Region | 0 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 2 |
| Events | 7 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Orion`, `1: Generic_Light_Freighter` |
| Scripts | `PLAYER.SCR`, `DILL.SCR`, `SAMA.SCR` |
| Scenes | None |
| Labels | `SHUT`, `bfnf_03`, `PLAYER`, `ORION03`, `ORION02`, `ORION01`, `PEGASUS01`, `PEGASUS02`, `PEGASUS03`, `MAKO01`, `MAKO03`, `PIRANHA01`, `PIRANHA02`, `PIRANHA03`, `PIRANHA04`, `DART01`, `DART02`, `DART03`, `DART04`, `FRGT`, `CPSH`, `SAMA`, `FREIGHT01` |
| Aliases | `fred2`, `fred1`, `fred3` |
| Groups | `CAYUGAN_HAULER`, `CONT_016`, `SAMANTHA_CRAWLEY`, `CONT_012` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 18, subtype 0, value 0
- Mission objective/state: param 5, subtype 0, param 0
- Gate state/action: param 1, subtype 2, param 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 18, op 1, value 18

**Action**

- Play dialog: PLAYER.SCR, line/variant 43

### Event 2

**Trigger**

- Object event: subject Generic_Light_Freighter (object 0, id 807), op 4, value 10

**Action**

- Play dialog: DILL.SCR, line/variant 4

### Event 3

**Trigger**

- Object event: subject Generic_Light_Freighter (object 0, id 807), op 4, value 100

**Action**

- Play dialog: DILL.SCR, line/variant 5

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 12, variable 11, op 0, value 1

**Action**

- Set runtime trigger variable: variable group 20, variable 19, subtype 0, value 0
- Object spawn/action: GalSpan_Orion (object 1, id 927), subtype 0

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 5

**Action**

- Play dialog: SAMA.SCR, line/variant 0

### Event 6

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 0
- Variable comparison: subject variable group 21, variable 24, op 1, value 1
- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)

**Action**

- Set/add variable: variable group 21, variable 23, subtype 0, value 1

## Waypoints

### Waypoint 0

- Tag: `301`
- Members: `GalSpan_Orion (object 1, id 927, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1115.61, 344.00, 4051.47) | None |
| 1 | (-1017.46, 344.00, 2837.51) | on arrival play dialog/script or enter gate, param 301 |

### Waypoint 1

- Tag: `8`
- Members: `Generic_Light_Freighter (object 0, id 807, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2665.85, 376.00, -383.22) | None |
| 1 | (1515.08, 376.00, -1088.88) | None |
| 2 | (-120.21, 376.00, -1049.68) | None |
| 3 | (-1560.31, 376.00, -186.61) | None |
| 4 | (-1244.19, 376.00, 1397.18) | None |
| 5 | (-393.30, 376.00, 370.92) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Generic_Light_Freighter` | 807 | Interactive | 2809.45,376.00,-115.35 | 296,0,0 | secondary groups: CONT_016, CAYUGAN_HAULER; waypoint: Waypoint 1 (tag 8, 6 point(s)), starting point 0, arrival event value 524288 |
| 1 | `GalSpan_Orion` | 927 | Interactive | -884.21,344.00,4984.34 | 300,0,0 | label: SAMA; secondary groups: CONT_012, SAMANTHA_CRAWLEY; waypoint: Waypoint 0 (tag 301, 2 point(s)), starting point 0, arrival event value 19726336 |
