# Tachyon: The Fringe FRON05C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON05C.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 4 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 3 |
| Events | 10 |
| Waypoints | 0 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Navigational_Bouy`, `1: Crate_7`, `2: Crate_5` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFGF_05`, `Ripstar`, `BFGE_05`, `Cephius` |
| Aliases | `Kimodo 4`, `Python 2`, `Python 1`, `Python 4`, `Kimodo 3`, `Kimodo 1`, `Kimodo 2`, `Python 3`, `Jerome13`, `Cephius` |
| Groups | `CONT_030`, `CONT_005` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 25, subtype 0, value 1
- Object spawn/action: Navigational_Bouy (object 2, id 1017), subtype 14
- Show/update HUD contact: contact/list 0, subtype 9, param 32
- Play dialog: PLAYER.SCR, line/variant 109
- Show/update HUD contact: contact/list 0, subtype 9, param 46

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 3000 (extra 1, 1017; flags 2)
- Sector/startup condition family: subject 0, op 0, value 109

**Action**

- Play dialog: PLAYER.SCR, line/variant 206

### Event 2

**Trigger**

- Object event: subject Crate_7 (object 1, id 961), op 10, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 181
- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 5

**Action**

- Play dialog: PLAYER.SCR, line/variant 172
- Set runtime trigger variable: variable group 20, variable 1, subtype 0, value 0

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 5

**Action**

- Play dialog: PLAYER.SCR, line/variant 220

### Event 5

**Trigger**

- Object event: subject Crate_5 (object 0, id 811), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Crate_5 (object 0, id 811), subtype 7

### Event 6

**Trigger**

- Object event: subject Crate_5 (object 0, id 811), op 10, value 0 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 110
- Hide/remove HUD contact: contact/list 0, subtype 9, param 46

### Event 7

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 811; flags 2)

**Action**

- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 37
- Set/add variable: variable group 16, variable 418, subtype 0, value 1
- Set/add variable: variable group 16, variable 419, subtype 0, value 2
- Play dialog: PLAYER.SCR, line/variant 111
- Set/add variable: variable group 16, variable 802, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 32
- Object spawn/action: Navigational_Bouy (object 2, id 1017), subtype 15

### Event 8

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 111

**Action**

- Set/add variable: variable group 21, variable 25, subtype 0, value 0

### Event 9

**Trigger**

- Object event: subject Crate_5 (object 0, id 811), op 2, value 0

**Action**

- Set/add variable: variable group 16, variable 418, subtype 0, value 1
- Set/add variable: variable group 16, variable 419, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 11, param 38
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 46
- Hide/remove HUD contact: contact/list 0, subtype 9, param 32

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Crate_5` | 811 | Interactive | -3053.54,-54.18,3168.99 | 0,0,0 | secondary groups: CONT_030, none |
| 1 | `Crate_7` | 961 | Interactive | -3460.72,221.52,2710.96 | 0,0,0 | secondary groups: CONT_005, none |
| 2 | `Navigational_Bouy` | 1017 | Interactive | -3285.84,260.17,3000.85 | 0,0,0 | None |
