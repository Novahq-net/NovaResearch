# Tachyon: The Fringe EARTH03G.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH03G.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `(none)` |
| Region | 0 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 6 |
| Entities | 19 |
| Events | 12 |
| Waypoints | 6 |
| Child Sectors | 0 |
| Scripts | 0 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Light_Freighter`, `1: Independent_Merc_Dart`, `2: Independent_Merc_Piranha`, `3: Independent_Merc_Mako`, `4: GalSpan_Pegasus`, `5: GalSpan_Orion` |
| Scripts | None |
| Scenes | None |
| Labels | `SHUT`, `bfnf_03`, `PLAYER`, `ORION03`, `ORION02`, `ORION01`, `PEGASUS01`, `PEGASUS02`, `PEGASUS03`, `MAKO01`, `MAKO03`, `PIRANHA01`, `PIRANHA02`, `PIRANHA03`, `PIRANHA04`, `DART01`, `DART02`, `DART03`, `DART04`, `FRGT`, `CPSH`, `SAMA`, `FREIGHT01` |
| Aliases | `fred2`, `fred1`, `fred3` |
| Groups | `FG_ADDER`, `FG_ARA` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 12, variable 205, op 0, value 1

**Action**

- Play scene: unknown index 0, param 0
- Set/add variable: variable group 0, variable 3, subtype 0, value 0
- Set/add variable: variable group 0, variable 12, subtype 0, value 0
- Set/add variable: variable group 12, variable 205, subtype 0, value 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 2

**Action**

- Object spawn/action: Independent_Merc_Dart (object 14, id 952), subtype 5

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 5

**Action**

- Object spawn/action: Independent_Merc_Mako (object 7, id 944), subtype 5

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 10

**Action**

- Group/spawn-list action: spawn list/group 67, subtype 2
- Object spawn/action: GalSpan_Orion (object 2, id 939), subtype 5

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 13

**Action**

- Group/spawn-list action: spawn list/group 97, subtype 2
- Object spawn/action: GalSpan_Orion (object 3, id 940), subtype 5

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 16

**Action**

- Object spawn/action: GalSpan_Pegasus (object 5, id 942), subtype 5

### Event 7

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 19

**Action**

- Object spawn/action: GalSpan_Pegasus (object 4, id 941), subtype 5

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 31

**Action**

- Object spawn/action: Independent_Merc_Piranha (object 10, id 947), subtype 5

### Event 9

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 34

**Action**

- Object spawn/action: Independent_Merc_Dart (object 15, id 953), subtype 5

### Event 10

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 37

**Action**

- Object spawn/action: Independent_Merc_Mako (object 8, id 945), subtype 5

### Event 11

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 5

**Action**

- Object spawn/action: Generic_Light_Freighter (object 18, id 956), subtype 5

## Waypoints

### Waypoint 0

- Tag: `406`
- Members: `GalSpan_Orion (object 2, id 939, starts at point 0)`, `GalSpan_Orion (object 3, id 940, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (41.92, 0.00, 677.01) | None |
| 1 | (30.49, 0.00, 598.50) | None |
| 2 | (38.11, 0.00, 501.39) | None |
| 3 | (40.02, 0.00, 375.36) | None |

### Waypoint 1

- Tag: `405`
- Members: `Independent_Merc_Dart (object 16, id 954, starts at point 0)`, `Independent_Merc_Dart (object 17, id 955, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (93.32, 0.00, 632.47) | on arrival redirect to Waypoint 2 (tag 404), point 0 |

### Waypoint 2

- Tag: `404`
- Members: `Independent_Merc_Piranha (object 11, id 948, starts at point 0)`, `Independent_Merc_Piranha (object 12, id 949, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (84.15, 0.00, 301.73) | on arrival redirect to Waypoint 1 (tag 405), point 0 |

### Waypoint 3

- Tag: `403`
- Members: `Generic_Light_Freighter (object 18, id 956, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (259.75, 0.00, 1407.84) | None |
| 1 | (272.25, 0.00, 1841.56) | None |

### Waypoint 4

- Tag: `402`
- Members: `GalSpan_Pegasus (object 4, id 941, starts at point 0)`, `GalSpan_Pegasus (object 5, id 942, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-33.37, 0.00, 591.42) | None |
| 1 | (-36.19, 0.00, 402.23) | None |
| 2 | (-36.45, 0.00, 292.06) | on arrival action 4, param -1 |

### Waypoint 5

- Tag: `401`
- Members: `Independent_Merc_Mako (object 7, id 944, starts at point 0)`, `Independent_Merc_Mako (object 8, id 945, starts at point 0)`, `Independent_Merc_Piranha (object 10, id 947, starts at point 0)`, `Independent_Merc_Dart (object 14, id 952, starts at point 0)`, `Independent_Merc_Dart (object 15, id 953, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (15.81, 0.00, 229.84) | None |
| 1 | (14.11, 0.00, 565.34) | None |
| 2 | (37.14, 0.00, 997.87) | on arrival action 4, param -1 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `GalSpan_Orion` | 937 | Interactive | -296.85,0.00,2031.34 | 0,0,0 | label: PLAYER |
| 1 | `GalSpan_Orion` | 938 | Interactive | -294.39,0.00,1865.95 | 0,0,0 | label: ORION03 |
| 2 | `GalSpan_Orion` | 939 | Interactive | 236.93,0.00,804.41 | 320,0,0 | label: ORION02; waypoint: Waypoint 0 (tag 406, 4 point(s)), starting point 0, arrival event value 26607616 |
| 3 | `GalSpan_Orion` | 940 | Interactive | 274.84,0.00,864.38 | 309,0,0 | label: ORION01; waypoint: Waypoint 0 (tag 406, 4 point(s)), starting point 0, arrival event value 26607616 |
| 4 | `GalSpan_Pegasus` | 941 | Interactive | 212.78,0.00,1183.13 | 314,0,0 | label: PEGASUS01; waypoint: Waypoint 4 (tag 402, 3 point(s)), starting point 0, arrival event value 26345472 |
| 5 | `GalSpan_Pegasus` | 942 | Interactive | 174.93,0.00,1150.85 | 314,0,0 | label: PEGASUS02; waypoint: Waypoint 4 (tag 402, 3 point(s)), starting point 0, arrival event value 26345472 |
| 6 | `GalSpan_Pegasus` | 943 | Interactive | -299.91,0.00,1733.38 | 0,0,0 | label: PEGASUS03 |
| 7 | `Independent_Merc_Mako` | 944 | Interactive | 14.11,-1.57,73.94 | 0,0,0 | label: MAKO01; waypoint: Waypoint 5 (tag 401, 3 point(s)), starting point 0, arrival event value 26279936 |
| 8 | `Independent_Merc_Mako` | 945 | Interactive | 16.01,0.66,-8.04 | 0,0,0 | waypoint: Waypoint 5 (tag 401, 3 point(s)), starting point 0, arrival event value 26279936 |
| 9 | `Independent_Merc_Mako` | 946 | Interactive | -124.50,0.00,1967.04 | 0,0,0 | label: MAKO03 |
| 10 | `Independent_Merc_Piranha` | 947 | Interactive | 14.29,0.00,51.66 | 0,0,0 | label: PIRANHA01; waypoint: Waypoint 5 (tag 401, 3 point(s)), starting point 0, arrival event value 26279936 |
| 11 | `Independent_Merc_Piranha` | 948 | Interactive | -236.09,-23.97,619.25 | 174,0,0 | label: PIRANHA02; group/role: FG_ADDER / 0; waypoint: Waypoint 2 (tag 404, 1 point(s)), starting point 0, arrival event value 26476544 |
| 12 | `Independent_Merc_Piranha` | 949 | Interactive | -240.15,-23.97,594.71 | 174,0,0 | label: PIRANHA03; group/role: FG_ADDER / 0; waypoint: Waypoint 2 (tag 404, 1 point(s)), starting point 0, arrival event value 26476544 |
| 13 | `Independent_Merc_Piranha` | 950 | Interactive | -134.19,0.00,1860.06 | 0,0,0 | label: PIRANHA04 |
| 14 | `Independent_Merc_Dart` | 952 | Interactive | 13.84,0.00,100.95 | 0,0,0 | label: DART01; waypoint: Waypoint 5 (tag 401, 3 point(s)), starting point 0, arrival event value 26279936 |
| 15 | `Independent_Merc_Dart` | 953 | Interactive | 15.07,0.00,25.28 | 0,0,0 | label: DART02; waypoint: Waypoint 5 (tag 401, 3 point(s)), starting point 0, arrival event value 26279936 |
| 16 | `Independent_Merc_Dart` | 954 | Interactive | -238.17,-9.59,1098.28 | 169,0,0 | label: DART03; group/role: FG_ARA / 0; waypoint: Waypoint 1 (tag 405, 1 point(s)), starting point 0, arrival event value 26542080 |
| 17 | `Independent_Merc_Dart` | 955 | Interactive | -237.83,-9.59,1126.02 | 169,0,0 | label: DART04; group/role: FG_ARA / 0; waypoint: Waypoint 1 (tag 405, 1 point(s)), starting point 0, arrival event value 26542080 |
| 18 | `Generic_Light_Freighter` | 956 | Interactive | -5.30,0.00,1002.34 | 0,0,0 | label: FREIGHT01; waypoint: Waypoint 3 (tag 403, 2 point(s)), starting point 0, arrival event value 26411008 |
