# Tachyon: The Fringe GALS01C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `GALS01C.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 2 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 4 |
| Events | 5 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Shuttle_Medium` |
| Scripts | `AQUAR.SCR` |
| Scenes | None |
| Labels | `bfge_02` |
| Aliases | `stocks01`, `Jerome10`, `Jerome11`, `Jerome09`, `Jerome08`, `Jerome07`, `Jerome12`, `frank05`, `frank06`, `frank07`, `frank08`, `wing_man`, `stocks02`, `stocks03`, `stocks04`, `frank10` |
| Groups | `FG_CENTAURUS`, `AQUARIUS` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 25, op 3, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 6, param 240
- Object spawn/action: GalSpan_Shuttle_Medium (object 3, id 240), subtype 14

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 240; flags 2)

**Action**

- Group/spawn-list action: spawn list/group 260, subtype 2
- Object spawn/action: GalSpan_Shuttle_Medium (object 3, id 240), subtype 5
- Play dialog: AQUAR.SCR, line/variant 0

### Event 2

**Trigger**

- Group/spawn-list event: subject 260, op 2, value 13172738 (Waypoint 0 (tag 201), point 2)
- Object arrival: GalSpan_Shuttle_Medium (object 3, id 240) reached Waypoint 0 (tag 201), point 2 (raw value 13172738)

**Action**

- Group/spawn-list action: spawn list/group 260, subtype 3, param 1
- Object spawn/action: GalSpan_Shuttle_Medium (object 3, id 240), subtype 2, param 1

### Event 3

**Trigger**

- Object event: subject GalSpan_Shuttle_Medium (object 3, id 240), op 2, value 0

**Action**

- Mark/flash contact: contact/list 0, subtype 6, param 240
- Set/add variable: variable group 14, variable 408, subtype 0, value 1
- Set/add variable: variable group 14, variable 409, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 11, param 21
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 4

**Trigger**

- Object event: subject GalSpan_Shuttle_Medium (object 3, id 240), op 7, value 0 (join 2)
- Object event: subject GalSpan_Shuttle_Medium (object 3, id 240), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 25, subtype 0, value 2
- Hide/remove HUD contact: contact/list 0, subtype 6, param 240

## Waypoints

### Waypoint 0

- Tag: `201`
- Members: `GalSpan_Shuttle_Medium (object 0, id 194, starts at point 0)`, `GalSpan_Shuttle_Medium (object 1, id 238, starts at point 0)`, `GalSpan_Shuttle_Medium (object 2, id 239, starts at point 0)`, `GalSpan_Shuttle_Medium (object 3, id 240, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (147.34, 242.55, 1089.57) | None |
| 1 | (-48.01, 143.80, 1079.26) | None |
| 2 | (-241.24, 33.00, 1077.31) | on arrival play dialog/script or enter gate, param 1; listened by Event 2 for GalSpan_Shuttle_Medium (object 3, id 240) |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `GalSpan_Shuttle_Medium` | 194 | Interactive | 410.73,340.94,1061.50 | 384,0,0 | group/role: FG_CENTAURUS / 0; alias: stocks01; waypoint: Waypoint 0 (tag 201, 3 point(s)), starting point 0, arrival event value 13172736 |
| 1 | `GalSpan_Shuttle_Medium` | 238 | Interactive | 346.29,341.74,1132.37 | 387,0,0 | group/role: FG_CENTAURUS / 0; alias: stocks02; waypoint: Waypoint 0 (tag 201, 3 point(s)), starting point 0, arrival event value 13172736 |
| 2 | `GalSpan_Shuttle_Medium` | 239 | Interactive | 341.92,342.08,983.48 | 382,0,0 | group/role: FG_CENTAURUS / 0; alias: stocks03; waypoint: Waypoint 0 (tag 201, 3 point(s)), starting point 0, arrival event value 13172736 |
| 3 | `GalSpan_Shuttle_Medium` | 240 | Interactive | 297.72,346.74,1069.47 | 382,0,0 | alias: stocks04; secondary groups: none, AQUARIUS; waypoint: Waypoint 0 (tag 201, 3 point(s)), starting point 0, arrival event value 13172736 |
