# Tachyon: The Fringe GALS01B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `GALS01B.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 2 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 6 |
| Events | 4 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Void_Pirate_Fighter` |
| Scripts | `TRISH.SCR` |
| Scenes | None |
| Labels | `bfge_02` |
| Aliases | `stocks01`, `Jerome10`, `Jerome11`, `Jerome09`, `Jerome08`, `Jerome07`, `Jerome12`, `frank05`, `frank06`, `frank07`, `frank08`, `wing_man`, `stocks02`, `stocks03`, `stocks04`, `frank10` |
| Groups | `FG_COBRA`, `FG_BOA` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 9, value 0

**Action**

- Object spawn/action: Void_Pirate_Fighter (object 2, id 124), subtype 14
- Play dialog: TRISH.SCR, line/variant 18
- Show/update HUD contact: contact/list 0, subtype 7, param 69
- Show/update HUD contact: contact/list 0, subtype 7, param 70

### Event 1

**Trigger**

- Group/spawn-list event: subject 70, op 2, value 131074 (Waypoint 0 (tag 2), point 2)

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 7, param 70
- Hide/remove HUD contact: contact/list 0, subtype 7, param 69
- Mission objective/state: param 131073, subtype 0, param 0

### Event 2

**Trigger**

- Object event: subject Void_Pirate_Fighter (object 0, id 122), op 7, value 0
- Object event: subject Void_Pirate_Fighter (object 1, id 123), op 7, value 0
- Object event: subject Void_Pirate_Fighter (object 2, id 124), op 7, value 0
- Object event: subject Void_Pirate_Fighter (object 3, id 125), op 7, value 0
- Object event: subject Void_Pirate_Fighter (object 4, id 126), op 7, value 0
- Object event: subject Void_Pirate_Fighter (object 5, id 127), op 7, value 0

**Action**

- Set/add variable: variable group 21, variable 11, subtype 0, value 1

### Event 3

**Trigger**

- Group/spawn-list event: subject 69, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 70, op 4, value 0 (join 2; flags 2)

**Action**

- Group/spawn-list action: spawn list/group 69, subtype 4, param 9
- Group/spawn-list action: spawn list/group 70, subtype 4, param 9
- Object spawn/action: Void_Pirate_Fighter (object 2, id 124), subtype 15

## Waypoints

### Waypoint 0

- Tag: `2`
- Members: `Void_Pirate_Fighter (object 0, id 122, starts at point 0)`, `Void_Pirate_Fighter (object 1, id 123, starts at point 0)`, `Void_Pirate_Fighter (object 5, id 127, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (338.11, 252.16, 726.78) | None |
| 1 | (-0.30, 89.84, 657.02) | None |
| 2 | (-262.11, 12.01, 785.09) | on arrival play dialog/script or enter gate, param 1 |

### Waypoint 1

- Tag: `1`
- Members: `Void_Pirate_Fighter (object 2, id 124, starts at point 0)`, `Void_Pirate_Fighter (object 3, id 125, starts at point 0)`, `Void_Pirate_Fighter (object 4, id 126, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (306.40, 252.16, 738.85) | None |
| 1 | (-1.41, 89.84, 663.15) | None |
| 2 | (-264.13, 12.01, 792.05) | on arrival play dialog/script or enter gate, param 1 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Void_Pirate_Fighter` | 122 | Interactive | 904.55,427.56,784.16 | 373,489,495 | label: bfge_02; group/role: FG_COBRA / 0; alias: Jerome10; waypoint: Waypoint 0 (tag 2, 3 point(s)), starting point 0, arrival event value 131072 |
| 1 | `Void_Pirate_Fighter` | 123 | Interactive | 875.00,427.56,764.63 | 373,489,495 | group/role: FG_COBRA / 0; alias: Jerome11; waypoint: Waypoint 0 (tag 2, 3 point(s)), starting point 0, arrival event value 131072 |
| 2 | `Void_Pirate_Fighter` | 124 | Interactive | 548.82,336.33,745.58 | 378,489,495 | label: bfge_02; group/role: FG_BOA / 0; alias: Jerome09; waypoint: Waypoint 1 (tag 1, 3 point(s)), starting point 0, arrival event value 65536 |
| 3 | `Void_Pirate_Fighter` | 125 | Interactive | 579.67,336.33,728.98 | 378,489,495 | group/role: FG_BOA / 0; alias: Jerome08; waypoint: Waypoint 1 (tag 1, 3 point(s)), starting point 0, arrival event value 65536 |
| 4 | `Void_Pirate_Fighter` | 126 | Interactive | 577.66,336.33,765.85 | 378,489,495 | group/role: FG_BOA / 0; alias: Jerome07; waypoint: Waypoint 1 (tag 1, 3 point(s)), starting point 0, arrival event value 65536 |
| 5 | `Void_Pirate_Fighter` | 127 | Interactive | 907.35,427.56,747.59 | 373,489,495 | group/role: FG_COBRA / 0; alias: Jerome12; waypoint: Waypoint 0 (tag 2, 3 point(s)), starting point 0, arrival event value 131072 |
