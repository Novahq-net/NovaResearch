# Tachyon: The Fringe FRON10B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON10B.SPX` |
| Sector | `QUAD_10` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 9 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 1 |
| Events | 7 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Malkar_Sistine_Chapel` |
| Scripts | `MALKR.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `Susan`, `BFGE_01`, `BFGE_1`, `Malkar1` |
| Aliases | `BC05_sistine_chapel`, `Susan Bradley` |
| Groups | `SISTINE_CHAPEL` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Variable comparison: subject variable group 21, variable 4, op 1, value 1

**Action**

- Object spawn/action: Malkar_Sistine_Chapel (object 0, id 1138), subtype 3

### Event 1

**Trigger**

- Variable comparison: subject variable group 21, variable 30, op 1, value 1
- Variable comparison: subject variable group 21, variable 31, op 1, value 1

**Action**

- Object spawn/action: Malkar_Sistine_Chapel (object 0, id 1138), subtype 5
- Object spawn/action: Malkar_Sistine_Chapel (object 0, id 1138), subtype 13, param 9895937
- Play dialog: MALKR.SCR, line/variant 5
- Show/update HUD contact: contact/list 0, subtype 9, param 15

### Event 2

**Trigger**

- Object event: subject Malkar_Sistine_Chapel (object 0, id 1138), op 15, value 0

**Action**

- Set/add variable: variable group 21, variable 30, subtype 0, value 1

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 31, subtype 0, value 1

### Event 4

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 5
- Variable comparison: subject variable group 21, variable 21, op 1, value 0

**Action**

- Set/add variable: variable group 16, variable 404, subtype 0, value 1
- Set/add variable: variable group 16, variable 405, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 37
- Broadcast hide/remove contact: contact/list 0, subtype 0, param 15
- Set/add variable: variable group 21, variable 0, subtype 0, value 1
- Set/add variable: variable group 38, variable 1, subtype 0, value 1

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 18, op 1, value 1 (join 2)

**Action**

- Set/add variable: variable group 16, variable 404, subtype 0, value 1
- Set/add variable: variable group 16, variable 405, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 15
- Play dialog: PLAYER.SCR, line/variant 68
- Show/update HUD contact: contact/list 0, subtype 11, param 38

### Event 6

**Trigger**

- Object event: subject Malkar_Sistine_Chapel (object 0, id 1138), op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 18, subtype 0, value 0
- Hide/remove HUD contact: contact/list 0, subtype 10, param 0

## Waypoints

### Waypoint 0

- Tag: `151`
- Members: `Malkar_Sistine_Chapel (object 0, id 1138, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-263.98, 8.60, -246.41) | on arrival activate current object (raw param -1 ignored) |
| 1 | (311.15, -120.74, -2699.87) | None |
| 2 | (917.58, -270.74, -1978.92) | None |
| 3 | (917.29, -395.87, -1611.42) | on arrival activate current object (raw param -1 ignored) |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Malkar_Sistine_Chapel` | 1138 | Interactive | -387.14,0.00,103.17 | 229,0,0 | alias: BC05_sistine_chapel; secondary groups: none, SISTINE_CHAPEL; waypoint: Waypoint 0 (tag 151, 4 point(s)), starting point 0, arrival event value 9895936 |
