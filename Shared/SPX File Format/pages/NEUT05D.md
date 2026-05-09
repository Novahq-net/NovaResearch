# Tachyon: The Fringe NEUT05D.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT05D.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 4 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 1 |
| Events | 5 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Light_Freighter` |
| Scripts | `VENET.SCR` |
| Scenes | None |
| Labels | `aobul` |
| Aliases | `bagel`, `bagel_1`, `bagel_2`, `oside`, `oside_1`, `oside_2`, `Will_01`, `SHIP1_HYPER`, `ohshit`, `SHIP3_HYPER`, `SHIP2_HYPER` |
| Groups | `VENETIAN`, `CONT_022` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 27

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 500 (extra 1, 1028; flags 2)

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 6, param 1028
- Play dialog: VENET.SCR, line/variant 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 27

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 10

**Action**

- Mission objective/state: param 65541, subtype 0, param 0
- Object spawn/action: Generic_Light_Freighter (object 0, id 1028), subtype 4

### Event 3

**Trigger**

- Object event: subject Generic_Light_Freighter (object 0, id 1028), op 8, value 0

**Action**

- Set/add variable: variable group 21, variable 2, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 6, param 1028

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 6, param 1028
- Hide/remove HUD contact: contact/list 0, subtype 9, param 27

## Waypoints

### Waypoint 0

- Tag: `251`
- Members: `Generic_Light_Freighter (object 0, id 1028, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (157.88, -19.79, 629.31) | None |
| 1 | (168.82, -125.77, 1994.53) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Generic_Light_Freighter` | 1028 | Interactive | 601.49,83.01,100.25 | 0,0,0 | alias: Will_01; secondary groups: CONT_022, VENETIAN; waypoint: Waypoint 0 (tag 251, 2 point(s)), starting point 0, arrival event value 16449536 |
