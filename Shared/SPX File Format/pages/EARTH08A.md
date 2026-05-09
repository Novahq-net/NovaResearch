# Tachyon: The Fringe EARTH08A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH08A.SPX` |
| Sector | `QUAD_08` |
| Backdrop | `(none)` |
| Region | 0 |
| Sector ID | 7 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 5 |
| Entities | 36 |
| Events | 25 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Minelayer`, `1: Crate_7`, `2: Navigational_Bouy`, `3: Training_Fighter`, `4: Training_Mine` |
| Scripts | `TINS.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | None |
| Aliases | None |
| Groups | `FG_DRAGON`, `FG_AGT_RIVAL1`, `CONT_012`, `FG_AGT3`, `FG_ACE`, `CONT_034` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 2, subtype 0, value 0
- Gate state/action: param 15, subtype 3, param 0
- Group/spawn-list action: spawn list/group 32, subtype 6
- Group/spawn-list action: spawn list/group 270, subtype 6
- Group/spawn-list action: spawn list/group 3, subtype 6
- Group/spawn-list action: spawn list/group 270, subtype 4, param 5
- Group/spawn-list action: spawn list/group 32, subtype 4, param 5

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 3

**Action**

- Play dialog: TINS.SCR, line/variant 7
- Show/update HUD contact: contact/list 0, subtype 9, param 37

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 34

**Action**

- Show/update HUD contact: contact/list 0, subtype 1, param 32

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 41

**Action**

- Play dialog: TINS.SCR, line/variant 8

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 65

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 23
- Show/update HUD contact: contact/list 0, subtype 9, param 24
- Set runtime trigger variable: variable group 20, variable 2, subtype 1, value 0

### Event 5

**Trigger**

- Group/spawn-list event: subject 32, op 0, value 0
- Sector/startup condition family: subject 0, op 0, value 8

**Action**

- Play dialog: TINS.SCR, line/variant 9
- Set runtime trigger variable: variable group 20, variable 2, subtype 0, value 0
- Hide/remove HUD contact: contact/list 0, subtype 1, param 32
- Hide/remove HUD contact: contact/list 0, subtype 9, param 23
- Hide/remove HUD contact: contact/list 0, subtype 9, param 24
- Show/update HUD contact: contact/list 0, subtype 9, param 38
- Show/update HUD contact: contact/list 0, subtype 9, param 40
- Show/update HUD contact: contact/list 0, subtype 9, param 39

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 85

**Action**

- Set runtime trigger variable: variable group 20, variable 2, subtype 1, value 0
- Show/update HUD contact: contact/list 0, subtype 1, param 270
- Group/spawn-list action: spawn list/group 270, subtype 2
- Group/spawn-list action: spawn list/group 270, subtype 6

### Event 7

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 9
- Group/spawn-list event: subject 270, op 0, value 0

**Action**

- Play dialog: TINS.SCR, line/variant 10
- Group/spawn-list action: spawn list/group 10, subtype 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 38
- Hide/remove HUD contact: contact/list 0, subtype 9, param 39
- Hide/remove HUD contact: contact/list 0, subtype 9, param 40
- Show/update HUD contact: contact/list 0, subtype 9, param 25
- Show/update HUD contact: contact/list 0, subtype 9, param 41
- Hide/remove HUD contact: contact/list 0, subtype 1, param 270

### Event 8

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 10
- Group/spawn-list event: subject 10, op 0, value 0

**Action**

- Object spawn/action: Generic_Minelayer (object 35, id 128), subtype 3
- Play dialog: TINS.SCR, line/variant 12
- Object spawn/action: Generic_Minelayer (object 35, id 128), subtype 14
- Hide/remove HUD contact: contact/list 0, subtype 9, param 25
- Hide/remove HUD contact: contact/list 0, subtype 9, param 41
- Show/update HUD contact: contact/list 0, subtype 9, param 42
- Show/update HUD contact: contact/list 0, subtype 9, param 50
- Show/update HUD contact: contact/list 0, subtype 9, param 24

### Event 9

**Trigger**

- Object arrival: Generic_Minelayer (object 35, id 128) reached Waypoint 0 (tag 2), point 0 (raw value 131072)

**Action**

- Object spawn/action: Generic_Minelayer (object 35, id 128), subtype 6

### Event 10

**Trigger**

- Object event: subject Generic_Minelayer (object 35, id 128), op 14, value 24
- Object event: subject Generic_Minelayer (object 35, id 128), op 14, value 25

**Action**

- Set/add variable: variable group 21, variable 21, subtype 1, value 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 42
- Hide/remove HUD contact: contact/list 0, subtype 9, param 50

### Event 11

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 1 (join 2)
- Object event: subject Generic_Minelayer (object 35, id 128), op 2, value 0

**Action**

- Play dialog: TINS.SCR, line/variant 13
- Object spawn/action: Generic_Minelayer (object 35, id 128), subtype 15
- Show/update HUD contact: contact/list 0, subtype 9, param 23
- Hide/remove HUD contact: contact/list 0, subtype 9, param 37
- Hide/remove HUD contact: contact/list 0, subtype 9, param 42
- Hide/remove HUD contact: contact/list 0, subtype 9, param 50
- Set/add variable: variable group 21, variable 22, subtype 1, value 1

### Event 12

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 131; flags 2)
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Object spawn/action: Training_Mine (object 13, id 139), subtype 17
- Object spawn/action: Training_Mine (object 9, id 135), subtype 17
- Object spawn/action: Training_Mine (object 10, id 136), subtype 17
- Object spawn/action: Training_Mine (object 11, id 137), subtype 17
- Object spawn/action: Training_Mine (object 12, id 138), subtype 17
- Object spawn/action: Training_Mine (object 14, id 140), subtype 17

### Event 13

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 131; flags 2)
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Object spawn/action: Training_Mine (object 15, id 141), subtype 17
- Object spawn/action: Training_Mine (object 16, id 142), subtype 17
- Object spawn/action: Training_Mine (object 17, id 143), subtype 17
- Object spawn/action: Training_Mine (object 18, id 145), subtype 17
- Group/spawn-list action: spawn list/group 3, subtype 2
- Group/spawn-list action: spawn list/group 3, subtype 4, param 5

### Event 14

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 10

**Action**

- Play dialog: PLAYER.SCR, line/variant 53
- Set runtime trigger variable: variable group 20, variable 2, subtype 0, value 0

### Event 15

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 95 (join 2)
- Area/player/sector/dock/time event: subject 0, op 0, value 50

**Action**

- Group/spawn-list action: spawn list/group 3, subtype 6
- Group/spawn-list action: spawn list/group 3, subtype 4

### Event 16

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 97

**Action**

- Play dialog: TINS.SCR, line/variant 15

### Event 17

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 114

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 26
- Hide/remove HUD contact: contact/list 0, subtype 9, param 23
- Hide/remove HUD contact: contact/list 0, subtype 9, param 24

### Event 18

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 141

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 27
- Show/update HUD contact: contact/list 0, subtype 9, param 28
- Show/update HUD contact: contact/list 0, subtype 9, param 43
- Hide/remove HUD contact: contact/list 0, subtype 9, param 26

### Event 19

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 161

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 27
- Hide/remove HUD contact: contact/list 0, subtype 9, param 28
- Hide/remove HUD contact: contact/list 0, subtype 9, param 43
- Show/update HUD contact: contact/list 0, subtype 9, param 44
- Show/update HUD contact: contact/list 0, subtype 9, param 45
- Show/update HUD contact: contact/list 0, subtype 9, param 46
- Show/update HUD contact: contact/list 0, subtype 9, param 47
- Set runtime trigger variable: variable group 20, variable 2, subtype 1, value 0

### Event 20

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 15

**Action**

- Play dialog: TINS.SCR, line/variant 18
- Set runtime trigger variable: variable group 20, variable 2, subtype 0, value 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 44
- Hide/remove HUD contact: contact/list 0, subtype 9, param 45
- Hide/remove HUD contact: contact/list 0, subtype 9, param 46
- Hide/remove HUD contact: contact/list 0, subtype 9, param 47

### Event 21

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 163

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 23
- Show/update HUD contact: contact/list 0, subtype 9, param 24
- Hide/remove HUD contact: contact/list 0, subtype 9, param 27
- Hide/remove HUD contact: contact/list 0, subtype 9, param 28
- Object spawn/action: Crate_7 (object 8, id 133), subtype 0

### Event 22

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 181

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 23
- Hide/remove HUD contact: contact/list 0, subtype 9, param 24
- Set runtime trigger variable: variable group 20, variable 2, subtype 1, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 48
- Show/update HUD contact: contact/list 0, subtype 9, param 49

### Event 23

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 133; flags 2)

**Action**

- Play dialog: TINS.SCR, line/variant 19
- Mission objective/state: param 2, subtype 0, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 30
- Set/add variable: variable group 12, variable 13, subtype 0, value 1
- Set/add variable: variable group 12, variable 14, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 24

**Trigger**

- Variable comparison: subject variable group 12, variable 13, op 1, value 1
- Variable comparison: subject variable group 12, variable 14, op 1, value 2

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1
- Gate state/action: param 15, subtype 2, param 0
- Show/update HUD contact: contact/list 0, subtype 9, param 36
- Hide/remove HUD contact: contact/list 0, subtype 9, param 48
- Hide/remove HUD contact: contact/list 0, subtype 9, param 49

## Waypoints

### Waypoint 0

- Tag: `2`
- Members: `Generic_Minelayer (object 35, id 128, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (3238.66, 0.00, 518.94) | on arrival activate current object (raw param -1 ignored); listened by Event 9 for Generic_Minelayer (object 35, id 128) |

### Waypoint 1

- Tag: `1`
- Members: `Training_Fighter (object 3, id 12, starts at point 0)`, `Training_Fighter (object 4, id 13, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2267.42, 0.00, -925.20) | None |
| 1 | (2641.93, 0.00, 167.80) | None |
| 2 | (1614.84, 0.00, 1284.04) | on arrival redirect to Waypoint 1 (tag 1), point 0 |

## Spawn Lists

### Spawn List 0

- ID: `10`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 9 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Training_Mine` | 5 | Interactive | 742.82,0.00,278.38 | 0,0,0 | group/role: FG_DRAGON / 0 |
| 1 | `Training_Mine` | 9 | Interactive | 1121.09,0.00,639.56 | 0,0,0 | group/role: FG_DRAGON / 0 |
| 2 | `Training_Mine` | 10 | Interactive | 522.53,0.00,1091.95 | 0,0,0 | group/role: FG_DRAGON / 0 |
| 3 | `Training_Fighter` | 12 | Interactive | 2206.41,0.00,-1040.96 | 47,0,0 | group/role: FG_AGT_RIVAL1 / 1; waypoint: Waypoint 1 (tag 1, 3 point(s)), starting point 0, arrival event value 65536 |
| 4 | `Training_Fighter` | 13 | Interactive | 2117.61,0.00,-953.11 | 75,0,0 | group/role: FG_AGT_RIVAL1 / 2; waypoint: Waypoint 1 (tag 1, 3 point(s)), starting point 0, arrival event value 65536 |
| 5 | `Training_Mine` | 95 | Interactive | 989.56,0.00,1405.24 | 0,0,0 | group/role: FG_DRAGON / 0 |
| 6 | `Training_Mine` | 96 | Interactive | 881.16,0.00,2452.11 | 0,0,0 | group/role: FG_DRAGON / 0 |
| 7 | `Navigational_Bouy` | 131 | Interactive | 3402.20,191.79,-1177.07 | 0,0,0 | None |
| 8 | `Crate_7` | 133 | Interactive | 3311.97,191.79,-1172.63 | 0,0,0 | secondary groups: CONT_012, none |
| 9 | `Training_Mine` | 135 | Interactive | 3291.89,191.79,-977.94 | 0,0,0 | group/role: FG_AGT3 / 0 |
| 10 | `Training_Mine` | 136 | Interactive | 3420.42,191.79,-983.04 | 0,0,0 | group/role: FG_AGT3 / 0 |
| 11 | `Training_Mine` | 137 | Interactive | 3548.96,191.79,-1056.13 | 0,0,0 | group/role: FG_AGT3 / 0 |
| 12 | `Training_Mine` | 138 | Interactive | 3555.23,191.79,-1181.90 | 0,0,0 | group/role: FG_AGT3 / 0 |
| 13 | `Training_Mine` | 139 | Interactive | 3552.09,191.79,-1304.27 | 0,0,0 | group/role: FG_AGT3 / 0 |
| 14 | `Training_Mine` | 140 | Interactive | 3418.86,191.79,-1372.26 | 0,0,0 | group/role: FG_AGT3 / 0 |
| 15 | `Training_Mine` | 141 | Interactive | 3280.91,191.79,-1368.86 | 0,0,0 | group/role: FG_AGT3 / 0 |
| 16 | `Training_Mine` | 142 | Interactive | 3169.62,191.79,-1299.17 | 0,0,0 | group/role: FG_AGT3 / 0 |
| 17 | `Training_Mine` | 143 | Interactive | 3169.62,191.79,-1175.10 | 0,0,0 | group/role: FG_AGT3 / 0 |
| 18 | `Training_Mine` | 145 | Interactive | 3169.62,191.79,-1052.73 | 0,0,0 | group/role: FG_AGT3 / 0 |
| 19 | `Training_Mine` | 147 | Interactive | 3834.48,0.00,2055.98 | 0,0,0 | group/role: FG_ACE / 0 |
| 20 | `Training_Mine` | 148 | Interactive | 3743.83,0.00,1207.56 | 0,0,0 | group/role: FG_ACE / 0 |
| 21 | `Training_Mine` | 149 | Interactive | 4107.38,0.00,1584.25 | 0,0,0 | group/role: FG_ACE / 0 |
| 22 | `Training_Mine` | 150 | Interactive | 4300.31,0.00,892.41 | 0,0,0 | group/role: FG_ACE / 0 |
| 23 | `Training_Mine` | 152 | Interactive | 541.96,0.00,1832.81 | 0,0,0 | group/role: FG_DRAGON / 0 |
| 24 | `Training_Mine` | 153 | Interactive | 573.24,0.00,2849.07 | 0,0,0 | group/role: FG_DRAGON / 0 |
| 25 | `Training_Mine` | 154 | Interactive | 4070.87,0.00,512.23 | 0,0,0 | group/role: FG_ACE / 0 |
| 26 | `Training_Mine` | 155 | Interactive | 3892.35,0.00,98.02 | 0,0,0 | group/role: FG_ACE / 0 |
| 27 | `Training_Mine` | 157 | Interactive | 1017.66,0.00,3735.30 | 0,0,0 | group/role: FG_DRAGON / 0 |
| 28 | `Training_Mine` | 158 | Interactive | 1183.62,0.00,3121.32 | 0,0,0 | group/role: FG_DRAGON / 0 |
| 29 | `Training_Mine` | 159 | Interactive | 3352.80,0.00,2933.74 | 0,0,0 | group/role: FG_DRAGON / 0 |
| 30 | `Training_Mine` | 160 | Interactive | 2657.85,0.00,2836.29 | 0,0,0 | group/role: FG_DRAGON / 0 |
| 31 | `Training_Mine` | 162 | Interactive | 1742.89,0.00,3791.32 | 0,0,0 | group/role: FG_DRAGON / 0 |
| 32 | `Training_Mine` | 163 | Interactive | 1996.28,0.00,3399.68 | 0,0,0 | group/role: FG_DRAGON / 0 |
| 33 | `Training_Mine` | 164 | Interactive | 2639.51,0.00,3463.19 | 0,0,0 | group/role: FG_DRAGON / 0 |
| 34 | `Training_Mine` | 165 | Interactive | 3273.00,0.00,2298.84 | 0,0,0 | group/role: FG_DRAGON / 0 |
| 35 | `Generic_Minelayer` | 128 | Interactive | 2207.69,0.00,525.61 | 128,0,0 | secondary groups: CONT_034, none; waypoint: Waypoint 0 (tag 2, 1 point(s)), starting point 0, arrival event value 131072 |
