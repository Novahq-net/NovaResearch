# Tachyon: The Fringe MYST05A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST05A.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `(none)` |
| Region | 5 |
| Sector ID | 4 |
| SectorHazardFlags | Radiation hazard, Twilight fog / fog-radar impairment (0x00000003) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 2 |
| Events | 4 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Cassitor_Advanced_Drone` |
| Scripts | `DRCAS.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `WRKR1`, `WRKR2` |
| Aliases | `Will_02` |
| Groups | `CONT_005`, `CONT_UNKNOWN` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 16

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 2

**Action**

- Play dialog: DRCAS.SCR, line/variant 0

### Event 2

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 0
- Area/player/sector/dock/time event: subject 0, op 8, value 0 (extra 1, 34; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 20
- Play scene: unknown index 0, param 0

### Event 3

**Trigger**

- Runtime condition family: subject 0, op 0, value 0

**Action**

- Set/add variable: variable group 8, variable 7, subtype 0, value 1
- Mission objective/state: param 327686, subtype 0, param 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 16

## Waypoints

### Waypoint 0

- Tag: `101`
- Members: `Cassitor_Advanced_Drone (object 0, id 42, starts at point 0)`, `Cassitor_Advanced_Drone (object 1, id 43, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-841.13, 403.71, 1476.61) | on arrival activate current object (raw param -1 ignored) |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Cassitor_Advanced_Drone` | 42 | Interactive | -670.49,417.77,1817.20 | 256,0,0 | label: WRKR1; group/role: none / 1; secondary groups: CONT_005, none; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 1 | `Cassitor_Advanced_Drone` | 43 | Interactive | -651.63,417.77,1832.38 | 256,0,0 | label: WRKR2; group/role: none / 2; secondary groups: CONT_UNKNOWN, none; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
