# Tachyon: The Fringe FRON01B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON01B.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 12 |
| Events | 4 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Independent_Merc_Piranha`, `1: Shuttle_Small` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFGF_05`, `BFNE_03`, `BFNF_03`, `BFGE_01`, `BFGF_01`, `bfne_05` |
| Aliases | `Python 4`, `Python 3`, `Python 1`, `Python 2`, `Kimodo 1`, `Jerome02`, `Jerome03`, `Jerome04`, `Jerome05`, `Jerome06`, `Jerome01`, `BC05_sistine_chapel`, `bc05_1`, `bc05_2`, `bc05_4`, `bc05_5`, `Mantis1`, `Mantis2`, `Mantis3`, `Mantis4`, `Aphid1`, `Aphid2`, `Aphid3`, `Aphid4`, `Python1`, `Python2`, `Python3`, `Python4`, `Komodo1`, `Komodo2`, `Komodo3`, `Komodo4`, `Kimodo 2`, `Kimodo 3`, `Kimodo 4`, `Cephius`, `Stocks01` |
| Groups | `FG_TYRANT`, `FG_NEW_VEGAS` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Group/spawn-list event: subject 131, op 3, value 0 (Waypoint 2 (tag 0), point 0)

**Action**

- Show/update HUD contact: contact/list 0, subtype 7, param 131

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Group/spawn-list event: subject 131, op 2, value 327680 (Waypoint 0 (tag 5), point 0)
- Variable comparison: subject variable group 21, variable 20, op 3, value 3

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 7, param 131
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 37
- Play dialog: PLAYER.SCR, line/variant 198
- Set/add variable: variable group 16, variable 428, subtype 0, value 1
- Set/add variable: variable group 16, variable 429, subtype 0, value 2

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 20, op 2, value 2

**Action**

- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 3

**Trigger**

- Group/spawn-list event: subject 131, op 4, value 0 (Waypoint 2 (tag 0), point 0) (flags 2)

**Action**

- Group/spawn-list action: spawn list/group 280, subtype 0

## Waypoints

### Waypoint 0

- Tag: `5`
- Members: `Shuttle_Small (object 0, id 194, starts at point 0)`, `Shuttle_Small (object 1, id 195, starts at point 0)`, `Shuttle_Small (object 2, id 196, starts at point 0)`, `Shuttle_Small (object 3, id 197, starts at point 0)`, `Shuttle_Small (object 4, id 198, starts at point 0)`, `Shuttle_Small (object 5, id 200, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1209.72, 22.67, 1747.07) | None |
| 1 | (-1304.86, -476.30, -1110.63) | None |
| 2 | (-355.58, -1136.79, -2836.09) | None |
| 3 | (-79.47, -1138.52, -3464.38) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 1

- Tag: `151`
- Members: `Independent_Merc_Piranha (object 6, id 600, starts at point 0)`, `Independent_Merc_Piranha (object 7, id 601, starts at point 0)`, `Independent_Merc_Piranha (object 8, id 602, starts at point 0)`, `Independent_Merc_Piranha (object 9, id 603, starts at point 0)`, `Independent_Merc_Piranha (object 10, id 604, starts at point 0)`, `Independent_Merc_Piranha (object 11, id 605, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-76.07, -1071.36, -191.84) | None |

### Waypoint 2

- Tag: `0`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1357.00, 8.01, -2256.00) | None |

## Spawn Lists

### Spawn List 0

- ID: `280`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 5 | id 131 | None |
| 2 | 6 | id 336 | None |
| 3 | 6 | id 337 | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Shuttle_Small` | 194 | Interactive | -1971.15,0.00,2896.35 | 201,0,0 | group/role: FG_TYRANT / 0; alias: Jerome02; waypoint: Waypoint 0 (tag 5, 4 point(s)), starting point 0, arrival event value 327680 |
| 1 | `Shuttle_Small` | 195 | Interactive | -1868.14,0.00,2896.34 | 201,0,0 | group/role: FG_TYRANT / 0; alias: Jerome03; waypoint: Waypoint 0 (tag 5, 4 point(s)), starting point 0, arrival event value 327680 |
| 2 | `Shuttle_Small` | 196 | Interactive | -2065.57,0.00,2784.66 | 201,0,0 | group/role: FG_TYRANT / 0; alias: Jerome04; waypoint: Waypoint 0 (tag 5, 4 point(s)), starting point 0, arrival event value 327680 |
| 3 | `Shuttle_Small` | 197 | Interactive | -1988.32,0.00,2784.66 | 201,0,0 | group/role: FG_TYRANT / 0; alias: Jerome05; waypoint: Waypoint 0 (tag 5, 4 point(s)), starting point 0, arrival event value 327680 |
| 4 | `Shuttle_Small` | 198 | Interactive | -1893.89,0.00,2803.27 | 201,0,0 | group/role: FG_TYRANT / 0; alias: Jerome06; waypoint: Waypoint 0 (tag 5, 4 point(s)), starting point 0, arrival event value 327680 |
| 5 | `Shuttle_Small` | 200 | Interactive | -2054.45,0.00,2903.87 | 201,0,0 | group/role: FG_TYRANT / 0; alias: Jerome01; waypoint: Waypoint 0 (tag 5, 4 point(s)), starting point 0, arrival event value 327680 |
| 6 | `Independent_Merc_Piranha` | 600 | Interactive | -89.87,-1177.85,-407.34 | 0,0,0 | group/role: FG_NEW_VEGAS / 0; waypoint: Waypoint 1 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 7 | `Independent_Merc_Piranha` | 601 | Interactive | -71.83,-1177.85,-412.92 | 0,0,0 | group/role: FG_NEW_VEGAS / 0; waypoint: Waypoint 1 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 8 | `Independent_Merc_Piranha` | 602 | Interactive | -46.07,-1177.85,-412.92 | 0,0,0 | group/role: FG_NEW_VEGAS / 0; waypoint: Waypoint 1 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 9 | `Independent_Merc_Piranha` | 603 | Interactive | -89.87,-1177.85,-438.07 | 0,0,0 | group/role: FG_NEW_VEGAS / 0; waypoint: Waypoint 1 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 10 | `Independent_Merc_Piranha` | 604 | Interactive | -74.41,-1177.85,-438.07 | 0,0,0 | group/role: FG_NEW_VEGAS / 0; waypoint: Waypoint 1 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 11 | `Independent_Merc_Piranha` | 605 | Interactive | -53.80,-1177.85,-440.86 | 0,0,0 | group/role: FG_NEW_VEGAS / 0; waypoint: Waypoint 1 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
