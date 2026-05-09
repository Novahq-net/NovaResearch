# Tachyon: The Fringe FRON12C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON12C.SPX` |
| Sector | `QUAD_12` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 11 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 12 |
| Events | 7 |
| Waypoints | 4 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Red_Pirate_Fighter_2` |
| Scripts | `RRORY.SCR` |
| Scenes | None |
| Labels | `BFNF_01`, `BFGE_01`, `BFNE_02` |
| Aliases | `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1`, `Stocks01` |
| Groups | `FG_RAGE`, `FG_PRIDE`, `FG_GREED` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Gate state/action: param 2, subtype 3, param 0
- Gate state/action: param 3, subtype 3, param 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 7, subtype 0, value 0

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 7, op 1, value 15

**Action**

- Group/spawn-list action: spawn list/group 62, subtype 7
- Play dialog: RRORY.SCR, line/variant 0

### Event 3

**Trigger**

- Group/spawn-list event: subject 62, op 1, value 60

**Action**

- Group/spawn-list action: spawn list/group 62, subtype 7
- Group/spawn-list action: spawn list/group 63, subtype 7

### Event 4

**Trigger**

- Group/spawn-list event: subject 62, op 1, value 60 (join 2)
- Group/spawn-list event: subject 63, op 1, value 60 (join 2)

**Action**

- Group/spawn-list action: spawn list/group 64, subtype 7

### Event 5

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 0

**Action**

- Group/spawn-list action: spawn list/group 62, subtype 4, param 9
- Group/spawn-list action: spawn list/group 63, subtype 4, param 9
- Group/spawn-list action: spawn list/group 60, subtype 4, param 9
- Group/spawn-list action: spawn list/group 64, subtype 4, param 9
- Object spawn/action: id 1366, subtype 8, param 9

### Event 6

**Trigger**

- Variable comparison: subject variable group 21, variable 23, op 1, value 1

**Action**

- Gate state/action: param 3, subtype 2, param 0
- Gate state/action: param 2, subtype 2, param 0

## Waypoints

### Waypoint 0

- Tag: `19`
- Members: `Red_Pirate_Fighter_2 (object 4, id 1402, starts at point -1)`, `Red_Pirate_Fighter_2 (object 5, id 1403, starts at point -1)`, `Red_Pirate_Fighter_2 (object 6, id 1404, starts at point -1)`, `Red_Pirate_Fighter_2 (object 7, id 1405, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1675.24, 278.83, 585.65) | None |
| 1 | (1676.13, 488.23, 320.04) | None |
| 2 | (662.87, 603.06, 313.74) | None |
| 3 | (662.87, 603.06, 1921.44) | None |
| 4 | (2622.50, 603.06, 1905.98) | None |
| 5 | (2633.40, 603.06, 325.49) | None |

### Waypoint 1

- Tag: `18`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1397.30, -458.53, 557.30) | None |
| 1 | (977.37, -249.13, 675.38) | None |
| 2 | (-2645.55, 0.87, -1.41) | None |
| 3 | (-3004.00, 0.00, 255.09) | None |
| 4 | (-2976.86, 0.00, -259.17) | on arrival redirect to Waypoint 1 (tag 18), point 2 |

### Waypoint 2

- Tag: `17`
- Members: `Red_Pirate_Fighter_2 (object 8, id 1411, starts at point -1)`, `Red_Pirate_Fighter_2 (object 9, id 1410, starts at point -1)`, `Red_Pirate_Fighter_2 (object 10, id 1412, starts at point -1)`, `Red_Pirate_Fighter_2 (object 11, id 1413, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1746.91, 288.55, 160.59) | None |
| 1 | (1748.24, 497.95, -117.47) | None |
| 2 | (332.41, 747.08, -128.39) | None |
| 3 | (168.91, 747.08, 150.43) | None |
| 4 | (33.54, 747.08, -192.85) | on arrival redirect to Waypoint 2 (tag 17), point 2 |

### Waypoint 3

- Tag: `16`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2941.14, -458.53, -459.47) | None |
| 1 | (1887.65, -51.51, -563.27) | None |
| 2 | (1888.05, 127.89, -563.11) | None |
| 3 | (1206.59, 129.43, 239.28) | None |
| 4 | (300.46, -43.58, -411.35) | on arrival redirect to Waypoint 3 (tag 16), point 1 |

## Spawn Lists

### Spawn List 0

- ID: `64`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 1

- ID: `63`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Red_Pirate_Fighter_2` | 1398 | Interactive | 3417.98,0.00,-528.52 | 0,0,0 | group/role: FG_RAGE / 0 |
| 1 | `Red_Pirate_Fighter_2` | 1399 | Interactive | 3391.95,0.00,-552.72 | 0,0,0 | group/role: FG_RAGE / 0 |
| 2 | `Red_Pirate_Fighter_2` | 1400 | Interactive | 3436.58,0.00,-550.70 | 0,0,0 | group/role: FG_RAGE / 0 |
| 3 | `Red_Pirate_Fighter_2` | 1401 | Interactive | 3414.26,0.00,-572.89 | 0,0,0 | group/role: FG_RAGE / 0 |
| 4 | `Red_Pirate_Fighter_2` | 1402 | Interactive | 1753.77,0.00,547.30 | 0,0,0 | group/role: FG_PRIDE / 0; waypoint: Waypoint 0 (tag 19, 6 point(s)), starting point -1 |
| 5 | `Red_Pirate_Fighter_2` | 1403 | Interactive | 1732.38,0.00,521.08 | 0,0,0 | group/role: FG_PRIDE / 0; waypoint: Waypoint 0 (tag 19, 6 point(s)), starting point -1 |
| 6 | `Red_Pirate_Fighter_2` | 1404 | Interactive | 1771.44,0.00,523.10 | 0,0,0 | group/role: FG_PRIDE / 0; waypoint: Waypoint 0 (tag 19, 6 point(s)), starting point -1 |
| 7 | `Red_Pirate_Fighter_2` | 1405 | Interactive | 1749.12,0.00,497.89 | 0,0,0 | group/role: FG_PRIDE / 0; waypoint: Waypoint 0 (tag 19, 6 point(s)), starting point -1 |
| 8 | `Red_Pirate_Fighter_2` | 1411 | Interactive | 1789.85,0.00,405.37 | 0,0,0 | group/role: FG_GREED / 0; waypoint: Waypoint 2 (tag 17, 5 point(s)), starting point -1 |
| 9 | `Red_Pirate_Fighter_2` | 1410 | Interactive | 1814.02,0.00,430.58 | 0,0,0 | group/role: FG_GREED / 0; waypoint: Waypoint 2 (tag 17, 5 point(s)), starting point -1 |
| 10 | `Red_Pirate_Fighter_2` | 1412 | Interactive | 1834.48,0.00,407.39 | 0,0,0 | group/role: FG_GREED / 0; waypoint: Waypoint 2 (tag 17, 5 point(s)), starting point -1 |
| 11 | `Red_Pirate_Fighter_2` | 1413 | Interactive | 1808.44,0.00,381.17 | 0,0,0 | group/role: FG_GREED / 0; waypoint: Waypoint 2 (tag 17, 5 point(s)), starting point -1 |
