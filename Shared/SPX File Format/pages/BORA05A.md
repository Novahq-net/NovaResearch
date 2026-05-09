# Tachyon: The Fringe BORA05A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `BORA05A.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `(none)` |
| Region | 3 |
| Sector ID | 4 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 6 |
| Events | 4 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Navigational_Bouy`, `1: Bora_Mace`, `2: Bora_Warhammer` |
| Scripts | `NDAWN.scr` |
| Scenes | None |
| Labels | `bfbe_08`, `bfbf_08` |
| Aliases | None |
| Groups | `FG_BORA7`, `FG_BORA6` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 2, op 1, value 1

**Action**

- Object spawn/action: Navigational_Bouy (object 5, id 2171), subtype 14
- Play dialog: NDAWN.scr, line/variant 0
- Show/update HUD contact: contact/list 0, subtype 9, param 24

### Event 1

**Trigger**

- Object event: subject 255, op 0, value 0 (flags 2)

**Action**

- Play dialog: NDAWN.scr, line/variant 3

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 350 (extra 1, 2171; flags 2)

**Action**

- Broadcast hide/remove contact: contact/list 0, subtype 0, param 9
- Mission objective/state: param 196608, subtype 0, param 0
- Object spawn/action: Navigational_Bouy (object 5, id 2171), subtype 15
- Set/add variable: variable group 21, variable 20, subtype 0, value 2
- Hide/remove HUD contact: contact/list 0, subtype 9, param 24
- Set/add variable: variable group 21, variable 2, subtype 0, value 2

### Event 3

**Trigger**

- Variable comparison: subject variable group 21, variable 34, op 1, value 1

**Action**

- Object spawn/action: id 255, subtype 7
- Set/add variable: variable group 15, variable 802, subtype 0, value 1

## Waypoints

### Waypoint 0

- Tag: `1`
- Members: `Bora_Warhammer (object 0, id 248, starts at point 3)`, `Bora_Warhammer (object 1, id 249, starts at point 3)`, `Bora_Mace (object 2, id 250, starts at point 0)`, `Bora_Mace (object 3, id 251, starts at point 0)`, `Bora_Mace (object 4, id 252, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (515.54, -181.86, 679.41) | None |
| 1 | (1873.13, -157.61, 2239.70) | None |
| 2 | (1736.95, -157.61, 5038.19) | None |
| 3 | (-2036.95, -157.61, 5192.44) | None |
| 4 | (-1895.23, -157.61, 2413.91) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Bora_Warhammer` | 248 | Interactive | 423.48,0.00,5865.97 | 384,0,0 | group/role: FG_BORA7 / 0; waypoint: Waypoint 0 (tag 1, 5 point(s)), starting point 3, arrival event value 65539 |
| 1 | `Bora_Warhammer` | 249 | Interactive | 423.48,0.00,6020.21 | 384,0,0 | group/role: FG_BORA7 / 0; waypoint: Waypoint 0 (tag 1, 5 point(s)), starting point 3, arrival event value 65539 |
| 2 | `Bora_Mace` | 250 | Interactive | -1273.79,0.00,2169.67 | 128,0,0 | group/role: FG_BORA6 / 0; waypoint: Waypoint 0 (tag 1, 5 point(s)), starting point 0, arrival event value 65536 |
| 3 | `Bora_Mace` | 251 | Interactive | -1293.24,0.00,1971.35 | 128,0,0 | group/role: FG_BORA6 / 0; waypoint: Waypoint 0 (tag 1, 5 point(s)), starting point 0, arrival event value 65536 |
| 4 | `Bora_Mace` | 252 | Interactive | -1332.15,0.00,1795.07 | 0,0,0 | group/role: FG_BORA6 / 0; waypoint: Waypoint 0 (tag 1, 5 point(s)), starting point 0, arrival event value 65536 |
| 5 | `Navigational_Bouy` | 2171 | Interactive | -1701.30,0.00,4145.81 | 0,0,0 | None |
