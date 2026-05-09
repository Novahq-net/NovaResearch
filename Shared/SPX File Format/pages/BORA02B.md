# Tachyon: The Fringe BORA02B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `BORA02B.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `(none)` |
| Region | 3 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 2 |
| Events | 3 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Cruiser`, `1: Navigational_Bouy` |
| Scripts | `PLAYER.SCR`, `CHAMP.scr` |
| Scenes | None |
| Labels | `chaas`, `bfbf_01`, `BFBE_05`, `BFGE_05`, `BFBF_05` |
| Aliases | `frank01`, `frank02`, `frank03`, `frank04`, `stocks06` |
| Groups | `CANDOR` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Object spawn/action: Navigational_Bouy (object 0, id 350), subtype 14
- Play dialog: PLAYER.SCR, line/variant 23
- Object spawn/action: Bora_Cruiser (object 1, id 136), subtype 5
- Show/update HUD contact: contact/list 0, subtype 9, param 24

### Event 1

**Trigger**

- Object event: subject 18, op 0, value 0 (flags 2)

**Action**

- Play dialog: CHAMP.scr, line/variant 1

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 300 (extra 1, 350; flags 2)

**Action**

- Object spawn/action: Bora_Cruiser (object 1, id 136), subtype 4
- Broadcast hide/remove contact: contact/list 0, subtype 0, param 10
- Mission objective/state: param 196608, subtype 0, param 0
- Object spawn/action: Navigational_Bouy (object 0, id 350), subtype 15
- Set/add variable: variable group 21, variable 21, subtype 0, value 2
- Hide/remove HUD contact: contact/list 0, subtype 9, param 24
- Set/add variable: variable group 21, variable 2, subtype 0, value 1

## Waypoints

### Waypoint 0

- Tag: `151`
- Members: `Bora_Cruiser (object 1, id 136, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2902.99, 0.00, 1493.42) | None |
| 1 | (-3488.85, 0.00, 2200.71) | None |
| 2 | (-3914.02, 0.00, 2686.00) | on arrival action 1, param -1 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Navigational_Bouy` | 350 | Interactive | -1577.54,0.00,840.20 | 0,0,0 | None |
| 1 | `Bora_Cruiser` | 136 | Interactive | -1985.28,-75.00,382.79 | 457,509,0 | secondary groups: none, CANDOR; waypoint: Waypoint 0 (tag 151, 3 point(s)), starting point 0, arrival event value 9895936 |
