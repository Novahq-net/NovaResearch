# Tachyon: The Fringe FRON01G.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON01G.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 5 |
| Events | 11 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Hajod_Fighter_2`, `1: Hajod_Fighter_1`, `2: Malkar_Sistine_Chapel` |
| Scripts | `ANNAH.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFGF_05`, `BFNE_03`, `BFNF_03`, `BFGE_01`, `BFGF_01`, `bfne_05` |
| Aliases | `Python 4`, `Python 3`, `Python 1`, `Python 2`, `Kimodo 1`, `Jerome02`, `Jerome03`, `Jerome04`, `Jerome05`, `Jerome06`, `Jerome01`, `BC05_sistine_chapel`, `bc05_1`, `bc05_2`, `bc05_4`, `bc05_5`, `Mantis1`, `Mantis2`, `Mantis3`, `Mantis4`, `Aphid1`, `Aphid2`, `Aphid3`, `Aphid4`, `Python1`, `Python2`, `Python3`, `Python4`, `Komodo1`, `Komodo2`, `Komodo3`, `Komodo4`, `Kimodo 2`, `Kimodo 3`, `Kimodo 4`, `Cephius`, `Stocks01` |
| Groups | `SISTINE_CHAPEL`, `FG_DESPOT`, `FG_PUNISHER` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 13, subtype 0, value 0
- Mission objective/state: param 262151, subtype 0, param 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 13, op 1, value 21

**Action**

- Play dialog: ANNAH.SCR, line/variant 4
- Set runtime trigger variable: variable group 20, variable 13, subtype 1, value 0

### Event 2

**Trigger**

- Variable comparison: subject variable group 21, variable 2, op 1, value 1

**Action**

- Object spawn/action: Malkar_Sistine_Chapel (object 0, id 306), subtype 3

### Event 3

**Trigger**

- Variable comparison: subject variable group 21, variable 22, op 1, value 1
- Variable comparison: subject variable group 21, variable 23, op 1, value 1
- Variable comparison: subject variable group 21, variable 21, op 1, value 0

**Action**

- Play scene: unknown index 0, param 1
- Play dialog: PLAYER.SCR, line/variant 64
- Show/update HUD contact: contact/list 0, subtype 9, param 15

### Event 4

**Trigger**

- Object event: subject Malkar_Sistine_Chapel (object 0, id 306), op 8, value 0

**Action**

- Set/add variable: variable group 21, variable 3, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 15
- Mission objective/state: param 262154, subtype 0, param 0

### Event 5

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 64

**Action**

- Object spawn/action: Malkar_Sistine_Chapel (object 0, id 306), subtype 5
- Object spawn/action: Malkar_Sistine_Chapel (object 0, id 306), subtype 13, param 26279936
- Set/add variable: variable group 21, variable 24, subtype 0, value 1

### Event 6

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Set/add variable: variable group 21, variable 22, subtype 0, value 1

### Event 7

**Trigger**

- Object event: subject Malkar_Sistine_Chapel (object 0, id 306), op 15, value 0

**Action**

- Set/add variable: variable group 21, variable 23, subtype 0, value 1

### Event 8

**Trigger**

- Variable comparison: subject variable group 21, variable 25, op 1, value 1
- Group/spawn-list event: subject 86, op 3, value 0

**Action**

- Group/spawn-list action: spawn list/group 86, subtype 3, param 5

### Event 9

**Trigger**

- Variable comparison: subject variable group 21, variable 25, op 1, value 1
- Group/spawn-list event: subject 87, op 3, value 0

**Action**

- Group/spawn-list action: spawn list/group 87, subtype 3, param 5

### Event 10

**Trigger**

- Object event: subject Malkar_Sistine_Chapel (object 0, id 306), op 2, value 0

**Action**

- Set/add variable: variable group 16, variable 404, subtype 0, value 1
- Set/add variable: variable group 16, variable 405, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 15
- Play dialog: PLAYER.SCR, line/variant 68
- Show/update HUD contact: contact/list 0, subtype 11, param 38

## Waypoints

### Waypoint 0

- Tag: `403`
- Members: `Hajod_Fighter_1 (object 1, id 647, starts at point 0)`, `Hajod_Fighter_1 (object 2, id 648, starts at point 0)`, `Hajod_Fighter_2 (object 3, id 650, starts at point 0)`, `Hajod_Fighter_2 (object 4, id 651, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1628.76, 0.00, 2639.38) | None |
| 1 | (-1610.43, 0.00, 1989.17) | None |
| 2 | (-2037.46, 0.00, 1994.36) | None |
| 3 | (-1963.33, 0.00, 2455.52) | on arrival redirect to Waypoint 0 (tag 403), point 0 |

### Waypoint 1

- Tag: `402`
- Members: `Malkar_Sistine_Chapel (object 0, id 306, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1506.94, -4.96, 2275.94) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 2

- Tag: `401`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1506.12, -4.96, 1984.64) | None |
| 1 | (-1507.28, -4.96, 1676.79) | on arrival action 1, param -1 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Malkar_Sistine_Chapel` | 306 | Interactive | -1504.54,-4.96,2357.29 | 258,0,0 | alias: BC05_sistine_chapel; secondary groups: none, SISTINE_CHAPEL; waypoint: Waypoint 1 (tag 402, 1 point(s)), starting point 0, arrival event value 26345472 |
| 1 | `Hajod_Fighter_1` | 647 | Interactive | -3108.24,0.00,1535.33 | 0,0,0 | group/role: FG_DESPOT / 0; alias: bc05_1; waypoint: Waypoint 0 (tag 403, 4 point(s)), starting point 0, arrival event value 26411008 |
| 2 | `Hajod_Fighter_1` | 648 | Interactive | -3170.78,0.00,1428.27 | 0,0,0 | group/role: FG_DESPOT / 1; alias: bc05_2; waypoint: Waypoint 0 (tag 403, 4 point(s)), starting point 0, arrival event value 26411008 |
| 3 | `Hajod_Fighter_2` | 650 | Interactive | -2673.80,0.00,1521.06 | 0,0,0 | group/role: FG_PUNISHER / 0; alias: bc05_4; waypoint: Waypoint 0 (tag 403, 4 point(s)), starting point 0, arrival event value 26411008 |
| 4 | `Hajod_Fighter_2` | 651 | Interactive | -2733.04,0.00,1421.13 | 0,0,0 | group/role: FG_PUNISHER / 1; alias: bc05_5; waypoint: Waypoint 0 (tag 403, 4 point(s)), starting point 0, arrival event value 26411008 |
