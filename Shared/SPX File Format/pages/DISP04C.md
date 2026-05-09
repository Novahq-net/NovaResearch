# Tachyon: The Fringe DISP04C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP04C.SPX` |
| Sector | `QUAD_04` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 3 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 11 |
| Events | 13 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Cruiser`, `1: Satellite`, `2: Spy_Probe`, `3: Bora_Battleaxe` |
| Scripts | `CANST.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFNE_01`, `CLEON`, `SPIKE` |
| Aliases | `Coward`, `spy_1`, `SPIKE` |
| Groups | `QUASAR`, `CONT_054`, `CONT_005`, `RESPECT`, `PLEDGE` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 3008

**Action**

- Set runtime trigger variable: variable group 20, variable 19, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 3
- Variable comparison: subject variable group 0, variable 4, op 1, value 3008

**Action**

- Play dialog: CANST.SCR, line/variant 5
- Set runtime trigger variable: variable group 20, variable 19, subtype 1, value 0

### Event 2

**Trigger**

- Object event: subject Bora_Battleaxe (object 0, id 34), op 15, value 0

**Action**

- Object spawn/action: Bora_Battleaxe (object 0, id 34), subtype 2, param 2

### Event 3

**Trigger**

- Object event: subject Spy_Probe (object 1, id 125), op 2, value 0

**Action**

- Object spawn/action: Satellite (object 8, id 126), subtype 0
- Show/update HUD contact: contact/list 0, subtype 0, param 126

### Event 4

**Trigger**

- Variable comparison: subject variable group 21, variable 12, op 1, value 1

**Action**

- Object spawn/action: Satellite (object 2, id 127), subtype 0
- Object spawn/action: Satellite (object 3, id 128), subtype 0
- Object spawn/action: Satellite (object 4, id 129), subtype 0
- Object spawn/action: Satellite (object 5, id 130), subtype 0
- Object spawn/action: Satellite (object 6, id 131), subtype 0
- Object spawn/action: Satellite (object 7, id 134), subtype 0
- Show/update HUD contact: contact/list 0, subtype 0, param 127

### Event 5

**Trigger**

- Object event: subject Satellite (object 8, id 126), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Satellite (object 8, id 126), subtype 7

### Event 6

**Trigger**

- Object event: subject Satellite (object 2, id 127), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Satellite (object 2, id 127), subtype 7

### Event 7

**Trigger**

- Object event: subject Satellite (object 2, id 127), op 2, value 0

**Action**

- Object spawn/action: Satellite (object 3, id 128), subtype 7
- Object spawn/action: Satellite (object 4, id 129), subtype 7
- Object spawn/action: Satellite (object 5, id 130), subtype 7
- Object spawn/action: Satellite (object 6, id 131), subtype 7
- Object spawn/action: Satellite (object 7, id 134), subtype 7
- Play dialog: PLAYER.SCR, line/variant 125

### Event 8

**Trigger**

- Object event: subject Satellite (object 7, id 134), op 2, value 0

**Action**

- Object spawn/action: Bora_Cruiser (object 9, id 124), subtype 3
- Object spawn/action: Bora_Cruiser (object 10, id 135), subtype 3
- Set runtime trigger variable: variable group 20, variable 8, subtype 0, value 0

### Event 9

**Trigger**

- Variable comparison: subject variable group 20, variable 8, op 1, value 120

**Action**

- Object spawn/action: Bora_Cruiser (object 9, id 124), subtype 5
- Object spawn/action: Bora_Cruiser (object 10, id 135), subtype 5

### Event 10

**Trigger**

- Object event: subject Satellite (object 8, id 126), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 12, subtype 0, value 1

### Event 11

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 125

**Action**

- Play dialog: PLAYER.SCR, line/variant 146

### Event 12

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 146

**Action**

- Play dialog: PLAYER.SCR, line/variant 188

## Waypoints

### Waypoint 0

- Tag: `202`
- Members: `Bora_Cruiser (object 10, id 135, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2286.92, 0.00, 4709.44) | None |
| 1 | (2945.95, 0.00, 2592.44) | None |
| 2 | (2182.25, 0.00, 668.34) | None |
| 3 | (934.90, 0.00, -843.70) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 1

- Tag: `201`
- Members: `Bora_Cruiser (object 9, id 124, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-651.11, 0.00, 5467.32) | None |
| 1 | (-816.20, 0.00, 3215.53) | None |
| 2 | (-1090.60, 0.00, 530.96) | on arrival activate current object (raw param -1 ignored) |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Bora_Battleaxe` | 34 | Interactive | -907.09,0.00,339.83 | 148,0,0 | alias: spy_1; secondary groups: CONT_054, QUASAR |
| 1 | `Spy_Probe` | 125 | Interactive | 131.11,-251.45,-168.24 | 493,0,0 | secondary groups: CONT_005, none |
| 2 | `Satellite` | 127 | Interactive | 964.83,429.75,6793.07 | 0,0,0 | None |
| 3 | `Satellite` | 128 | Interactive | 993.61,431.38,6913.97 | 0,0,0 | None |
| 4 | `Satellite` | 129 | Interactive | 902.88,422.65,6884.31 | 0,0,0 | None |
| 5 | `Satellite` | 130 | Interactive | 924.57,428.60,6905.82 | 0,0,0 | None |
| 6 | `Satellite` | 131 | Interactive | 958.06,422.41,6913.62 | 0,0,0 | None |
| 7 | `Satellite` | 134 | Interactive | 1023.09,428.11,6895.60 | 0,0,0 | None |
| 8 | `Satellite` | 126 | Interactive | 721.49,-423.14,3652.69 | 0,0,0 | None |
| 9 | `Bora_Cruiser` | 124 | Interactive | 1192.88,562.48,7443.97 | 383,0,0 | secondary groups: none, RESPECT; waypoint: Waypoint 1 (tag 201, 3 point(s)), starting point -1 |
| 10 | `Bora_Cruiser` | 135 | Interactive | 591.23,621.92,6102.82 | 129,0,0 | secondary groups: none, PLEDGE; waypoint: Waypoint 0 (tag 202, 4 point(s)), starting point -1 |
