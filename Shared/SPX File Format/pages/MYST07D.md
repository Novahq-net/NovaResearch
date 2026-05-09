# Tachyon: The Fringe MYST07D.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST07D.SPX` |
| Sector | `QUAD_07` |
| Backdrop | `(none)` |
| Region | 5 |
| Sector ID | 6 |
| SectorHazardFlags | Twilight fog / fog-radar impairment (0x00000002) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 3 |
| Events | 8 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Luxury_Liner`, `1: Demon_Pirate_Fighter` |
| Scripts | `SIGHT.SCR`, `CROWD.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `pisce`, `minotaur`, `cerbs`, `hydras`, `MPP1` |
| Aliases | `PISCES1`, `PISCES2`, `PISCES3`, `PISCES4`, `stocks02` |
| Groups | `FG_WISP`, `THE_SIGHTSEER` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Set runtime trigger variable: variable group 20, variable 29, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Variable comparison: subject variable group 20, variable 29, op 1, value 3

**Action**

- Object spawn/action: Luxury_Liner (object 1, id 1425), subtype 3
- Set runtime trigger variable: variable group 20, variable 30, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 2, param 1425
- Play dialog: SIGHT.SCR, line/variant 2
- Object spawn/action: Luxury_Liner (object 1, id 1425), subtype 14

### Event 2

**Trigger**

- Object event: subject 766, op 2, value 0 (join 2)
- Object event: subject 767, op 2, value 0
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Play dialog: CROWD.SCR, line/variant 1

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 30, op 2, value 50

**Action**

- Object spawn/action: Luxury_Liner (object 1, id 1425), subtype 4
- Set/add variable: variable group 21, variable 20, subtype 0, value 2
- Hide/remove HUD contact: contact/list 0, subtype 2, param 1425
- Hide/remove HUD contact: contact/list 0, subtype 11, param 0
- Mission objective/state: param 327687, subtype 0, param 0

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 3

**Action**

- Set runtime trigger variable: variable group 20, variable 24, subtype 1, value 0
- Set/add variable: variable group 20, variable 24, subtype 0, value 0
- Object spawn/action: Luxury_Liner (object 2, id 1633), subtype 3
- Show/update HUD contact: contact/list 0, subtype 2, param 1633
- Group/spawn-list action: spawn list/group 186, subtype 0
- Object spawn/action: Luxury_Liner (object 2, id 1633), subtype 14

### Event 5

**Trigger**

- Object event: subject Luxury_Liner (object 2, id 1633), op 9, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 3

**Action**

- Set runtime trigger variable: variable group 20, variable 24, subtype 0, value 0
- Play dialog: PLAYER.SCR, line/variant 59

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 24, op 1, value 6 (flags 1)

**Action**

- Object spawn/action: Luxury_Liner (object 2, id 1633), subtype 4
- Set/add variable: variable group 21, variable 20, subtype 0, value 4
- Hide/remove HUD contact: contact/list 0, subtype 2, param 1633
- Mission objective/state: param 327685, subtype 0, param 0

### Event 7

**Trigger**

- Object event: subject Luxury_Liner (object 1, id 1425), op 16, value 0 (join 2)
- Object event: subject Luxury_Liner (object 2, id 1633), op 16, value 0 (join 2)
- Object event: subject Luxury_Liner (object 1, id 1425), op 6, value 0 (join 2)
- Object event: subject Luxury_Liner (object 2, id 1633), op 6, value 0 (join 2)

**Action**

- Set/add variable: variable group 17, variable 408, subtype 0, value 1
- Set/add variable: variable group 17, variable 409, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 29
- Mark/flash contact: contact/list 0, subtype 2, param 1425

## Waypoints

### Waypoint 0

- Tag: `251`
- Members: `Demon_Pirate_Fighter (object 0, id 1668, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-149.18, 0.00, 240.92) | None |
| 1 | (-57.61, 0.00, 154.04) | None |
| 2 | (45.41, 0.00, 17.51) | on arrival redirect to Waypoint 0 (tag 251), point 0 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Demon_Pirate_Fighter` | 1668 | Interactive | -172.07,0.00,340.21 | 0,0,0 | group/role: FG_WISP / 0; waypoint: Waypoint 0 (tag 251, 3 point(s)), starting point 0, arrival event value 16449536 |
| 1 | `Luxury_Liner` | 1425 | Interactive | 463.65,0.00,408.48 | 195,0,0 | alias: stocks02; secondary groups: none, THE_SIGHTSEER |
| 2 | `Luxury_Liner` | 1633 | Interactive | 56.86,0.00,-1931.11 | 457,0,0 | alias: stocks02; secondary groups: none, THE_SIGHTSEER |
