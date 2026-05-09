# Tachyon: The Fringe NEUT01E.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT01E.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 3 |
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
| Labels | `MISHK`, `FakeJake`, `Daymir` |
| Aliases | `Courage`, `kwi03_7`, `Jerome26`, `Jerome25`, `Jerome24`, `Jerome22`, `Jerome21`, `Jerome20`, `kevin01`, `Intrepid`, `kwI03_10`, `SHIP1_HYPER`, `ohshit`, `SHIP2_HYPER`, `SHIP3_HYPER` |
| Groups | `GALLURAN`, `CONT_041` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 9, value 0

**Action**

- Object spawn/action: Generic_Light_Freighter (object 0, id 291), subtype 5
- Show/update HUD contact: contact/list 0, subtype 6, param 291

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 3100 (extra 1, 291; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 114

### Event 2

**Trigger**

- Object event: subject Generic_Light_Freighter (object 0, id 291), op 8, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 6, param 291

### Event 3

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 114

**Action**

- Object spawn/action: Generic_Light_Freighter (object 0, id 291), subtype 4

## Waypoints

### Waypoint 0

- Tag: `301`
- Members: `Generic_Light_Freighter (object 0, id 291, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (4311.08, -15.10, -9851.29) | None |
| 1 | (4655.51, 12.41, -10559.57) | on arrival action 1, param -1 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Generic_Light_Freighter` | 291 | Interactive | 4099.61,-29.36,-9396.64 | 232,0,0 | alias: kevin01; secondary groups: CONT_041, GALLURAN; waypoint: Waypoint 0 (tag 301, 2 point(s)), starting point 0, arrival event value 19726336 |
| 1 | `Generic_Light_Freighter` | 513 | Interactive | 7688.38,-1366.12,-7695.39 | 114,64,370 | None |
| 2 | `Generic_Light_Freighter` | 514 | Interactive | 7643.13,-1243.64,-7917.29 | 434,0,57 | None |
