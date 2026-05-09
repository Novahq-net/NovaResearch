# Tachyon: The Fringe BORA08A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `BORA08A.SPX` |
| Sector | `QUAD_08` |
| Backdrop | `(none)` |
| Region | 3 |
| Sector ID | 7 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 8 |
| Events | 7 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Mace`, `1: Bora_Warhammer`, `2: Bora_Battleaxe` |
| Scripts | `PLAYER.SCR`, `NOLTL.SCR`, `NGAIA.SCR` |
| Scenes | None |
| Labels | `BFBE_08` |
| Aliases | None |
| Groups | `FG_WORTHY`, `FG_MERIT`, `FG_NOBLE` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 0, variable 7, op 1, value 10
- Variable comparison: subject variable group 36, variable 10, op 1, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 51
- Group/spawn-list action: spawn list/group 188, subtype 0
- Show/update HUD contact: contact/list 0, subtype 9, param 23
- Object spawn/action: id 7, subtype 14

### Event 1

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 51
- Variable comparison: subject variable group 0, variable 7, op 1, value 10

**Action**

- Play dialog: PLAYER.SCR, line/variant 108
- Hide/remove HUD contact: contact/list 0, subtype 9, param 23
- Show/update HUD contact: contact/list 0, subtype 1, param 188
- Group/spawn-list action: spawn list/group 188, subtype 4, param 9

### Event 2

**Trigger**

- Group/spawn-list event: subject 188, op 0, value 0
- Variable comparison: subject variable group 0, variable 7, op 1, value 10

**Action**

- Play dialog: NOLTL.SCR, line/variant 1
- Show/update HUD contact: contact/list 0, subtype 9, param 23

### Event 3

**Trigger**

- Variable comparison: subject variable group 36, variable 10, op 1, value 0
- Group/spawn-list event: subject 188, op 0, value 0
- Sector/startup condition family: subject 1, op 0, value 1

**Action**

- Set/add variable: variable group 15, variable 410, subtype 0, value 1
- Set/add variable: variable group 15, variable 411, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Object spawn/action: id 7, subtype 15
- Show/update HUD contact: contact/list 0, subtype 12, param 19
- Hide/remove HUD contact: contact/list 0, subtype 9, param 23

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (join 1)
- Variable comparison: subject variable group 0, variable 7, op 1, value 10 (join 2)
- Variable comparison: subject variable group 36, variable 10, op 1, value 1 (join 1)

**Action**

- Play dialog: PLAYER.SCR, line/variant 45
- Object spawn/action: id 7, subtype 14
- Group/spawn-list action: spawn list/group 188, subtype 0
- Group/spawn-list action: spawn list/group 190, subtype 0
- Group/spawn-list action: spawn list/group 189, subtype 0
- Show/update HUD contact: contact/list 0, subtype 9, param 23

### Event 5

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 45

**Action**

- Group/spawn-list action: spawn list/group 188, subtype 4, param 9
- Group/spawn-list action: spawn list/group 190, subtype 4, param 9
- Group/spawn-list action: spawn list/group 189, subtype 4, param 9
- Show/update HUD contact: contact/list 0, subtype 1, param 188
- Show/update HUD contact: contact/list 0, subtype 1, param 190
- Show/update HUD contact: contact/list 0, subtype 1, param 189
- Hide/remove HUD contact: contact/list 0, subtype 9, param 23

### Event 6

**Trigger**

- Group/spawn-list event: subject 188, op 0, value 0
- Group/spawn-list event: subject 190, op 0, value 0
- Group/spawn-list event: subject 189, op 0, value 0

**Action**

- Set/add variable: variable group 15, variable 410, subtype 0, value 1
- Set/add variable: variable group 15, variable 411, subtype 0, value 3
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Play dialog: NGAIA.SCR, line/variant 2
- Object spawn/action: id 7, subtype 15
- Show/update HUD contact: contact/list 0, subtype 12, param 19

## Waypoints

### Waypoint 0

- Tag: `103`
- Members: `Bora_Mace (object 6, id 13, starts at point 0)`, `Bora_Mace (object 7, id 14, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (844.40, 0.00, 4883.34) | None |
| 1 | (527.51, 0.00, 4482.47) | None |
| 2 | (429.21, 0.00, 4096.45) | None |
| 3 | (344.52, 0.00, 3740.17) | None |
| 4 | (257.78, 0.00, 3456.94) | None |

### Waypoint 1

- Tag: `102`
- Members: `Bora_Battleaxe (object 0, id 9, starts at point 0)`, `Bora_Battleaxe (object 1, id 10, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (138.07, -105.00, 4756.07) | None |
| 1 | (845.74, -193.00, 4500.29) | None |
| 2 | (1253.70, -183.00, 4144.77) | None |
| 3 | (1405.04, -152.00, 3778.86) | None |
| 4 | (1842.13, -118.00, 3246.79) | on arrival redirect to Waypoint 0 (tag 103), point 0 |

### Waypoint 2

- Tag: `101`
- Members: `Bora_Warhammer (object 2, id 17, starts at point 0)`, `Bora_Warhammer (object 3, id 18, starts at point 0)`, `Bora_Warhammer (object 4, id 19, starts at point 0)`, `Bora_Warhammer (object 5, id 20, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1663.16, 98.00, 3158.27) | None |
| 1 | (1161.83, 104.00, 3179.46) | None |
| 2 | (828.36, 133.00, 3149.62) | None |
| 3 | (392.24, 144.00, 2806.88) | on arrival redirect to Waypoint 1 (tag 102), point 0 |

## Spawn Lists

### Spawn List 0

- ID: `190`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 1

- ID: `189`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 2

- ID: `188`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Bora_Battleaxe` | 9 | Interactive | -938.70,0.00,4675.50 | 149,0,0 | label: BFBE_08; group/role: FG_WORTHY / 0; waypoint: Waypoint 1 (tag 102, 5 point(s)), starting point 0, arrival event value 6684672 |
| 1 | `Bora_Battleaxe` | 10 | Interactive | -786.92,0.00,4675.50 | 150,0,0 | group/role: FG_WORTHY / 0; waypoint: Waypoint 1 (tag 102, 5 point(s)), starting point 0, arrival event value 6684672 |
| 2 | `Bora_Warhammer` | 17 | Interactive | 1801.78,0.00,3109.64 | 304,0,0 | group/role: FG_MERIT / 0; waypoint: Waypoint 2 (tag 101, 4 point(s)), starting point 0, arrival event value 6619136 |
| 3 | `Bora_Warhammer` | 18 | Interactive | 1915.62,0.00,3109.64 | 304,0,0 | label: BFBE_08; group/role: FG_MERIT / 0; waypoint: Waypoint 2 (tag 101, 4 point(s)), starting point 0, arrival event value 6619136 |
| 4 | `Bora_Warhammer` | 19 | Interactive | 2105.34,0.00,3089.07 | 304,0,0 | group/role: FG_MERIT / 0; waypoint: Waypoint 2 (tag 101, 4 point(s)), starting point 0, arrival event value 6619136 |
| 5 | `Bora_Warhammer` | 20 | Interactive | 2238.15,0.00,3068.50 | 304,0,0 | label: BFBE_08; group/role: FG_MERIT / 0; waypoint: Waypoint 2 (tag 101, 4 point(s)), starting point 0, arrival event value 6619136 |
| 6 | `Bora_Mace` | 13 | Interactive | 802.46,0.00,5012.03 | 314,0,0 | label: BFBE_08; group/role: FG_NOBLE / 0; waypoint: Waypoint 0 (tag 103, 5 point(s)), starting point 0, arrival event value 6750208 |
| 7 | `Bora_Mace` | 14 | Interactive | 935.27,0.00,5012.03 | 313,0,0 | group/role: FG_NOBLE / 0; waypoint: Waypoint 0 (tag 103, 5 point(s)), starting point 0, arrival event value 6750208 |
