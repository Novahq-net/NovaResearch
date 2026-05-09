# Tachyon: The Fringe FRON12A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON12A.SPX` |
| Sector | `QUAD_12` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 11 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 4 |
| Events | 17 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 4 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Red_Pirate_Fighter_2`, `1: Red_Pirate_Shrike` |
| Scripts | `RRORY.SCR`, `PRSPH.SCR`, `BLODB.SCR`, `BLODA.SCR` |
| Scenes | None |
| Labels | `BFNF_01`, `BFGE_01`, `BFNE_02` |
| Aliases | `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1`, `Stocks01` |
| Groups | `FG_DEATH`, `FG_WAR` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Object spawn/action: id 1333, subtype 17
- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0
- Object spawn/action: id 1333, subtype 8, param 4

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Play scene: unknown index 0, param 0

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 2

**Action**

- Play dialog: RRORY.SCR, line/variant 2
- Set runtime trigger variable: variable group 20, variable 0, subtype 1, value 0

### Event 3

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 2

**Action**

- Set/add variable: variable group 21, variable 29, subtype 0, value 1

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 2450 (extra 1, 1333; flags 3)
- Variable comparison: subject variable group 21, variable 29, op 1, value 1
- Variable comparison: subject variable group 21, variable 30, op 1, value 0
- Variable comparison: subject variable group 21, variable 20, op 1, value 0

**Action**

- Play dialog: PRSPH.SCR, line/variant 0
- Set runtime trigger variable: variable group 20, variable 9, subtype 0, value 0
- Set/add variable: variable group 21, variable 30, subtype 0, value 1

### Event 5

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 1

**Action**

- Set/add variable: variable group 21, variable 30, subtype 0, value 0

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 35

**Action**

- Object spawn/action: id 1333, subtype 8, param 2
- Set runtime trigger variable: variable group 20, variable 9, subtype 1, value 0

### Event 7

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 1400 (extra 1, 964; flags 3)
- Variable comparison: subject variable group 21, variable 29, op 1, value 1
- Variable comparison: subject variable group 21, variable 20, op 1, value 0
- Variable comparison: subject variable group 21, variable 30, op 1, value 0

**Action**

- Group/spawn-list action: spawn list/group 61, subtype 2
- Play dialog: BLODB.SCR, line/variant 0
- Set/add variable: variable group 21, variable 30, subtype 0, value 1

### Event 8

**Trigger**

- Sector/startup condition family: subject 2, op 0, value 0

**Action**

- Set/add variable: variable group 21, variable 30, subtype 0, value 0

### Event 9

**Trigger**

- Group/spawn-list event: subject 61, op 0, value 0
- Variable comparison: subject variable group 21, variable 30, op 0, value 0

**Action**

- Play dialog: RRORY.SCR, line/variant 6
- Set/add variable: variable group 21, variable 30, subtype 0, value 1

### Event 10

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 6

**Action**

- Set/add variable: variable group 21, variable 30, subtype 0, value 0

### Event 11

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 2000 (extra 1, 1333; flags 3)
- Variable comparison: subject variable group 16, variable 401, op 1, value 2
- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)

**Action**

- Set runtime trigger variable: variable group 20, variable 19, subtype 0, value 0
- Play dialog: PRSPH.SCR, line/variant 4

### Event 12

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 20

**Action**

- Object spawn/action: id 1333, subtype 8, param 2
- Set runtime trigger variable: variable group 20, variable 19, subtype 1, value 0

### Event 13

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 66, subtype 0

### Event 14

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 2500 (extra 1, 967; flags 3)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 66, subtype 2
- Play dialog: BLODA.SCR, line/variant 1

### Event 15

**Trigger**

- Group/spawn-list event: subject 61, op 4, value 0 (flags 2)

**Action**

- Group/spawn-list action: spawn list/group 61, subtype 2

### Event 16

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Object spawn/action: id 1333, subtype 8, param 4

## Waypoints

### Waypoint 0

- Tag: `125`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2798.65, 0.00, 21.52) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 1

- Tag: `2`
- Members: `Red_Pirate_Fighter_2 (object 2, id 966, starts at point 0)`, `Red_Pirate_Fighter_2 (object 3, id 967, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1289.46, 0.00, 1098.96) | None |
| 1 | (1629.28, 0.00, 1339.41) | None |
| 2 | (240.62, 0.00, -515.66) | None |
| 3 | (383.14, 0.00, 180.00) | on arrival redirect to Waypoint 1 (tag 2), point 2 |

### Waypoint 2

- Tag: `1`
- Members: `Red_Pirate_Shrike (object 0, id 963, starts at point 0)`, `Red_Pirate_Shrike (object 1, id 964, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (864.93, 0.00, 27.49) | None |
| 1 | (1719.80, 0.00, 1694.42) | on arrival redirect to Waypoint 2 (tag 1), point 1 |
| 2 | (2840.13, 0.00, 1999.22) | None |
| 3 | (3829.50, 0.00, 2190.28) | on arrival redirect to Waypoint 2 (tag 1), point 1 |
| 4 | (3897.55, 0.00, 1569.13) | on arrival redirect to Waypoint 2 (tag 1), point 2 |

## Spawn Lists

### Spawn List 0

- ID: `66`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Red_Pirate_Shrike` | 963 | Interactive | 1777.79,-98.18,526.82 | 414,0,0 | group/role: FG_DEATH / 1; waypoint: Waypoint 2 (tag 1, 5 point(s)), starting point 0, arrival event value 65536 |
| 1 | `Red_Pirate_Shrike` | 964 | Interactive | 1700.64,-98.18,379.75 | 414,0,0 | group/role: FG_DEATH / 0; waypoint: Waypoint 2 (tag 1, 5 point(s)), starting point 0, arrival event value 65536 |
| 2 | `Red_Pirate_Fighter_2` | 966 | Interactive | 3398.93,-99.17,-525.69 | 420,0,0 | group/role: FG_WAR / 1; waypoint: Waypoint 1 (tag 2, 4 point(s)), starting point 0, arrival event value 131072 |
| 3 | `Red_Pirate_Fighter_2` | 967 | Interactive | 3451.32,-99.17,-621.31 | 420,0,0 | group/role: FG_WAR / 0; waypoint: Waypoint 1 (tag 2, 4 point(s)), starting point 0, arrival event value 131072 |
