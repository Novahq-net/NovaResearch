# Tachyon: The Fringe NEUT10B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT10B.SPX` |
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
| Object Types | `0: Training_Combat_Beacon`, `1: Bora_Warhammer`, `2: Bora_Mace`, `3: Bora_Cutlass`, `4: Bora_Claymore`, `5: Bora_Battleaxe` |
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
- Object spawn/action: Training_Combat_Beacon (object 20, id 27), subtype 14

### Event 1

**Trigger**

- Object event: subject Training_Combat_Beacon (object 20, id 27), op 2, value 0 (join 2)
- Object event: subject Training_Combat_Beacon (object 21, id 28), op 2, value 0 (join 2)
- Object event: subject Training_Combat_Beacon (object 22, id 29), op 2, value 0 (join 2)
- Object event: subject Training_Combat_Beacon (object 23, id 30), op 2, value 0 (join 2)

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 32
- Object spawn/action: Training_Combat_Beacon (object 20, id 27), subtype 15

### Event 2

**Trigger**

- Object event: subject Training_Combat_Beacon (object 20, id 27), op 0, value 0 (flags 3)
- Variable comparison: subject variable group 21, variable 29, op 1, value 0

**Action**

- Object spawn/action: Training_Combat_Beacon (object 20, id 27), subtype 7
- Hide/remove HUD contact: contact/list 0, subtype 8, param 0
- Group/spawn-list action: spawn list/group 268, subtype 0
- Set/add variable: variable group 21, variable 29, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 9, param 43
- Show/update HUD contact: contact/list 0, subtype 9, param 44
- Show/update HUD contact: contact/list 0, subtype 9, param 45
- Show/update HUD contact: contact/list 0, subtype 1, param 268

### Event 3

**Trigger**

- Object event: subject Training_Combat_Beacon (object 21, id 28), op 0, value 0 (flags 3)
- Variable comparison: subject variable group 21, variable 29, op 1, value 0

**Action**

- Object spawn/action: Training_Combat_Beacon (object 21, id 28), subtype 7
- Hide/remove HUD contact: contact/list 0, subtype 8, param 0
- Group/spawn-list action: spawn list/group 269, subtype 0
- Set/add variable: variable group 21, variable 29, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 9, param 43
- Show/update HUD contact: contact/list 0, subtype 9, param 44
- Show/update HUD contact: contact/list 0, subtype 9, param 45
- Show/update HUD contact: contact/list 0, subtype 1, param 269

### Event 4

**Trigger**

- Object event: subject Training_Combat_Beacon (object 22, id 29), op 0, value 0 (flags 3)
- Variable comparison: subject variable group 21, variable 29, op 1, value 0

**Action**

- Object spawn/action: Training_Combat_Beacon (object 22, id 29), subtype 7
- Hide/remove HUD contact: contact/list 0, subtype 8, param 0
- Group/spawn-list action: spawn list/group 270, subtype 0
- Set/add variable: variable group 21, variable 29, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 9, param 43
- Show/update HUD contact: contact/list 0, subtype 9, param 44
- Show/update HUD contact: contact/list 0, subtype 9, param 45
- Show/update HUD contact: contact/list 0, subtype 1, param 270

### Event 5

**Trigger**

- Object event: subject Training_Combat_Beacon (object 23, id 30), op 0, value 0 (flags 3)
- Variable comparison: subject variable group 21, variable 29, op 1, value 0

**Action**

- Object spawn/action: Training_Combat_Beacon (object 23, id 30), subtype 7
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

- Set/add variable: variable group 13, variable 430, subtype 0, value 1
- Set/add variable: variable group 13, variable 431, subtype 0, value 2

### Event 7

**Trigger**

- Group/spawn-list event: subject 268, op 1, value 40

**Action**

- Play dialog: PLAYER.SCR, line/variant 180

### Event 8

**Trigger**

- Group/spawn-list event: subject 269, op 1, value 80

**Action**

- Play dialog: PLAYER.SCR, line/variant 178

### Event 9

**Trigger**

- Group/spawn-list event: subject 270, op 1, value 60

**Action**

- Play dialog: PLAYER.SCR, line/variant 165

### Event 10

**Trigger**

- Group/spawn-list event: subject 271, op 1, value 40

**Action**

- Play dialog: PLAYER.SCR, line/variant 181

### Event 11

**Trigger**

- Group/spawn-list event: subject 268, op 0, value 0 (join 2)
- Group/spawn-list event: subject 270, op 0, value 0 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 175

### Event 12

**Trigger**

- Group/spawn-list event: subject 269, op 0, value 0 (join 2)
- Group/spawn-list event: subject 271, op 0, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 176

### Event 13

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 10

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

- Object event: subject Training_Combat_Beacon (object 20, id 27), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 11, param 0

### Event 19

**Trigger**

- Object event: subject Training_Combat_Beacon (object 21, id 28), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 11, param 0

### Event 20

**Trigger**

- Object event: subject Training_Combat_Beacon (object 22, id 29), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 11, param 0

### Event 21

**Trigger**

- Object event: subject Training_Combat_Beacon (object 23, id 30), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 11, param 0

## Waypoints

### Waypoint 0

- Tag: `151`
- Members: `Bora_Battleaxe (object 0, id 32, starts at point 0)`, `Bora_Battleaxe (object 1, id 33, starts at point 0)`, `Bora_Battleaxe (object 2, id 34, starts at point 0)`, `Bora_Battleaxe (object 3, id 35, starts at point 0)`, `Bora_Claymore (object 4, id 36, starts at point 0)`, `Bora_Claymore (object 5, id 37, starts at point 0)`, `Bora_Claymore (object 6, id 38, starts at point 0)`, `Bora_Claymore (object 7, id 39, starts at point 0)`, `Bora_Cutlass (object 8, id 40, starts at point 0)`, `Bora_Cutlass (object 9, id 41, starts at point 0)`, `Bora_Cutlass (object 10, id 42, starts at point 0)`, `Bora_Cutlass (object 11, id 43, starts at point 0)`, `Bora_Mace (object 12, id 44, starts at point 0)`, `Bora_Mace (object 13, id 45, starts at point 0)`, `Bora_Mace (object 14, id 46, starts at point 0)`, `Bora_Mace (object 15, id 47, starts at point 0)`, `Bora_Warhammer (object 16, id 48, starts at point 0)`, `Bora_Warhammer (object 17, id 49, starts at point 0)`, `Bora_Warhammer (object 18, id 50, starts at point 0)`, `Bora_Warhammer (object 19, id 51, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-153.37, 0.00, 399.45) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Bora_Battleaxe` | 32 | Interactive | -1799.17,0.00,4679.96 | 242,0,0 | group/role: FG_ROOKIE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 1 | `Bora_Battleaxe` | 33 | Interactive | -855.86,0.00,4985.48 | 256,0,0 | group/role: FG_VETERAN / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 2 | `Bora_Battleaxe` | 34 | Interactive | 136.45,0.00,5025.33 | 256,0,0 | group/role: FG_ACE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 3 | `Bora_Battleaxe` | 35 | Interactive | 1067.51,0.00,4600.26 | 270,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 4 | `Bora_Claymore` | 36 | Interactive | -1897.18,0.00,4560.41 | 242,0,0 | group/role: FG_ROOKIE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 5 | `Bora_Claymore` | 37 | Interactive | -757.86,0.00,5025.33 | 256,0,0 | group/role: FG_VETERAN / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 6 | `Bora_Claymore` | 38 | Interactive | 295.71,0.00,4972.19 | 256,0,0 | group/role: FG_ACE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 7 | `Bora_Claymore` | 39 | Interactive | 1141.01,0.00,4480.71 | 270,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 8 | `Bora_Cutlass` | 40 | Interactive | -1664.41,0.00,4786.23 | 242,0,0 | group/role: FG_ROOKIE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 9 | `Bora_Cutlass` | 41 | Interactive | -1064.12,0.00,4905.78 | 256,0,0 | group/role: FG_VETERAN / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 10 | `Bora_Cutlass` | 42 | Interactive | -22.81,0.00,5091.75 | 256,0,0 | group/role: FG_ACE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 11 | `Bora_Cutlass` | 43 | Interactive | 957.25,0.00,4746.38 | 270,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 12 | `Bora_Mace` | 44 | Interactive | -1529.66,0.00,4905.78 | 242,0,0 | group/role: FG_ROOKIE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 13 | `Bora_Mace` | 45 | Interactive | -598.60,0.00,5051.90 | 256,0,0 | group/role: FG_VETERAN / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 14 | `Bora_Mace` | 46 | Interactive | 430.47,0.00,4892.49 | 256,0,0 | group/role: FG_ACE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 15 | `Bora_Mace` | 47 | Interactive | 1239.02,0.00,4321.31 | 270,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 16 | `Bora_Warhammer` | 48 | Interactive | -1407.15,0.00,5025.33 | 242,0,0 | group/role: FG_ROOKIE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 17 | `Bora_Warhammer` | 49 | Interactive | -500.59,0.00,5051.90 | 256,0,0 | group/role: FG_VETERAN / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 18 | `Bora_Warhammer` | 50 | Interactive | -218.82,0.00,5171.45 | 256,0,0 | group/role: FG_ACE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 19 | `Bora_Warhammer` | 51 | Interactive | 822.49,0.00,4879.21 | 270,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
| 20 | `Training_Combat_Beacon` | 27 | Interactive | -182.09,0.00,948.94 | 43,7,0 | secondary groups: FG_ROOKIE, none |
| 21 | `Training_Combat_Beacon` | 28 | Interactive | -44.43,136.36,1084.64 | 484,0,505 | secondary groups: FG_VETERAN, none |
| 22 | `Training_Combat_Beacon` | 29 | Interactive | 80.72,268.18,1215.81 | 0,0,0 | secondary groups: FG_ACE, none |
| 23 | `Training_Combat_Beacon` | 30 | Interactive | 218.38,404.55,1342.45 | 71,0,0 | secondary groups: FG_ELITE, none |
