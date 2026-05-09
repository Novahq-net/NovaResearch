# Tachyon: The Fringe MYST05B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST05B.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `(none)` |
| Region | 5 |
| Sector ID | 4 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 20 |
| Events | 17 |
| Waypoints | 4 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Demon_Pirate_Fighter`, `1: Cassitor_Assault_Drone`, `2: Skav_Pirate_Manta` |
| Scripts | `PLAYER.SCR`, `DRCAS.SCR`, `BARGH.SCR` |
| Scenes | None |
| Labels | `WRKR1`, `WRKR2` |
| Aliases | `Will_02` |
| Groups | `BARGHEST`, `CONT_046`, `FG_GHOUL`, `FG_GHAST`, `FG_LEMUR`, `FG_ALLIGATOR`, `FG_AFFAIRE` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Object spawn/action: Skav_Pirate_Manta (object 0, id 4), subtype 1, param 1
- Show/update HUD contact: contact/list 0, subtype 2, param 4
- Object spawn/action: Skav_Pirate_Manta (object 0, id 4), subtype 8, param 4
- Play dialog: PLAYER.SCR, line/variant 64
- Object spawn/action: id 10, subtype 6
- Object spawn/action: id 34, subtype 8, param 4

### Event 1

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 64

**Action**

- Group/spawn-list action: spawn list/group 237, subtype 1, param 10
- Group/spawn-list action: spawn list/group 238, subtype 1, param 10

### Event 2

**Trigger**

- Object arrival: Skav_Pirate_Manta (object 0, id 4) reached Waypoint 3 (tag 151), point 3 (raw value 9895939)

**Action**

- Object spawn/action: Skav_Pirate_Manta (object 0, id 4), subtype 9, param 41

### Event 3

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 0, id 4), op 11, value 0 (extra 1, 41; flags 2)

**Action**

- Play dialog: DRCAS.SCR, line/variant 19
- Set runtime trigger variable: variable group 20, variable 1, subtype 0, value 0
- Group/spawn-list action: spawn list/group 187, subtype 1, param 1
- Group/spawn-list action: spawn list/group 139, subtype 1, param 1
- Group/spawn-list action: spawn list/group 243, subtype 1, param 1

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 10

**Action**

- Object spawn/action: Skav_Pirate_Manta (object 0, id 4), subtype 12
- Object spawn/action: Skav_Pirate_Manta (object 0, id 4), subtype 2, param 1

### Event 5

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 0, id 4), op 7, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 2, value 10 (join 1)
- Object event: subject Skav_Pirate_Manta (object 0, id 4), op 2, value 0

**Action**

- Set/add variable: variable group 17, variable 412, subtype 0, value 1
- Set/add variable: variable group 17, variable 413, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Object spawn/action: id 10, subtype 5
- Hide/remove HUD contact: contact/list 0, subtype 2, param 4
- Show/update HUD contact: contact/list 0, subtype 12, param 28

### Event 7

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 3, value 10
- Object event: subject Skav_Pirate_Manta (object 0, id 4), op 2, value 0

**Action**

- Set/add variable: variable group 17, variable 412, subtype 0, value 1
- Set/add variable: variable group 17, variable 413, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 29

### Event 8

**Trigger**

- Object event: subject Cassitor_Assault_Drone (object 1, id 11), op 4, value 100

**Action**

- Object spawn/action: Cassitor_Assault_Drone (object 1, id 11), subtype 7
- Object spawn/action: Cassitor_Assault_Drone (object 7, id 47), subtype 7

### Event 9

**Trigger**

- Object event: subject Cassitor_Assault_Drone (object 2, id 13), op 4, value 100

**Action**

- Object spawn/action: Cassitor_Assault_Drone (object 2, id 13), subtype 7

### Event 10

**Trigger**

- Object event: subject Cassitor_Assault_Drone (object 3, id 14), op 4, value 100

**Action**

- Object spawn/action: Cassitor_Assault_Drone (object 3, id 14), subtype 7
- Object spawn/action: Cassitor_Assault_Drone (object 6, id 20), subtype 7

### Event 11

**Trigger**

- Object event: subject Cassitor_Assault_Drone (object 5, id 18), op 4, value 100

**Action**

- Object spawn/action: Cassitor_Assault_Drone (object 5, id 18), subtype 7
- Object spawn/action: id 19, subtype 7

### Event 12

**Trigger**

- Object event: subject 19, op 4, value 100

**Action**

- Object spawn/action: id 19, subtype 7

### Event 13

**Trigger**

- Object event: subject Cassitor_Assault_Drone (object 6, id 20), op 4, value 100

**Action**

- Object spawn/action: Cassitor_Assault_Drone (object 6, id 20), subtype 7

### Event 14

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 19

**Action**

- Play dialog: BARGH.SCR, line/variant 3

### Event 15

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 100

**Action**

- Play dialog: PLAYER.SCR, line/variant 135

### Event 16

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 135

**Action**

- Play dialog: PLAYER.SCR, line/variant 136

## Waypoints

### Waypoint 0

- Tag: `154`
- Members: `Demon_Pirate_Fighter (object 12, id 52, starts at point 0)`, `Demon_Pirate_Fighter (object 13, id 53, starts at point 0)`, `Demon_Pirate_Fighter (object 14, id 54, starts at point 0)`, `Demon_Pirate_Fighter (object 15, id 55, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-473.94, 0.00, 603.10) | None |
| 1 | (503.07, 0.00, 1594.80) | None |
| 2 | (1434.42, 0.00, 841.11) | None |
| 3 | (-455.68, 0.00, 176.67) | None |
| 4 | (-136.10, 0.00, 5045.92) | None |

### Waypoint 1

- Tag: `152`
- Members: `Cassitor_Assault_Drone (object 7, id 47, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2584.80, 879.00, 0.00) | None |
| 1 | (0.00, 2338.40, 3215.60) | None |
| 2 | (0.00, 880.86, 4361.22) | None |
| 3 | (0.00, -310.07, 3444.73) | None |
| 4 | (0.00, 116.53, 1955.43) | None |
| 5 | (-1819.72, 0.00, 4821.77) | None |
| 6 | (-2121.08, 0.00, 2505.50) | None |
| 7 | (-1437.23, 0.00, 1687.25) | None |

### Waypoint 2

- Tag: `153`
- Members: `Demon_Pirate_Fighter (object 8, id 48, starts at point 0)`, `Demon_Pirate_Fighter (object 9, id 49, starts at point 0)`, `Demon_Pirate_Fighter (object 10, id 50, starts at point 0)`, `Demon_Pirate_Fighter (object 11, id 51, starts at point 0)`, `Demon_Pirate_Fighter (object 16, id 56, starts at point 0)`, `Demon_Pirate_Fighter (object 17, id 57, starts at point 0)`, `Demon_Pirate_Fighter (object 18, id 58, starts at point 0)`, `Demon_Pirate_Fighter (object 19, id 59, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-3410.92, 754.83, 0.00) | None |
| 1 | (809.35, 547.88, 1368.54) | None |
| 2 | (222.08, 699.64, 0.00) | None |
| 3 | (0.00, 900.90, 388.70) | None |
| 4 | (0.00, 995.29, 1309.90) | None |
| 5 | (0.00, 1278.45, 2491.82) | None |
| 6 | (0.00, 221.31, 4143.02) | None |
| 7 | (0.00, 259.07, 1779.19) | None |

### Waypoint 3

- Tag: `151`
- Members: `Skav_Pirate_Manta (object 0, id 4, starts at point 0)`, `Cassitor_Assault_Drone (object 1, id 11, starts at point 0)`, `Cassitor_Assault_Drone (object 2, id 13, starts at point 0)`, `Cassitor_Assault_Drone (object 3, id 14, starts at point 0)`, `Cassitor_Assault_Drone (object 4, id 17, starts at point 0)`, `Cassitor_Assault_Drone (object 5, id 18, starts at point 0)`, `Cassitor_Assault_Drone (object 6, id 20, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-801.53, 472.17, 238.00) | None |
| 1 | (-901.88, 672.66, 499.86) | None |
| 2 | (140.26, 623.49, 639.23) | None |
| 3 | (142.40, 506.93, 869.40) | None; listened by Event 2 for Skav_Pirate_Manta (object 0, id 4) |

## Spawn Lists

### Spawn List 0

- ID: `237`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 9 | none | None |
| 1 | 0 | none | None |

### Spawn List 1

- ID: `238`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 2

- ID: `187`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | id 34 | None |
| 1 | 0 | none | None |

### Spawn List 3

- ID: `139`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | id 34 | None |
| 1 | 0 | none | None |

### Spawn List 4

- ID: `243`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | id 34 | None |
| 1 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Skav_Pirate_Manta` | 4 | Interactive | -1162.01,0.00,-678.31 | 0,0,0 | alias: Will_02; secondary groups: CONT_046, BARGHEST; waypoint: Waypoint 3 (tag 151, 4 point(s)), starting point 0, arrival event value 9895936 |
| 1 | `Cassitor_Assault_Drone` | 11 | Interactive | 3965.88,420.61,10585.97 | 0,0,0 | group/role: FG_GHOUL / 0; waypoint: Waypoint 3 (tag 151, 4 point(s)), starting point 0, arrival event value 9895936 |
| 2 | `Cassitor_Assault_Drone` | 13 | Interactive | 4328.25,420.61,10581.81 | 0,0,0 | group/role: FG_GHOUL / 0; waypoint: Waypoint 3 (tag 151, 4 point(s)), starting point 0, arrival event value 9895936 |
| 3 | `Cassitor_Assault_Drone` | 14 | Interactive | 4142.02,420.61,10457.65 | 0,0,0 | group/role: FG_GHOUL / 0; waypoint: Waypoint 3 (tag 151, 4 point(s)), starting point 0, arrival event value 9895936 |
| 4 | `Cassitor_Assault_Drone` | 17 | Interactive | 5471.49,480.01,9021.11 | 0,0,0 | group/role: FG_GHAST / 0; waypoint: Waypoint 3 (tag 151, 4 point(s)), starting point 0, arrival event value 9895936 |
| 5 | `Cassitor_Assault_Drone` | 18 | Interactive | 5194.67,420.61,10671.75 | 0,0,0 | group/role: FG_GHAST / 0; waypoint: Waypoint 3 (tag 151, 4 point(s)), starting point 0, arrival event value 9895936 |
| 6 | `Cassitor_Assault_Drone` | 20 | Interactive | 5301.40,420.61,10439.92 | 0,0,0 | group/role: FG_GHAST / 0; waypoint: Waypoint 3 (tag 151, 4 point(s)), starting point 0, arrival event value 9895936 |
| 7 | `Cassitor_Assault_Drone` | 47 | Interactive | 5380.17,410.23,10560.08 | 0,0,0 | group/role: FG_GHAST / 0; waypoint: Waypoint 1 (tag 152, 8 point(s)), starting point -1 |
| 8 | `Demon_Pirate_Fighter` | 48 | Interactive | -3341.22,0.00,9585.43 | 0,0,0 | group/role: FG_LEMUR / 0; waypoint: Waypoint 2 (tag 153, 8 point(s)), starting point 0, arrival event value 10027008 |
| 9 | `Demon_Pirate_Fighter` | 49 | Interactive | -3214.52,0.00,9551.03 | 0,0,0 | group/role: FG_LEMUR / 0; waypoint: Waypoint 2 (tag 153, 8 point(s)), starting point 0, arrival event value 10027008 |
| 10 | `Demon_Pirate_Fighter` | 50 | Interactive | -3008.62,0.00,9602.63 | 0,0,0 | group/role: FG_LEMUR / 0; waypoint: Waypoint 2 (tag 153, 8 point(s)), starting point 0, arrival event value 10027008 |
| 11 | `Demon_Pirate_Fighter` | 51 | Interactive | -2771.05,0.00,9637.04 | 0,0,0 | group/role: FG_LEMUR / 0; waypoint: Waypoint 2 (tag 153, 8 point(s)), starting point 0, arrival event value 10027008 |
| 12 | `Demon_Pirate_Fighter` | 52 | Interactive | -664.57,0.00,9740.25 | 0,0,0 | group/role: FG_ALLIGATOR / 0; waypoint: Waypoint 0 (tag 154, 5 point(s)), starting point 0, arrival event value 10092544 |
| 13 | `Demon_Pirate_Fighter` | 53 | Interactive | -506.18,0.00,9723.05 | 0,0,0 | group/role: FG_ALLIGATOR / 0; waypoint: Waypoint 0 (tag 154, 5 point(s)), starting point 0, arrival event value 10092544 |
| 14 | `Demon_Pirate_Fighter` | 54 | Interactive | -300.29,0.00,9723.05 | 0,0,0 | group/role: FG_ALLIGATOR / 0; waypoint: Waypoint 0 (tag 154, 5 point(s)), starting point 0, arrival event value 10092544 |
| 15 | `Demon_Pirate_Fighter` | 55 | Interactive | -126.07,0.00,9723.05 | 0,0,0 | group/role: FG_ALLIGATOR / 0; waypoint: Waypoint 0 (tag 154, 5 point(s)), starting point 0, arrival event value 10092544 |
| 16 | `Demon_Pirate_Fighter` | 56 | Interactive | 2012.09,0.00,9447.82 | 0,0,0 | group/role: FG_AFFAIRE / 0; waypoint: Waypoint 2 (tag 153, 8 point(s)), starting point 0, arrival event value 10027008 |
| 17 | `Demon_Pirate_Fighter` | 57 | Interactive | 2170.47,0.00,9430.62 | 0,0,0 | group/role: FG_AFFAIRE / 0; waypoint: Waypoint 2 (tag 153, 8 point(s)), starting point 0, arrival event value 10027008 |
| 18 | `Demon_Pirate_Fighter` | 58 | Interactive | 2328.86,0.00,9396.21 | 0,0,0 | group/role: FG_AFFAIRE / 0; waypoint: Waypoint 2 (tag 153, 8 point(s)), starting point 0, arrival event value 10027008 |
| 19 | `Demon_Pirate_Fighter` | 59 | Interactive | 2518.91,0.00,9379.01 | 0,0,0 | group/role: FG_AFFAIRE / 0; waypoint: Waypoint 2 (tag 153, 8 point(s)), starting point 0, arrival event value 10027008 |
