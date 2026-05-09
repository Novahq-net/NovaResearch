# Tachyon: The Fringe BORA04A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `BORA04A.SPX` |
| Sector | `QUAD_04` |
| Backdrop | `(none)` |
| Region | 3 |
| Sector ID | 3 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 14 |
| Entities | 31 |
| Events | 32 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 8 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Destroyer`, `1: Bora_Cruiser`, `2: Mad_Pirate_Platform`, `3: GalSpan_Cruiser`, `4: GalSpan_Destroyer`, `5: GalSpan_Carrier`, `6: Navigational_Bouy`, `7: Bflat02_BC06_Only`, `8: Bflat01_BC06_Only`, `9: GalSpan_Poseidon`, `10: Bora_Mace`, `11: Bora_Claymore`, `12: GalSpan_Orion`, `13: GalSpan_Phoenix` |
| Scripts | `PLAYER.SCR`, `NDAWN.SCR`, `MERCY.SCR`, `BMACE.scr`, `BCLAY.SCR`, `CERBS.SCR`, `MINOT.SCR`, `HYDRA.SCR` |
| Scenes | None |
| Labels | `BFBE_09`, `BFBF_09`, `dummy` |
| Aliases | None |
| Groups | `FG_LEO`, `FG_VIRGO`, `FG_SWORD`, `FG_MORNING_STAR`, `FG_GEMINI`, `ZEUS`, `CONT_023`, `CHIMAERA`, `MINOTAUR`, `ARION`, `HYDRAS`, `CANDOR`, `JUDGEMENT` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Set runtime trigger variable: variable group 20, variable 1, subtype 0, value 0
- Play dialog: PLAYER.SCR, line/variant 26
- Show/update HUD contact: contact/list 0, subtype 9, param 24
- Object spawn/action: Navigational_Bouy (object 19, id 402), subtype 14

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 15

**Action**

- Play dialog: NDAWN.SCR, line/variant 2

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 27

**Action**

- Play dialog: MERCY.SCR, line/variant 1
- Object spawn/action: GalSpan_Carrier (object 22, id 214), subtype 3
- Object spawn/action: GalSpan_Cruiser (object 25, id 296), subtype 3
- Object spawn/action: GalSpan_Destroyer (object 24, id 107), subtype 3
- Object spawn/action: GalSpan_Destroyer (object 23, id 332), subtype 3
- Object spawn/action: GalSpan_Destroyer (object 26, id 353), subtype 3
- Hide/remove HUD contact: contact/list 0, subtype 9, param 24
- Object spawn/action: Navigational_Bouy (object 19, id 402), subtype 15

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 30

**Action**

- Group/spawn-list action: spawn list/group 59, subtype 1, param 214
- Show/update HUD contact: contact/list 0, subtype 1, param 59
- Broadcast hide/remove contact: contact/list 0, subtype 0, param 8

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 35

**Action**

- Group/spawn-list action: spawn list/group 43, subtype 1, param 296
- Show/update HUD contact: contact/list 0, subtype 1, param 43

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 38

**Action**

- Group/spawn-list action: spawn list/group 41, subtype 1, param 296
- Show/update HUD contact: contact/list 0, subtype 1, param 41

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 47

**Action**

- Play dialog: MERCY.SCR, line/variant 2
- Object spawn/action: GalSpan_Carrier (object 22, id 214), subtype 4
- Object spawn/action: GalSpan_Cruiser (object 25, id 296), subtype 4
- Object spawn/action: GalSpan_Destroyer (object 24, id 107), subtype 4
- Object spawn/action: GalSpan_Destroyer (object 23, id 332), subtype 4

### Event 7

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 65

**Action**

- Object spawn/action: Bora_Mace (object 10, id 157), subtype 1, param 4
- Object spawn/action: Bora_Mace (object 11, id 158), subtype 1, param 4
- Play dialog: BMACE.scr, line/variant 0
- Object spawn/action: Bora_Cruiser (object 29, id 400), subtype 3

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 66

**Action**

- Object spawn/action: Bora_Mace (object 12, id 159), subtype 1, param 4
- Object spawn/action: Bora_Mace (object 13, id 160), subtype 1, param 4

### Event 9

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 67

**Action**

- Object spawn/action: Bora_Claymore (object 6, id 143), subtype 1, param 4
- Object spawn/action: Bora_Claymore (object 7, id 147), subtype 1, param 4

### Event 10

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 75

**Action**

- Object spawn/action: Bora_Claymore (object 8, id 148), subtype 1, param 4
- Object spawn/action: Bora_Claymore (object 9, id 149), subtype 1, param 4
- Gate state/action: param 4, subtype 3, param 0
- Play dialog: BCLAY.SCR, line/variant 0

### Event 11

**Trigger**

- Group/spawn-list event: subject 43, op 0, value 0
- Group/spawn-list event: subject 41, op 0, value 0
- Group/spawn-list event: subject 59, op 0, value 0
- Object event: subject GalSpan_Destroyer (object 26, id 353), op 2, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 29
- Object spawn/action: Bflat01_BC06_Only (object 17, id 355), subtype 0
- Object spawn/action: Bflat02_BC06_Only (object 18, id 356), subtype 0
- Object spawn/action: GalSpan_Destroyer (object 27, id 387), subtype 3

### Event 12

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 29

**Action**

- Play scene: unknown index 0, param 0
- Object spawn/action: Bflat01_BC06_Only (object 17, id 355), subtype 21, param 20
- Set runtime trigger variable: variable group 20, variable 15, subtype 0, value 0
- Set/add variable: variable group 21, variable 34, subtype 0, value 1

### Event 13

**Trigger**

- Variable comparison: subject variable group 20, variable 15, op 1, value 2

**Action**

- Play dialog: CERBS.SCR, line/variant 0

### Event 14

**Trigger**

- Sector/startup condition family: subject 5, op 0, value 0

**Action**

- Play dialog: NDAWN.SCR, line/variant 4
- Set runtime trigger variable: variable group 20, variable 16, subtype 0, value 0

### Event 15

**Trigger**

- Variable comparison: subject variable group 20, variable 16, op 1, value 6

**Action**

- Object spawn/action: Bflat02_BC06_Only (object 18, id 356), subtype 21, param 5

### Event 16

**Trigger**

- Object event: subject Bflat02_BC06_Only (object 18, id 356), op 16, value 0

**Action**

- Play dialog: MINOT.SCR, line/variant 0

### Event 17

**Trigger**

- Sector/startup condition family: subject 6, op 0, value 0

**Action**

- Object spawn/action: GalSpan_Destroyer (object 27, id 387), subtype 4

### Event 18

**Trigger**

- Runtime condition family: subject 0, op 0, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 12, param 19
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 15, variable 404, subtype 0, value 1
- Set/add variable: variable group 15, variable 405, subtype 0, value 2
- Play dialog: MERCY.SCR, line/variant 4
- Gate state/action: param 4, subtype 2, param 0
- Object spawn/action: Bora_Destroyer (object 30, id 401), subtype 3

### Event 19

**Trigger**

- Object event: subject 352, op 0, value 0 (flags 2)

**Action**

- Play dialog: MERCY.SCR, line/variant 3

### Event 20

**Trigger**

- Object event: subject Bora_Claymore (object 6, id 143), op 4, value 10 (join 2)

**Action**

- Object spawn/action: Bora_Claymore (object 6, id 143), subtype 7

### Event 21

**Trigger**

- Object event: subject Bora_Claymore (object 6, id 143), op 2, value 0

**Action**

- Play dialog: BCLAY.SCR, line/variant 1

### Event 22

**Trigger**

- Object event: subject Bora_Mace (object 10, id 157), op 4, value 10 (join 2)

**Action**

- Object spawn/action: Bora_Mace (object 10, id 157), subtype 7

### Event 23

**Trigger**

- Object event: subject Bora_Mace (object 10, id 157), op 2, value 0

**Action**

- Play dialog: BMACE.scr, line/variant 1

### Event 24

**Trigger**

- Object event: subject GalSpan_Orion (object 3, id 135), op 0, value 0 (flags 2)
- Object event: subject GalSpan_Orion (object 3, id 135), op 2, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 75

### Event 25

**Trigger**

- Object event: subject GalSpan_Poseidon (object 14, id 139), op 0, value 0 (flags 2)
- Object event: subject GalSpan_Poseidon (object 14, id 139), op 2, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 81

### Event 26

**Trigger**

- Object event: subject GalSpan_Phoenix (object 0, id 127), op 0, value 0 (flags 2)
- Object event: subject GalSpan_Phoenix (object 0, id 127), op 2, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 104

### Event 27

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 50

**Action**

- Play dialog: PLAYER.SCR, line/variant 85

### Event 28

**Trigger**

- Object event: subject Bora_Mace (object 11, id 158), op 3, value 30

**Action**

- Object spawn/action: Bora_Mace (object 11, id 158), subtype 7

### Event 29

**Trigger**

- Object event: subject Bora_Mace (object 12, id 159), op 3, value 30

**Action**

- Object spawn/action: Bora_Mace (object 12, id 159), subtype 7

### Event 30

**Trigger**

- Object event: subject GalSpan_Destroyer (object 26, id 353), op 4, value 80

**Action**

- Play dialog: HYDRA.SCR, line/variant 0
- Show/update HUD contact: contact/list 0, subtype 0, param 353

### Event 31

**Trigger**

- Object event: subject GalSpan_Destroyer (object 26, id 353), op 2, value 0

**Action**

- Object spawn/action: GalSpan_Destroyer (object 26, id 353), subtype 21, param 14

## Waypoints

### Waypoint 0

- Tag: `101`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-816.34, 0.00, 5120.67) | None |
| 1 | (-2419.31, 0.00, 4614.91) | None |
| 2 | (-2206.44, 0.00, 2524.94) | None |
| 3 | (-433.57, 0.00, 2031.14) | None |
| 4 | (1938.16, 176.99, 2417.90) | None |
| 5 | (1967.60, 176.99, 5082.65) | None |
| 6 | (247.58, 0.00, 5089.77) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 1

- Tag: `102`
- Members: `GalSpan_Phoenix (object 0, id 127, starts at point 0)`, `GalSpan_Phoenix (object 1, id 132, starts at point 0)`, `GalSpan_Phoenix (object 2, id 133, starts at point 0)`, `GalSpan_Poseidon (object 14, id 139, starts at point 0)`, `GalSpan_Poseidon (object 15, id 140, starts at point 0)`, `GalSpan_Poseidon (object 16, id 141, starts at point 0)`, `GalSpan_Phoenix (object 20, id 403, starts at point 0)`, `GalSpan_Poseidon (object 21, id 404, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (224.31, 0.00, 1391.31) | None |
| 1 | (-891.71, 0.00, 2691.69) | None |

### Waypoint 2

- Tag: `103`
- Members: `GalSpan_Orion (object 3, id 135, starts at point 0)`, `GalSpan_Orion (object 4, id 136, starts at point 0)`, `GalSpan_Orion (object 5, id 137, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1077.24, 0.00, 1744.36) | None |
| 1 | (-172.09, 0.00, 3072.58) | None |

## Spawn Lists

### Spawn List 0

- ID: `59`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 5 | spawn list 56 | None |

### Spawn List 1

- ID: `43`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 5 | spawn list 56 | None |

### Spawn List 2

- ID: `41`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 5 | spawn list 56 | None |

### Spawn List 3

- ID: `56`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `GalSpan_Phoenix` | 127 | Interactive | 1919.13,1058.80,-1180.51 | 0,0,0 | group/role: FG_LEO / 0; waypoint: Waypoint 1 (tag 102, 2 point(s)), starting point 0, arrival event value 6684672 |
| 1 | `GalSpan_Phoenix` | 132 | Interactive | 2055.53,1058.80,-1242.32 | 0,0,0 | group/role: FG_LEO / 0; waypoint: Waypoint 1 (tag 102, 2 point(s)), starting point 0, arrival event value 6684672 |
| 2 | `GalSpan_Phoenix` | 133 | Interactive | 2191.94,1058.80,-1273.23 | 0,0,0 | label: BFBE_09; group/role: FG_LEO / 0; waypoint: Waypoint 1 (tag 102, 2 point(s)), starting point 0, arrival event value 6684672 |
| 3 | `GalSpan_Orion` | 135 | Interactive | 2602.23,1058.80,-1082.26 | 0,0,0 | label: BFBE_09; group/role: FG_VIRGO / 0; waypoint: Waypoint 2 (tag 103, 2 point(s)), starting point 0, arrival event value 6750208 |
| 4 | `GalSpan_Orion` | 136 | Interactive | 2738.62,1058.80,-1174.96 | 0,0,0 | group/role: FG_VIRGO / 0; waypoint: Waypoint 2 (tag 103, 2 point(s)), starting point 0, arrival event value 6750208 |
| 5 | `GalSpan_Orion` | 137 | Interactive | 2902.30,1058.80,-1236.75 | 0,0,0 | group/role: FG_VIRGO / 0; waypoint: Waypoint 2 (tag 103, 2 point(s)), starting point 0, arrival event value 6750208 |
| 6 | `Bora_Claymore` | 143 | Interactive | 2327.40,0.00,7779.40 | 240,0,0 | group/role: FG_SWORD / 0 |
| 7 | `Bora_Claymore` | 147 | Interactive | 2845.72,0.00,7748.50 | 240,0,0 | label: BFBF_09; group/role: FG_SWORD / 0 |
| 8 | `Bora_Claymore` | 148 | Interactive | 2483.44,0.00,7757.77 | 240,0,0 | group/role: FG_SWORD / 0 |
| 9 | `Bora_Claymore` | 149 | Interactive | 2674.40,0.00,7757.77 | 240,0,0 | group/role: FG_SWORD / 0 |
| 10 | `Bora_Mace` | 157 | Interactive | 2293.57,0.00,7191.05 | 240,0,0 | group/role: FG_MORNING_STAR / 0 |
| 11 | `Bora_Mace` | 158 | Interactive | 2457.25,0.00,7191.05 | 240,0,0 | group/role: FG_MORNING_STAR / 0 |
| 12 | `Bora_Mace` | 159 | Interactive | 2620.93,0.00,7160.15 | 240,0,0 | label: BFBF_09; group/role: FG_MORNING_STAR / 0 |
| 13 | `Bora_Mace` | 160 | Interactive | 2811.89,0.00,7129.24 | 240,0,0 | group/role: FG_MORNING_STAR / 0 |
| 14 | `GalSpan_Poseidon` | 139 | Interactive | 2273.78,1053.20,-1576.78 | 0,0,0 | group/role: FG_GEMINI / 0; waypoint: Waypoint 1 (tag 102, 2 point(s)), starting point 0, arrival event value 6684672 |
| 15 | `GalSpan_Poseidon` | 140 | Interactive | 2410.16,1053.20,-1638.58 | 0,0,0 | label: BFBE_09; group/role: FG_GEMINI / 0; waypoint: Waypoint 1 (tag 102, 2 point(s)), starting point 0, arrival event value 6684672 |
| 16 | `GalSpan_Poseidon` | 141 | Interactive | 2546.57,1053.20,-1731.27 | 0,0,0 | group/role: FG_GEMINI / 0; waypoint: Waypoint 1 (tag 102, 2 point(s)), starting point 0, arrival event value 6684672 |
| 17 | `Bflat01_BC06_Only` | 355 | Interactive | -1207.37,0.00,-10105.99 | 0,0,0 | None |
| 18 | `Bflat02_BC06_Only` | 356 | Interactive | 145.76,0.00,-10091.85 | 0,0,0 | None |
| 19 | `Navigational_Bouy` | 402 | Interactive | 267.54,0.00,2899.89 | 0,0,0 | None |
| 20 | `GalSpan_Phoenix` | 403 | Interactive | 2107.78,0.00,-1315.95 | 0,0,0 | group/role: FG_LEO / 0; waypoint: Waypoint 1 (tag 102, 2 point(s)), starting point 0, arrival event value 6684672 |
| 21 | `GalSpan_Poseidon` | 404 | Interactive | 2454.42,0.00,-1745.16 | 0,0,0 | group/role: FG_GEMINI / 0; waypoint: Waypoint 1 (tag 102, 2 point(s)), starting point 0, arrival event value 6684672 |
| 22 | `GalSpan_Carrier` | 214 | Interactive | 2175.63,1035.49,1264.56 | 314,0,0 | secondary groups: CONT_023, ZEUS |
| 23 | `GalSpan_Destroyer` | 332 | Interactive | 3010.86,1355.84,641.73 | 309,0,0 | secondary groups: none, CHIMAERA |
| 24 | `GalSpan_Destroyer` | 107 | Interactive | 1615.31,1147.35,2143.17 | 319,0,0 | secondary groups: CONT_023, MINOTAUR |
| 25 | `GalSpan_Cruiser` | 296 | Interactive | 1075.05,1403.89,7.68 | 310,0,0 | secondary groups: none, ARION |
| 26 | `GalSpan_Destroyer` | 353 | Interactive | 3766.91,1057.86,3225.03 | 316,0,0 | secondary groups: none, HYDRAS |
| 27 | `GalSpan_Destroyer` | 387 | Interactive | -60.60,0.00,-12277.72 | 171,0,0 | label: dummy; secondary groups: none, MINOTAUR |
| 28 | `Mad_Pirate_Platform` | 388 | Interactive | -454.34,-175.14,5169.64 | 0,0,0 | None |
| 29 | `Bora_Cruiser` | 400 | Interactive | 4125.37,1658.00,2743.20 | 50,0,0 | secondary groups: none, CANDOR |
| 30 | `Bora_Destroyer` | 401 | Interactive | -1176.20,1502.00,6127.98 | 74,0,0 | secondary groups: CONT_023, JUDGEMENT |
