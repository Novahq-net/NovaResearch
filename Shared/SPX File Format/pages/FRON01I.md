# Tachyon: The Fringe FRON01I.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON01I.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 13 |
| Events | 47 |
| Waypoints | 8 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Luxury_Liner`, `1: GalSpan_Merc_Corvus`, `2: Independent_Merc_Gar`, `3: Skav_Pirate_Manta` |
| Scripts | `FLINT.SCR`, `PLAYER.SCR`, `SKAVP.SCR` |
| Scenes | None |
| Labels | `BFGF_05`, `BFNE_03`, `BFNF_03`, `BFGE_01`, `BFGF_01`, `bfne_05` |
| Aliases | `Python 4`, `Python 3`, `Python 1`, `Python 2`, `Kimodo 1`, `Jerome02`, `Jerome03`, `Jerome04`, `Jerome05`, `Jerome06`, `Jerome01`, `BC05_sistine_chapel`, `bc05_1`, `bc05_2`, `bc05_4`, `bc05_5`, `Mantis1`, `Mantis2`, `Mantis3`, `Mantis4`, `Aphid1`, `Aphid2`, `Aphid3`, `Aphid4`, `Python1`, `Python2`, `Python3`, `Python4`, `Komodo1`, `Komodo2`, `Komodo3`, `Komodo4`, `Kimodo 2`, `Kimodo 3`, `Kimodo 4`, `Cephius`, `Stocks01` |
| Groups | `FG_LOCUST`, `FG_DRAGONFLY`, `FG_APHID`, `FG_RUBY`, `FG_ONYX`, `FG_BLOODSTONE`, `STAR_PRINCESS`, `CONT_032` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 9, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 28, subtype 0, value 0
- Group/spawn-list action: spawn list/group 72, subtype 4, param 9
- Group/spawn-list action: spawn list/group 134, subtype 4, param 9
- Group/spawn-list action: spawn list/group 164, subtype 4, param 9
- Object spawn/action: id 801, subtype 8, param 9
- Object spawn/action: id 802, subtype 8, param 9

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 9, value 0 (join 2)

**Action**

- Object spawn/action: id 397, subtype 14
- Show/update HUD contact: contact/list 0, subtype 9, param 28
- Show/update HUD contact: contact/list 0, subtype 9, param 27
- Play dialog: FLINT.SCR, line/variant 0

### Event 2

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 91

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 28, op 1, value 45
- Sector/startup condition family: subject 0, op 0, value 0

**Action**

- Play dialog: FLINT.SCR, line/variant 1
- Set/add variable: variable group 21, variable 20, subtype 0, value 0
- Set/add variable: variable group 21, variable 21, subtype 0, value 0

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 28, op 1, value 70
- Sector/startup condition family: subject 0, op 0, value 1

**Action**

- Play dialog: FLINT.SCR, line/variant 2
- Hide/remove HUD contact: contact/list 0, subtype 9, param 27
- Hide/remove HUD contact: contact/list 0, subtype 9, param 28
- Show/update HUD contact: contact/list 0, subtype 1, param 72
- Show/update HUD contact: contact/list 0, subtype 1, param 164
- Show/update HUD contact: contact/list 0, subtype 1, param 134
- Set runtime trigger variable: variable group 20, variable 28, subtype 1, value 0
- Set/add variable: variable group 21, variable 22, subtype 0, value 1

### Event 5

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 2

**Action**

- Play dialog: PLAYER.SCR, line/variant 176

### Event 6

**Trigger**

- Object event: subject Luxury_Liner (object 12, id 495), op 3, value 50

**Action**

- Object spawn/action: Luxury_Liner (object 12, id 495), subtype 4

### Event 7

**Trigger**

- Group/spawn-list event: subject 134, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 164, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 72, op 4, value 0 (join 2; flags 2)
- Object event: subject 350, op 0, value 0 (join 2; flags 2)
- Object event: subject 351, op 0, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 134, op 4, value 0 (extra 1, 356; join 2; flags 2)

**Action**

- Group/spawn-list action: spawn list/group 72, subtype 2
- Group/spawn-list action: spawn list/group 164, subtype 2
- Object spawn/action: id 397, subtype 15
- Play dialog: SKAVP.SCR, line/variant 0

### Event 8

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 0, id 338), op 0, value 0 (flags 3)
- Object event: subject Skav_Pirate_Manta (object 0, id 338), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 9

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 1, id 339), op 0, value 0 (flags 3)
- Object event: subject Skav_Pirate_Manta (object 1, id 339), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 10

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 2, id 340), op 0, value 0 (flags 3)
- Object event: subject Skav_Pirate_Manta (object 2, id 340), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 11

**Trigger**

- Object event: subject 337, op 0, value 0 (flags 3)
- Object event: subject 341, op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 12

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 3, id 342), op 0, value 0 (flags 3)
- Object event: subject Skav_Pirate_Manta (object 3, id 342), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 13

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 4, id 343), op 0, value 0 (flags 3)
- Object event: subject Skav_Pirate_Manta (object 4, id 343), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 14

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 5, id 344), op 0, value 0 (flags 3)
- Object event: subject Skav_Pirate_Manta (object 5, id 344), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 15

**Trigger**

- Object event: subject 337, op 0, value 0 (flags 3)
- Object event: subject 345, op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 16

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 6, id 346), op 0, value 0 (flags 3)
- Object event: subject Skav_Pirate_Manta (object 6, id 346), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 17

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 7, id 347), op 0, value 0 (flags 3)
- Object event: subject Skav_Pirate_Manta (object 7, id 347), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 18

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 8, id 348), op 0, value 0 (flags 3)
- Object event: subject Skav_Pirate_Manta (object 8, id 348), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 19

**Trigger**

- Object event: subject 337, op 0, value 0 (flags 3)
- Object event: subject 349, op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 20

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 0, id 338), op 0, value 0 (extra 1, 356; flags 3)
- Object event: subject Skav_Pirate_Manta (object 0, id 338), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 21, subtype 1, value 1

### Event 21

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 1, id 339), op 0, value 0 (extra 1, 356; flags 3)
- Object event: subject Skav_Pirate_Manta (object 1, id 339), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 21, subtype 1, value 1

### Event 22

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 2, id 340), op 0, value 0 (extra 1, 356; flags 3)
- Object event: subject Skav_Pirate_Manta (object 2, id 340), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 21, subtype 1, value 1

### Event 23

**Trigger**

- Object event: subject 337, op 0, value 0 (extra 1, 356; flags 3)
- Object event: subject 341, op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 21, subtype 1, value 1

### Event 24

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 3, id 342), op 0, value 0 (extra 1, 356; flags 3)
- Object event: subject Skav_Pirate_Manta (object 3, id 342), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 21, subtype 1, value 1

### Event 25

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 4, id 343), op 0, value 0 (extra 1, 356; flags 3)
- Object event: subject Skav_Pirate_Manta (object 4, id 343), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 21, subtype 1, value 1

### Event 26

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 5, id 344), op 0, value 0 (extra 1, 356; flags 3)
- Object event: subject Skav_Pirate_Manta (object 5, id 344), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 21, subtype 1, value 1

### Event 27

**Trigger**

- Object event: subject 337, op 0, value 0 (extra 1, 356; flags 3)
- Object event: subject 345, op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 21, subtype 1, value 1

### Event 28

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 6, id 346), op 0, value 0 (extra 1, 356; flags 3)
- Object event: subject Skav_Pirate_Manta (object 6, id 346), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 21, subtype 1, value 1

### Event 29

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 7, id 347), op 0, value 0 (extra 1, 356; flags 3)
- Object event: subject Skav_Pirate_Manta (object 7, id 347), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 21, subtype 1, value 1

### Event 30

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 8, id 348), op 0, value 0 (extra 1, 356; flags 3)
- Object event: subject Skav_Pirate_Manta (object 8, id 348), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 21, subtype 1, value 1

### Event 31

**Trigger**

- Object event: subject 337, op 0, value 0 (extra 1, 356; flags 3)
- Object event: subject 349, op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 21, subtype 1, value 1

### Event 32

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 3
- Variable comparison: subject variable group 21, variable 21, op 3, value 3

**Action**

- Play dialog: FLINT.SCR, line/variant 6
- Set/add variable: variable group 0, variable 2, subtype 1, value 100

### Event 33

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 3
- Variable comparison: subject variable group 21, variable 20, op 3, value 3

**Action**

- Play dialog: PLAYER.SCR, line/variant 96
- Set/add variable: variable group 0, variable 2, subtype 2, value 100

### Event 34

**Trigger**

- Object event: subject GalSpan_Merc_Corvus (object 10, id 356), op 2, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 97

### Event 35

**Trigger**

- Group/spawn-list event: subject 72, op 0, value 0
- Group/spawn-list event: subject 164, op 0, value 0
- Group/spawn-list event: subject 134, op 0, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Set/add variable: variable group 16, variable 413, subtype 0, value 3
- Set/add variable: variable group 16, variable 412, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 37
- Play dialog: PLAYER.SCR, line/variant 243
- Set/add variable: variable group 21, variable 22, subtype 0, value 2

### Event 36

**Trigger**

- Group/spawn-list event: subject 72, op 0, value 0
- Group/spawn-list event: subject 164, op 0, value 0
- Group/spawn-list event: subject 134, op 0, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Set/add variable: variable group 16, variable 413, subtype 0, value 2
- Play dialog: PLAYER.SCR, line/variant 243
- Set/add variable: variable group 16, variable 412, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 37
- Set/add variable: variable group 21, variable 22, subtype 0, value 2

### Event 37

**Trigger**

- Variable comparison: subject variable group 21, variable 22, op 1, value 1
- Area/player/sector/dock/time event: subject 0, op 1, value 150 (extra 1, 722; join 1; flags 3)
- Group/spawn-list event: subject 72, op 0, value 0 (join 1)
- Group/spawn-list event: subject 164, op 0, value 0 (join 1)

**Action**

- Set/add variable: variable group 16, variable 413, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 38
- Set/add variable: variable group 16, variable 412, subtype 0, value 1

### Event 38

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 1 (join 1)
- Sector/startup condition family: subject 0, op 0, value 6

**Action**

- Play dialog: FLINT.SCR, line/variant 4

### Event 39

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1 (join 1)
- Sector/startup condition family: subject 1, op 0, value 96

**Action**

- Play dialog: PLAYER.SCR, line/variant 94

### Event 40

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 2 (join 1)
- Sector/startup condition family: subject 0, op 0, value 6

**Action**

- Play dialog: FLINT.SCR, line/variant 5

### Event 41

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 2 (join 1)
- Sector/startup condition family: subject 1, op 0, value 96

**Action**

- Play dialog: PLAYER.SCR, line/variant 95

### Event 42

**Trigger**

- Variable comparison: subject variable group 0, variable 0, op 1, value 2
- Area/player/sector/dock/time event: subject 0, op 9, value 0

**Action**

- Group/spawn-list action: spawn list/group 127, subtype 4, param 1
- Group/spawn-list action: spawn list/group 129, subtype 4, param 1
- Group/spawn-list action: spawn list/group 146, subtype 4, param 1
- Object spawn/action: Luxury_Liner (object 12, id 495), subtype 8, param 1

### Event 43

**Trigger**

- Variable comparison: subject variable group 0, variable 0, op 1, value 1
- Area/player/sector/dock/time event: subject 0, op 9, value 0

**Action**

- Group/spawn-list action: spawn list/group 127, subtype 4, param 2
- Group/spawn-list action: spawn list/group 129, subtype 4, param 2
- Group/spawn-list action: spawn list/group 146, subtype 4, param 2
- Object spawn/action: Luxury_Liner (object 12, id 495), subtype 8, param 2

### Event 44

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 90

**Action**

- Play dialog: PLAYER.SCR, line/variant 245

### Event 45

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 243

**Action**

- Play dialog: FLINT.SCR, line/variant 7

### Event 46

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 7

**Action**

- Play dialog: PLAYER.SCR, line/variant 239

## Waypoints

### Waypoint 0

- Tag: `505`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-6431.75, -1610.50, -9211.63) | None |
| 1 | (-4196.54, -1234.21, -9279.27) | on arrival redirect to Waypoint 0 (tag 505), point 2 |
| 2 | (-4186.02, -1234.21, -10016.78) | on arrival action 1, param -1 |

### Waypoint 1

- Tag: `520`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-50.21, 0.00, -2255.97) | None |
| 1 | (853.82, 0.00, -1815.20) | None |
| 2 | (814.82, 0.00, -357.60) | None |
| 3 | (-110.89, 0.00, -149.38) | None |
| 4 | (-1085.84, 0.00, -597.86) | None |
| 5 | (-1036.60, 0.00, -2060.77) | None |

### Waypoint 2

- Tag: `523`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1561.20, 0.00, -2016.11) | None |
| 1 | (-1363.02, 0.00, -487.95) | None |
| 2 | (-181.53, -1060.08, 262.74) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 3

- Tag: `522`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2609.25, 0.00, 3567.79) | None |
| 1 | (-2813.73, 0.00, -5816.33) | None |
| 2 | (1876.74, 0.00, -4911.37) | None |
| 3 | (1581.26, 0.00, 3179.88) | on arrival redirect to Waypoint 3 (tag 522), point 0 |

### Waypoint 4

- Tag: `506`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-5673.98, 0.00, -9904.04) | None |
| 1 | (-5093.49, 0.00, -9455.57) | None |
| 2 | (-3718.58, 0.00, -9633.03) | None |
| 3 | (-3667.79, 0.00, -10608.64) | on arrival action 1, param -1 |

### Waypoint 5

- Tag: `503`
- Members: `Skav_Pirate_Manta (object 0, id 338, starts at point -1)`, `Skav_Pirate_Manta (object 1, id 339, starts at point -1)`, `Skav_Pirate_Manta (object 2, id 340, starts at point -1)`, `Skav_Pirate_Manta (object 3, id 342, starts at point -1)`, `Skav_Pirate_Manta (object 4, id 343, starts at point -1)`, `Skav_Pirate_Manta (object 5, id 344, starts at point -1)`, `Skav_Pirate_Manta (object 6, id 346, starts at point -1)`, `Skav_Pirate_Manta (object 7, id 347, starts at point -1)`, `Skav_Pirate_Manta (object 8, id 348, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-5516.39, 0.00, -8921.30) | None |
| 1 | (-4601.44, 0.00, -10012.01) | None |
| 2 | (-3681.13, 0.00, -9315.81) | None |
| 3 | (-5452.19, 0.00, -7749.36) | None |
| 4 | (-6730.98, 0.00, -9025.73) | on arrival redirect to Waypoint 5 (tag 503), point 0 |

### Waypoint 6

- Tag: `502`
- Members: `Independent_Merc_Gar (object 9, id 355, starts at point 0)`, `Independent_Merc_Gar (object 11, id 357, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-79.54, -1164.58, 980.08) | None |
| 1 | (-4484.74, 0.00, -8691.26) | None |

### Waypoint 7

- Tag: `501`
- Members: `GalSpan_Merc_Corvus (object 10, id 356, starts at point 0)`, `Luxury_Liner (object 12, id 495, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1845.92, -975.49, -7508.43) | None |
| 1 | (-3442.38, -975.49, -4871.24) | on arrival activate current object (raw param -1 ignored) |

## Spawn Lists

### Spawn List 0

- ID: `127`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 1 | id 72 | None |

### Spawn List 1

- ID: `129`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 1 | id 134 | None |
| 1 | 1 | id 72 | None |
| 2 | 1 | id 164 | None |

### Spawn List 2

- ID: `146`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 1 | id 164 | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Skav_Pirate_Manta` | 338 | Interactive | -5666.67,-581.32,-9710.29 | 57,0,0 | label: BFNE_03; group/role: FG_LOCUST / 0; waypoint: Waypoint 5 (tag 503, 5 point(s)), starting point -1 |
| 1 | `Skav_Pirate_Manta` | 339 | Interactive | -5666.67,-581.32,-9755.83 | 57,0,0 | group/role: FG_LOCUST / 0; waypoint: Waypoint 5 (tag 503, 5 point(s)), starting point -1 |
| 2 | `Skav_Pirate_Manta` | 340 | Interactive | -5666.67,-581.32,-9798.23 | 57,0,0 | group/role: FG_LOCUST / 0; waypoint: Waypoint 5 (tag 503, 5 point(s)), starting point -1 |
| 3 | `Skav_Pirate_Manta` | 342 | Interactive | -5174.68,0.00,-8687.66 | 0,0,0 | label: BFNE_03; group/role: FG_DRAGONFLY / 0; waypoint: Waypoint 5 (tag 503, 5 point(s)), starting point -1 |
| 4 | `Skav_Pirate_Manta` | 343 | Interactive | -5117.52,0.00,-8706.26 | 0,0,0 | group/role: FG_DRAGONFLY / 0; waypoint: Waypoint 5 (tag 503, 5 point(s)), starting point -1 |
| 5 | `Skav_Pirate_Manta` | 344 | Interactive | -5071.78,0.00,-8737.25 | 0,0,0 | group/role: FG_DRAGONFLY / 0; waypoint: Waypoint 5 (tag 503, 5 point(s)), starting point -1 |
| 6 | `Skav_Pirate_Manta` | 346 | Interactive | -5666.67,-581.32,-9523.93 | 57,0,0 | label: BFNE_03; group/role: FG_APHID / 0; waypoint: Waypoint 5 (tag 503, 5 point(s)), starting point -1 |
| 7 | `Skav_Pirate_Manta` | 347 | Interactive | -5666.67,-581.32,-9573.52 | 57,0,0 | group/role: FG_APHID / 0; waypoint: Waypoint 5 (tag 503, 5 point(s)), starting point -1 |
| 8 | `Skav_Pirate_Manta` | 348 | Interactive | -5666.67,-581.32,-9623.11 | 57,0,0 | group/role: FG_APHID / 0; waypoint: Waypoint 5 (tag 503, 5 point(s)), starting point -1 |
| 9 | `Independent_Merc_Gar` | 355 | Interactive | -80.35,-1189.97,-1330.17 | 0,0,0 | label: BFNF_03; group/role: FG_RUBY / 0; waypoint: Waypoint 6 (tag 502, 2 point(s)), starting point 0, arrival event value 32899072 |
| 10 | `GalSpan_Merc_Corvus` | 356 | Interactive | -916.17,-1189.97,-393.41 | 384,0,0 | group/role: FG_ONYX / 0; waypoint: Waypoint 7 (tag 501, 2 point(s)), starting point 0, arrival event value 32833536 |
| 11 | `Independent_Merc_Gar` | 357 | Interactive | -69.52,-1189.97,-1349.81 | 0,0,0 | label: BFNF_03; group/role: FG_BLOODSTONE / 0; waypoint: Waypoint 6 (tag 502, 2 point(s)), starting point 0, arrival event value 32899072 |
| 12 | `Luxury_Liner` | 495 | Interactive | -1956.72,-975.49,-8086.40 | 85,0,0 | secondary groups: CONT_032, STAR_PRINCESS; waypoint: Waypoint 7 (tag 501, 2 point(s)), starting point -1 |
