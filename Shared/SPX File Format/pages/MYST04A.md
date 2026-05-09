# Tachyon: The Fringe MYST04A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST04A.SPX` |
| Sector | `QUAD_04` |
| Backdrop | `(none)` |
| Region | 5 |
| Sector ID | 3 |
| SectorHazardFlags | Twilight fog / fog-radar impairment (0x00000002) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 35 |
| Events | 55 |
| Waypoints | 11 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Cassitor_Shipyard`, `1: Cassitor_Advanced_Drone_Cargo`, `2: Cassitor_Assault_Drone`, `3: Cassitor_Advanced_Drone` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | None |
| Aliases | None |
| Groups | `FG_STRAIN_CHI`, `FG_STRAIN_LAMBDA`, `FG_STRAIN_OMEGA`, `FG_STRAIN_NU`, `FG_STRAIN_THETA`, `FG_STRAIN_XI` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Play scene: unknown index 0, param 0
- Play dialog: PLAYER.SCR, line/variant 39
- Show/update HUD contact: contact/list 0, subtype 9, param 23

### Event 1

**Trigger**

- Object event: subject 191, op 14, value 41
- Variable comparison: subject variable group 21, variable 27, op 1, value 0

**Action**

- Group/spawn-list action: spawn list/group 207, subtype 4, param 1
- Group/spawn-list action: spawn list/group 208, subtype 4, param 1
- Group/spawn-list action: spawn list/group 212, subtype 4, param 1
- Group/spawn-list action: spawn list/group 215, subtype 4, param 1
- Set/add variable: variable group 21, variable 20, subtype 0, value 1
- Object spawn/action: id 190, subtype 8, param 1

### Event 2

**Trigger**

- Object event: subject 191, op 14, value 33
- Variable comparison: subject variable group 21, variable 27, op 1, value 0

**Action**

- Group/spawn-list action: spawn list/group 214, subtype 4, param 1
- Group/spawn-list action: spawn list/group 208, subtype 4, param 1
- Group/spawn-list action: spawn list/group 212, subtype 4, param 1
- Group/spawn-list action: spawn list/group 215, subtype 4, param 1
- Set/add variable: variable group 21, variable 21, subtype 0, value 1
- Object spawn/action: id 190, subtype 8, param 1

### Event 3

**Trigger**

- Object event: subject 191, op 14, value 25
- Variable comparison: subject variable group 21, variable 27, op 1, value 0

**Action**

- Group/spawn-list action: spawn list/group 207, subtype 4, param 1
- Group/spawn-list action: spawn list/group 214, subtype 4, param 1
- Object spawn/action: id 190, subtype 8, param 1
- Group/spawn-list action: spawn list/group 212, subtype 4, param 1
- Group/spawn-list action: spawn list/group 215, subtype 4, param 1
- Set/add variable: variable group 21, variable 22, subtype 0, value 1

### Event 4

**Trigger**

- Object event: subject 191, op 14, value 59
- Variable comparison: subject variable group 21, variable 27, op 1, value 0

**Action**

- Group/spawn-list action: spawn list/group 207, subtype 4, param 1
- Group/spawn-list action: spawn list/group 214, subtype 4, param 1
- Group/spawn-list action: spawn list/group 208, subtype 4, param 1
- Object spawn/action: id 190, subtype 8, param 1
- Group/spawn-list action: spawn list/group 215, subtype 4, param 1
- Set/add variable: variable group 21, variable 23, subtype 0, value 1

### Event 5

**Trigger**

- Object event: subject 191, op 14, value 57
- Variable comparison: subject variable group 21, variable 27, op 1, value 0

**Action**

- Group/spawn-list action: spawn list/group 207, subtype 4, param 1
- Group/spawn-list action: spawn list/group 214, subtype 4, param 1
- Group/spawn-list action: spawn list/group 208, subtype 4, param 1
- Set/add variable: variable group 21, variable 24, subtype 0, value 1
- Object spawn/action: id 190, subtype 8, param 1
- Group/spawn-list action: spawn list/group 212, subtype 4, param 1

### Event 6

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 241; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 242; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 243; flags 3)
- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Set/add variable: variable group 21, variable 29, subtype 0, value 1
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 19, id 241), subtype 15
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 20, id 242), subtype 15
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 21, id 243), subtype 15

### Event 7

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 244; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 245; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 246; flags 2)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Set/add variable: variable group 21, variable 29, subtype 0, value 1
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 22, id 244), subtype 15
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 23, id 245), subtype 15
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 24, id 246), subtype 15

### Event 8

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 253; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 254; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 255; flags 2)
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Set/add variable: variable group 21, variable 29, subtype 0, value 1
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 31, id 253), subtype 15
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 32, id 254), subtype 15
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 33, id 255), subtype 15

### Event 9

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 247; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 248; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 249; flags 2)
- Variable comparison: subject variable group 21, variable 23, op 1, value 1

**Action**

- Set/add variable: variable group 21, variable 29, subtype 0, value 1
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 25, id 247), subtype 15
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 26, id 248), subtype 15
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 27, id 249), subtype 15

### Event 10

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 250; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 251; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 252; flags 2)
- Variable comparison: subject variable group 21, variable 24, op 1, value 1

**Action**

- Set/add variable: variable group 21, variable 29, subtype 0, value 1
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 28, id 250), subtype 15
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 29, id 251), subtype 15
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 30, id 252), subtype 15

### Event 11

**Trigger**

- Variable comparison: subject variable group 21, variable 29, op 1, value 1

**Action**

- Set/add variable: variable group 17, variable 404, subtype 0, value 1
- Set/add variable: variable group 17, variable 405, subtype 0, value 2
- Hide/remove HUD contact: contact/list 0, subtype 9, param 24
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Play dialog: PLAYER.SCR, line/variant 42
- Group/spawn-list action: spawn list/group 206, subtype 1, param 2
- Show/update HUD contact: contact/list 0, subtype 12, param 28
- Set/add variable: variable group 38, variable 9, subtype 0, value 1

### Event 12

**Trigger**

- Variable comparison: subject variable group 21, variable 29, op 1, value 1

**Action**

- Set runtime trigger variable: variable group 20, variable 9, subtype 0, value 0

### Event 13

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 214, subtype 8, param 6881280 (Waypoint 4 (tag 105), point 0)
- Group/spawn-list action: spawn list/group 212, subtype 8, param 6881280 (Waypoint 4 (tag 105), point 0)
- Group/spawn-list action: spawn list/group 215, subtype 8, param 6881280 (Waypoint 4 (tag 105), point 0)
- Group/spawn-list action: spawn list/group 208, subtype 8, param 6881280 (Waypoint 4 (tag 105), point 0)

### Event 14

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 207, subtype 8, param 6946816 (Waypoint 3 (tag 106), point 0)
- Group/spawn-list action: spawn list/group 212, subtype 8, param 6946816 (Waypoint 3 (tag 106), point 0)
- Group/spawn-list action: spawn list/group 215, subtype 8, param 6946816 (Waypoint 3 (tag 106), point 0)
- Group/spawn-list action: spawn list/group 208, subtype 8, param 6946816 (Waypoint 3 (tag 106), point 0)

### Event 15

**Trigger**

- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 207, subtype 8, param 7012352 (Waypoint 2 (tag 107), point 0)
- Group/spawn-list action: spawn list/group 214, subtype 8, param 7012352 (Waypoint 2 (tag 107), point 0)
- Group/spawn-list action: spawn list/group 212, subtype 8, param 7012352 (Waypoint 2 (tag 107), point 0)
- Group/spawn-list action: spawn list/group 215, subtype 8, param 7012352 (Waypoint 2 (tag 107), point 0)

### Event 16

**Trigger**

- Variable comparison: subject variable group 21, variable 23, op 1, value 1 (join 2)
- Variable comparison: subject variable group 21, variable 24, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 207, subtype 8, param 7077888 (Waypoint 1 (tag 108), point 0)
- Group/spawn-list action: spawn list/group 214, subtype 8, param 7077888 (Waypoint 1 (tag 108), point 0)
- Group/spawn-list action: spawn list/group 208, subtype 8, param 7077888 (Waypoint 1 (tag 108), point 0)

### Event 17

**Trigger**

- Object event: subject 191, op 14, value 33 (join 2)
- Object event: subject 191, op 14, value 41 (join 2)
- Object event: subject 191, op 14, value 59 (join 2)
- Object event: subject 191, op 14, value 57 (join 2)
- Object event: subject 191, op 14, value 25 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 40
- Set/add variable: variable group 21, variable 27, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 23
- Show/update HUD contact: contact/list 0, subtype 9, param 24

### Event 18

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Object spawn/action: Cassitor_Advanced_Drone (object 3, id 117), subtype 19
- Object spawn/action: Cassitor_Advanced_Drone (object 4, id 118), subtype 19
- Object spawn/action: Cassitor_Advanced_Drone (object 7, id 136), subtype 19
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 22, id 244), subtype 0
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 23, id 245), subtype 0
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 24, id 246), subtype 0

### Event 19

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Object spawn/action: Cassitor_Advanced_Drone (object 0, id 113), subtype 19
- Object spawn/action: Cassitor_Advanced_Drone (object 1, id 114), subtype 19
- Object spawn/action: Cassitor_Advanced_Drone (object 2, id 115), subtype 19
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 19, id 241), subtype 0
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 20, id 242), subtype 0
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 21, id 243), subtype 0

### Event 20

**Trigger**

- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Object spawn/action: Cassitor_Advanced_Drone (object 9, id 212), subtype 19
- Object spawn/action: Cassitor_Advanced_Drone (object 10, id 213), subtype 19
- Object spawn/action: Cassitor_Advanced_Drone (object 11, id 214), subtype 19
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 31, id 253), subtype 0
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 32, id 254), subtype 0
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 33, id 255), subtype 0

### Event 21

**Trigger**

- Variable comparison: subject variable group 21, variable 23, op 1, value 1

**Action**

- Object spawn/action: Cassitor_Advanced_Drone (object 5, id 125), subtype 19
- Object spawn/action: Cassitor_Advanced_Drone (object 6, id 126), subtype 19
- Object spawn/action: Cassitor_Advanced_Drone (object 8, id 138), subtype 19
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 25, id 247), subtype 0
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 26, id 248), subtype 0
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 27, id 249), subtype 0

### Event 22

**Trigger**

- Variable comparison: subject variable group 21, variable 24, op 1, value 1

**Action**

- Object spawn/action: Cassitor_Advanced_Drone (object 12, id 220), subtype 19
- Object spawn/action: Cassitor_Advanced_Drone (object 13, id 221), subtype 19
- Object spawn/action: Cassitor_Advanced_Drone (object 14, id 222), subtype 19
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 28, id 250), subtype 0
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 29, id 251), subtype 0
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 30, id 252), subtype 0

### Event 23

**Trigger**

- Variable comparison: subject variable group 21, variable 30, op 1, value 1
- Variable comparison: subject variable group 21, variable 31, op 1, value 1
- Variable comparison: subject variable group 21, variable 32, op 1, value 1
- Variable comparison: subject variable group 21, variable 33, op 1, value 1
- Variable comparison: subject variable group 21, variable 34, op 1, value 1
- Variable comparison: subject variable group 21, variable 27, op 1, value 0

**Action**

- Set/add variable: variable group 21, variable 28, subtype 0, value 1

### Event 24

**Trigger**

- Object event: subject Cassitor_Advanced_Drone_Cargo (object 19, id 241), op 2, value 0
- Object event: subject Cassitor_Advanced_Drone_Cargo (object 20, id 242), op 2, value 0
- Object event: subject Cassitor_Advanced_Drone_Cargo (object 21, id 243), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 28, subtype 0, value 1

### Event 25

**Trigger**

- Object event: subject Cassitor_Advanced_Drone_Cargo (object 22, id 244), op 2, value 0
- Object event: subject Cassitor_Advanced_Drone_Cargo (object 23, id 245), op 2, value 0
- Object event: subject Cassitor_Advanced_Drone_Cargo (object 24, id 246), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 28, subtype 0, value 1

### Event 26

**Trigger**

- Object event: subject Cassitor_Advanced_Drone_Cargo (object 25, id 247), op 2, value 0
- Object event: subject Cassitor_Advanced_Drone_Cargo (object 26, id 248), op 2, value 0
- Object event: subject Cassitor_Advanced_Drone_Cargo (object 27, id 249), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 28, subtype 0, value 1

### Event 27

**Trigger**

- Object event: subject Cassitor_Advanced_Drone_Cargo (object 28, id 250), op 2, value 0
- Object event: subject Cassitor_Advanced_Drone_Cargo (object 29, id 251), op 2, value 0
- Object event: subject Cassitor_Advanced_Drone_Cargo (object 30, id 252), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 28, subtype 0, value 1

### Event 28

**Trigger**

- Object event: subject Cassitor_Advanced_Drone_Cargo (object 31, id 253), op 2, value 0
- Object event: subject Cassitor_Advanced_Drone_Cargo (object 32, id 254), op 2, value 0
- Object event: subject Cassitor_Advanced_Drone_Cargo (object 33, id 255), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 28, subtype 0, value 1

### Event 29

**Trigger**

- Variable comparison: subject variable group 21, variable 28, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 11, param 29
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 17, variable 405, subtype 0, value 1
- Set/add variable: variable group 17, variable 404, subtype 0, value 0

### Event 30

**Trigger**

- Object event: subject Cassitor_Advanced_Drone (object 0, id 113), op 2, value 0
- Object event: subject Cassitor_Advanced_Drone (object 1, id 114), op 2, value 0
- Object event: subject Cassitor_Advanced_Drone (object 2, id 115), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 31, subtype 0, value 1

### Event 31

**Trigger**

- Object event: subject Cassitor_Advanced_Drone (object 3, id 117), op 2, value 0
- Object event: subject Cassitor_Advanced_Drone (object 4, id 118), op 2, value 0
- Object event: subject Cassitor_Advanced_Drone (object 7, id 136), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 30, subtype 0, value 1

### Event 32

**Trigger**

- Object event: subject Cassitor_Advanced_Drone (object 5, id 125), op 2, value 0
- Object event: subject Cassitor_Advanced_Drone (object 6, id 126), op 2, value 0
- Object event: subject Cassitor_Advanced_Drone (object 8, id 138), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 33, subtype 0, value 1

### Event 33

**Trigger**

- Object event: subject Cassitor_Advanced_Drone (object 12, id 220), op 2, value 0
- Object event: subject Cassitor_Advanced_Drone (object 13, id 221), op 2, value 0
- Object event: subject Cassitor_Advanced_Drone (object 14, id 222), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 34, subtype 0, value 1

### Event 34

**Trigger**

- Object event: subject Cassitor_Advanced_Drone (object 9, id 212), op 2, value 0
- Object event: subject Cassitor_Advanced_Drone (object 10, id 213), op 2, value 0
- Object event: subject Cassitor_Advanced_Drone (object 11, id 214), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 32, subtype 0, value 1

### Event 35

**Trigger**

- Object event: subject Cassitor_Advanced_Drone_Cargo (object 19, id 241), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 19, id 241), subtype 7

### Event 36

**Trigger**

- Object event: subject Cassitor_Advanced_Drone_Cargo (object 20, id 242), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 20, id 242), subtype 7

### Event 37

**Trigger**

- Object event: subject Cassitor_Advanced_Drone_Cargo (object 21, id 243), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 21, id 243), subtype 7

### Event 38

**Trigger**

- Object event: subject Cassitor_Advanced_Drone_Cargo (object 22, id 244), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 22, id 244), subtype 7

### Event 39

**Trigger**

- Object event: subject Cassitor_Advanced_Drone_Cargo (object 23, id 245), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 23, id 245), subtype 7

### Event 40

**Trigger**

- Object event: subject Cassitor_Advanced_Drone_Cargo (object 24, id 246), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 24, id 246), subtype 7

### Event 41

**Trigger**

- Object event: subject Cassitor_Advanced_Drone_Cargo (object 25, id 247), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 25, id 247), subtype 7

### Event 42

**Trigger**

- Object event: subject Cassitor_Advanced_Drone_Cargo (object 26, id 248), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 26, id 248), subtype 7

### Event 43

**Trigger**

- Object event: subject Cassitor_Advanced_Drone_Cargo (object 27, id 249), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 27, id 249), subtype 7

### Event 44

**Trigger**

- Object event: subject Cassitor_Advanced_Drone_Cargo (object 28, id 250), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 28, id 250), subtype 7

### Event 45

**Trigger**

- Object event: subject Cassitor_Advanced_Drone_Cargo (object 29, id 251), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 29, id 251), subtype 7

### Event 46

**Trigger**

- Object event: subject Cassitor_Advanced_Drone_Cargo (object 30, id 252), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 30, id 252), subtype 7

### Event 47

**Trigger**

- Object event: subject Cassitor_Advanced_Drone_Cargo (object 31, id 253), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 31, id 253), subtype 7

### Event 48

**Trigger**

- Object event: subject Cassitor_Advanced_Drone_Cargo (object 32, id 254), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 32, id 254), subtype 7

### Event 49

**Trigger**

- Object event: subject Cassitor_Advanced_Drone_Cargo (object 33, id 255), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 33, id 255), subtype 7

### Event 50

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 22, id 244), subtype 14
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 23, id 245), subtype 14
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 24, id 246), subtype 14

### Event 51

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 19, id 241), subtype 14
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 20, id 242), subtype 14
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 21, id 243), subtype 14

### Event 52

**Trigger**

- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 31, id 253), subtype 14
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 32, id 254), subtype 14
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 33, id 255), subtype 14

### Event 53

**Trigger**

- Variable comparison: subject variable group 21, variable 23, op 1, value 1

**Action**

- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 25, id 247), subtype 14
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 26, id 248), subtype 14
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 27, id 249), subtype 14

### Event 54

**Trigger**

- Variable comparison: subject variable group 21, variable 24, op 1, value 1

**Action**

- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 28, id 250), subtype 14
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 29, id 251), subtype 14
- Object spawn/action: Cassitor_Advanced_Drone_Cargo (object 30, id 252), subtype 14

## Waypoints

### Waypoint 0

- Tag: `109`
- Members: `Cassitor_Assault_Drone (object 15, id 234, starts at point 0)`, `Cassitor_Assault_Drone (object 16, id 235, starts at point 0)`, `Cassitor_Assault_Drone (object 17, id 236, starts at point 0)`, `Cassitor_Assault_Drone (object 18, id 237, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1597.79, 592.07, 1958.61) | None |

### Waypoint 1

- Tag: `108`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (782.71, 170.17, -70.00) | None |

### Waypoint 2

- Tag: `107`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-116.17, 254.13, -484.91) | None |

### Waypoint 3

- Tag: `106`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-922.39, 358.10, 447.29) | None |

### Waypoint 4

- Tag: `105`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-457.23, 233.14, 1196.28) | None |

### Waypoint 5

- Tag: `103`
- Members: `Cassitor_Advanced_Drone (object 12, id 220, starts at point 1)`, `Cassitor_Advanced_Drone (object 13, id 221, starts at point 2)`, `Cassitor_Advanced_Drone (object 14, id 222, starts at point 3)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (599.19, 156.20, -314.97) | None |
| 1 | (1019.10, 123.97, -627.13) | None |
| 2 | (1356.81, 160.41, -102.34) | None |
| 3 | (892.78, 151.32, 238.85) | None |

### Waypoint 6

- Tag: `102`
- Members: `Cassitor_Advanced_Drone (object 9, id 212, starts at point 0)`, `Cassitor_Advanced_Drone (object 10, id 213, starts at point 2)`, `Cassitor_Advanced_Drone (object 11, id 214, starts at point 3)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-290.65, 270.09, -1011.62) | None |
| 1 | (320.58, 230.66, -965.23) | None |
| 2 | (176.42, 252.24, -336.19) | None |
| 3 | (-398.58, 217.03, -382.81) | None |

### Waypoint 7

- Tag: `4`
- Members: `Cassitor_Advanced_Drone (object 5, id 125, starts at point 0)`, `Cassitor_Advanced_Drone (object 6, id 126, starts at point 2)`, `Cassitor_Advanced_Drone (object 8, id 138, starts at point 3)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-10.49, 455.78, 610.41) | None |
| 1 | (540.68, 351.07, 803.24) | None |
| 2 | (813.78, 497.68, 213.29) | None |
| 3 | (184.59, 519.50, -1.25) | on arrival redirect to Waypoint 7 (tag 4), point 0 |

### Waypoint 8

- Tag: `3`
- Members: `Cassitor_Advanced_Drone (object 3, id 117, starts at point 0)`, `Cassitor_Advanced_Drone (object 4, id 118, starts at point 6)`, `Cassitor_Advanced_Drone (object 7, id 136, starts at point 4)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1384.55, 395.87, 515.37) | None |
| 1 | (-1070.26, 402.48, 780.77) | None |
| 2 | (-738.51, 322.64, 424.13) | None |
| 3 | (-978.86, 350.00, 40.77) | None |
| 4 | (-1334.45, 276.12, 125.04) | on arrival redirect to Waypoint 8 (tag 3), point 0 |

### Waypoint 9

- Tag: `2`
- Members: `Cassitor_Advanced_Drone (object 1, id 114, starts at point 0)`, `Cassitor_Advanced_Drone (object 2, id 115, starts at point 2)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-862.93, 265.52, 1250.42) | None |
| 1 | (-1053.18, 265.52, 1612.02) | None |
| 2 | (-712.50, 272.55, 1914.63) | None |
| 3 | (-372.64, 257.09, 1628.32) | None |
| 4 | (-528.83, 257.09, 1250.94) | on arrival redirect to Waypoint 9 (tag 2), point 0 |

### Waypoint 10

- Tag: `1`
- Members: `Cassitor_Advanced_Drone (object 0, id 113, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-873.61, 90.63, 1600.96) | None |
| 1 | (-834.77, 179.65, 1567.17) | None |
| 2 | (-744.06, 255.57, 1612.85) | None |
| 3 | (-650.13, 81.65, 1433.17) | None |
| 4 | (-550.69, 119.60, 1409.82) | None |
| 5 | (-627.33, 132.69, 1560.07) | on arrival redirect to Waypoint 10 (tag 1), point 1 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Cassitor_Advanced_Drone` | 113 | Interactive | -475.59,257.08,1600.90 | 385,46,3 | group/role: FG_STRAIN_CHI / 3; waypoint: Waypoint 10 (tag 1, 6 point(s)), starting point 0, arrival event value 65536 |
| 1 | `Cassitor_Advanced_Drone` | 114 | Interactive | -741.49,265.52,1317.75 | 384,0,0 | group/role: FG_STRAIN_CHI / 2; waypoint: Waypoint 9 (tag 2, 5 point(s)), starting point 0, arrival event value 131072 |
| 2 | `Cassitor_Advanced_Drone` | 115 | Interactive | -961.61,23.95,1558.73 | 0,0,0 | group/role: FG_STRAIN_CHI / 1; waypoint: Waypoint 9 (tag 2, 5 point(s)), starting point 2, arrival event value 131074 |
| 3 | `Cassitor_Advanced_Drone` | 117 | Interactive | -1293.81,395.87,550.65 | 0,0,0 | group/role: FG_STRAIN_LAMBDA / 2; waypoint: Waypoint 8 (tag 3, 5 point(s)), starting point 0, arrival event value 196608 |
| 4 | `Cassitor_Advanced_Drone` | 118 | Interactive | -1100.09,362.56,222.68 | 0,0,0 | group/role: FG_STRAIN_LAMBDA / 3; waypoint: Waypoint 8 (tag 3, 5 point(s)), starting point 6 |
| 5 | `Cassitor_Advanced_Drone` | 125 | Interactive | 387.64,515.87,194.24 | 0,0,0 | group/role: FG_STRAIN_OMEGA / 3; waypoint: Waypoint 7 (tag 4, 4 point(s)), starting point 0, arrival event value 262144 |
| 6 | `Cassitor_Advanced_Drone` | 126 | Interactive | 550.25,217.68,634.49 | 64,0,0 | group/role: FG_STRAIN_OMEGA / 2; waypoint: Waypoint 7 (tag 4, 4 point(s)), starting point 2, arrival event value 262146 |
| 7 | `Cassitor_Advanced_Drone` | 136 | Interactive | -1079.98,355.20,566.78 | 0,0,0 | group/role: FG_STRAIN_LAMBDA / 1; waypoint: Waypoint 8 (tag 3, 5 point(s)), starting point 4, arrival event value 196612 |
| 8 | `Cassitor_Advanced_Drone` | 138 | Interactive | 889.55,140.00,505.19 | 192,0,0 | group/role: FG_STRAIN_OMEGA / 1; waypoint: Waypoint 7 (tag 4, 4 point(s)), starting point 3, arrival event value 262147 |
| 9 | `Cassitor_Advanced_Drone` | 212 | Interactive | -181.07,243.56,-563.54 | 320,0,0 | group/role: FG_STRAIN_NU / 1; waypoint: Waypoint 6 (tag 102, 4 point(s)), starting point 0, arrival event value 6684672 |
| 10 | `Cassitor_Advanced_Drone` | 213 | Interactive | -130.76,243.56,-795.07 | 192,0,0 | group/role: FG_STRAIN_NU / 2; waypoint: Waypoint 6 (tag 102, 4 point(s)), starting point 2, arrival event value 6684674 |
| 11 | `Cassitor_Advanced_Drone` | 214 | Interactive | 22.87,243.56,-760.36 | 64,0,0 | group/role: FG_STRAIN_NU / 3; waypoint: Waypoint 6 (tag 102, 4 point(s)), starting point 3, arrival event value 6684675 |
| 12 | `Cassitor_Advanced_Drone` | 220 | Interactive | 945.14,133.80,-216.77 | 256,0,0 | group/role: FG_STRAIN_THETA / 1; waypoint: Waypoint 5 (tag 103, 4 point(s)), starting point 1, arrival event value 6750209 |
| 13 | `Cassitor_Advanced_Drone` | 221 | Interactive | 1108.74,155.37,-344.01 | 0,0,0 | group/role: FG_STRAIN_THETA / 3; waypoint: Waypoint 5 (tag 103, 4 point(s)), starting point 2, arrival event value 6750210 |
| 14 | `Cassitor_Advanced_Drone` | 222 | Interactive | 1150.88,180.08,-201.90 | 0,0,0 | group/role: FG_STRAIN_THETA / 2; waypoint: Waypoint 5 (tag 103, 4 point(s)), starting point 3, arrival event value 6750211 |
| 15 | `Cassitor_Assault_Drone` | 234 | Interactive | -2049.77,0.00,1997.70 | 0,0,0 | group/role: FG_STRAIN_XI / 1; waypoint: Waypoint 0 (tag 109, 1 point(s)), starting point 0, arrival event value 7143424 |
| 16 | `Cassitor_Assault_Drone` | 235 | Interactive | -1967.84,0.00,2146.96 | 0,0,0 | group/role: FG_STRAIN_XI / 2; waypoint: Waypoint 0 (tag 109, 1 point(s)), starting point 0, arrival event value 7143424 |
| 17 | `Cassitor_Assault_Drone` | 236 | Interactive | -1813.80,0.00,2246.46 | 0,0,0 | group/role: FG_STRAIN_XI / 3; waypoint: Waypoint 0 (tag 109, 1 point(s)), starting point 0, arrival event value 7143424 |
| 18 | `Cassitor_Assault_Drone` | 237 | Interactive | -1626.98,0.00,2282.00 | 0,0,0 | group/role: FG_STRAIN_XI / 4; waypoint: Waypoint 0 (tag 109, 1 point(s)), starting point 0, arrival event value 7143424 |
| 19 | `Cassitor_Advanced_Drone_Cargo` | 241 | Interactive | -982.03,271.32,1435.78 | 299,0,0 | group/role: FG_STRAIN_CHI / 1 |
| 20 | `Cassitor_Advanced_Drone_Cargo` | 242 | Interactive | -686.33,314.30,1243.53 | 206,0,0 | group/role: FG_STRAIN_CHI / 2 |
| 21 | `Cassitor_Advanced_Drone_Cargo` | 243 | Interactive | -369.66,271.16,1598.35 | 391,43,50 | group/role: FG_STRAIN_CHI / 3 |
| 22 | `Cassitor_Advanced_Drone_Cargo` | 244 | Interactive | -1139.45,400.00,71.07 | 220,0,0 | group/role: FG_STRAIN_LAMBDA / 3 |
| 23 | `Cassitor_Advanced_Drone_Cargo` | 245 | Interactive | -857.57,324.26,424.50 | 71,57,0 | group/role: FG_STRAIN_LAMBDA / 1 |
| 24 | `Cassitor_Advanced_Drone_Cargo` | 246 | Interactive | -1260.95,332.23,665.69 | 0,0,0 | group/role: FG_STRAIN_LAMBDA / 2 |
| 25 | `Cassitor_Advanced_Drone_Cargo` | 247 | Interactive | 51.71,461.73,671.75 | 185,28,0 | group/role: FG_STRAIN_OMEGA / 3 |
| 26 | `Cassitor_Advanced_Drone_Cargo` | 248 | Interactive | 303.57,466.69,15.05 | 455,434,0 | group/role: FG_STRAIN_OMEGA / 1 |
| 27 | `Cassitor_Advanced_Drone_Cargo` | 249 | Interactive | 709.92,456.20,570.47 | 313,0,0 | group/role: FG_STRAIN_OMEGA / 2 |
| 28 | `Cassitor_Advanced_Drone_Cargo` | 250 | Interactive | 1036.13,170.17,187.73 | 448,85,78 | group/role: FG_STRAIN_THETA / 2 |
| 29 | `Cassitor_Advanced_Drone_Cargo` | 251 | Interactive | 574.62,164.68,-280.42 | 85,427,85 | group/role: FG_STRAIN_THETA / 3 |
| 30 | `Cassitor_Advanced_Drone_Cargo` | 252 | Interactive | 1230.14,170.17,-491.80 | 36,484,484 | group/role: FG_STRAIN_THETA / 1 |
| 31 | `Cassitor_Advanced_Drone_Cargo` | 253 | Interactive | -77.57,261.57,-1010.71 | 128,43,14 | group/role: FG_STRAIN_NU / 3 |
| 32 | `Cassitor_Advanced_Drone_Cargo` | 254 | Interactive | -292.26,278.98,-394.57 | 334,0,0 | group/role: FG_STRAIN_NU / 1 |
| 33 | `Cassitor_Advanced_Drone_Cargo` | 255 | Interactive | 279.26,261.57,-590.77 | 498,71,50 | group/role: FG_STRAIN_NU / 2 |
| 34 | `Cassitor_Shipyard` | 189 | Interactive | 356.71,477.77,378.31 | 128,0,0 | None |
