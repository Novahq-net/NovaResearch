# Tachyon: The Fringe GALS02B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `GALS02B.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `(none)` |
| Region | 2 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 6 |
| Events | 14 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Void_Pirate_Fighter` |
| Scripts | `VOIDL.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `bfge_02`, `BFGF_03`, `BFGE_03` |
| Aliases | `stocks04`, `Jerome07`, `Jerome08`, `Jerome09`, `Jerome10`, `Jerome11`, `Jerome12`, `stocks03`, `stocks02`, `stocks01` |
| Groups | `FG_BOA`, `FG_COBRA` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 11, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 69, subtype 2
- Group/spawn-list action: spawn list/group 70, subtype 2

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (join 1)
- Group/spawn-list event: subject 69, op 0, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 7, param 69
- Show/update HUD contact: contact/list 0, subtype 7, param 70
- Object spawn/action: Void_Pirate_Fighter (object 0, id 122), subtype 14

### Event 2

**Trigger**

- Group/spawn-list event: subject 69, op 2, value 65536 (Waypoint 2 (tag 1), point 0) (join 2)
- Group/spawn-list event: subject 70, op 2, value 131072 (Waypoint 1 (tag 2), point 0) (join 2)

**Action**

- Play dialog: VOIDL.SCR, line/variant 1

### Event 3

**Trigger**

- Group/spawn-list event: subject 69, op 2, value 65538 (Waypoint 2 (tag 1), point 2)

**Action**

- Group/spawn-list action: spawn list/group 69, subtype 4, param 9
- Group/spawn-list action: spawn list/group 70, subtype 4, param 9
- Hide/remove HUD contact: contact/list 0, subtype 7, param 69
- Hide/remove HUD contact: contact/list 0, subtype 7, param 70
- Show/update HUD contact: contact/list 0, subtype 1, param 69
- Show/update HUD contact: contact/list 0, subtype 1, param 70
- Object spawn/action: Void_Pirate_Fighter (object 0, id 122), subtype 15

### Event 4

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 3

**Action**

- Group/spawn-list action: spawn list/group 69, subtype 8, param 196608 (Waypoint 0 (tag 3), point 0)
- Group/spawn-list action: spawn list/group 70, subtype 8, param 196608 (Waypoint 0 (tag 3), point 0)

### Event 5

**Trigger**

- Object event: subject Void_Pirate_Fighter (object 0, id 122), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 6

**Trigger**

- Object event: subject Void_Pirate_Fighter (object 1, id 123), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 7

**Trigger**

- Object event: subject Void_Pirate_Fighter (object 2, id 124), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 8

**Trigger**

- Object event: subject Void_Pirate_Fighter (object 3, id 125), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 9

**Trigger**

- Object event: subject Void_Pirate_Fighter (object 4, id 126), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 10

**Trigger**

- Object event: subject Void_Pirate_Fighter (object 5, id 127), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 11

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 1

**Action**

- Gate state/action: param 3, subtype 3, param 0

### Event 12

**Trigger**

- Group/spawn-list event: subject 69, op 2, value 196611 (Waypoint 0 (tag 3), point 3) (join 2)
- Group/spawn-list event: subject 70, op 2, value 196611 (Waypoint 0 (tag 3), point 3)
- Unknown runtime event: subject 3, op 1, value 0

**Action**

- Group/spawn-list action: spawn list/group 69, subtype 8, param 131072 (Waypoint 1 (tag 2), point 0)
- Group/spawn-list action: spawn list/group 70, subtype 8, param 131072 (Waypoint 1 (tag 2), point 0)

### Event 13

**Trigger**

- Group/spawn-list event: subject 69, op 0, value 0
- Group/spawn-list event: subject 70, op 0, value 0

**Action**

- Set/add variable: variable group 14, variable 410, subtype 0, value 1
- Set/add variable: variable group 14, variable 411, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Play dialog: PLAYER.SCR, line/variant 39
- Show/update HUD contact: contact/list 0, subtype 12, param 20

## Waypoints

### Waypoint 0

- Tag: `3`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (924.92, 87.19, 1568.63) | None |
| 1 | (1191.31, 0.00, 1110.12) | None |
| 2 | (1085.82, 0.00, 512.56) | None |
| 3 | (1185.87, 0.00, 99.50) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 1

- Tag: `2`
- Members: `Void_Pirate_Fighter (object 3, id 125, starts at point 0)`, `Void_Pirate_Fighter (object 4, id 126, starts at point 0)`, `Void_Pirate_Fighter (object 5, id 127, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (528.97, 0.00, 1428.86) | None |
| 1 | (723.02, -40.95, 1472.38) | None |
| 2 | (813.34, -107.63, 1219.97) | None |
| 3 | (664.86, -148.66, 960.03) | None |

### Waypoint 2

- Tag: `1`
- Members: `Void_Pirate_Fighter (object 0, id 122, starts at point 0)`, `Void_Pirate_Fighter (object 1, id 123, starts at point 0)`, `Void_Pirate_Fighter (object 2, id 124, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (450.99, 0.00, 1500.33) | None |
| 1 | (311.08, -40.95, 1712.10) | None |
| 2 | (127.15, -107.63, 1699.04) | None |
| 3 | (44.10, -148.66, 1395.84) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Void_Pirate_Fighter` | 122 | Interactive | 42.13,0.00,951.38 | 53,0,0 | group/role: FG_BOA / 0; alias: Jerome07; waypoint: Waypoint 2 (tag 1, 4 point(s)), starting point 0, arrival event value 65536 |
| 1 | `Void_Pirate_Fighter` | 123 | Interactive | -17.80,0.00,953.35 | 53,0,0 | label: bfge_02; group/role: FG_BOA / 0; alias: Jerome08; waypoint: Waypoint 2 (tag 1, 4 point(s)), starting point 0, arrival event value 65536 |
| 2 | `Void_Pirate_Fighter` | 124 | Interactive | 48.88,0.00,891.15 | 53,0,0 | group/role: FG_BOA / 0; alias: Jerome09; waypoint: Waypoint 2 (tag 1, 4 point(s)), starting point 0, arrival event value 65536 |
| 3 | `Void_Pirate_Fighter` | 125 | Interactive | 64.48,0.00,797.27 | 53,0,0 | label: bfge_02; group/role: FG_COBRA / 0; alias: Jerome10; waypoint: Waypoint 1 (tag 2, 4 point(s)), starting point 0, arrival event value 131072 |
| 4 | `Void_Pirate_Fighter` | 126 | Interactive | 7.86,0.00,787.02 | 53,0,0 | group/role: FG_COBRA / 0; alias: Jerome11; waypoint: Waypoint 1 (tag 2, 4 point(s)), starting point 0, arrival event value 131072 |
| 5 | `Void_Pirate_Fighter` | 127 | Interactive | 70.51,0.00,733.61 | 53,0,0 | group/role: FG_COBRA / 0; alias: Jerome12; waypoint: Waypoint 1 (tag 2, 4 point(s)), starting point 0, arrival event value 131072 |
