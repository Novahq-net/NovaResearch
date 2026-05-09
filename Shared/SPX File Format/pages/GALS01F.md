# Tachyon: The Fringe GALS01F.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `GALS01F.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 2 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 9 |
| Events | 8 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Carrier`, `1: GalSpan_Orion`, `2: GalSpan_Phoenix`, `3: Wingman_Ramos` |
| Scripts | `TRISH.SCR` |
| Scenes | None |
| Labels | `bfge_02` |
| Aliases | `stocks01`, `Jerome10`, `Jerome11`, `Jerome09`, `Jerome08`, `Jerome07`, `Jerome12`, `frank05`, `frank06`, `frank07`, `frank08`, `wing_man`, `stocks02`, `stocks03`, `stocks04`, `frank10` |
| Groups | `LAKITA_CELENE`, `FG_LEO`, `FG_FORNAX`, `HYLLUS` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Object event: subject Wingman_Ramos (object 0, id 210), op 15, value 0
- Variable comparison: subject variable group 21, variable 20, op 0, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 0, value 1
- Set/add variable: variable group 14, variable 404, subtype 0, value 1
- Set/add variable: variable group 14, variable 405, subtype 0, value 1
- Set/add variable: variable group 21, variable 25, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 11, param 21
- Set/add variable: variable group 21, variable 23, subtype 0, value 1

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 0, value 0
- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Set/add variable: variable group 21, variable 20, subtype 0, value 1
- Set/add variable: variable group 14, variable 404, subtype 0, value 1
- Set/add variable: variable group 14, variable 405, subtype 0, value 2
- Play dialog: TRISH.SCR, line/variant 6
- Show/update HUD contact: contact/list 0, subtype 12, param 20
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Mission objective/state: param 131077, subtype 0, param 0
- Gate state/action: param 4, subtype 3, param 0

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 9, value 0

**Action**

- Group/spawn-list action: spawn list/group 43, subtype 2
- Group/spawn-list action: spawn list/group 178, subtype 2

### Event 4

**Trigger**

- Group/spawn-list event: subject 178, op 2, value 23003136 (Waypoint 1 (tag 351), point 0)

**Action**

- Group/spawn-list action: spawn list/group 178, subtype 5, param 245
- Group/spawn-list action: spawn list/group 43, subtype 5, param 245

### Event 5

**Trigger**

- Object event: subject GalSpan_Phoenix (object 1, id 246), op 13, value 0 (extra 1, 245; flags 2)
- Object event: subject GalSpan_Phoenix (object 2, id 247), op 13, value 0 (extra 1, 245; flags 2)
- Object event: subject GalSpan_Phoenix (object 4, id 249), op 13, value 0 (extra 1, 245; flags 2)
- Object event: subject GalSpan_Phoenix (object 3, id 248), op 13, value 0 (extra 1, 245; flags 2)

**Action**

- Object spawn/action: GalSpan_Carrier (object 8, id 245), subtype 4

### Event 6

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 23, op 1, value 1

**Action**

- Play dialog: TRISH.SCR, line/variant 5

### Event 7

**Trigger**

- Object event: subject Wingman_Ramos (object 0, id 210), op 2, value 0

**Action**

- Set/add variable: variable group 14, variable 404, subtype 0, value 1
- Set/add variable: variable group 14, variable 405, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 21
- Show/update HUD contact: contact/list 0, subtype 8, param 0

## Waypoints

### Waypoint 0

- Tag: `352`
- Members: `GalSpan_Phoenix (object 1, id 246, starts at point -1)`, `GalSpan_Phoenix (object 2, id 247, starts at point -1)`, `GalSpan_Phoenix (object 3, id 248, starts at point -1)`, `GalSpan_Phoenix (object 4, id 249, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (861.35, 0.00, -44.47) | None |
| 1 | (1373.75, 0.00, 730.41) | None |

### Waypoint 1

- Tag: `351`
- Members: `GalSpan_Orion (object 5, id 251, starts at point -1)`, `GalSpan_Orion (object 6, id 252, starts at point -1)`, `GalSpan_Orion (object 7, id 253, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1175.07, 331.61, 1362.63) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Wingman_Ramos` | 210 | Interactive | 814.21,0.00,340.29 | 337,0,0 | alias: wing_man; secondary groups: none, LAKITA_CELENE |
| 1 | `GalSpan_Phoenix` | 246 | Interactive | 967.45,0.00,-416.85 | 499,0,0 | group/role: FG_LEO / 0; waypoint: Waypoint 0 (tag 352, 2 point(s)), starting point -1 |
| 2 | `GalSpan_Phoenix` | 247 | Interactive | 1019.53,0.00,-411.01 | 499,0,0 | group/role: FG_LEO / 0; waypoint: Waypoint 0 (tag 352, 2 point(s)), starting point -1 |
| 3 | `GalSpan_Phoenix` | 248 | Interactive | 967.45,0.00,-486.87 | 499,0,0 | group/role: FG_LEO / 0; waypoint: Waypoint 0 (tag 352, 2 point(s)), starting point -1 |
| 4 | `GalSpan_Phoenix` | 249 | Interactive | 1021.26,0.00,-486.86 | 499,0,0 | group/role: FG_LEO / 0; waypoint: Waypoint 0 (tag 352, 2 point(s)), starting point -1 |
| 5 | `GalSpan_Orion` | 251 | Interactive | 578.60,334.83,1619.07 | 139,0,0 | group/role: FG_FORNAX / 0; waypoint: Waypoint 1 (tag 351, 1 point(s)), starting point -1 |
| 6 | `GalSpan_Orion` | 252 | Interactive | 620.26,334.83,1613.23 | 139,0,0 | group/role: FG_FORNAX / 0; waypoint: Waypoint 1 (tag 351, 1 point(s)), starting point -1 |
| 7 | `GalSpan_Orion` | 253 | Interactive | 594.22,334.83,1572.39 | 139,0,0 | group/role: FG_FORNAX / 0; waypoint: Waypoint 1 (tag 351, 1 point(s)), starting point -1 |
| 8 | `GalSpan_Carrier` | 245 | Interactive | 1910.17,390.00,1981.92 | 186,0,0 | secondary groups: none, HYLLUS |
