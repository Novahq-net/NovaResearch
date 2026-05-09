# Tachyon: The Fringe GALS04A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `GALS04A.SPX` |
| Sector | `QUAD_04` |
| Backdrop | `(none)` |
| Region | 2 |
| Sector ID | 3 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 5 |
| Events | 13 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Carrier`, `1: GalSpan_Orion` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `bfge_03` |
| Aliases | `frank11` |
| Groups | `FG_GRUS`, `AQUILA`, `CONT_026` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 24, op 3, value 1
- Variable comparison: subject variable group 21, variable 21, op 1, value 1 (join 1)
- Variable comparison: subject variable group 0, variable 7, op 1, value 13

**Action**

- Set runtime trigger variable: variable group 20, variable 2, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 13
- Show/update HUD contact: contact/list 0, subtype 9, param 18
- Group/spawn-list action: spawn list/group 241, subtype 1, param 5
- Play dialog: PLAYER.SCR, line/variant 24

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 7
- Group/spawn-list event: subject 241, op 3, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 25
- Set runtime trigger variable: variable group 20, variable 2, subtype 1, value 0

### Event 2

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 25

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 13
- Hide/remove HUD contact: contact/list 0, subtype 9, param 18
- Group/spawn-list action: spawn list/group 241, subtype 4, param 1
- Show/update HUD contact: contact/list 0, subtype 1, param 241

### Event 3

**Trigger**

- Group/spawn-list event: subject 241, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 241
- Show/update HUD contact: contact/list 0, subtype 9, param 18
- Object spawn/action: GalSpan_Carrier (object 4, id 6), subtype 14

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 24, op 1, value 1 (join 1)
- Variable comparison: subject variable group 0, variable 7, op 1, value 13

**Action**

- Object spawn/action: GalSpan_Orion (object 0, id 8), subtype 7
- Object spawn/action: GalSpan_Orion (object 1, id 9), subtype 7
- Object spawn/action: GalSpan_Orion (object 2, id 10), subtype 7
- Object spawn/action: GalSpan_Orion (object 3, id 11), subtype 7
- Show/update HUD contact: contact/list 0, subtype 9, param 13
- Show/update HUD contact: contact/list 0, subtype 9, param 18

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 6; flags 2)
- Variable comparison: subject variable group 21, variable 20, op 1, value 0

**Action**

- Play scene: unknown index 0, param 0
- Set/add variable: variable group 21, variable 20, subtype 1, value 1
- Object spawn/action: GalSpan_Carrier (object 4, id 6), subtype 15
- Hide/remove HUD contact: contact/list 0, subtype 9, param 13
- Hide/remove HUD contact: contact/list 0, subtype 9, param 18
- Set runtime trigger variable: variable group 20, variable 2, subtype 0, value 0
- Play dialog: PLAYER.SCR, line/variant 136

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 11

**Action**

- Set runtime trigger variable: variable group 20, variable 2, subtype 1, value 0

### Event 7

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 5, value 0 (extra 1, 6; flags 2)

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0
- Mission objective/state: param 131072, subtype 0, param 0

### Event 8

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 0, variable 7, op 1, value 13

**Action**

- Object spawn/action: GalSpan_Carrier (object 4, id 6), subtype 14
- Show/update HUD contact: contact/list 0, subtype 9, param 18

### Event 9

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 6; flags 2)
- Variable comparison: subject variable group 21, variable 20, op 1, value 0

**Action**

- Play scene: unknown index 0, param 0
- Set/add variable: variable group 21, variable 20, subtype 1, value 1
- Object spawn/action: GalSpan_Carrier (object 4, id 6), subtype 15
- Hide/remove HUD contact: contact/list 0, subtype 9, param 18
- Play dialog: PLAYER.SCR, line/variant 136

### Event 10

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 5, value 0 (extra 1, 6; flags 2)

**Action**

- Mission objective/state: param 131072, subtype 0, param 0
- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0

### Event 11

**Trigger**

- Object event: subject GalSpan_Carrier (object 4, id 6), op 2, value 0
- Variable comparison: subject variable group 21, variable 20, op 1, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 21
- Hide/remove HUD contact: contact/list 0, subtype 9, param 13
- Hide/remove HUD contact: contact/list 0, subtype 9, param 18
- Set/add variable: variable group 14, variable 413, subtype 0, value 1
- Set/add variable: variable group 14, variable 412, subtype 0, value 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 20

### Event 12

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 5

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 1, value 0

## Waypoints

### Waypoint 0

- Tag: `101`
- Members: `GalSpan_Orion (object 0, id 8, starts at point 0)`, `GalSpan_Orion (object 1, id 9, starts at point 0)`, `GalSpan_Orion (object 2, id 10, starts at point 0)`, `GalSpan_Orion (object 3, id 11, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (266.07, 0.00, -60.95) | None |
| 1 | (-58.93, 333.04, 1987.19) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `GalSpan_Orion` | 8 | Interactive | 280.22,0.00,-184.25 | 0,0,0 | label: bfge_03; group/role: FG_GRUS / 1; waypoint: Waypoint 0 (tag 101, 2 point(s)), starting point 0, arrival event value 6619136 |
| 1 | `GalSpan_Orion` | 9 | Interactive | 230.87,0.00,-243.49 | 0,0,0 | group/role: FG_GRUS / 2; waypoint: Waypoint 0 (tag 101, 2 point(s)), starting point 0, arrival event value 6619136 |
| 2 | `GalSpan_Orion` | 10 | Interactive | 303.13,0.00,-237.76 | 0,0,0 | group/role: FG_GRUS / 3; waypoint: Waypoint 0 (tag 101, 2 point(s)), starting point 0, arrival event value 6619136 |
| 3 | `GalSpan_Orion` | 11 | Interactive | 267.88,0.00,-298.92 | 0,0,0 | group/role: FG_GRUS / 4; waypoint: Waypoint 0 (tag 101, 2 point(s)), starting point 0, arrival event value 6619136 |
| 4 | `GalSpan_Carrier` | 6 | Interactive | -203.96,416.87,3975.76 | 178,0,0 | alias: frank11; secondary groups: CONT_026, AQUILA |
