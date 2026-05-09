# Tachyon: The Fringe MYST03D.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST03D.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `(none)` |
| Region | 5 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 5 |
| Events | 7 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Cassitor_Assault_Drone`, `1: Skav_Pirate_Manta` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFNE_06` |
| Aliases | `Will_02` |
| Groups | `BARGHEST`, `FG_WIGHT` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Object spawn/action: Skav_Pirate_Manta (object 0, id 186), subtype 1, param 2
- Group/spawn-list action: spawn list/group 239, subtype 1, param 3
- Show/update HUD contact: contact/list 0, subtype 2, param 186
- Play dialog: PLAYER.SCR, line/variant 76
- Object spawn/action: Skav_Pirate_Manta (object 0, id 186), subtype 8, param 4

### Event 1

**Trigger**

- Group/spawn-list event: subject 239, op 0, value 0

**Action**

- Object spawn/action: Skav_Pirate_Manta (object 0, id 186), subtype 2, param 2
- Mission objective/state: param 327684, subtype 0, param 0

### Event 2

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Object spawn/action: Skav_Pirate_Manta (object 0, id 186), subtype 1, param 1
- Object spawn/action: Skav_Pirate_Manta (object 0, id 186), subtype 13, param 16515072
- Hide/remove HUD contact: contact/list 0, subtype 2, param 186

### Event 3

**Trigger**

- Object arrival: Skav_Pirate_Manta (object 0, id 186) reached Waypoint 1 (tag 252), point 2 (raw value 16515074)

**Action**

- Object spawn/action: Skav_Pirate_Manta (object 0, id 186), subtype 2, param 1

### Event 4

**Trigger**

- Group/spawn-list event: subject 239, op 0, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 121

### Event 5

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 121

**Action**

- Play dialog: PLAYER.SCR, line/variant 98

### Event 6

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 0, id 186), op 2, value 0

**Action**

- Set/add variable: variable group 17, variable 412, subtype 0, value 1
- Set/add variable: variable group 17, variable 413, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 11, param 29
- Show/update HUD contact: contact/list 0, subtype 8, param 0

## Waypoints

### Waypoint 0

- Tag: `253`
- Members: `Cassitor_Assault_Drone (object 1, id 198, starts at point 0)`, `Cassitor_Assault_Drone (object 2, id 199, starts at point 0)`, `Cassitor_Assault_Drone (object 3, id 200, starts at point 0)`, `Cassitor_Assault_Drone (object 4, id 201, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (894.41, 0.00, 426.92) | None |
| 1 | (145.26, 0.00, 218.01) | None |
| 2 | (-502.66, 0.00, 212.52) | None |

### Waypoint 1

- Tag: `252`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (713.99, 0.00, 650.28) | None |
| 1 | (291.36, 0.00, 587.68) | None |
| 2 | (-1101.87, 0.00, 432.62) | None; listened by Event 3 for Skav_Pirate_Manta (object 0, id 186) |

### Waypoint 2

- Tag: `251`
- Members: `Skav_Pirate_Manta (object 0, id 186, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-696.64, 0.00, 327.23) | None |
| 1 | (12.18, 0.00, 138.23) | None |
| 2 | (844.08, 0.00, 253.47) | None |
| 3 | (984.14, 0.00, 387.16) | None |

## Spawn Lists

### Spawn List 0

- ID: `239`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Skav_Pirate_Manta` | 186 | Interactive | -1367.25,0.00,912.67 | 0,0,0 | alias: Will_02; secondary groups: none, BARGHEST; waypoint: Waypoint 2 (tag 251, 4 point(s)), starting point 0, arrival event value 16449536 |
| 1 | `Cassitor_Assault_Drone` | 198 | Interactive | 1026.02,0.00,1476.97 | 0,0,0 | label: BFNE_06; group/role: FG_WIGHT / 0; waypoint: Waypoint 0 (tag 253, 3 point(s)), starting point 0, arrival event value 16580608 |
| 2 | `Cassitor_Assault_Drone` | 199 | Interactive | 1142.44,0.00,1482.47 | 0,0,0 | label: BFNE_06; group/role: FG_WIGHT / 0; waypoint: Waypoint 0 (tag 253, 3 point(s)), starting point 0, arrival event value 16580608 |
| 3 | `Cassitor_Assault_Drone` | 200 | Interactive | 1198.12,0.00,1400.01 | 0,0,0 | label: BFNE_06; group/role: FG_WIGHT / 0; waypoint: Waypoint 0 (tag 253, 3 point(s)), starting point 0, arrival event value 16580608 |
| 4 | `Cassitor_Assault_Drone` | 201 | Interactive | 1218.37,0.00,1273.56 | 0,0,0 | label: BFNE_06; group/role: FG_WIGHT / 0; waypoint: Waypoint 0 (tag 253, 3 point(s)), starting point 0, arrival event value 16580608 |
