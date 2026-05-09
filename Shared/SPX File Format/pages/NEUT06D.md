# Tachyon: The Fringe NEUT06D.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT06D.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 5 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 5 |
| Events | 20 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Light_Freighter`, `1: Navigational_Bouy`, `2: Independent_Merc_Piranha`, `3: Independent_Merc_Dart` |
| Scripts | `VENET.SCR`, `MERCI.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFNE_02`, `bfbe_08`, `BFNE_01`, `bfne_09`, `bfbe_01`, `BLACK`, `repar` |
| Aliases | `Todd08`, `Todd09`, `Todd10`, `oside`, `oside_1`, `oside_2`, `bagel`, `bagel_1`, `bagel_2`, `kwB10_01`, `kwB10_02`, `Todd13`, `Todd12`, `Todd02`, `Todd03`, `Todd04`, `Todd05`, `Todd06`, `Todd07`, `will_01`, `kevin01`, `SHIP1_HYPER`, `SHIP2_HYPER`, `SHIP3_HYPER`, `ohshit` |
| Groups | `FG_ENVY`, `FG_SHALE`, `VENETIAN`, `CONT_022` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 2, op 1, value 1

**Action**

- Object spawn/action: Generic_Light_Freighter (object 4, id 4888), subtype 3
- Show/update HUD contact: contact/list 0, subtype 6, param 4888

### Event 1

**Trigger**

- Object event: subject Generic_Light_Freighter (object 4, id 4888), op 9, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 1, subtype 0, value 0
- Set/add variable: variable group 21, variable 12, subtype 0, value 0

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 10

**Action**

- Play dialog: VENET.SCR, line/variant 1

### Event 3

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 1

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 6, param 4888
- Show/update HUD contact: contact/list 0, subtype 9, param 40

### Event 4

**Trigger**

- Object event: subject Generic_Light_Freighter (object 4, id 4888), op 0, value 0 (flags 2)

**Action**

- Play dialog: VENET.SCR, line/variant 8

### Event 5

**Trigger**

- Object arrival: Generic_Light_Freighter (object 4, id 4888) reached Waypoint 2 (tag 251), point 2 (raw value 16449538)

**Action**

- Group/spawn-list action: spawn list/group 152, subtype 1, param 4689
- Group/spawn-list action: spawn list/group 130, subtype 1, param 4689
- Set runtime trigger variable: variable group 20, variable 2, subtype 0, value 0

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 5

**Action**

- Play dialog: MERCI.SCR, line/variant 0

### Event 7

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 40
- Show/update HUD contact: contact/list 0, subtype 2, param 4888

### Event 8

**Trigger**

- Variable comparison: subject variable group 21, variable 12, op 3, value 1
- Group/spawn-list event: subject 152, op 0, value 0

**Action**

- Play dialog: VENET.SCR, line/variant 6

### Event 9

**Trigger**

- Object arrival: Generic_Light_Freighter (object 4, id 4888) reached Waypoint 2 (tag 251), point 3 (raw value 16449539)
- Variable comparison: subject variable group 21, variable 12, op 3, value 1

**Action**

- Play dialog: VENET.SCR, line/variant 6

### Event 10

**Trigger**

- Variable comparison: subject variable group 21, variable 12, op 3, value 1
- Group/spawn-list event: subject 130, op 0, value 0 (join 2)

**Action**

- Play dialog: VENET.SCR, line/variant 6

### Event 11

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 6

**Action**

- Object spawn/action: Generic_Light_Freighter (object 4, id 4888), subtype 4
- Hide/remove HUD contact: contact/list 0, subtype 2, param 4888
- Show/update HUD contact: contact/list 0, subtype 6, param 4888
- Mission objective/state: param 65542, subtype 0, param 0
- Set/add variable: variable group 21, variable 3, subtype 0, value 1

### Event 12

**Trigger**

- Object event: subject Generic_Light_Freighter (object 4, id 4888), op 2, value 0 (join 2)
- Object event: subject Generic_Light_Freighter (object 4, id 4888), op 14, value 27

**Action**

- Set/add variable: variable group 13, variable 408, subtype 0, value 1
- Set/add variable: variable group 13, variable 409, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 2, param 4888
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Mission objective/state: param 65536, subtype 0, param 0
- Set/add variable: variable group 21, variable 12, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 11, param 34

### Event 13

**Trigger**

- Object event: subject Independent_Merc_Piranha (object 2, id 6570), op 0, value 0 (flags 2)
- Object event: subject Independent_Merc_Piranha (object 2, id 6570), op 4, value 100

**Action**

- Play dialog: PLAYER.SCR, line/variant 192

### Event 14

**Trigger**

- Object event: subject 6582, op 0, value 0 (flags 2)
- Object event: subject 6582, op 4, value 100

**Action**

- Object spawn/action: id 6582, subtype 7

### Event 15

**Trigger**

- Object event: subject Independent_Merc_Piranha (object 2, id 6570), op 0, value 0 (flags 2)
- Object event: subject Independent_Merc_Piranha (object 2, id 6570), op 4, value 100

**Action**

- Object spawn/action: Independent_Merc_Piranha (object 2, id 6570), subtype 7

### Event 16

**Trigger**

- Object event: subject Independent_Merc_Dart (object 1, id 6572), op 0, value 0 (flags 2)
- Object event: subject Independent_Merc_Dart (object 1, id 6572), op 4, value 100

**Action**

- Object spawn/action: Independent_Merc_Dart (object 1, id 6572), subtype 7

### Event 17

**Trigger**

- Object event: subject Independent_Merc_Dart (object 0, id 6571), op 0, value 0 (flags 2)
- Object event: subject Independent_Merc_Dart (object 0, id 6571), op 4, value 100

**Action**

- Object spawn/action: Independent_Merc_Dart (object 0, id 6571), subtype 7

### Event 18

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 13, variable 408, op 1, value 1

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 6, param 4888

### Event 19

**Trigger**

- Object event: subject Independent_Merc_Dart (object 0, id 6571), op 2, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 180

## Waypoints

### Waypoint 0

- Tag: `253`
- Members: `Independent_Merc_Dart (object 0, id 6571, starts at point 0)`, `Independent_Merc_Dart (object 1, id 6572, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (7.53, 0.00, 2042.40) | None |
| 1 | (601.75, 0.00, 1427.47) | None |
| 2 | (1033.40, 0.00, 1171.75) | None |
| 3 | (-59.74, 0.00, 3284.45) | None |

### Waypoint 1

- Tag: `252`
- Members: `Independent_Merc_Piranha (object 2, id 6570, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (97.77, -677.29, 2067.94) | None |
| 1 | (501.34, -1046.89, 1404.11) | None |
| 2 | (866.31, -1084.27, 1145.37) | None |
| 3 | (-298.30, -959.40, 3499.13) | None |

### Waypoint 2

- Tag: `251`
- Members: `Generic_Light_Freighter (object 4, id 4888, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1428.38, -992.22, 222.61) | None |
| 1 | (1351.58, -994.86, 558.63) | None |
| 2 | (1269.23, -989.35, 755.68) | None; listened by Event 5 for Generic_Light_Freighter (object 4, id 4888) |
| 3 | (-991.49, -868.34, 4285.56) | on arrival action 1, param -1; listened by Event 9 for Generic_Light_Freighter (object 4, id 4888) |

## Spawn Lists

### Spawn List 0

- ID: `130`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Generic_Light_Freighter (object 4, id 4888) | None |
| 1 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Independent_Merc_Dart` | 6571 | Interactive | -7451.27,403.14,-8000.08 | 128,0,0 | label: BFNE_01; group/role: FG_ENVY / 0; waypoint: Waypoint 0 (tag 253, 4 point(s)), starting point 0, arrival event value 16580608 |
| 1 | `Independent_Merc_Dart` | 6572 | Interactive | -7453.62,403.14,-7870.00 | 128,0,0 | group/role: FG_ENVY / 0; waypoint: Waypoint 0 (tag 253, 4 point(s)), starting point 0, arrival event value 16580608 |
| 2 | `Independent_Merc_Piranha` | 6570 | Interactive | -7451.27,403.14,-8047.27 | 128,0,0 | label: BFNE_01; group/role: FG_SHALE / 0; waypoint: Waypoint 1 (tag 252, 4 point(s)), starting point 0, arrival event value 16515072 |
| 3 | `Navigational_Bouy` | 6839 | Interactive | -2899.76,0.00,2368.14 | 0,0,0 | None |
| 4 | `Generic_Light_Freighter` | 4888 | Interactive | 1498.56,-990.97,-244.77 | 502,0,0 | alias: will_01; secondary groups: CONT_022, VENETIAN; waypoint: Waypoint 2 (tag 251, 4 point(s)), starting point 0, arrival event value 16449536 |
