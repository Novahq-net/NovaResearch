# Tachyon: The Fringe MYST01C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST01C.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 5 |
| Sector ID | 0 |
| SectorHazardFlags | Twilight fog / fog-radar impairment (0x00000002) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 1 |
| Events | 4 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Light_Freighter` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `bfne_07`, `bfbf_07`, `bfgf_05` |
| Aliases | None |
| Groups | `CONT_006` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Object spawn/action: Generic_Light_Freighter (object 0, id 201), subtype 12
- Object spawn/action: id 204, subtype 12
- Set runtime trigger variable: variable group 20, variable 1, subtype 0, value 0

### Event 1

**Trigger**

- Object event: subject 204, op 12, value 0 (extra 1, 59; flags 2)

**Action**

- Object spawn/action: id 204, subtype 2, param 60

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 18

**Action**

- Play dialog: PLAYER.SCR, line/variant 17

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 30, op 3, value 3

**Action**

- Set/add variable: variable group 17, variable 402, subtype 0, value 0
- Set/add variable: variable group 17, variable 403, subtype 0, value 1

## Waypoints

### Waypoint 0

- Tag: `201`
- Members: `Generic_Light_Freighter (object 0, id 201, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1807.62, 111.75, 1918.54) | on arrival action 1, param -1 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Generic_Light_Freighter` | 201 | Interactive | -2047.70,59.87,1612.66 | 50,0,0 | label: bfne_07; secondary groups: CONT_006, none; waypoint: Waypoint 0 (tag 201, 1 point(s)), starting point 0, arrival event value 13172736 |
