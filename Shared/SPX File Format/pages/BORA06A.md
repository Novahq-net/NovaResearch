# Tachyon: The Fringe BORA06A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `BORA06A.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `(none)` |
| Region | 3 |
| Sector ID | 5 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 0 |
| Entities | 0 |
| Events | 5 |
| Waypoints | 0 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | None |
| Scripts | `PLAYER.SCR`, `DRMAC.SCR` |
| Scenes | None |
| Labels | None |
| Aliases | None |
| Groups | None |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 12
- Play dialog: PLAYER.SCR, line/variant 5
- Object spawn/action: id 926, subtype 14

### Event 1

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 9
- Show/update HUD contact: contact/list 0, subtype 9, param 13
- Hide/remove HUD contact: contact/list 0, subtype 9, param 12
- Object spawn/action: id 926, subtype 15

### Event 2

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 12
- Object spawn/action: id 917, subtype 6
- Object spawn/action: id 917, subtype 8, param 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 13
- Show/update HUD contact: contact/list 0, subtype 9, param 12
- Object spawn/action: id 926, subtype 14

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 8, value 0 (extra 1, 926; flags 3)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Play scene: unknown index 0, param 0
- Play dialog: DRMAC.SCR, line/variant 6

### Event 4

**Trigger**

- Runtime condition family: subject 0, op 0, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 15, variable 400, subtype 0, value 1
- Set/add variable: variable group 15, variable 401, subtype 0, value 2
- Set/add variable: variable group 21, variable 29, subtype 0, value 1
- Set runtime trigger variable: variable group 20, variable 29, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 12, param 19
- Hide/remove HUD contact: contact/list 0, subtype 9, param 12
- Object spawn/action: id 926, subtype 15

## Waypoints

None
## Spawn Lists

None

## Objects

None
