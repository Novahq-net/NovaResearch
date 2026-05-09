# Tachyon: The Fringe EARTH03D.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH03D.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `(none)` |
| Region | 0 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 5 |
| Events | 8 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Light_Freighter`, `1: GalSpan_Heavy_Freighter`, `2: GalSpan_Poseidon` |
| Scripts | `DILL.SCR` |
| Scenes | None |
| Labels | `SHUT`, `bfnf_03`, `PLAYER`, `ORION03`, `ORION02`, `ORION01`, `PEGASUS01`, `PEGASUS02`, `PEGASUS03`, `MAKO01`, `MAKO03`, `PIRANHA01`, `PIRANHA02`, `PIRANHA03`, `PIRANHA04`, `DART01`, `DART02`, `DART03`, `DART04`, `FRGT`, `CPSH`, `SAMA`, `FREIGHT01` |
| Aliases | `fred2`, `fred1`, `fred3` |
| Groups | `FG_GALSPAN7`, `CONT_021`, `FG_GALSPAN8`, `CONT_012` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 26, subtype 0, value 0
- Mission objective/state: param 6, subtype 0, param 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 26, op 1, value 30

**Action**

- Object spawn/action: GalSpan_Heavy_Freighter (object 3, id 783), subtype 3

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 12, variable 9, op 1, value 1
- Variable comparison: subject variable group 12, variable 10, op 1, value 2

**Action**

- Set runtime trigger variable: variable group 20, variable 29, subtype 0, value 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 29, op 1, value 35

**Action**

- Object spawn/action: Generic_Light_Freighter (object 4, id 816), subtype 4

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 26, op 1, value 15

**Action**

- Play dialog: DILL.SCR, line/variant 43

### Event 5

**Trigger**

- Object arrival: GalSpan_Poseidon (object 0, id 771) reached Waypoint 0 (tag 5), point 0 (raw value 327680)

**Action**

- Object spawn/action: GalSpan_Poseidon (object 0, id 771), subtype 2, param 770

### Event 6

**Trigger**

- Object event: subject GalSpan_Poseidon (object 0, id 771), op 7, value 0

**Action**

- Object spawn/action: GalSpan_Poseidon (object 1, id 772), subtype 2, param 770

### Event 7

**Trigger**

- Object event: subject GalSpan_Poseidon (object 1, id 772), op 7, value 0

**Action**

- Object spawn/action: GalSpan_Poseidon (object 2, id 830), subtype 2, param 770

## Waypoints

### Waypoint 0

- Tag: `5`
- Members: `GalSpan_Poseidon (object 0, id 771, starts at point 0)`, `GalSpan_Poseidon (object 1, id 772, starts at point 0)`, `GalSpan_Poseidon (object 2, id 830, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (905.67, -247.57, 183.39) | None; listened by Event 5 for GalSpan_Poseidon (object 0, id 771) |
| 1 | (50.49, -247.57, 191.14) | None |
| 2 | (-532.55, -247.57, 466.94) | on arrival redirect to Waypoint 0 (tag 5), point 1 |

### Waypoint 1

- Tag: `7`
- Members: `Generic_Light_Freighter (object 4, id 816, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1456.55, 0.00, 29.61) | None |
| 1 | (7.91, 0.00, 803.06) | None |
| 2 | (640.42, 0.00, 2057.50) | None |
| 3 | (952.48, 0.00, 3394.74) | None |
| 4 | (1154.68, 0.00, 5502.85) | None |

### Waypoint 2

- Tag: `6`
- Members: `GalSpan_Heavy_Freighter (object 3, id 783, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1748.76, 0.00, -165.74) | None |
| 1 | (436.45, 0.00, -916.76) | None |
| 2 | (-1347.91, 175.00, -534.49) | None |
| 3 | (-796.66, 565.36, 922.70) | None |
| 4 | (-798.24, 561.81, 108.76) | on arrival activate current object (raw param -1 ignored) |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `GalSpan_Poseidon` | 771 | Interactive | 1278.30,-232.19,-237.51 | 384,0,0 | group/role: FG_GALSPAN7 / 0; alias: fred2; waypoint: Waypoint 0 (tag 5, 3 point(s)), starting point 0, arrival event value 327680 |
| 1 | `GalSpan_Poseidon` | 772 | Interactive | 1105.75,-287.19,-181.12 | 384,0,0 | group/role: FG_GALSPAN7 / 0; alias: fred1; waypoint: Waypoint 0 (tag 5, 3 point(s)), starting point 0, arrival event value 327680 |
| 2 | `GalSpan_Poseidon` | 830 | Interactive | 1186.37,-232.19,-19.93 | 384,0,0 | group/role: FG_GALSPAN7 / 0; alias: fred3; waypoint: Waypoint 0 (tag 5, 3 point(s)), starting point 0, arrival event value 327680 |
| 3 | `GalSpan_Heavy_Freighter` | 783 | Interactive | 2696.53,0.00,-360.46 | 384,0,0 | secondary groups: CONT_021, none; waypoint: Waypoint 2 (tag 6, 5 point(s)), starting point 0, arrival event value 393216 |
| 4 | `Generic_Light_Freighter` | 816 | Interactive | -1454.03,0.00,-293.81 | 0,0,0 | label: SAMA; group/role: FG_GALSPAN8 / 0; secondary groups: CONT_012, none; waypoint: Waypoint 1 (tag 7, 5 point(s)), starting point 0, arrival event value 458752 |
