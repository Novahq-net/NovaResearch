# Tachyon: The Fringe NEUT01A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT01A.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 4 |
| Events | 8 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Hvy_Freighter`, `1: Bora_Light_Freighter`, `2: Medical_Frigate` |
| Scripts | `HONOR.SCR` |
| Scenes | None |
| Labels | `MISHK`, `FakeJake`, `Daymir` |
| Aliases | `Courage`, `kwi03_7`, `Jerome26`, `Jerome25`, `Jerome24`, `Jerome22`, `Jerome21`, `Jerome20`, `kevin01`, `Intrepid`, `kwI03_10`, `SHIP1_HYPER`, `ohshit`, `SHIP2_HYPER`, `SHIP3_HYPER` |
| Groups | `DROMEDARY`, `CONT_002`, `FINDER`, `CONT_030`, `BOLD`, `CONT_004`, `TRAVELER`, `CONT_028` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Gate state/action: param 67, subtype 3, param 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 12, subtype 0, value 0
- Mission objective/state: param 65542, subtype 0, param 0
- Show/update HUD contact: contact/list 0, subtype 9, param 19
- Show/update HUD contact: contact/list 0, subtype 9, param 22
- Show/update HUD contact: contact/list 0, subtype 9, param 23

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 12, op 1, value 20

**Action**

- Play dialog: HONOR.SCR, line/variant 0
- Set runtime trigger variable: variable group 20, variable 12, subtype 1, value 0

### Event 3

**Trigger**

- Object event: subject Bora_Hvy_Freighter (object 2, id 134), op 8, value 0

**Action**

- Set/add variable: variable group 21, variable 2, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 23

### Event 4

**Trigger**

- Object event: subject Bora_Hvy_Freighter (object 3, id 143), op 8, value 0

**Action**

- Set/add variable: variable group 21, variable 4, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 22

### Event 5

**Trigger**

- Object event: subject Medical_Frigate (object 0, id 126), op 8, value 0

**Action**

- Set/add variable: variable group 21, variable 3, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 19

### Event 6

**Trigger**

- Object event: subject Bora_Light_Freighter (object 1, id 694), op 10, value 0

**Action**

- Object spawn/action: Bora_Light_Freighter (object 1, id 694), subtype 4
- Set/add variable: variable group 21, variable 33, subtype 0, value 1

### Event 7

**Trigger**

- Variable comparison: subject variable group 21, variable 34, op 1, value 1

**Action**

- Object spawn/action: Bora_Light_Freighter (object 1, id 694), subtype 3

## Waypoints

### Waypoint 0

- Tag: `3`
- Members: `Bora_Hvy_Freighter (object 2, id 134, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (5854.21, 15.23, -9283.64) | None |
| 1 | (5712.58, 15.23, -9510.58) | on arrival action 1, param -1 |

### Waypoint 1

- Tag: `2`
- Members: `Bora_Hvy_Freighter (object 3, id 143, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (6470.60, 15.23, -9279.59) | None |
| 1 | (6263.40, 15.23, -9738.48) | on arrival action 1, param -1 |

### Waypoint 2

- Tag: `1`
- Members: `Medical_Frigate (object 0, id 126, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (6175.46, 15.23, -9268.59) | None |
| 1 | (6067.63, 15.23, -9533.00) | on arrival action 1, param -1 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Medical_Frigate` | 126 | Interactive | 6372.29,15.23,-8849.01 | 292,0,0 | alias: SHIP1_HYPER; secondary groups: CONT_002, DROMEDARY; waypoint: Waypoint 2 (tag 1, 2 point(s)), starting point 0, arrival event value 65536 |
| 1 | `Bora_Light_Freighter` | 694 | Interactive | 3691.37,0.00,-3841.91 | 127,0,0 | alias: ohshit; secondary groups: CONT_030, FINDER |
| 2 | `Bora_Hvy_Freighter` | 134 | Interactive | 5987.30,15.23,-9031.40 | 302,0,0 | alias: SHIP2_HYPER; secondary groups: CONT_004, BOLD; waypoint: Waypoint 0 (tag 3, 2 point(s)), starting point 0, arrival event value 196608 |
| 3 | `Bora_Hvy_Freighter` | 143 | Interactive | 6572.43,15.23,-9060.47 | 284,0,0 | alias: SHIP3_HYPER; secondary groups: CONT_028, TRAVELER; waypoint: Waypoint 1 (tag 2, 2 point(s)), starting point 0, arrival event value 131072 |
