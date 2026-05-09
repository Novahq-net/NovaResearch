# Tachyon: The Fringe FRON05A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON05A.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 4 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 2 |
| Events | 6 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Sol_Shuttle_Exile_Cinematic`, `1: Star_Patrol_Enforcer` |
| Scripts | `SPBLT.SCR`, `PLAYER.SCR`, `VIRTU.SCR` |
| Scenes | None |
| Labels | `BFGF_05`, `Ripstar`, `BFGE_05`, `Cephius` |
| Aliases | `Kimodo 4`, `Python 2`, `Python 1`, `Python 4`, `Kimodo 3`, `Kimodo 1`, `Kimodo 2`, `Python 3`, `Jerome13`, `Cephius` |
| Groups | `FG_BOLT`, `CHANCELLOR` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 0, value 1
- Object spawn/action: id 820, subtype 14
- Show/update HUD contact: contact/list 0, subtype 9, param 23
- Play dialog: SPBLT.SCR, line/variant 0
- Set runtime trigger variable: variable group 20, variable 29, subtype 0, value 0

### Event 1

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 105

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 600 (extra 1, 555; flags 2)

**Action**

- Object spawn/action: Star_Patrol_Enforcer (object 0, id 555), subtype 12
- Play dialog: SPBLT.SCR, line/variant 1

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 8, value 0 (extra 1, 820; flags 2)

**Action**

- Play scene: unknown index 0, param 0

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 820; flags 2)

**Action**

- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 23
- Object spawn/action: id 820, subtype 15
- Play dialog: VIRTU.SCR, line/variant 3
- Show/update HUD contact: contact/list 0, subtype 12, param 37
- Set/add variable: variable group 16, variable 417, subtype 0, value 3

### Event 5

**Trigger**

- Object event: subject Star_Patrol_Enforcer (object 0, id 555), op 12, value 0 (extra 1, 820; flags 2)

**Action**

- Object spawn/action: Star_Patrol_Enforcer (object 0, id 555), subtype 2, param 1

## Waypoints

### Waypoint 0

- Tag: `6`
- Members: `Star_Patrol_Enforcer (object 0, id 555, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1778.33, 27.70, 124.51) | None |
| 1 | (-1766.47, 195.20, -357.28) | None |
| 2 | (-2333.66, 404.37, -816.39) | None |
| 3 | (-2909.73, 569.97, -1393.81) | None |
| 4 | (-3423.04, 783.02, -1867.74) | on arrival play dialog/script or enter gate, param 1 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Star_Patrol_Enforcer` | 555 | Interactive | -1316.63,-69.16,286.64 | 252,0,0 | group/role: FG_BOLT / 1; alias: Jerome13; waypoint: Waypoint 0 (tag 6, 5 point(s)), starting point 0, arrival event value 393216 |
| 1 | `Sol_Shuttle_Exile_Cinematic` | 546 | Interactive | -1317.76,-57.33,377.04 | 252,0,0 | secondary groups: none, CHANCELLOR |
