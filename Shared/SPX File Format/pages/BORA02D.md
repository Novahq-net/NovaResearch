# Tachyon: The Fringe BORA02D.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `BORA02D.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `(none)` |
| Region | 3 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 9 |
| Entities | 22 |
| Events | 26 |
| Waypoints | 5 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Destroyer`, `1: Bora_Cruiser`, `2: GalSpan_Frigate`, `3: GalSpan_Shuttle_Medium`, `4: Bora_Mace`, `5: GalSpan_Phoenix`, `6: GalSpan_Pegasus`, `7: GalSpan_Poseidon`, `8: Bora_Shuttle_Medium` |
| Scripts | `ARCHA.SCR`, `PLAYER.SCR`, `ANNAH.SCR` |
| Scenes | None |
| Labels | `chaas`, `bfbf_01`, `BFBE_05`, `BFGE_05`, `BFBF_05` |
| Aliases | `frank01`, `frank02`, `frank03`, `frank04`, `stocks06` |
| Groups | `FG_ROVER`, `FG_ASTERION`, `FG_AEGIPAN`, `FG_MENSA`, `FG_ANTLIA`, `FG_AGENOR`, `FG_IXION`, `FG_JACKHAMMER`, `FG_CENTAURUS`, `CORONIS`, `CANDOR`, `CONT_025`, `CHIMAERA` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 1, param 148
- Object spawn/action: id 18, subtype 6
- Object spawn/action: id 18, subtype 8, param 2
- Show/update HUD contact: contact/list 0, subtype 1, param 234
- Play dialog: ARCHA.SCR, line/variant 0
- Group/spawn-list action: spawn list/group 148, subtype 0
- Group/spawn-list action: spawn list/group 234, subtype 0

### Event 1

**Trigger**

- Group/spawn-list event: subject 148, op 0, value 0
- Group/spawn-list event: subject 234, op 0, value 0

**Action**

- Object spawn/action: Bora_Shuttle_Medium (object 0, id 166), subtype 1, param 6
- Play dialog: PLAYER.SCR, line/variant 55
- Set runtime trigger variable: variable group 20, variable 22, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 2, param 166

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 22, op 1, value 4

**Action**

- Group/spawn-list action: spawn list/group 103, subtype 1, param 6
- Object spawn/action: Bora_Shuttle_Medium (object 0, id 166), subtype 14

### Event 3

**Trigger**

- Object arrival: Bora_Shuttle_Medium (object 0, id 166) reached Waypoint 3 (tag 251), point 1 (raw value 16449537)

**Action**

- Object spawn/action: GalSpan_Frigate (object 19, id 215), subtype 3
- Set runtime trigger variable: variable group 20, variable 19, subtype 0, value 0
- Play dialog: PLAYER.SCR, line/variant 57

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 6

**Action**

- Group/spawn-list action: spawn list/group 177, subtype 1, param 215
- Show/update HUD contact: contact/list 0, subtype 1, param 177

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 14

**Action**

- Group/spawn-list action: spawn list/group 149, subtype 1, param 215

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 24, op 1, value 15
- Variable comparison: subject variable group 21, variable 27, op 1, value 0

**Action**

- Set/add variable: variable group 21, variable 34, subtype 0, value 2

### Event 7

**Trigger**

- Object arrival: Bora_Shuttle_Medium (object 0, id 166) reached Waypoint 3 (tag 251), point 6 (raw value 16449542)

**Action**

- Set runtime trigger variable: variable group 20, variable 24, subtype 0, value 0

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 24, op 1, value 20
- Variable comparison: subject variable group 21, variable 34, op 1, value 2

**Action**

- Play dialog: ANNAH.SCR, line/variant 18
- Set/add variable: variable group 21, variable 25, subtype 0, value 1
- Object spawn/action: Bora_Shuttle_Medium (object 0, id 166), subtype 15

### Event 9

**Trigger**

- Variable comparison: subject variable group 20, variable 24, op 1, value 27

**Action**

- Object spawn/action: GalSpan_Destroyer (object 21, id 332), subtype 3

### Event 10

**Trigger**

- Variable comparison: subject variable group 20, variable 24, op 1, value 35
- Variable comparison: subject variable group 21, variable 34, op 1, value 2

**Action**

- Group/spawn-list action: spawn list/group 260, subtype 1, param 332
- Group/spawn-list action: spawn list/group 95, subtype 1, param 332
- Show/update HUD contact: contact/list 0, subtype 1, param 260
- Play dialog: PLAYER.SCR, line/variant 110
- Object spawn/action: GalSpan_Shuttle_Medium (object 15, id 315), subtype 14
- Object spawn/action: GalSpan_Shuttle_Medium (object 16, id 316), subtype 14
- Object spawn/action: id 317, subtype 14
- Hide/remove HUD contact: contact/list 0, subtype 2, param 166

### Event 11

**Trigger**

- Group/spawn-list event: subject 260, op 2, value 16711684 (Waypoint 1 (tag 255), point 4)

**Action**

- Object spawn/action: GalSpan_Shuttle_Medium (object 15, id 315), subtype 9, param 18
- Object spawn/action: GalSpan_Shuttle_Medium (object 16, id 316), subtype 9, param 18
- Object spawn/action: id 317, subtype 9, param 18

### Event 12

**Trigger**

- Variable comparison: subject variable group 20, variable 24, op 1, value 60

**Action**

- Object spawn/action: GalSpan_Destroyer (object 21, id 332), subtype 4

### Event 13

**Trigger**

- Group/spawn-list event: subject 95, op 0, value 0

**Action**

- Group/spawn-list action: spawn list/group 96, subtype 1, param 215

### Event 14

**Trigger**

- Group/spawn-list event: subject 260, op 0, value 0
- Variable comparison: subject variable group 21, variable 18, op 3, value 2

**Action**

- Play dialog: PLAYER.SCR, line/variant 112
- Object spawn/action: Bora_Cruiser (object 20, id 266), subtype 3
- Set runtime trigger variable: variable group 20, variable 13, subtype 0, value 0

### Event 15

**Trigger**

- Object event: subject GalSpan_Frigate (object 19, id 215), op 4, value 60

**Action**

- Group/spawn-list action: spawn list/group 95, subtype 1, param 215
- Group/spawn-list action: spawn list/group 96, subtype 1, param 215
- Group/spawn-list action: spawn list/group 157, subtype 1, param 215

### Event 16

**Trigger**

- Variable comparison: subject variable group 21, variable 34, op 1, value 2
- Group/spawn-list event: subject 260, op 0, value 0
- Variable comparison: subject variable group 20, variable 13, op 1, value 10
- Variable comparison: subject variable group 21, variable 18, op 3, value 2

**Action**

- Set/add variable: variable group 15, variable 412, subtype 0, value 1
- Set/add variable: variable group 15, variable 413, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Object spawn/action: id 18, subtype 5
- Object spawn/action: id 18, subtype 8, param 1
- Play dialog: ANNAH.SCR, line/variant 20
- Show/update HUD contact: contact/list 0, subtype 12, param 19

### Event 17

**Trigger**

- Object event: subject Bora_Shuttle_Medium (object 0, id 166), op 2, value 0
- Variable comparison: subject variable group 21, variable 34, op 3, value 2 (join 2)

**Action**

- Play dialog: ANNAH.SCR, line/variant 22
- Set/add variable: variable group 15, variable 412, subtype 0, value 1
- Set/add variable: variable group 15, variable 413, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Mark/flash contact: contact/list 0, subtype 2, param 166
- Show/update HUD contact: contact/list 0, subtype 11, param 20
- Hide/remove HUD contact: contact/list 0, subtype 1, param 177

### Event 18

**Trigger**

- Object event: subject GalSpan_Shuttle_Medium (object 15, id 315), op 11, value 0 (extra 1, 18; join 2; flags 2)
- Object event: subject GalSpan_Shuttle_Medium (object 16, id 316), op 11, value 0 (extra 1, 18; join 2; flags 2)
- Object event: subject 317, op 11, value 0 (extra 1, 18; join 2; flags 2)

**Action**

- Set runtime trigger variable: variable group 20, variable 14, subtype 0, value 0

### Event 19

**Trigger**

- Variable comparison: subject variable group 20, variable 14, op 1, value 7

**Action**

- Play dialog: PLAYER.SCR, line/variant 111
- Set/add variable: variable group 15, variable 412, subtype 0, value 1
- Set/add variable: variable group 15, variable 413, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 20
- Hide/remove HUD contact: contact/list 0, subtype 1, param 260
- Set/add variable: variable group 21, variable 18, subtype 0, value 2

### Event 20

**Trigger**

- Object event: subject Bora_Shuttle_Medium (object 0, id 166), op 0, value 0 (flags 2)
- Variable comparison: subject variable group 21, variable 34, op 3, value 2

**Action**

- Play dialog: ANNAH.SCR, line/variant 21

### Event 21

**Trigger**

- Object event: subject Bora_Shuttle_Medium (object 0, id 166), op 4, value 10
- Variable comparison: subject variable group 21, variable 34, op 3, value 2

**Action**

- Play dialog: PLAYER.SCR, line/variant 59

### Event 22

**Trigger**

- Object event: subject GalSpan_Frigate (object 19, id 215), op 14, value 39
- Object event: subject GalSpan_Frigate (object 19, id 215), op 14, value 40
- Variable comparison: subject variable group 15, variable 413, op 1, value 2

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 1500

### Event 23

**Trigger**

- Object event: subject Bora_Shuttle_Medium (object 0, id 166), op 0, value 0 (join 2; flags 2)
- Object event: subject 18, op 0, value 0 (join 2; flags 2)

**Action**

- Play dialog: ANNAH.SCR, line/variant 21

### Event 24

**Trigger**

- Group/spawn-list event: subject 103, op 2, value 16449541 (Waypoint 3 (tag 251), point 5)

**Action**

- Group/spawn-list action: spawn list/group 103, subtype 8, param 16842752 (Waypoint 0 (tag 257), point 0)

### Event 25

**Trigger**

- Object event: subject Bora_Shuttle_Medium (object 0, id 166), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 27, subtype 0, value 1

## Waypoints

### Waypoint 0

- Tag: `257`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-594.51, 87.93, 71.14) | None |

### Waypoint 1

- Tag: `255`
- Members: `GalSpan_Shuttle_Medium (object 15, id 315, starts at point 0)`, `GalSpan_Shuttle_Medium (object 16, id 316, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1990.82, -144.00, 1360.24) | None |
| 1 | (-1739.58, -146.00, 1211.72) | None |
| 2 | (-1448.30, -166.00, 1027.40) | None |
| 3 | (-1220.15, -212.00, 868.57) | None |
| 4 | (-904.27, -257.00, 676.64) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 2

- Tag: `254`
- Members: `GalSpan_Poseidon (object 1, id 169, starts at point 0)`, `GalSpan_Poseidon (object 4, id 223, starts at point 0)`, `GalSpan_Phoenix (object 11, id 167, starts at point 0)`, `GalSpan_Phoenix (object 12, id 168, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (411.65, 0.00, 2431.92) | None |
| 1 | (72.19, 0.00, 1883.82) | None |
| 2 | (-107.04, 0.00, 1548.84) | None |
| 3 | (-269.65, 0.00, 1125.58) | None |

### Waypoint 3

- Tag: `251`
- Members: `Bora_Shuttle_Medium (object 0, id 166, starts at point 0)`, `Bora_Mace (object 13, id 313, starts at point 0)`, `Bora_Mace (object 14, id 314, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2176.36, -228.00, 362.72) | None |
| 1 | (1755.35, -238.00, 116.52) | None; listened by Event 3 for Bora_Shuttle_Medium (object 0, id 166) |
| 2 | (1411.26, -240.00, 27.04) | None |
| 3 | (980.49, -241.43, 31.53) | None |
| 4 | (604.94, -233.00, 212.20) | None |
| 5 | (129.46, -244.98, 403.27) | None |
| 6 | (-130.93, -248.00, 493.83) | on arrival activate current object (raw param -1 ignored); listened by Event 7 for Bora_Shuttle_Medium (object 0, id 166) |

### Waypoint 4

- Tag: `252`
- Members: `GalSpan_Poseidon (object 2, id 160, starts at point 0)`, `GalSpan_Poseidon (object 3, id 162, starts at point 0)`, `GalSpan_Pegasus (object 5, id 161, starts at point 0)`, `GalSpan_Pegasus (object 6, id 163, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-324.20, 0.00, -1326.23) | None |
| 1 | (70.30, 0.00, -1341.79) | None |
| 2 | (691.93, 0.00, -1053.18) | None |
| 3 | (1565.11, 0.00, -456.24) | None |
| 4 | (2122.67, 0.00, 758.48) | None |
| 5 | (1626.88, 0.00, 1714.67) | None |
| 6 | (558.99, 0.00, 1906.57) | None |
| 7 | (-197.64, 0.00, 1673.56) | None |
| 8 | (-684.60, 15.72, 1132.27) | None |
| 9 | (-1235.13, 0.00, 611.16) | on arrival redirect to Waypoint 4 (tag 252), point 0 |

## Spawn Lists

### Spawn List 0

- ID: `103`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 8 | id 51 | None |
| 1 | 7 | id 51 | None |

### Spawn List 1

- ID: `148`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 2

- ID: `234`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 3

- ID: `149`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | Bora_Shuttle_Medium (object 0, id 166) | None |
| 1 | 0 | none | None |

### Spawn List 4

- ID: `177`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Bora_Shuttle_Medium (object 0, id 166) | None |

### Spawn List 5

- ID: `95`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 7 | id 260 | None |
| 1 | 8 | id 260 | None |

### Spawn List 6

- ID: `96`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Bora_Shuttle_Medium` | 166 | Interactive | 2571.32,0.00,331.66 | 358,0,0 | group/role: FG_ROVER / 0; waypoint: Waypoint 3 (tag 251, 7 point(s)), starting point 0, arrival event value 16449536 |
| 1 | `GalSpan_Poseidon` | 169 | Interactive | -1522.87,0.00,3034.92 | 312,0,0 | group/role: FG_ASTERION / 0; waypoint: Waypoint 2 (tag 254, 4 point(s)), starting point 0, arrival event value 16646144 |
| 2 | `GalSpan_Poseidon` | 160 | Interactive | 1706.73,0.00,-80.09 | 82,0,0 | group/role: FG_AEGIPAN / 0; waypoint: Waypoint 4 (tag 252, 10 point(s)), starting point 0, arrival event value 16515072 |
| 3 | `GalSpan_Poseidon` | 162 | Interactive | 1594.18,0.00,-17.13 | 65,0,0 | label: BFBE_05; group/role: FG_AEGIPAN / 0; waypoint: Waypoint 4 (tag 252, 10 point(s)), starting point 0, arrival event value 16515072 |
| 4 | `GalSpan_Poseidon` | 223 | Interactive | -1453.89,0.00,3009.73 | 316,0,0 | label: BFBE_05; group/role: FG_ASTERION / 0; waypoint: Waypoint 2 (tag 254, 4 point(s)), starting point 0, arrival event value 16646144 |
| 5 | `GalSpan_Pegasus` | 161 | Interactive | -467.42,0.00,-1480.73 | 304,0,0 | label: BFGE_05; group/role: FG_MENSA / 0; waypoint: Waypoint 4 (tag 252, 10 point(s)), starting point 0, arrival event value 16515072 |
| 6 | `GalSpan_Pegasus` | 163 | Interactive | -549.94,0.00,-1473.57 | 287,0,0 | group/role: FG_MENSA / 0; waypoint: Waypoint 4 (tag 252, 10 point(s)), starting point 0, arrival event value 16515072 |
| 7 | `GalSpan_Pegasus` | 284 | Interactive | -1085.28,0.00,3125.43 | 284,0,0 | group/role: FG_ANTLIA / 0 |
| 8 | `GalSpan_Pegasus` | 285 | Interactive | -1008.06,0.00,3125.44 | 282,0,0 | label: BFBE_05; group/role: FG_ANTLIA / 0 |
| 9 | `GalSpan_Pegasus` | 286 | Interactive | -809.50,0.00,3257.00 | 280,0,0 | group/role: FG_AGENOR / 0 |
| 10 | `GalSpan_Pegasus` | 287 | Interactive | -699.20,0.00,3280.92 | 291,0,0 | group/role: FG_AGENOR / 0 |
| 11 | `GalSpan_Phoenix` | 167 | Interactive | -1211.42,0.00,2766.51 | 277,0,0 | group/role: FG_IXION / 0; waypoint: Waypoint 2 (tag 254, 4 point(s)), starting point 0, arrival event value 16646144 |
| 12 | `GalSpan_Phoenix` | 168 | Interactive | -1160.00,0.00,2780.45 | 277,0,0 | label: BFBE_05; group/role: FG_IXION / 0; waypoint: Waypoint 2 (tag 254, 4 point(s)), starting point 0, arrival event value 16646144 |
| 13 | `Bora_Mace` | 313 | Interactive | 2555.18,0.00,428.76 | 0,0,0 | label: BFBF_05; group/role: FG_JACKHAMMER / 0; waypoint: Waypoint 3 (tag 251, 7 point(s)), starting point 0, arrival event value 16449536 |
| 14 | `Bora_Mace` | 314 | Interactive | 2609.60,0.00,428.76 | 0,0,0 | group/role: FG_JACKHAMMER / 0; waypoint: Waypoint 3 (tag 251, 7 point(s)), starting point 0, arrival event value 16449536 |
| 15 | `GalSpan_Shuttle_Medium` | 315 | Interactive | -1897.62,0.00,1698.02 | 244,0,0 | group/role: FG_CENTAURUS / 0; waypoint: Waypoint 1 (tag 255, 5 point(s)), starting point 0, arrival event value 16711680 |
| 16 | `GalSpan_Shuttle_Medium` | 316 | Interactive | -1821.44,0.00,1698.02 | 245,0,0 | label: BFBE_05; group/role: FG_CENTAURUS / 0; waypoint: Waypoint 1 (tag 255, 5 point(s)), starting point 0, arrival event value 16711680 |
| 17 | `GalSpan_Pegasus` | 325 | Interactive | -760.65,0.00,3231.62 | 269,0,0 | group/role: FG_AGENOR / 0 |
| 18 | `GalSpan_Pegasus` | 326 | Interactive | -690.23,0.00,3216.35 | 269,0,0 | label: BFBE_05; group/role: FG_AGENOR / 0 |
| 19 | `GalSpan_Frigate` | 215 | Interactive | 705.50,-76.00,2895.75 | 405,0,0 | label: BFBE_05; alias: stocks06; secondary groups: none, CORONIS |
| 20 | `Bora_Cruiser` | 266 | Interactive | 907.13,314.00,3348.84 | 146,0,0 | secondary groups: CONT_025, CANDOR |
| 21 | `GalSpan_Destroyer` | 332 | Interactive | -2240.82,0.00,1599.07 | 43,0,0 | secondary groups: none, CHIMAERA |
