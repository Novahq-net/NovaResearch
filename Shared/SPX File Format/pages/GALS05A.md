# Tachyon: The Fringe GALS05A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `GALS05A.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `(none)` |
| Region | 2 |
| Sector ID | 4 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 8 |
| Entities | 21 |
| Events | 22 |
| Waypoints | 5 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Lt_Freighter`, `1: GalSpan_Heavy_Freighter`, `2: Bora_Cutlass`, `3: GalSpan_Pegasus`, `4: Bora_Warhammer`, `5: Satellite`, `6: Skav_Pirate_Manta`, `7: GalSpan_Poseidon` |
| Scripts | `TRISH.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `bfne_02`, `BFGE_04`, `bfne_03`, `bfgf_02`, `bfne_08`, `bfge_02` |
| Aliases | `wing_man` |
| Groups | `FG_EROS`, `FG_LOCUST`, `CONT_005`, `FG_TRIUMPH`, `FG_MOSQUITO`, `FG_WEEVIL`, `FG_CERES`, `FG_CLAW` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 1, param 164
- Show/update HUD contact: contact/list 0, subtype 1, param 240
- Set runtime trigger variable: variable group 20, variable 5, subtype 0, value 0
- Group/spawn-list action: spawn list/group 165, subtype 0
- Group/spawn-list action: spawn list/group 164, subtype 0
- Group/spawn-list action: spawn list/group 240, subtype 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Group/spawn-list action: spawn list/group 112, subtype 2
- Group/spawn-list action: spawn list/group 30, subtype 2

### Event 2

**Trigger**

- Group/spawn-list event: subject 112, op 2, value 6684673 (Waypoint 4 (tag 102), point 1)

**Action**

- Set runtime trigger variable: variable group 20, variable 20, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 10
- Hide/remove HUD contact: contact/list 0, subtype 1, param 164
- Play dialog: TRISH.SCR, line/variant 8
- Hide/remove HUD contact: contact/list 0, subtype 1, param 240
- Object spawn/action: Satellite (object 5, id 11), subtype 14

### Event 3

**Trigger**

- Object event: subject Satellite (object 5, id 11), op 2, value 0
- Variable comparison: subject variable group 20, variable 20, op 3, value 70
- Variable comparison: subject variable group 21, variable 32, op 1, value 0

**Action**

- Set/add variable: variable group 14, variable 406, subtype 0, value 1
- Set/add variable: variable group 14, variable 407, subtype 0, value 3
- Set/add variable: variable group 21, variable 34, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 10
- Play dialog: TRISH.SCR, line/variant 12
- Set/add variable: variable group 21, variable 30, subtype 0, value 1

### Event 4

**Trigger**

- Group/spawn-list event: subject 112, op 0, value 0
- Variable comparison: subject variable group 21, variable 30, op 1, value 0
- Variable comparison: subject variable group 20, variable 20, op 2, value 44

**Action**

- Set/add variable: variable group 14, variable 406, subtype 0, value 1
- Set/add variable: variable group 14, variable 407, subtype 0, value 2
- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Play dialog: TRISH.SCR, line/variant 15
- Set/add variable: variable group 21, variable 34, subtype 0, value 1

### Event 5

**Trigger**

- Group/spawn-list event: subject 112, op 4, value 0 (join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 900 (extra 1, 11; join 2; flags 2)
- Group/spawn-list event: subject 30, op 4, value 0 (flags 2)

**Action**

- Group/spawn-list action: spawn list/group 30, subtype 2

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 20, op 2, value 70
- Variable comparison: subject variable group 21, variable 30, op 1, value 0
- Variable comparison: subject variable group 21, variable 32, op 1, value 0

**Action**

- Group/spawn-list action: spawn list/group 30, subtype 2
- Hide/remove HUD contact: contact/list 0, subtype 9, param 10
- Show/update HUD contact: contact/list 0, subtype 1, param 112
- Play dialog: TRISH.SCR, line/variant 10
- Group/spawn-list action: spawn list/group 112, subtype 2
- Set/add variable: variable group 21, variable 27, subtype 0, value 1
- Object spawn/action: Satellite (object 5, id 11), subtype 15

### Event 7

**Trigger**

- Variable comparison: subject variable group 21, variable 27, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 112, subtype 3, param 2

### Event 8

**Trigger**

- Object event: subject Bora_Warhammer (object 6, id 12), op 7, value 0 (join 2)
- Object event: subject Bora_Warhammer (object 7, id 13), op 7, value 0
- Variable comparison: subject variable group 21, variable 27, op 1, value 1
- Variable comparison: subject variable group 21, variable 30, op 1, value 0

**Action**

- Set/add variable: variable group 14, variable 406, subtype 0, value 1
- Set/add variable: variable group 14, variable 407, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 21
- Mark/flash contact: contact/list 0, subtype 1, param 112
- Play dialog: TRISH.SCR, line/variant 11

### Event 9

**Trigger**

- Object event: subject Bora_Warhammer (object 6, id 12), op 7, value 0 (join 2)
- Object event: subject Bora_Warhammer (object 7, id 13), op 7, value 0

**Action**

- Group/spawn-list action: spawn list/group 164, subtype 3, param 2
- Group/spawn-list action: spawn list/group 240, subtype 3, param 2
- Group/spawn-list action: spawn list/group 261, subtype 3, param 2
- Group/spawn-list action: spawn list/group 30, subtype 3, param 2

### Event 10

**Trigger**

- Object arrival: GalSpan_Lt_Freighter (object 20, id 58) reached Waypoint 3 (tag 103), point 0 (raw value 6750208)

**Action**

- Object spawn/action: GalSpan_Lt_Freighter (object 20, id 58), subtype 4

### Event 11

**Trigger**

- Variable comparison: subject variable group 20, variable 5, op 1, value 4

**Action**

- Play dialog: PLAYER.SCR, line/variant 29

### Event 12

**Trigger**

- Variable comparison: subject variable group 20, variable 20, op 1, value 45
- Variable comparison: subject variable group 21, variable 30, op 1, value 0
- Variable comparison: subject variable group 21, variable 32, op 1, value 0

**Action**

- Play dialog: TRISH.SCR, line/variant 9

### Event 13

**Trigger**

- Object event: subject Satellite (object 5, id 11), op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 30, op 1, value 0
- Variable comparison: subject variable group 21, variable 32, op 1, value 1

**Action**

- Play dialog: TRISH.SCR, line/variant 13

### Event 14

**Trigger**

- Group/spawn-list event: subject 112, op 0, value 0
- Variable comparison: subject variable group 20, variable 20, op 3, value 45 (flags 1)
- Variable comparison: subject variable group 21, variable 30, op 1, value 0

**Action**

- Play dialog: TRISH.SCR, line/variant 14
- Hide/remove HUD contact: contact/list 0, subtype 9, param 10
- Group/spawn-list action: spawn list/group 30, subtype 2
- Set/add variable: variable group 21, variable 34, subtype 0, value 1

### Event 15

**Trigger**

- Group/spawn-list event: subject 164, op 0, value 0
- Group/spawn-list event: subject 240, op 0, value 0 (join 1)
- Group/spawn-list event: subject 112, op 0, value 0
- Group/spawn-list event: subject 261, op 0, value 0

**Action**

- Play dialog: TRISH.SCR, line/variant 16

### Event 16

**Trigger**

- Group/spawn-list event: subject 30, op 0, value 0
- Group/spawn-list event: subject 164, op 0, value 0
- Group/spawn-list event: subject 240, op 0, value 0
- Group/spawn-list event: subject 112, op 0, value 0
- Group/spawn-list event: subject 261, op 0, value 0

**Action**

- Play dialog: TRISH.SCR, line/variant 17

### Event 17

**Trigger**

- Variable comparison: subject variable group 20, variable 5, op 1, value 35

**Action**

- Group/spawn-list action: spawn list/group 261, subtype 1, param 2

### Event 18

**Trigger**

- Variable comparison: subject variable group 20, variable 5, op 1, value 46

**Action**

- Group/spawn-list action: spawn list/group 29, subtype 1, param 1

### Event 19

**Trigger**

- Object event: subject Satellite (object 5, id 11), op 2, value 0 (flags 1)
- Variable comparison: subject variable group 20, variable 20, op 3, value 70

**Action**

- Group/spawn-list action: spawn list/group 112, subtype 3, param 2
- Group/spawn-list action: spawn list/group 30, subtype 2

### Event 20

**Trigger**

- Variable comparison: subject variable group 21, variable 34, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 20

### Event 21

**Trigger**

- Group/spawn-list event: subject 112, op 0, value 0

**Action**

- Set/add variable: variable group 21, variable 32, subtype 0, value 1

## Waypoints

### Waypoint 0

- Tag: `106`
- Members: `Skav_Pirate_Manta (object 12, id 86, starts at point 0)`, `Skav_Pirate_Manta (object 13, id 87, starts at point 0)`, `Skav_Pirate_Manta (object 14, id 88, starts at point 0)`, `GalSpan_Pegasus (object 15, id 90, starts at point 0)`, `GalSpan_Pegasus (object 16, id 91, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-331.24, 0.00, 639.46) | None |

### Waypoint 1

- Tag: `105`
- Members: `Bora_Cutlass (object 17, id 93, starts at point 0)`, `Bora_Cutlass (object 18, id 94, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1201.59, 10.41, 47.92) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 2

- Tag: `104`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (281.87, 0.00, 443.45) | None |

### Waypoint 3

- Tag: `103`
- Members: `GalSpan_Lt_Freighter (object 20, id 58, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1461.54, 612.00, 1480.34) | None; listened by Event 10 for GalSpan_Lt_Freighter (object 20, id 58) |

### Waypoint 4

- Tag: `102`
- Members: `Bora_Warhammer (object 6, id 12, starts at point 0)`, `Bora_Warhammer (object 7, id 13, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (883.07, -29.82, -905.48) | None |
| 1 | (967.79, -124.02, -702.28) | on arrival activate current object (raw param -1 ignored) |

## Spawn Lists

### Spawn List 0

- ID: `164`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | id 17 | None |
| 1 | 6 | id 18 | None |
| 2 | 0 | none | None |
| 3 | 6 | Satellite (object 5, id 11) | None |

### Spawn List 1

- ID: `261`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | id 18 | None |
| 1 | 6 | id 17 | None |
| 2 | 9 | none | None |
| 3 | 6 | Satellite (object 5, id 11) | None |
| 4 | 0 | none | None |

### Spawn List 2

- ID: `240`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 6 | Satellite (object 5, id 11) | None |

### Spawn List 3

- ID: `30`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 5 | id 29 | None |
| 1 | 5 | spawn list 165 | None |
| 2 | 0 | none | None |
| 3 | 6 | Satellite (object 5, id 11) | None |

### Spawn List 4

- ID: `165`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 1 | spawn list 261 | None |
| 1 | 1 | spawn list 164 | None |
| 2 | 5 | spawn list 112 | None |

### Spawn List 5

- ID: `112`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 5 | spawn list 165 | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `GalSpan_Poseidon` | 3 | Interactive | -462.92,-25.01,585.43 | 0,28,0 | group/role: FG_EROS / 1 |
| 1 | `Skav_Pirate_Manta` | 7 | Interactive | -462.92,34.82,909.86 | 256,491,0 | label: bfne_02; group/role: FG_LOCUST / 0 |
| 2 | `Skav_Pirate_Manta` | 8 | Interactive | -572.51,85.12,1021.55 | 256,484,0 | group/role: FG_LOCUST / 0 |
| 3 | `Skav_Pirate_Manta` | 9 | Interactive | -325.95,85.12,1021.55 | 256,484,0 | group/role: FG_LOCUST / 0 |
| 4 | `Skav_Pirate_Manta` | 10 | Interactive | -449.23,83.18,1149.86 | 256,0,0 | group/role: FG_LOCUST / 0 |
| 5 | `Satellite` | 11 | Interactive | 987.77,-132.40,-609.95 | 7,71,71 | secondary groups: CONT_005, none |
| 6 | `Bora_Warhammer` | 12 | Interactive | -1124.79,868.19,-2492.59 | 28,0,0 | group/role: FG_TRIUMPH / 1; waypoint: Waypoint 4 (tag 102, 2 point(s)), starting point 0, arrival event value 6684672 |
| 7 | `Bora_Warhammer` | 13 | Interactive | -1286.89,835.70,-2561.65 | 61,0,0 | group/role: FG_TRIUMPH / 2; waypoint: Waypoint 4 (tag 102, 2 point(s)), starting point 0, arrival event value 6684672 |
| 8 | `Skav_Pirate_Manta` | 52 | Interactive | -1053.50,-107.09,739.38 | 36,21,398 | group/role: FG_MOSQUITO / 1 |
| 9 | `Skav_Pirate_Manta` | 53 | Interactive | -1127.80,-107.09,729.34 | 50,21,398 | label: bfne_03; group/role: FG_MOSQUITO / 2 |
| 10 | `Skav_Pirate_Manta` | 54 | Interactive | -1064.55,-104.19,668.85 | 50,28,420 | group/role: FG_MOSQUITO / 3 |
| 11 | `GalSpan_Poseidon` | 79 | Interactive | -398.71,0.00,536.58 | 0,0,0 | label: bfgf_02; group/role: FG_EROS / 2 |
| 12 | `Skav_Pirate_Manta` | 86 | Interactive | 803.78,0.00,-124.32 | 0,0,0 | label: bfne_08; group/role: FG_WEEVIL / 1; waypoint: Waypoint 0 (tag 106, 1 point(s)), starting point 0, arrival event value 6946816 |
| 13 | `Skav_Pirate_Manta` | 87 | Interactive | 696.90,0.00,-294.74 | 0,0,0 | group/role: FG_WEEVIL / 2; waypoint: Waypoint 0 (tag 106, 1 point(s)), starting point 0, arrival event value 6946816 |
| 14 | `Skav_Pirate_Manta` | 88 | Interactive | 942.10,0.00,-301.56 | 0,0,0 | group/role: FG_WEEVIL / 3; waypoint: Waypoint 0 (tag 106, 1 point(s)), starting point 0, arrival event value 6946816 |
| 15 | `GalSpan_Pegasus` | 90 | Interactive | -778.37,0.00,-178.78 | 0,0,0 | group/role: FG_CERES / 2; waypoint: Waypoint 0 (tag 106, 1 point(s)), starting point 0, arrival event value 6946816 |
| 16 | `GalSpan_Pegasus` | 91 | Interactive | -567.31,0.00,-218.24 | 0,0,0 | group/role: FG_CERES / 1; waypoint: Waypoint 0 (tag 106, 1 point(s)), starting point 0, arrival event value 6946816 |
| 17 | `Bora_Cutlass` | 93 | Interactive | -1285.95,0.00,-3594.97 | 0,0,0 | group/role: FG_CLAW / 1; waypoint: Waypoint 1 (tag 105, 1 point(s)), starting point 0, arrival event value 6881280 |
| 18 | `Bora_Cutlass` | 94 | Interactive | -1271.39,0.00,-3737.02 | 0,0,0 | label: bfge_02; group/role: FG_CLAW / 2; waypoint: Waypoint 1 (tag 105, 1 point(s)), starting point 0, arrival event value 6881280 |
| 19 | `GalSpan_Heavy_Freighter` | 56 | Interactive | -1146.77,231.98,1593.69 | 0,0,0 | None |
| 20 | `GalSpan_Lt_Freighter` | 58 | Interactive | 553.86,157.37,1251.85 | 107,0,0 | waypoint: Waypoint 3 (tag 103, 1 point(s)), starting point 0, arrival event value 6750208 |
