# Tachyon: The Fringe GALS02C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `GALS02C.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `(none)` |
| Region | 2 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 16 |
| Events | 19 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Carrier`, `1: Bora_Dagger`, `2: GalSpan_Shuttle_Medium` |
| Scripts | `AQUAR.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `bfge_02`, `BFGF_03`, `BFGE_03` |
| Aliases | `stocks04`, `Jerome07`, `Jerome08`, `Jerome09`, `Jerome10`, `Jerome11`, `Jerome12`, `stocks03`, `stocks02`, `stocks01` |
| Groups | `AQUARIUS`, `FG_CENTAURUS`, `FG_VALOR`, `FG_MAUL`, `FG_WORTHY`, `FG_METTLE`, `FG_FIDELITY`, `FG_FAITH`, `GALLANT` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Object event: subject GalSpan_Shuttle_Medium (object 0, id 248), op 15, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 6, param 248
- Set/add variable: variable group 21, variable 25, subtype 0, value 1
- Play dialog: AQUAR.SCR, line/variant 1

### Event 1

**Trigger**

- Object event: subject GalSpan_Shuttle_Medium (object 0, id 248), op 15, value 0

**Action**

- Object spawn/action: GalSpan_Shuttle_Medium (object 0, id 248), subtype 14

### Event 2

**Trigger**

- Object arrival: GalSpan_Shuttle_Medium (object 0, id 248) reached Waypoint 2 (tag 201), point 1 (raw value 13172737)

**Action**

- Object spawn/action: Bora_Carrier (object 15, id 403), subtype 3
- Set runtime trigger variable: variable group 20, variable 19, subtype 0, value 0
- Play dialog: AQUAR.SCR, line/variant 2
- Hide/remove HUD contact: contact/list 0, subtype 6, param 248
- Show/update HUD contact: contact/list 0, subtype 2, param 248

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 5

**Action**

- Group/spawn-list action: spawn list/group 85, subtype 0

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 25

**Action**

- Group/spawn-list action: spawn list/group 46, subtype 1, param 403

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 45

**Action**

- Group/spawn-list action: spawn list/group 189, subtype 1, param 403

### Event 6

**Trigger**

- Object arrival: GalSpan_Shuttle_Medium (object 0, id 248) reached Waypoint 2 (tag 201), point 9 (raw value 13172745)

**Action**

- Object spawn/action: GalSpan_Shuttle_Medium (object 0, id 248), subtype 2, param 1
- Play dialog: AQUAR.SCR, line/variant 3

### Event 7

**Trigger**

- Group/spawn-list event: subject 260, op 2, value 13172745 (Waypoint 2 (tag 201), point 9)

**Action**

- Group/spawn-list action: spawn list/group 260, subtype 3, param 1

### Event 8

**Trigger**

- Object event: subject GalSpan_Shuttle_Medium (object 0, id 248), op 7, value 0

**Action**

- Set/add variable: variable group 14, variable 408, subtype 0, value 1
- Set/add variable: variable group 14, variable 409, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 20

### Event 9

**Trigger**

- Object event: subject GalSpan_Shuttle_Medium (object 0, id 248), op 2, value 0

**Action**

- Set/add variable: variable group 14, variable 408, subtype 0, value 1
- Set/add variable: variable group 14, variable 409, subtype 0, value 1
- Mark/flash contact: contact/list 0, subtype 2, param 248
- Play dialog: PLAYER.SCR, line/variant 34
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 21

### Event 10

**Trigger**

- Object event: subject GalSpan_Shuttle_Medium (object 0, id 248), op 7, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 2, param 248
- Hide/remove HUD contact: contact/list 0, subtype 6, param 248

### Event 11

**Trigger**

- Object event: subject GalSpan_Shuttle_Medium (object 0, id 248), op 0, value 0 (extra 5, 46; join 2; flags 2)
- Object event: subject GalSpan_Shuttle_Medium (object 0, id 248), op 0, value 0 (extra 5, 85; join 2; flags 2)
- Object event: subject GalSpan_Shuttle_Medium (object 0, id 248), op 0, value 0 (extra 5, 189; join 2; flags 2)

**Action**

- Play dialog: AQUAR.SCR, line/variant 4

### Event 12

**Trigger**

- Object arrival: GalSpan_Shuttle_Medium (object 0, id 248) reached Waypoint 2 (tag 201), point 6 (raw value 13172742)
- Group/spawn-list event: subject 46, op 0, value 0
- Group/spawn-list event: subject 85, op 0, value 0
- Group/spawn-list event: subject 189, op 0, value 0

**Action**

- Group/spawn-list action: spawn list/group 262, subtype 1, param 403
- Set runtime trigger variable: variable group 20, variable 2, subtype 0, value 0

### Event 13

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 4

**Action**

- Group/spawn-list action: spawn list/group 265, subtype 1, param 403

### Event 14

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 6

**Action**

- Group/spawn-list action: spawn list/group 263, subtype 1, param 403

### Event 15

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 10

**Action**

- Object spawn/action: Bora_Carrier (object 15, id 403), subtype 4

### Event 16

**Trigger**

- Object event: subject Bora_Carrier (object 15, id 403), op 14, value 78
- Object event: subject Bora_Carrier (object 15, id 403), op 14, value 73

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 1500

### Event 17

**Trigger**

- Group/spawn-list event: subject 262, op 0, value 0
- Group/spawn-list event: subject 265, op 0, value 0
- Group/spawn-list event: subject 46, op 0, value 0
- Group/spawn-list event: subject 263, op 0, value 0
- Group/spawn-list event: subject 189, op 0, value 0
- Group/spawn-list event: subject 85, op 0, value 0 (join 1)
- Object event: subject GalSpan_Shuttle_Medium (object 0, id 248), op 2, value 0 (join 1)
- Object arrival: GalSpan_Shuttle_Medium (object 0, id 248) reached Waypoint 2 (tag 201), point 9 (raw value 13172745)

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 2, param 248
- Show/update HUD contact: contact/list 0, subtype 6, param 248

### Event 18

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 3

**Action**

- None

## Waypoints

### Waypoint 0

- Tag: `203`
- Members: `Bora_Dagger (object 9, id 450, starts at point 0)`, `Bora_Dagger (object 10, id 451, starts at point 0)`, `Bora_Dagger (object 11, id 452, starts at point 0)`, `Bora_Dagger (object 12, id 453, starts at point 0)`, `Bora_Dagger (object 13, id 455, starts at point 0)`, `Bora_Dagger (object 14, id 467, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1667.12, 0.00, 4750.35) | None |
| 1 | (-1987.47, 0.00, 3550.99) | None |
| 2 | (-2228.44, 0.00, 2563.96) | None |

### Waypoint 1

- Tag: `202`
- Members: `Bora_Dagger (object 4, id 423, starts at point 0)`, `Bora_Dagger (object 5, id 424, starts at point 0)`, `Bora_Dagger (object 6, id 306, starts at point 0)`, `Bora_Dagger (object 7, id 304, starts at point 0)`, `Bora_Dagger (object 8, id 303, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-579.29, 98.92, 4755.17) | None |
| 1 | (-195.68, 94.26, 3724.43) | None |
| 2 | (111.76, 93.10, 2942.24) | None |

### Waypoint 2

- Tag: `201`
- Members: `GalSpan_Shuttle_Medium (object 0, id 248, starts at point 0)`, `GalSpan_Shuttle_Medium (object 1, id 416, starts at point 0)`, `GalSpan_Shuttle_Medium (object 2, id 417, starts at point 0)`, `GalSpan_Shuttle_Medium (object 3, id 418, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (302.43, 105.00, 994.28) | None |
| 1 | (355.93, 105.00, 1662.95) | None; listened by Event 2 for GalSpan_Shuttle_Medium (object 0, id 248) |
| 2 | (327.89, 105.00, 2481.11) | None |
| 3 | (-29.04, 105.00, 3604.89) | None |
| 4 | (-626.59, 105.00, 3784.46) | None |
| 5 | (-1347.00, 105.00, 3763.03) | None |
| 6 | (-1781.92, 105.00, 3184.01) | None; listened by Event 12 for GalSpan_Shuttle_Medium (object 0, id 248) |
| 7 | (-1912.95, 159.00, 2594.21) | None |
| 8 | (-1839.36, 159.00, 1576.92) | None |
| 9 | (-1832.35, 0.00, 873.90) | on arrival play dialog/script or enter gate, param 1; listened by Event 6 for GalSpan_Shuttle_Medium (object 0, id 248), Event 17 for GalSpan_Shuttle_Medium (object 0, id 248) |

## Spawn Lists

### Spawn List 0

- ID: `189`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | GalSpan_Shuttle_Medium (object 0, id 248) | None |
| 1 | 0 | none | None |

### Spawn List 1

- ID: `85`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | GalSpan_Shuttle_Medium (object 0, id 248) | None |

### Spawn List 2

- ID: `46`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 6 | GalSpan_Shuttle_Medium (object 0, id 248) | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `GalSpan_Shuttle_Medium` | 248 | Interactive | 253.74,104.00,427.01 | 26,0,0 | alias: stocks04; secondary groups: none, AQUARIUS; waypoint: Waypoint 2 (tag 201, 10 point(s)), starting point 0, arrival event value 13172736 |
| 1 | `GalSpan_Shuttle_Medium` | 416 | Interactive | 394.60,105.95,534.70 | 26,0,0 | group/role: FG_CENTAURUS / 0; alias: stocks03; waypoint: Waypoint 2 (tag 201, 10 point(s)), starting point 0, arrival event value 13172736 |
| 2 | `GalSpan_Shuttle_Medium` | 417 | Interactive | 133.64,103.95,532.39 | 21,0,0 | label: BFGF_03; group/role: FG_CENTAURUS / 0; alias: stocks02; waypoint: Waypoint 2 (tag 201, 10 point(s)), starting point 0, arrival event value 13172736 |
| 3 | `GalSpan_Shuttle_Medium` | 418 | Interactive | 253.74,106.92,647.19 | 26,0,0 | label: BFGF_03; group/role: FG_CENTAURUS / 0; alias: stocks01; waypoint: Waypoint 2 (tag 201, 10 point(s)), starting point 0, arrival event value 13172736 |
| 4 | `Bora_Dagger` | 423 | Interactive | -827.95,131.00,5463.97 | 247,0,0 | group/role: FG_VALOR / 0; waypoint: Waypoint 1 (tag 202, 3 point(s)), starting point 0, arrival event value 13238272 |
| 5 | `Bora_Dagger` | 424 | Interactive | -727.83,131.00,5463.97 | 247,0,0 | label: BFGE_03; group/role: FG_VALOR / 0; waypoint: Waypoint 1 (tag 202, 3 point(s)), starting point 0, arrival event value 13238272 |
| 6 | `Bora_Dagger` | 306 | Interactive | -2714.30,111.00,3055.68 | 182,0,0 | label: BFGE_03; group/role: FG_MAUL / 0; waypoint: Waypoint 1 (tag 202, 3 point(s)), starting point 0, arrival event value 13238272 |
| 7 | `Bora_Dagger` | 304 | Interactive | -2800.30,89.83,3021.34 | 205,0,0 | group/role: FG_MAUL / 0; waypoint: Waypoint 1 (tag 202, 3 point(s)), starting point 0, arrival event value 13238272 |
| 8 | `Bora_Dagger` | 303 | Interactive | -2469.30,89.83,3002.70 | 257,0,0 | group/role: FG_WORTHY / 0; waypoint: Waypoint 1 (tag 202, 3 point(s)), starting point 0, arrival event value 13238272 |
| 9 | `Bora_Dagger` | 450 | Interactive | -2877.14,0.00,3972.49 | 251,0,0 | group/role: FG_METTLE / 0; waypoint: Waypoint 0 (tag 203, 3 point(s)), starting point 0, arrival event value 13303808 |
| 10 | `Bora_Dagger` | 451 | Interactive | -2759.98,0.00,3958.37 | 250,0,0 | label: BFGE_03; group/role: FG_METTLE / 0; waypoint: Waypoint 0 (tag 203, 3 point(s)), starting point 0, arrival event value 13303808 |
| 11 | `Bora_Dagger` | 452 | Interactive | -2460.57,0.00,3986.60 | 251,0,0 | group/role: FG_FIDELITY / 0; waypoint: Waypoint 0 (tag 203, 3 point(s)), starting point 0, arrival event value 13303808 |
| 12 | `Bora_Dagger` | 453 | Interactive | -2330.39,0.00,3972.49 | 250,0,0 | label: BFGE_03; group/role: FG_FIDELITY / 0; waypoint: Waypoint 0 (tag 203, 3 point(s)), starting point 0, arrival event value 13303808 |
| 13 | `Bora_Dagger` | 455 | Interactive | -2395.48,0.00,3661.95 | 250,0,0 | group/role: FG_FAITH / 0; waypoint: Waypoint 0 (tag 203, 3 point(s)), starting point 0, arrival event value 13303808 |
| 14 | `Bora_Dagger` | 467 | Interactive | -2350.78,0.00,3662.40 | 289,0,0 | label: BFGE_03; group/role: FG_FAITH / 0; waypoint: Waypoint 0 (tag 203, 3 point(s)), starting point 0, arrival event value 13303808 |
| 15 | `Bora_Carrier` | 403 | Interactive | -989.94,111.16,6133.02 | 101,0,0 | secondary groups: none, GALLANT |
