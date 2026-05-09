# Tachyon: The Fringe MYST06A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST06A.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `(none)` |
| Region | 5 |
| Sector ID | 5 |
| SectorHazardFlags | Twilight fog / fog-radar impairment (0x00000002) |
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
| Object Types | `0: Shuttle_Small` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `PISCE`, `RALPH` |
| Aliases | `PISCES1`, `PISCES2`, `pisces3`, `pisces4`, `stocks02` |
| Groups | `CONT_034` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Gate state/action: param 4, subtype 3, param 0
- Mission objective/state: param 327687, subtype 0, param 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 300 (extra 1, 11; flags 2)
- Variable comparison: subject variable group 21, variable 22, op 3, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 1
- Play scene: unknown index 0, param 0

### Event 2

**Trigger**

- Runtime condition family: subject 0, op 0, value 0

**Action**

- Object spawn/action: Shuttle_Small (object 0, id 11), subtype 5

### Event 3

**Trigger**

- Object event: subject Shuttle_Small (object 0, id 11), op 0, value 0 (flags 2)

**Action**

- Set/add variable: variable group 21, variable 22, subtype 1, value 1
- Object spawn/action: Shuttle_Small (object 0, id 11), subtype 13, param 6619136

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Object spawn/action: Shuttle_Small (object 0, id 11), subtype 7

## Waypoints

### Waypoint 0

- Tag: `101`
- Members: `Shuttle_Small (object 0, id 11, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (204.06, -400.05, 293.63) | None |
| 1 | (449.60, 0.00, 445.99) | on arrival play dialog/script or enter gate, param 2 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Shuttle_Small` | 11 | Interactive | 187.98,-413.80,282.28 | 70,50,21 | label: RALPH; secondary groups: CONT_034, none; waypoint: Waypoint 0 (tag 101, 2 point(s)), starting point 0, arrival event value 6619136 |
