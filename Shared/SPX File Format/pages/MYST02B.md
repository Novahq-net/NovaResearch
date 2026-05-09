# Tachyon: The Fringe MYST02B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST02B.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `(none)` |
| Region | 5 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
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
| Object Types | `0: Skav_Pirate_Manta` |
| Scripts | `BARGH.SCR` |
| Scenes | None |
| Labels | None |
| Aliases | `Will_02` |
| Groups | `BARGHEST`, `CONT_042` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Object spawn/action: Skav_Pirate_Manta (object 0, id 3), subtype 1, param 1
- Object spawn/action: Skav_Pirate_Manta (object 0, id 3), subtype 8, param 4
- Show/update HUD contact: contact/list 0, subtype 6, param 3

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 500 (extra 1, 3; flags 2)

**Action**

- Play dialog: BARGH.SCR, line/variant 0

### Event 2

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 0 (join 1)
- Object event: subject Skav_Pirate_Manta (object 0, id 3), op 2, value 0

**Action**

- Mission objective/state: param 327684, subtype 0, param 0
- Object spawn/action: Skav_Pirate_Manta (object 0, id 3), subtype 2, param 2

### Event 3

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 0, id 3), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Set/add variable: variable group 17, variable 412, subtype 0, value 1
- Set/add variable: variable group 17, variable 413, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 29

## Waypoints

### Waypoint 0

- Tag: `151`
- Members: `Skav_Pirate_Manta (object 0, id 3, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-170.72, 0.00, 172.00) | None |
| 1 | (91.26, 0.00, -88.83) | None |
| 2 | (234.73, 0.00, -241.26) | on arrival play dialog/script or enter gate, param 2 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Skav_Pirate_Manta` | 3 | Interactive | -1057.89,0.00,1090.80 | 0,0,0 | alias: Will_02; secondary groups: CONT_042, BARGHEST; waypoint: Waypoint 0 (tag 151, 3 point(s)), starting point 0, arrival event value 9895936 |
