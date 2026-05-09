# Tachyon: The Fringe DISP08B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP08B.SPX` |
| Sector | `QUAD_08` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 7 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 1 |
| Events | 7 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Battleaxe` |
| Scripts | `TRISH.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `SPIKE` |
| Aliases | `spy_1`, `SPIKE` |
| Groups | `QUASAR`, `CONT_054` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Broadcast HUD contact action: contact/list 0, subtype 0, param 16
- Set runtime trigger variable: variable group 20, variable 12, subtype 0, value 0
- Gate state/action: param 2, subtype 3, param 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 12, op 1, value 15

**Action**

- Play dialog: TRISH.SCR, line/variant 1
- Set runtime trigger variable: variable group 20, variable 12, subtype 1, value 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 23, op 1, value 1
- Object event: subject Bora_Battleaxe (object 0, id 4), op 15, value 0

**Action**

- Set/add variable: variable group 18, variable 408, subtype 0, value 1
- Set/add variable: variable group 18, variable 409, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 12, param 24
- Broadcast hide/remove contact: contact/list 0, subtype 0, param 15
- Set/add variable: variable group 38, variable 6, subtype 0, value 1

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1 (join 1)
- Variable comparison: subject variable group 21, variable 23, op 1, value 1

**Action**

- Set/add variable: variable group 18, variable 408, subtype 0, value 1
- Set/add variable: variable group 18, variable 409, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 12, param 24
- Set/add variable: variable group 38, variable 6, subtype 0, value 1

### Event 4

**Trigger**

- Object arrival: Bora_Battleaxe (object 0, id 4) reached Waypoint 0 (tag 151), point 2 (raw value 9895938)

**Action**

- Object spawn/action: Bora_Battleaxe (object 0, id 4), subtype 11, param 3

### Event 5

**Trigger**

- Object event: subject Bora_Battleaxe (object 0, id 4), op 15, value 0
- Variable comparison: subject variable group 21, variable 17, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 64

### Event 6

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Set/add variable: variable group 21, variable 17, subtype 0, value 1

## Waypoints

### Waypoint 0

- Tag: `151`
- Members: `Bora_Battleaxe (object 0, id 4, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1204.51, 0.00, -2414.60) | None |
| 1 | (-1196.57, 0.00, -1840.72) | None |
| 2 | (-1144.51, -164.55, -1239.37) | None; listened by Event 4 for Bora_Battleaxe (object 0, id 4) |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Bora_Battleaxe` | 4 | Interactive | -1173.41,0.00,-2575.20 | 0,0,0 | alias: spy_1; secondary groups: CONT_054, QUASAR; waypoint: Waypoint 0 (tag 151, 3 point(s)), starting point 0, arrival event value 9895936 |
