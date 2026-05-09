# Tachyon: The Fringe BORA03B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `BORA03B.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `(none)` |
| Region | 3 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 1 |
| Events | 3 |
| Waypoints | 0 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Navigational_Bouy` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `CHAAS`, `ORPHS` |
| Aliases | `frank01`, `frank02`, `frank03`, `frank04` |
| Groups | `BLANK` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1
- Gate state/action: param 6, subtype 3, param 0
- Gate state/action: param 7, subtype 3, param 0
- Show/update HUD contact: contact/list 0, subtype 9, param 17
- Show/update HUD contact: contact/list 0, subtype 9, param 24
- Object spawn/action: Navigational_Bouy (object 0, id 1300), subtype 14
- Set runtime trigger variable: variable group 20, variable 15, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 15, op 1, value 20

**Action**

- Play dialog: PLAYER.SCR, line/variant 38
- Mission objective/state: param 196609, subtype 0, param 0
- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Object spawn/action: Navigational_Bouy (object 0, id 1300), subtype 15

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 15, op 1, value 60

**Action**

- Play dialog: PLAYER.SCR, line/variant 60

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Navigational_Bouy` | 1300 | Interactive | 85.50,0.00,1241.30 | 0,0,0 | secondary groups: none, BLANK |
