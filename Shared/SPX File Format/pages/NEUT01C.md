# Tachyon: The Fringe NEUT01C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT01C.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 7 |
| Entities | 9 |
| Events | 7 |
| Waypoints | 4 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Light_Freighter`, `1: Bora_Carrier`, `2: Independent_Merc_Gar`, `3: Junk_03`, `4: Junk_04`, `5: Shuttle_Medium`, `6: Shuttle_Small` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `MISHK`, `FakeJake`, `Daymir` |
| Aliases | `Courage`, `kwi03_7`, `Jerome26`, `Jerome25`, `Jerome24`, `Jerome22`, `Jerome21`, `Jerome20`, `kevin01`, `Intrepid`, `kwI03_10`, `SHIP1_HYPER`, `ohshit`, `SHIP2_HYPER`, `SHIP3_HYPER` |
| Groups | `TRAVELER`, `CONT_022`, `COURAGE`, `CONT_025`, `INTREPID`, `CONT_004` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0 (join 2)

**Action**

- Set runtime trigger variable: variable group 20, variable 12, subtype 0, value 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Object spawn/action: Shuttle_Medium (object 1, id 339), subtype 8, param 1
- Object spawn/action: Shuttle_Medium (object 1, id 339), subtype 14

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 9, value 0 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 98
- Show/update HUD contact: contact/list 0, subtype 6, param 339
- Mission objective/state: param 65539, subtype 0, param 0

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 2, op 1, value 1

**Action**

- Object spawn/action: Bora_Carrier (object 6, id 365), subtype 3
- Object spawn/action: id 369, subtype 1, param 65
- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 13, variable 418, subtype 0, value 1
- Set/add variable: variable group 13, variable 419, subtype 0, value 2

### Event 4

**Trigger**

- Object event: subject Shuttle_Medium (object 1, id 339), op 7, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0

### Event 5

**Trigger**

- Object arrival: 369 reached Waypoint 1 (tag 204), point 1 (raw value 13369345)

**Action**

- Object spawn/action: id 369, subtype 9, param 184

### Event 6

**Trigger**

- Object event: subject Shuttle_Medium (object 1, id 339), op 6, value 0 (join 2)
- Object event: subject Shuttle_Medium (object 1, id 339), op 2, value 0 (join 2)

**Action**

- Set/add variable: variable group 21, variable 25, subtype 0, value 1

## Waypoints

### Waypoint 0

- Tag: `220`
- Members: `Generic_Light_Freighter (object 8, id 610, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2203.99, 255.70, -5943.00) | None |
| 1 | (6807.56, 255.70, -5940.32) | on arrival play dialog/script or enter gate, param 66 |

### Waypoint 1

- Tag: `204`
- Members: `Bora_Carrier (object 6, id 365, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (6420.62, -580.17, -7858.38) | None |
| 1 | (5113.50, -580.17, -5819.88) | None; listened by Event 5 for id 369 |
| 2 | (5113.50, -580.17, -1706.66) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 2

- Tag: `202`
- Members: `Shuttle_Medium (object 1, id 339, starts at point 1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (4790.50, 258.18, -7975.68) | None |
| 1 | (5327.35, 258.18, -7959.73) | on arrival play dialog/script or enter gate, param 65 |
| 2 | (6210.31, 0.00, -9351.77) | None |

### Waypoint 3

- Tag: `201`
- Members: `Shuttle_Small (object 0, id 313, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1987.00, -149.83, -7195.25) | None |
| 1 | (1978.99, -149.83, -4292.96) | None |
| 2 | (-123.80, -149.83, -4196.28) | None |
| 3 | (120.48, -153.88, -6830.48) | None |
| 4 | (911.96, -149.83, -7411.88) | None |
| 5 | (8601.41, -149.83, -7421.58) | on arrival play dialog/script or enter gate, param 66 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Shuttle_Small` | 313 | Interactive | 1994.85,0.00,-7615.14 | 0,0,0 | secondary groups: CONT_022, TRAVELER; waypoint: Waypoint 3 (tag 201, 6 point(s)), starting point -1 |
| 1 | `Shuttle_Medium` | 339 | Interactive | 4695.11,261.32,-7972.65 | 128,0,0 | alias: Courage; secondary groups: CONT_025, COURAGE; waypoint: Waypoint 2 (tag 202, 3 point(s)), starting point 1, arrival event value 13238273 |
| 2 | `Junk_04` | 608 | Object | 1125.38,234.55,-6240.62 | 0,405,501 | Scale/Radius: 1.00 |
| 3 | `Junk_03` | 609 | Object | 1142.07,252.94,-6237.36 | 0,0,0 | Scale/Radius: 1.00 |
| 4 | `Independent_Merc_Gar` | 613 | Interactive | 1222.72,229.26,-6059.68 | 441,0,0 | None |
| 5 | `Independent_Merc_Gar` | 614 | Interactive | 1233.78,229.26,-6046.91 | 441,0,0 | None |
| 6 | `Bora_Carrier` | 365 | Interactive | 4856.04,-567.27,-9225.88 | 462,0,0 | alias: Intrepid; secondary groups: CONT_025, INTREPID; waypoint: Waypoint 1 (tag 204, 3 point(s)), starting point 0, arrival event value 13369344 |
| 7 | `Generic_Light_Freighter` | 606 | Interactive | 1107.73,243.57,-6127.15 | 0,0,0 | secondary groups: CONT_022, none |
| 8 | `Generic_Light_Freighter` | 610 | Interactive | 1222.39,254.68,-5942.60 | 128,0,0 | secondary groups: CONT_004, none; waypoint: Waypoint 0 (tag 220, 2 point(s)), starting point -1 |
