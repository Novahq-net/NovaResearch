# Tachyon: The Fringe FRON11D.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON11D.SPX` |
| Sector | `QUAD_11` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 10 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 7 |
| Events | 8 |
| Waypoints | 4 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Hajod_Fighter_1`, `1: Hajod_Fighter_2`, `2: Malkar_Sistine_Chapel` |
| Scripts | `PODDS.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `bfne_05`, `BFBE_04`, `bfne_01`, `bfne_03`, `bfne_02`, `bfne_04`, `bfne_06`, `bfne_08`, `bfne_07`, `bfne_09` |
| Aliases | `BC05_sistine_chapel`, `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1`, `bc05_2`, `bc05_3`, `bc05_5`, `bc05_4`, `Stocks01` |
| Groups | `SISTINE_CHAPEL`, `FG_DISCIPLINE`, `FG_DESPOT`, `FG_PUNISHER` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 86, subtype 4, param 2
- Play dialog: PODDS.SCR, line/variant 2
- Set/add variable: variable group 21, variable 25, subtype 0, value 1

### Event 1

**Trigger**

- Variable comparison: subject variable group 21, variable 3, op 1, value 1

**Action**

- Object spawn/action: Malkar_Sistine_Chapel (object 0, id 187), subtype 3

### Event 2

**Trigger**

- Object event: subject Malkar_Sistine_Chapel (object 0, id 187), op 8, value 0

**Action**

- Set/add variable: variable group 21, variable 4, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 15
- Mission objective/state: param 262153, subtype 0, param 0

### Event 3

**Trigger**

- Object event: subject Malkar_Sistine_Chapel (object 0, id 187), op 2, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 68

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Set/add variable: variable group 21, variable 33, subtype 0, value 1

### Event 5

**Trigger**

- Object arrival: Malkar_Sistine_Chapel (object 0, id 187) reached Waypoint 0 (tag 254), point 0 (raw value 16646144)

**Action**

- Set/add variable: variable group 21, variable 34, subtype 0, value 1

### Event 6

**Trigger**

- Variable comparison: subject variable group 21, variable 33, op 1, value 1
- Variable comparison: subject variable group 21, variable 34, op 1, value 1

**Action**

- Object spawn/action: Malkar_Sistine_Chapel (object 0, id 187), subtype 5
- Object spawn/action: Malkar_Sistine_Chapel (object 0, id 187), subtype 13, param 16449536
- Show/update HUD contact: contact/list 0, subtype 9, param 15

### Event 7

**Trigger**

- Object event: subject Malkar_Sistine_Chapel (object 0, id 187), op 2, value 0

**Action**

- Set/add variable: variable group 16, variable 404, subtype 0, value 1
- Set/add variable: variable group 16, variable 405, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 15
- Show/update HUD contact: contact/list 0, subtype 11, param 38

## Waypoints

### Waypoint 0

- Tag: `254`
- Members: `Malkar_Sistine_Chapel (object 0, id 187, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-269.11, 0.00, 2260.51) | on arrival activate current object (raw param -1 ignored); listened by Event 5 for Malkar_Sistine_Chapel (object 0, id 187) |

### Waypoint 1

- Tag: `253`
- Members: `Hajod_Fighter_1 (object 3, id 702, starts at point 0)`, `Hajod_Fighter_1 (object 4, id 704, starts at point 0)`, `Hajod_Fighter_2 (object 5, id 705, starts at point 0)`, `Hajod_Fighter_2 (object 6, id 706, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (874.39, 0.00, 1748.97) | None |
| 1 | (-686.95, 0.00, 1887.04) | None |
| 2 | (-1456.54, 0.00, 746.40) | None |
| 3 | (531.11, 0.00, 764.41) | on arrival redirect to Waypoint 1 (tag 253), point 0 |

### Waypoint 2

- Tag: `252`
- Members: `Hajod_Fighter_2 (object 1, id 369, starts at point 0)`, `Hajod_Fighter_2 (object 2, id 370, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (172.57, 0.00, 2987.66) | None |
| 1 | (-19.65, 0.00, 1468.07) | None |
| 2 | (-268.47, 0.00, 1171.16) | None |
| 3 | (-926.16, 0.00, 1069.96) | None |
| 4 | (-1187.34, 0.00, 1189.67) | on arrival redirect to Waypoint 2 (tag 252), point 3 |

### Waypoint 3

- Tag: `251`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-698.72, 0.00, 1405.99) | None |
| 1 | (-927.23, 0.00, 1019.60) | on arrival action 1, param -1 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Malkar_Sistine_Chapel` | 187 | Interactive | -215.73,0.00,2342.15 | 294,0,0 | alias: BC05_sistine_chapel; secondary groups: none, SISTINE_CHAPEL; waypoint: Waypoint 0 (tag 254, 1 point(s)), starting point 0, arrival event value 16646144 |
| 1 | `Hajod_Fighter_2` | 369 | Interactive | 568.12,0.00,4442.41 | 269,0,0 | label: BFBE_04; group/role: FG_DISCIPLINE / 1; waypoint: Waypoint 2 (tag 252, 5 point(s)), starting point 0, arrival event value 16515072 |
| 2 | `Hajod_Fighter_2` | 370 | Interactive | 806.08,0.00,4170.28 | 267,0,0 | group/role: FG_DISCIPLINE / 0; waypoint: Waypoint 2 (tag 252, 5 point(s)), starting point 0, arrival event value 16515072 |
| 3 | `Hajod_Fighter_1` | 702 | Interactive | 1279.36,0.00,3185.71 | 256,0,0 | group/role: FG_DESPOT / 0; alias: bc05_2; waypoint: Waypoint 1 (tag 253, 4 point(s)), starting point 0, arrival event value 16580608 |
| 4 | `Hajod_Fighter_1` | 704 | Interactive | 1489.22,0.00,3317.22 | 256,0,0 | label: BFBE_04; group/role: FG_DESPOT / 1; alias: bc05_3; waypoint: Waypoint 1 (tag 253, 4 point(s)), starting point 0, arrival event value 16580608 |
| 5 | `Hajod_Fighter_2` | 705 | Interactive | 2221.38,0.00,3205.15 | 256,0,0 | group/role: FG_PUNISHER / 1; alias: bc05_5; waypoint: Waypoint 1 (tag 253, 4 point(s)), starting point 0, arrival event value 16580608 |
| 6 | `Hajod_Fighter_2` | 706 | Interactive | 1995.98,0.00,3128.73 | 256,0,0 | label: BFBE_04; group/role: FG_PUNISHER / 0; alias: bc05_4; waypoint: Waypoint 1 (tag 253, 4 point(s)), starting point 0, arrival event value 16580608 |
