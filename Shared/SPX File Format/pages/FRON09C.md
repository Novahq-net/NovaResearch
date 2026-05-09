# Tachyon: The Fringe FRON09C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON09C.SPX` |
| Sector | `QUAD_09` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 8 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 7 |
| Events | 11 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Gun_Platform1`, `1: Hajod_Fighter_2` |
| Scripts | `HAJOD.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFNE_04`, `BFNE_02`, `BFNE_07` |
| Aliases | None |
| Groups | `FG_MONARCH` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Play dialog: HAJOD.SCR, line/variant 23
- Set/add variable: variable group 21, variable 20, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 9, param 48

### Event 1

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 23

**Action**

- Play dialog: HAJOD.SCR, line/variant 25

### Event 2

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 25

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 48
- Show/update HUD contact: contact/list 0, subtype 9, param 16
- Object spawn/action: id 190, subtype 14

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 8, value 0 (extra 1, 190; flags 2)

**Action**

- Play scene: unknown index 0, param 1
- Play dialog: PLAYER.SCR, line/variant 119

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 190; flags 2)

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 16
- Set/add variable: variable group 21, variable 20, subtype 0, value 1
- Object spawn/action: id 190, subtype 15

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 5, value 0 (extra 1, 190; flags 2)

**Action**

- Group/spawn-list action: spawn list/group 162, subtype 1, param 1
- Play dialog: HAJOD.SCR, line/variant 22

### Event 6

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 22

**Action**

- Object spawn/action: id 121, subtype 5
- Object spawn/action: id 22, subtype 5
- Object spawn/action: Gun_Platform1 (object 6, id 23), subtype 5
- Object spawn/action: id 26, subtype 5
- Object spawn/action: id 27, subtype 5
- Object spawn/action: id 28, subtype 5

### Event 7

**Trigger**

- Group/spawn-list event: subject 162, op 3, value 0

**Action**

- Object spawn/action: id 29, subtype 5
- Object spawn/action: id 30, subtype 5
- Object spawn/action: Gun_Platform1 (object 4, id 7), subtype 5
- Object spawn/action: Gun_Platform1 (object 5, id 21), subtype 5

### Event 8

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 119

**Action**

- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 37
- Set/add variable: variable group 16, variable 420, subtype 0, value 1
- Set/add variable: variable group 16, variable 421, subtype 0, value 3

### Event 9

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 22

**Action**

- Object spawn/action: id 121, subtype 8, param 9
- Object spawn/action: id 22, subtype 8, param 9
- Object spawn/action: Gun_Platform1 (object 6, id 23), subtype 8, param 9
- Object spawn/action: id 26, subtype 8, param 9
- Object spawn/action: id 27, subtype 8, param 9
- Object spawn/action: id 28, subtype 8, param 9

### Event 10

**Trigger**

- Group/spawn-list event: subject 162, op 3, value 0

**Action**

- Object spawn/action: id 29, subtype 8, param 9
- Object spawn/action: id 30, subtype 8, param 9
- Object spawn/action: Gun_Platform1 (object 4, id 7), subtype 8, param 9
- Object spawn/action: Gun_Platform1 (object 5, id 21), subtype 8, param 9

## Waypoints

### Waypoint 0

- Tag: `201`
- Members: `Hajod_Fighter_2 (object 0, id 3, starts at point 0)`, `Hajod_Fighter_2 (object 1, id 4, starts at point 0)`, `Hajod_Fighter_2 (object 2, id 5, starts at point 0)`, `Hajod_Fighter_2 (object 3, id 6, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-3614.26, 796.86, 162.71) | None |
| 1 | (-2810.59, -2085.67, 1118.92) | None |
| 2 | (-5572.21, -131.41, -1673.01) | None |
| 3 | (-5611.45, -1244.09, 691.55) | None |
| 4 | (-373.92, 1024.54, 967.75) | None |
| 5 | (-1443.39, 0.00, -1176.80) | None |
| 6 | (-2245.33, 0.00, -1882.38) | None |

## Spawn Lists

### Spawn List 0

- ID: `162`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hajod_Fighter_2` | 3 | Interactive | -390.97,-187.66,-15494.95 | 385,28,0 | label: BFNE_04; group/role: FG_MONARCH / 0; waypoint: Waypoint 0 (tag 201, 7 point(s)), starting point 0, arrival event value 13172736 |
| 1 | `Hajod_Fighter_2` | 4 | Interactive | -422.33,-182.66,-15549.86 | 384,28,0 | group/role: FG_MONARCH / 0; waypoint: Waypoint 0 (tag 201, 7 point(s)), starting point 0, arrival event value 13172736 |
| 2 | `Hajod_Fighter_2` | 5 | Interactive | -404.15,-187.66,-15600.32 | 385,28,0 | label: BFNE_04; group/role: FG_MONARCH / 0; waypoint: Waypoint 0 (tag 201, 7 point(s)), starting point 0, arrival event value 13172736 |
| 3 | `Hajod_Fighter_2` | 6 | Interactive | -413.62,-185.66,-15665.00 | 384,28,0 | group/role: FG_MONARCH / 0; waypoint: Waypoint 0 (tag 201, 7 point(s)), starting point 0, arrival event value 13172736 |
| 4 | `Gun_Platform1` | 7 | Interactive | -6347.36,47.56,457.03 | 0,0,0 | None |
| 5 | `Gun_Platform1` | 21 | Interactive | -5675.79,137.55,-1409.16 | 0,0,0 | None |
| 6 | `Gun_Platform1` | 23 | Interactive | -3012.34,-1395.00,-1438.96 | 0,0,0 | None |
