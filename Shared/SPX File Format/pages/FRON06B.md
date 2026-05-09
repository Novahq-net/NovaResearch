# Tachyon: The Fringe FRON06B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON06B.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 5 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 1 |
| Events | 7 |
| Waypoints | 0 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Navigational_Bouy` |
| Scripts | `PLAYER.SCR`, `MIDAS.SCR` |
| Scenes | None |
| Labels | `CEPHS`, `valnt`, `dionysus` |
| Aliases | None |
| Groups | `BLANK` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 29, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 33
- Object spawn/action: Navigational_Bouy (object 0, id 1008), subtype 14

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 29, op 1, value 10

**Action**

- Play dialog: PLAYER.SCR, line/variant 1

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 8, value 0 (extra 1, 891; flags 2)

**Action**

- Set runtime trigger variable: variable group 20, variable 28, subtype 0, value 0
- Play scene: unknown index 0, param 1

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 28, op 1, value 5

**Action**

- Play dialog: MIDAS.SCR, line/variant 1
- Set/add variable: variable group 21, variable 29, subtype 0, value 1
- Object spawn/action: Navigational_Bouy (object 0, id 1008), subtype 15

### Event 4

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 1

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Hide/remove HUD contact: contact/list 0, subtype 11, param 0
- Play dialog: PLAYER.SCR, line/variant 2
- Set/add variable: variable group 21, variable 24, subtype 0, value 1
- Broadcast HUD contact action: contact/list 0, subtype 0, param 29
- Broadcast HUD contact action: contact/list 0, subtype 0, param 47

### Event 5

**Trigger**

- Object event: subject 892, op 0, value 0 (join 2; flags 2)
- Object event: subject 797, op 0, value 0 (join 2; flags 2)
- Object event: subject 798, op 0, value 0 (join 2; flags 2)
- Object event: subject 891, op 0, value 0 (join 2; flags 2)
- Object event: subject 146, op 0, value 0 (join 2; flags 2)
- Object event: subject 162, op 0, value 0 (join 2; flags 2)
- Object event: subject 178, op 0, value 0 (join 2; flags 2)
- Object event: subject 194, op 0, value 0 (join 2; flags 2)

**Action**

- Group/spawn-list action: spawn list/group 227, subtype 4, param 9
- Object spawn/action: id 970, subtype 8, param 9
- Object spawn/action: id 798, subtype 8, param 9
- Object spawn/action: id 146, subtype 8, param 9
- Object spawn/action: id 162, subtype 8, param 9
- Object spawn/action: id 178, subtype 8, param 9
- Object spawn/action: id 797, subtype 8, param 9
- Object spawn/action: id 194, subtype 8, param 9

### Event 6

**Trigger**

- Group/spawn-list event: subject 227, op 4, value 0 (flags 2)

**Action**

- Group/spawn-list action: spawn list/group 227, subtype 4, param 9
- Object spawn/action: id 970, subtype 8, param 9
- Object spawn/action: id 798, subtype 8, param 9
- Object spawn/action: id 146, subtype 8, param 9
- Object spawn/action: id 162, subtype 8, param 9
- Object spawn/action: id 178, subtype 8, param 9
- Object spawn/action: id 797, subtype 8, param 9
- Object spawn/action: id 194, subtype 8, param 9

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Navigational_Bouy` | 1008 | Interactive | 6.14,235.51,5.79 | 0,0,0 | secondary groups: none, BLANK |
