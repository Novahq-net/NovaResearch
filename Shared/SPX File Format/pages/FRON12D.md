# Tachyon: The Fringe FRON12D.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON12D.SPX` |
| Sector | `QUAD_12` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 11 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 8 |
| Events | 8 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Luxury_Liner`, `1: Red_Pirate_Shrike`, `2: Satellite` |
| Scripts | `PLAYER.SCR`, `REDSB.SCR` |
| Scenes | None |
| Labels | `BFNF_01`, `BFGE_01`, `BFNE_02` |
| Aliases | `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1`, `Stocks01` |
| Groups | `FG_PESTILENCE` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 34, subtype 0, value 1
- Object spawn/action: Red_Pirate_Shrike (object 3, id 1378), subtype 1, param 1
- Object spawn/action: Red_Pirate_Shrike (object 4, id 1379), subtype 1, param 1
- Show/update HUD contact: contact/list 0, subtype 1, param 138
- Object spawn/action: id 1366, subtype 8, param 9
- Set runtime trigger variable: variable group 20, variable 29, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 29, op 1, value 2

**Action**

- Play dialog: PLAYER.SCR, line/variant 140

### Event 2

**Trigger**

- Object event: subject Red_Pirate_Shrike (object 4, id 1379), op 0, value 0 (join 2; flags 2)
- Object event: subject Red_Pirate_Shrike (object 3, id 1378), op 0, value 0 (join 2; flags 2)
- Object event: subject Red_Pirate_Shrike (object 3, id 1378), op 2, value 0 (join 2)
- Object event: subject Red_Pirate_Shrike (object 4, id 1379), op 2, value 0 (join 2)

**Action**

- Object spawn/action: Red_Pirate_Shrike (object 5, id 1380), subtype 1, param 1
- Object spawn/action: Red_Pirate_Shrike (object 6, id 1381), subtype 1, param 1

### Event 3

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 140
- Object event: subject Red_Pirate_Shrike (object 5, id 1380), op 0, value 0 (flags 2)
- Variable comparison: subject variable group 21, variable 29, op 1, value 0

**Action**

- Play dialog: REDSB.SCR, line/variant 2
- Set/add variable: variable group 21, variable 29, subtype 0, value 1

### Event 4

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 140
- Object event: subject Red_Pirate_Shrike (object 6, id 1381), op 0, value 0 (flags 2)
- Variable comparison: subject variable group 21, variable 29, op 1, value 0

**Action**

- Play dialog: REDSB.SCR, line/variant 2
- Set/add variable: variable group 21, variable 29, subtype 0, value 1

### Event 5

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 2
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Set/add variable: variable group 16, variable 430, subtype 0, value 1
- Set/add variable: variable group 16, variable 431, subtype 0, value 3
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 37
- Hide/remove HUD contact: contact/list 0, subtype 1, param 138
- Set/add variable: variable group 21, variable 34, subtype 0, value 0

### Event 6

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 2
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Set/add variable: variable group 16, variable 430, subtype 0, value 1
- Set/add variable: variable group 16, variable 431, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 37
- Hide/remove HUD contact: contact/list 0, subtype 1, param 138
- Set/add variable: variable group 21, variable 34, subtype 0, value 0

### Event 7

**Trigger**

- Variable comparison: subject variable group 16, variable 431, op 0, value 1

**Action**

- Object spawn/action: Red_Pirate_Shrike (object 3, id 1378), subtype 19
- Object spawn/action: Red_Pirate_Shrike (object 4, id 1379), subtype 19
- Object spawn/action: Red_Pirate_Shrike (object 5, id 1380), subtype 19
- Object spawn/action: Red_Pirate_Shrike (object 6, id 1381), subtype 19

## Waypoints

### Waypoint 0

- Tag: `201`
- Members: `Red_Pirate_Shrike (object 3, id 1378, starts at point 0)`, `Red_Pirate_Shrike (object 4, id 1379, starts at point 0)`, `Red_Pirate_Shrike (object 5, id 1380, starts at point 0)`, `Red_Pirate_Shrike (object 6, id 1381, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1311.92, 0.00, 117.27) | None |
| 1 | (358.76, 323.78, -472.67) | None |
| 2 | (1964.32, -653.77, -504.33) | None |
| 3 | (2400.89, -255.89, -1140.42) | None |
| 4 | (2832.56, -219.33, -988.89) | None |
| 5 | (3159.10, 0.00, -2000.23) | None |

## Spawn Lists

### Spawn List 0

- ID: `138`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Satellite` | 1318 | Interactive | 1891.52,0.00,258.72 | 0,0,0 | None |
| 1 | `Satellite` | 1319 | Interactive | 1093.38,0.00,3328.85 | 0,0,0 | None |
| 2 | `Satellite` | 1320 | Interactive | 782.99,0.00,-632.22 | 0,0,0 | None |
| 3 | `Red_Pirate_Shrike` | 1378 | Interactive | 3357.48,0.00,-2771.00 | 0,0,0 | label: BFNE_02; group/role: FG_PESTILENCE / 0; waypoint: Waypoint 0 (tag 201, 6 point(s)), starting point 0, arrival event value 13172736 |
| 4 | `Red_Pirate_Shrike` | 1379 | Interactive | 3600.96,0.00,-2804.05 | 0,0,0 | group/role: FG_PESTILENCE / 0; waypoint: Waypoint 0 (tag 201, 6 point(s)), starting point 0, arrival event value 13172736 |
| 5 | `Red_Pirate_Shrike` | 1380 | Interactive | 3874.87,0.00,-2820.58 | 0,0,0 | label: BFNE_02; group/role: FG_PESTILENCE / 0; waypoint: Waypoint 0 (tag 201, 6 point(s)), starting point 0, arrival event value 13172736 |
| 6 | `Red_Pirate_Shrike` | 1381 | Interactive | 4087.91,0.00,-2787.52 | 0,0,0 | label: BFNE_02; group/role: FG_PESTILENCE / 0; waypoint: Waypoint 0 (tag 201, 6 point(s)), starting point 0, arrival event value 13172736 |
| 7 | `Luxury_Liner` | 1317 | Interactive | 694.30,0.00,1522.89 | 0,0,0 | None |
