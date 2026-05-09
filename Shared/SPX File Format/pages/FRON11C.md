# Tachyon: The Fringe FRON11C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON11C.SPX` |
| Sector | `QUAD_11` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 10 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 4 |
| Events | 5 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Red_Pirate_Shrike` |
| Scripts | `PLAYER.SCR`, `REDSA.SCR` |
| Scenes | None |
| Labels | `bfne_05`, `BFBE_04`, `bfne_01`, `bfne_03`, `bfne_02`, `bfne_04`, `bfne_06`, `bfne_08`, `bfne_07`, `bfne_09` |
| Aliases | `BC05_sistine_chapel`, `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1`, `bc05_2`, `bc05_3`, `bc05_5`, `bc05_4`, `Stocks01` |
| Groups | `FG_LUST` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Object spawn/action: Red_Pirate_Shrike (object 0, id 350), subtype 5
- Show/update HUD contact: contact/list 0, subtype 1, param 137
- Play dialog: PLAYER.SCR, line/variant 138
- Object spawn/action: Red_Pirate_Shrike (object 1, id 351), subtype 5

### Event 1

**Trigger**

- Group/spawn-list event: subject 137, op 1, value 50

**Action**

- Play dialog: REDSA.SCR, line/variant 1
- Object spawn/action: Red_Pirate_Shrike (object 2, id 352), subtype 5
- Object spawn/action: Red_Pirate_Shrike (object 3, id 413), subtype 5

### Event 2

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 185

### Event 3

**Trigger**

- Group/spawn-list event: subject 137, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 137
- Mission objective/state: param 262155, subtype 0, param 0

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 34, op 1, value 1

**Action**

- Set/add variable: variable group 16, variable 430, subtype 0, value 1
- Set/add variable: variable group 16, variable 431, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 11, param 38
- Show/update HUD contact: contact/list 0, subtype 8, param 0

## Waypoints

### Waypoint 0

- Tag: `201`
- Members: `Red_Pirate_Shrike (object 0, id 350, starts at point 0)`, `Red_Pirate_Shrike (object 1, id 351, starts at point 0)`, `Red_Pirate_Shrike (object 2, id 352, starts at point 0)`, `Red_Pirate_Shrike (object 3, id 413, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (120.75, 0.00, 7526.46) | None |
| 1 | (-1288.00, -146.86, 6398.52) | None |
| 2 | (658.96, -480.16, 6860.72) | None |
| 3 | (-645.70, -349.80, 3857.95) | None |
| 4 | (479.70, 0.00, 5991.60) | None |
| 5 | (-1969.06, 0.00, 3986.01) | None |

## Spawn Lists

### Spawn List 0

- ID: `137`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Red_Pirate_Shrike` | 350 | Interactive | 648.44,0.00,275.64 | 0,0,0 | label: bfne_04; group/role: FG_LUST / 0; waypoint: Waypoint 0 (tag 201, 6 point(s)), starting point 0, arrival event value 13172736 |
| 1 | `Red_Pirate_Shrike` | 351 | Interactive | 1050.01,0.00,341.06 | 0,0,0 | label: bfne_04; group/role: FG_LUST / 0; waypoint: Waypoint 0 (tag 201, 6 point(s)), starting point 0, arrival event value 13172736 |
| 2 | `Red_Pirate_Shrike` | 352 | Interactive | 2564.03,0.00,6160.86 | 0,0,0 | group/role: FG_LUST / 0; waypoint: Waypoint 0 (tag 201, 6 point(s)), starting point 0, arrival event value 13172736 |
| 3 | `Red_Pirate_Shrike` | 413 | Interactive | 2222.97,0.00,6119.03 | 0,0,0 | label: bfne_04; group/role: FG_LUST / 0; waypoint: Waypoint 0 (tag 201, 6 point(s)), starting point 0, arrival event value 13172736 |
