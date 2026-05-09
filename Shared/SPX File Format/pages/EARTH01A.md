# Tachyon: The Fringe EARTH01A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH01A.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 0 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 3 |
| Events | 15 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Shuttle_Medium` |
| Scripts | `PLAYER.SCR`, `ARGO.SCR`, `DILL.SCR` |
| Scenes | None |
| Labels | `argo`, `bfnf_04`, `bfnf_05`, `bfnf_06`, `bfnf_03`, `bfnf_09`, `bfnf_01`, `bfdnf_05`, `bfnf_02`, `bfnf_08` |
| Aliases | `Todd01` |
| Groups | `CONT_034`, `ARGOSO 914`, `CONT_UNKNOWN` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 1, subtype 0, value 0
- Play scene: unknown index 0, param 0
- Show/update HUD contact: contact/list 0, subtype 6, param 256
- Gate state/action: param 2, subtype 3, param 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 3

**Action**

- Object spawn/action: Shuttle_Medium (object 2, id 256), subtype 12
- Object spawn/action: Shuttle_Medium (object 2, id 256), subtype 14

### Event 2

**Trigger**

- Object arrival: Shuttle_Medium (object 2, id 256) reached Waypoint 0 (tag 3), point 4 (raw value 196612)

**Action**

- Object spawn/action: Shuttle_Medium (object 2, id 256), subtype 2, param 2
- Set/add variable: variable group 21, variable 22, subtype 1, value 1
- Object spawn/action: Shuttle_Medium (object 2, id 256), subtype 15

### Event 3

**Trigger**

- Object event: subject Shuttle_Medium (object 2, id 256), op 2, value 0

**Action**

- Set/add variable: variable group 12, variable 2, subtype 0, value 0
- Set/add variable: variable group 12, variable 6, subtype 0, value 1
- Gate state/action: param 2, subtype 3, param 0
- Set/add variable: variable group 21, variable 22, subtype 0, value 0
- Mark/flash contact: contact/list 0, subtype 6, param 256
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 31

### Event 4

**Trigger**

- Object arrival: Shuttle_Medium (object 2, id 256) reached Waypoint 0 (tag 3), point 3 (raw value 196611)

**Action**

- Gate state/action: param 2, subtype 2, param 0

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 5

**Action**

- Play dialog: PLAYER.SCR, line/variant 20

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 21

**Action**

- Play dialog: ARGO.SCR, line/variant 8

### Event 7

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 33

**Action**

- Play dialog: DILL.SCR, line/variant 22

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 65
- Object arrival: Shuttle_Medium (object 2, id 256) reached Waypoint 0 (tag 3), point 4 (raw value 196612)

**Action**

- Play dialog: DILL.SCR, line/variant 34

### Event 9

**Trigger**

- Object event: subject Shuttle_Medium (object 2, id 256), op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 2, subtype 0, value 0
- Set runtime trigger variable: variable group 20, variable 1, subtype 1, value 0
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Mission objective/state: param 2, subtype 0, param 0

### Event 10

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 3

**Action**

- Play dialog: DILL.SCR, line/variant 20

### Event 11

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 21

**Action**

- Play dialog: PLAYER.SCR, line/variant 36

### Event 12

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 27

**Action**

- Play dialog: DILL.SCR, line/variant 21
- Set runtime trigger variable: variable group 20, variable 2, subtype 1, value 0

### Event 13

**Trigger**

- Object event: subject Shuttle_Medium (object 2, id 256), op 6, value 0

**Action**

- Play dialog: DILL.SCR, line/variant 32
- Set runtime trigger variable: variable group 20, variable 1, subtype 1, value 0
- Mark/flash contact: contact/list 0, subtype 6, param 256
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Mission objective/state: param 2, subtype 0, param 0
- Gate state/action: param 2, subtype 3, param 0

### Event 14

**Trigger**

- Object event: subject Shuttle_Medium (object 2, id 256), op 7, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 6, param 256
- Mission objective/state: param 4, subtype 0, param 0

## Waypoints

### Waypoint 0

- Tag: `3`
- Members: `Shuttle_Medium (object 2, id 256, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1015.96, -695.18, -312.16) | None |
| 1 | (-1229.20, -681.52, -566.00) | None |
| 2 | (-1430.08, -551.62, -271.00) | None |
| 3 | (-1600.37, -292.01, 5.92) | None; listened by Event 4 for Shuttle_Medium (object 2, id 256) |
| 4 | (-1945.38, -292.01, 7.70) | on arrival play dialog/script or enter gate, param 2; listened by Event 2 for Shuttle_Medium (object 2, id 256), Event 8 for Shuttle_Medium (object 2, id 256) |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Shuttle_Medium` | 257 | Interactive | -952.80,-693.19,-174.33 | 320,0,0 | secondary groups: CONT_034, none |
| 1 | `Shuttle_Medium` | 258 | Interactive | -892.80,-693.19,-234.33 | 320,0,0 | secondary groups: CONT_034, none |
| 2 | `Shuttle_Medium` | 256 | Interactive | -949.80,-693.19,-233.33 | 320,0,0 | label: argo; alias: Todd01; secondary groups: CONT_UNKNOWN, ARGOSO 914; waypoint: Waypoint 0 (tag 3, 5 point(s)), starting point 0, arrival event value 196608 |
