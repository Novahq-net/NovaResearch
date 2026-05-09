# Tachyon: The Fringe EARTH02B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH02B.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `(none)` |
| Region | 0 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 9 |
| Events | 21 |
| Waypoints | 5 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Heavy_Freighter`, `1: Luxury_Liner`, `2: Generic_Light_Freighter`, `3: Shuttle_Medium` |
| Scripts | `3MRV.SCR`, `OFRT.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `bfnf_03`, `ariv`, `AGT FIGHTER`, `CAPB`, `CAPA`, `ofrt` |
| Aliases | `danc_blowfish1`, `danc_blowfish2`, `danc_blowfish5`, `danc_blowfish3`, `danc_blowfish4`, `Jerome50` |
| Groups | `FG_BORA7`, `CONT_003`, `FG_GALSPAN5`, `ONTARIO`, `CONT_018`, `CONT_035`, `CONT_021`, `CONT_033` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 2, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 1

**Action**

- Play dialog: 3MRV.SCR, line/variant 2

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 3

**Action**

- Object spawn/action: Generic_Light_Freighter (object 4, id 630), subtype 5

### Event 3

**Trigger**

- Object arrival: Generic_Light_Freighter (object 4, id 630) reached Waypoint 4 (tag 4), point 1 (raw value 262145)

**Action**

- Play dialog: OFRT.SCR, line/variant 1

### Event 4

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 2

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 13

### Event 5

**Trigger**

- Object arrival: Generic_Light_Freighter (object 4, id 630) reached Waypoint 4 (tag 4), point 2 (raw value 262146)

**Action**

- Play dialog: OFRT.SCR, line/variant 2

### Event 6

**Trigger**

- Object arrival: Generic_Light_Freighter (object 4, id 630) reached Waypoint 4 (tag 4), point 3 (raw value 262147)

**Action**

- Play dialog: OFRT.SCR, line/variant 4

### Event 7

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 18

**Action**

- Object spawn/action: GalSpan_Heavy_Freighter (object 8, id 1438), subtype 3

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 20

**Action**

- Object spawn/action: Shuttle_Medium (object 3, id 722), subtype 0
- Set runtime trigger variable: variable group 20, variable 2, subtype 1, value 0

### Event 9

**Trigger**

- Object arrival: Generic_Light_Freighter (object 4, id 630) reached Waypoint 4 (tag 4), point 5 (raw value 262149)

**Action**

- Object spawn/action: Generic_Light_Freighter (object 4, id 630), subtype 21, param 6
- Set runtime trigger variable: variable group 20, variable 2, subtype 0, value 0
- Mark/flash contact: contact/list 0, subtype 8, param 13
- Set/add variable: variable group 12, variable 8, subtype 0, value 1

### Event 10

**Trigger**

- Object arrival: Shuttle_Medium (object 3, id 722) reached Waypoint 2 (tag 6), point 3 (raw value 393219)

**Action**

- Set runtime trigger variable: variable group 20, variable 30, subtype 0, value 0

### Event 11

**Trigger**

- Variable comparison: subject variable group 20, variable 30, op 1, value 20

**Action**

- Object spawn/action: Shuttle_Medium (object 3, id 722), subtype 5

### Event 12

**Trigger**

- Object event: subject Generic_Light_Freighter (object 4, id 630), op 4, value 100 (join 2)
- Object event: subject Generic_Light_Freighter (object 4, id 630), op 14, value 25

**Action**

- Object spawn/action: Generic_Light_Freighter (object 4, id 630), subtype 6
- Play dialog: PLAYER.SCR, line/variant 41
- Hide/remove HUD contact: contact/list 0, subtype 9, param 13
- Set/add variable: variable group 12, variable 8, subtype 0, value 1
- Set/add variable: variable group 0, variable 2, subtype 1, value 1500

### Event 13

**Trigger**

- Variable comparison: subject variable group 20, variable 31, op 1, value 65

**Action**

- Group/spawn-list action: spawn list/group 25, subtype 1, param 1

### Event 14

**Trigger**

- Object event: subject Generic_Light_Freighter (object 4, id 630), op 4, value 90

**Action**

- Play dialog: PLAYER.SCR, line/variant 40

### Event 15

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 26

**Action**

- Play dialog: 3MRV.SCR, line/variant 8
- Hide/remove HUD contact: contact/list 0, subtype 9, param 13

### Event 16

**Trigger**

- Object event: subject Generic_Light_Freighter (object 4, id 630), op 3, value 20

**Action**

- Play dialog: 3MRV.SCR, line/variant 6

### Event 17

**Trigger**

- Object event: subject Generic_Light_Freighter (object 4, id 630), op 3, value 100

**Action**

- Play dialog: 3MRV.SCR, line/variant 9

### Event 18

**Trigger**

- Object arrival: Generic_Light_Freighter (object 4, id 630) reached Waypoint 4 (tag 4), point 4 (raw value 262148)

**Action**

- Play dialog: OFRT.SCR, line/variant 5
- Set runtime trigger variable: variable group 20, variable 26, subtype 0, value 0

### Event 19

**Trigger**

- Variable comparison: subject variable group 20, variable 26, op 1, value 20

**Action**

- Play dialog: OFRT.SCR, line/variant 6

### Event 20

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 53

**Action**

- Object spawn/action: id 670, subtype 3

## Waypoints

### Waypoint 0

- Tag: `8`
- Members: `Shuttle_Medium (object 0, id 761, starts at point 0)`, `Shuttle_Medium (object 1, id 762, starts at point 0)`, `Shuttle_Medium (object 2, id 763, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-735.33, 0.00, -229.24) | None |
| 1 | (-639.07, 0.00, -922.48) | None |
| 2 | (-1582.45, 39.07, -1049.89) | None |
| 3 | (-1578.28, 39.07, -1974.97) | None |
| 4 | (-1532.53, 0.00, -2300.33) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 1

- Tag: `7`
- Members: `GalSpan_Heavy_Freighter (object 8, id 1438, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-5332.13, 78.60, -163.67) | None |
| 1 | (-4388.49, 101.23, -760.46) | None |
| 2 | (-3845.33, 101.23, -2190.15) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 2

- Tag: `6`
- Members: `Shuttle_Medium (object 3, id 722, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1506.00, 39.07, -2197.15) | None |
| 1 | (-1505.44, 39.07, -1949.88) | None |
| 2 | (-1037.19, 81.70, -1953.96) | None |
| 3 | (-1039.57, 81.70, -2255.27) | on arrival activate current object (raw param -1 ignored); listened by Event 10 for Shuttle_Medium (object 3, id 722) |
| 4 | (-1053.25, 81.70, -2493.69) | None |
| 5 | (-1445.60, -243.61, -2668.86) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 3

- Tag: `5`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (299.76, -176.00, 722.20) | None |
| 1 | (368.96, 63.00, -592.87) | None |
| 2 | (383.22, 113.01, -877.09) | None |
| 3 | (382.46, 112.99, -1369.37) | on arrival activate current object (raw param -1 ignored) |
| 4 | (382.06, 82.01, -1626.14) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 4

- Tag: `4`
- Members: `Generic_Light_Freighter (object 4, id 630, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-3399.12, 100.00, -1024.32) | None |
| 1 | (-3397.60, 104.69, -917.90) | None; listened by Event 3 for Generic_Light_Freighter (object 4, id 630) |
| 2 | (-3397.79, 124.65, -372.11) | None; listened by Event 5 for Generic_Light_Freighter (object 4, id 630) |
| 3 | (-3402.63, 169.72, 1198.71) | None; listened by Event 6 for Generic_Light_Freighter (object 4, id 630) |
| 4 | (-3417.12, 188.72, 2984.62) | None; listened by Event 18 for Generic_Light_Freighter (object 4, id 630) |
| 5 | (-3432.36, 199.64, 5904.60) | on arrival activate current object (raw param -1 ignored); listened by Event 9 for Generic_Light_Freighter (object 4, id 630) |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Shuttle_Medium` | 761 | Interactive | -1116.67,-234.93,-57.46 | 242,0,0 | group/role: FG_BORA7 / 0; secondary groups: CONT_003, none; waypoint: Waypoint 0 (tag 8, 5 point(s)), starting point 0, arrival event value 524288 |
| 1 | `Shuttle_Medium` | 762 | Interactive | -1092.16,-234.93,-33.34 | 242,0,0 | group/role: FG_BORA7 / 0; secondary groups: CONT_003, none; waypoint: Waypoint 0 (tag 8, 5 point(s)), starting point 0, arrival event value 524288 |
| 2 | `Shuttle_Medium` | 763 | Interactive | -1139.37,-234.93,-43.21 | 242,0,0 | group/role: FG_BORA7 / 0; secondary groups: CONT_003, none; waypoint: Waypoint 0 (tag 8, 5 point(s)), starting point 0, arrival event value 524288 |
| 3 | `Shuttle_Medium` | 722 | Interactive | -1506.00,39.07,-2316.26 | 0,0,0 | group/role: FG_GALSPAN5 / 0; waypoint: Waypoint 2 (tag 6, 6 point(s)), starting point 0, arrival event value 393216 |
| 4 | `Generic_Light_Freighter` | 630 | Interactive | -3399.12,100.00,-1235.57 | 0,0,0 | label: ofrt; group/role: none / 1; secondary groups: CONT_018, ONTARIO; waypoint: Waypoint 4 (tag 4, 6 point(s)), starting point 0, arrival event value 262144 |
| 5 | `Generic_Light_Freighter` | 729 | Interactive | -2045.00,100.00,-2221.33 | 0,0,0 | secondary groups: CONT_035, none |
| 6 | `Generic_Light_Freighter` | 1328 | Interactive | -2045.00,100.00,-2378.13 | 0,0,0 | secondary groups: CONT_021, none |
| 7 | `Luxury_Liner` | 701 | Interactive | -999.68,172.98,-2055.56 | 0,0,0 | secondary groups: CONT_033, none |
| 8 | `GalSpan_Heavy_Freighter` | 1438 | Interactive | -5753.17,78.60,-100.90 | 135,0,0 | waypoint: Waypoint 1 (tag 7, 3 point(s)), starting point 0, arrival event value 458752 |
