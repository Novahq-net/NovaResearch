# Tachyon: The Fringe NEUT10A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT10A.SPX` |
| Sector | `QUAD_10` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 9 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 6 |
| Entities | 24 |
| Events | 22 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Training_Combat_Beacon`, `1: GalSpan_Archangel`, `2: GalSpan_Phoenix`, `3: GalSpan_Pegasus`, `4: GalSpan_Orion`, `5: GalSpan_Poseidon` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | None |
| Aliases | None |
| Groups | `FG_ROOKIE`, `FG_VETERAN`, `FG_ACE`, `FG_ELITE`, `CONT_055`, `CONT_056`, `CONT_057`, `CONT_058` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 32
- Object spawn/action: Training_Combat_Beacon (object 20, id 2), subtype 14

### Event 1

**Trigger**

- Object event: subject Training_Combat_Beacon (object 20, id 2), op 2, value 0 (join 2)
- Object event: subject Training_Combat_Beacon (object 21, id 3), op 2, value 0 (join 2)
- Object event: subject Training_Combat_Beacon (object 22, id 4), op 2, value 0 (join 2)
- Object event: subject Training_Combat_Beacon (object 23, id 5), op 2, value 0 (join 2)

**Action**

- Object spawn/action: Training_Combat_Beacon (object 20, id 2), subtype 15
- Hide/remove HUD contact: contact/list 0, subtype 9, param 32

### Event 2

**Trigger**

- Object event: subject Training_Combat_Beacon (object 20, id 2), op 0, value 0 (flags 3)
- Variable comparison: subject variable group 21, variable 29, op 1, value 0

**Action**

- Object spawn/action: Training_Combat_Beacon (object 20, id 2), subtype 7
- Group/spawn-list action: spawn list/group 268, subtype 0
- Hide/remove HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 21, variable 29, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 9, param 43
- Show/update HUD contact: contact/list 0, subtype 9, param 44
- Show/update HUD contact: contact/list 0, subtype 9, param 45
- Show/update HUD contact: contact/list 0, subtype 1, param 268

### Event 3

**Trigger**

- Object event: subject Training_Combat_Beacon (object 21, id 3), op 0, value 0 (flags 3)
- Variable comparison: subject variable group 21, variable 29, op 1, value 0

**Action**

- Object spawn/action: Training_Combat_Beacon (object 21, id 3), subtype 7
- Group/spawn-list action: spawn list/group 269, subtype 0
- Hide/remove HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 21, variable 29, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 9, param 43
- Show/update HUD contact: contact/list 0, subtype 9, param 44
- Show/update HUD contact: contact/list 0, subtype 9, param 45
- Show/update HUD contact: contact/list 0, subtype 1, param 269

### Event 4

**Trigger**

- Object event: subject Training_Combat_Beacon (object 22, id 4), op 0, value 0 (flags 3)
- Variable comparison: subject variable group 21, variable 29, op 1, value 0

**Action**

- Object spawn/action: Training_Combat_Beacon (object 22, id 4), subtype 7
- Group/spawn-list action: spawn list/group 270, subtype 0
- Hide/remove HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 21, variable 29, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 9, param 43
- Show/update HUD contact: contact/list 0, subtype 9, param 44
- Show/update HUD contact: contact/list 0, subtype 9, param 45
- Show/update HUD contact: contact/list 0, subtype 1, param 270

### Event 5

**Trigger**

- Object event: subject Training_Combat_Beacon (object 23, id 5), op 0, value 0 (flags 3)
- Variable comparison: subject variable group 21, variable 29, op 1, value 0

**Action**

- Object spawn/action: Training_Combat_Beacon (object 23, id 5), subtype 7
- Hide/remove HUD contact: contact/list 0, subtype 8, param 0
- Group/spawn-list action: spawn list/group 271, subtype 0
- Set/add variable: variable group 21, variable 29, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 9, param 43
- Show/update HUD contact: contact/list 0, subtype 9, param 44
- Show/update HUD contact: contact/list 0, subtype 9, param 45
- Show/update HUD contact: contact/list 0, subtype 1, param 271

### Event 6

**Trigger**

- Group/spawn-list event: subject 268, op 0, value 0 (join 2)
- Group/spawn-list event: subject 269, op 0, value 0 (join 2)
- Group/spawn-list event: subject 270, op 0, value 0 (join 2)
- Group/spawn-list event: subject 271, op 0, value 0 (join 2)

**Action**

- Set/add variable: variable group 13, variable 428, subtype 0, value 1
- Set/add variable: variable group 13, variable 429, subtype 0, value 2

### Event 7

**Trigger**

- Group/spawn-list event: subject 268, op 1, value 60

**Action**

- Play dialog: PLAYER.SCR, line/variant 177

### Event 8

**Trigger**

- Group/spawn-list event: subject 269, op 1, value 40

**Action**

- Play dialog: PLAYER.SCR, line/variant 179

### Event 9

**Trigger**

- Group/spawn-list event: subject 270, op 1, value 80

**Action**

- Play dialog: PLAYER.SCR, line/variant 182

### Event 10

**Trigger**

- Object event: subject GalSpan_Poseidon (object 3, id 10), op 0, value 0 (join 2; flags 2)
- Object event: subject GalSpan_Pegasus (object 11, id 18), op 0, value 0 (join 2; flags 2)
- Object event: subject GalSpan_Archangel (object 19, id 26), op 0, value 0 (flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 167

### Event 11

**Trigger**

- Group/spawn-list event: subject 268, op 0, value 0 (join 2)
- Group/spawn-list event: subject 270, op 0, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 174

### Event 12

**Trigger**

- Group/spawn-list event: subject 269, op 0, value 0 (join 2)
- Group/spawn-list event: subject 271, op 0, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 176

### Event 13

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 50

**Action**

- Play dialog: PLAYER.SCR, line/variant 172

### Event 14

**Trigger**

- Group/spawn-list event: subject 268, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 268
- Set/add variable: variable group 21, variable 29, subtype 0, value 0
- Set/add variable: variable group 0, variable 2, subtype 1, value 25
- Hide/remove HUD contact: contact/list 0, subtype 9, param 45
- Hide/remove HUD contact: contact/list 0, subtype 9, param 44
- Hide/remove HUD contact: contact/list 0, subtype 9, param 43
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 15

**Trigger**

- Group/spawn-list event: subject 269, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 269
- Set/add variable: variable group 21, variable 29, subtype 0, value 0
- Set/add variable: variable group 0, variable 2, subtype 1, value 50
- Hide/remove HUD contact: contact/list 0, subtype 9, param 45
- Hide/remove HUD contact: contact/list 0, subtype 9, param 44
- Hide/remove HUD contact: contact/list 0, subtype 9, param 43
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 16

**Trigger**

- Group/spawn-list event: subject 270, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 270
- Set/add variable: variable group 21, variable 29, subtype 0, value 0
- Set/add variable: variable group 0, variable 2, subtype 1, value 100
- Hide/remove HUD contact: contact/list 0, subtype 9, param 45
- Hide/remove HUD contact: contact/list 0, subtype 9, param 44
- Hide/remove HUD contact: contact/list 0, subtype 9, param 43
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 17

**Trigger**

- Group/spawn-list event: subject 271, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 271
- Set/add variable: variable group 21, variable 29, subtype 0, value 0
- Set/add variable: variable group 0, variable 2, subtype 1, value 200
- Hide/remove HUD contact: contact/list 0, subtype 9, param 45
- Hide/remove HUD contact: contact/list 0, subtype 9, param 44
- Hide/remove HUD contact: contact/list 0, subtype 9, param 43
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 18

**Trigger**

- Object event: subject Training_Combat_Beacon (object 20, id 2), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 11, param 0

### Event 19

**Trigger**

- Object event: subject Training_Combat_Beacon (object 21, id 3), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 11, param 0

### Event 20

**Trigger**

- Object event: subject Training_Combat_Beacon (object 22, id 4), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 11, param 0

### Event 21

**Trigger**

- Object event: subject Training_Combat_Beacon (object 23, id 5), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 11, param 0

## Waypoints

### Waypoint 0

- Tag: `101`
- Members: `GalSpan_Poseidon (object 0, id 7, starts at point 0)`, `GalSpan_Poseidon (object 1, id 8, starts at point 0)`, `GalSpan_Poseidon (object 2, id 9, starts at point 0)`, `GalSpan_Poseidon (object 3, id 10, starts at point 0)`, `GalSpan_Orion (object 4, id 11, starts at point 0)`, `GalSpan_Orion (object 5, id 12, starts at point 0)`, `GalSpan_Orion (object 6, id 13, starts at point 0)`, `GalSpan_Orion (object 7, id 14, starts at point 0)`, `GalSpan_Pegasus (object 8, id 15, starts at point 0)`, `GalSpan_Pegasus (object 9, id 16, starts at point 0)`, `GalSpan_Pegasus (object 10, id 17, starts at point 0)`, `GalSpan_Pegasus (object 11, id 18, starts at point 0)`, `GalSpan_Phoenix (object 12, id 19, starts at point 0)`, `GalSpan_Phoenix (object 13, id 20, starts at point 0)`, `GalSpan_Phoenix (object 14, id 21, starts at point 0)`, `GalSpan_Phoenix (object 15, id 22, starts at point 0)`, `GalSpan_Archangel (object 16, id 23, starts at point 0)`, `GalSpan_Archangel (object 17, id 24, starts at point 0)`, `GalSpan_Archangel (object 18, id 25, starts at point 0)`, `GalSpan_Archangel (object 19, id 26, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-138.12, 0.00, 264.16) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `GalSpan_Poseidon` | 7 | Interactive | -1913.32,0.00,4643.22 | 228,0,0 | group/role: FG_ROOKIE / 0; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 1 | `GalSpan_Poseidon` | 8 | Interactive | -1030.21,0.00,5019.07 | 256,0,0 | group/role: FG_VETERAN / 0; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 2 | `GalSpan_Poseidon` | 9 | Interactive | -217.40,0.00,5288.31 | 256,0,0 | group/role: FG_ACE / 0; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 3 | `GalSpan_Poseidon` | 10 | Interactive | 1129.19,0.00,4650.28 | 284,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 4 | `GalSpan_Orion` | 11 | Interactive | -1845.11,0.00,4791.14 | 228,0,0 | group/role: FG_ROOKIE / 0; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 5 | `GalSpan_Orion` | 12 | Interactive | -944.95,0.00,5111.52 | 256,0,0 | group/role: FG_VETERAN / 0; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 6 | `GalSpan_Orion` | 13 | Interactive | -98.03,0.00,5343.79 | 256,0,0 | group/role: FG_ACE / 0; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 7 | `GalSpan_Orion` | 14 | Interactive | 1060.98,0.00,4816.69 | 284,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 8 | `GalSpan_Pegasus` | 15 | Interactive | -1742.79,0.00,4902.08 | 228,0,0 | group/role: FG_ROOKIE / 0; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 9 | `GalSpan_Pegasus` | 16 | Interactive | -842.63,0.00,5203.98 | 256,0,0 | group/role: FG_VETERAN / 0; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 10 | `GalSpan_Pegasus` | 17 | Interactive | 21.34,0.00,5325.30 | 256,0,0 | group/role: FG_ACE / 0; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 11 | `GalSpan_Pegasus` | 18 | Interactive | 873.40,0.00,4964.61 | 284,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 12 | `GalSpan_Phoenix` | 19 | Interactive | -1640.48,0.00,5031.51 | 228,0,0 | group/role: FG_ROOKIE / 0; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 13 | `GalSpan_Phoenix` | 20 | Interactive | -689.16,0.00,5203.98 | 256,0,0 | group/role: FG_VETERAN / 0; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 14 | `GalSpan_Phoenix` | 21 | Interactive | 174.81,0.00,5325.30 | 256,0,0 | group/role: FG_ACE / 0; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 15 | `GalSpan_Phoenix` | 22 | Interactive | 1231.51,0.00,4539.34 | 284,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 16 | `GalSpan_Archangel` | 23 | Interactive | -1538.16,0.00,5160.94 | 228,0,0 | group/role: FG_ROOKIE / 0; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 17 | `GalSpan_Archangel` | 24 | Interactive | -518.63,0.00,5259.45 | 256,0,0 | group/role: FG_VETERAN / 0; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 18 | `GalSpan_Archangel` | 25 | Interactive | 328.28,0.00,5288.31 | 256,0,0 | group/role: FG_ACE / 0; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 19 | `GalSpan_Archangel` | 26 | Interactive | 1316.77,0.00,4391.42 | 284,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 0 (tag 101, 1 point(s)), starting point 0, arrival event value 6619136 |
| 20 | `Training_Combat_Beacon` | 2 | Interactive | -187.18,0.00,953.62 | 476,0,0 | secondary groups: FG_ROOKIE, none |
| 21 | `Training_Combat_Beacon` | 3 | Interactive | -28.82,72.73,1127.66 | 0,0,0 | secondary groups: FG_VETERAN, none |
| 22 | `Training_Combat_Beacon` | 4 | Interactive | 187.15,129.09,1273.24 | 363,7,0 | secondary groups: FG_ACE, none |
| 23 | `Training_Combat_Beacon` | 5 | Interactive | 379.76,189.09,1400.59 | 164,0,0 | secondary groups: FG_ELITE, none |
