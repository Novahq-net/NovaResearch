# Tachyon: The Fringe FRON06A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON06A.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 5 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 7 |
| Entities | 15 |
| Events | 24 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Destroyer`, `1: Valiant`, `2: GalSpan_Cruiser`, `3: Crate_5_Special_Placehold`, `4: GalSpan_Pegasus`, `5: GalSpan_Orion`, `6: Laser_Core` |
| Scripts | `PLAYER.SCR`, `VALNT.SCR`, `CEPHS.scr` |
| Scenes | None |
| Labels | `CEPHS`, `valnt`, `dionysus` |
| Aliases | None |
| Groups | `FG_GEMINI`, `FG_ARES`, `CEPHIUS`, `VALIANT`, `CONT_023`, `DIONYSUS` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 2, param 242
- Play dialog: PLAYER.SCR, line/variant 29
- Show/update HUD contact: contact/list 0, subtype 9, param 22

### Event 1

**Trigger**

- Object event: subject Valiant (object 13, id 242), op 0, value 0 (extra 1, 797; join 2; flags 2)
- Object event: subject Valiant (object 13, id 242), op 0, value 0 (extra 1, 798; flags 2)

**Action**

- Play dialog: VALNT.SCR, line/variant 0

### Event 2

**Trigger**

- Object event: subject 797, op 6, value 0 (join 2)
- Object event: subject 798, op 6, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 32

### Event 3

**Trigger**

- Object event: subject 797, op 6, value 0
- Object event: subject 798, op 6, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 33

### Event 4

**Trigger**

- Object event: subject 797, op 6, value 0
- Object event: subject 798, op 6, value 0
- Object event: subject 146, op 6, value 0
- Object event: subject 162, op 6, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 22

### Event 5

**Trigger**

- Object arrival: Valiant (object 13, id 242) reached Waypoint 2 (tag 101), point 1 (raw value 6619137)

**Action**

- Play dialog: VALNT.SCR, line/variant 2

### Event 6

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 2

**Action**

- Object spawn/action: Valiant (object 13, id 242), subtype 5

### Event 7

**Trigger**

- Object arrival: Valiant (object 13, id 242) reached Waypoint 2 (tag 101), point 2 (raw value 6619138)

**Action**

- Play dialog: VALNT.SCR, line/variant 4

### Event 8

**Trigger**

- Object arrival: Valiant (object 13, id 242) reached Waypoint 2 (tag 101), point 2 (raw value 6619138)
- Sector/startup condition family: subject 1, op 0, value 4

**Action**

- Object spawn/action: GalSpan_Cruiser (object 12, id 768), subtype 3
- Object spawn/action: GalSpan_Destroyer (object 14, id 1006), subtype 3

### Event 9

**Trigger**

- Object event: subject GalSpan_Cruiser (object 12, id 768), op 15, value 0

**Action**

- Group/spawn-list action: spawn list/group 41, subtype 1, param 768
- Play dialog: CEPHS.scr, line/variant 0

### Event 10

**Trigger**

- Object arrival: Valiant (object 13, id 242) reached Waypoint 2 (tag 101), point 3 (raw value 6619139)
- Sector/startup condition family: subject 2, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 2, param 242
- Hide/remove HUD contact: contact/list 0, subtype 9, param 22
- Show/update HUD contact: contact/list 0, subtype 9, param 18
- Object spawn/action: Laser_Core (object 0, id 777), subtype 1, param 242

### Event 11

**Trigger**

- Sector/startup condition family: subject 2, op 0, value 0

**Action**

- Object spawn/action: Crate_5_Special_Placehold (object 8, id 1019), subtype 15
- Object spawn/action: Crate_5_Special_Placehold (object 9, id 1020), subtype 15
- Object spawn/action: Crate_5_Special_Placehold (object 10, id 1031), subtype 15
- Object spawn/action: Crate_5_Special_Placehold (object 11, id 1032), subtype 15

### Event 12

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 800 (extra 1, 777; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 35

### Event 13

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 777; flags 2)

**Action**

- Group/spawn-list action: spawn list/group 16, subtype 1, param 1

### Event 14

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 777; flags 2)

**Action**

- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 16, variable 402, subtype 0, value 1
- Set/add variable: variable group 16, variable 403, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 12, param 37
- Hide/remove HUD contact: contact/list 0, subtype 9, param 18
- Play dialog: PLAYER.SCR, line/variant 36

### Event 15

**Trigger**

- Variable comparison: subject variable group 8, variable 9, op 1, value 1
- Group/spawn-list event: subject 41, op 4, value 0 (join 2; flags 2)
- Variable comparison: subject variable group 8, variable 9, op 1, value 1
- Object event: subject GalSpan_Cruiser (object 12, id 768), op 0, value 0 (join 2; flags 2)
- Variable comparison: subject variable group 8, variable 9, op 1, value 1
- Object event: subject 500, op 0, value 0 (join 2; flags 2)

**Action**

- Play dialog: VALNT.SCR, line/variant 7

### Event 16

**Trigger**

- Object arrival: Valiant (object 13, id 242) reached Waypoint 2 (tag 101), point 4 (raw value 6619140)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 777; flags 2)

**Action**

- Object spawn/action: Valiant (object 13, id 242), subtype 7
- Play scene: unknown index 0, param 0
- Play dialog: CEPHS.scr, line/variant 2

### Event 17

**Trigger**

- Object event: subject Laser_Core (object 0, id 777), op 2, value 0

**Action**

- Object spawn/action: Valiant (object 13, id 242), subtype 7
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 18
- Show/update HUD contact: contact/list 0, subtype 11, param 38
- Set/add variable: variable group 16, variable 403, subtype 0, value 1
- Set/add variable: variable group 16, variable 402, subtype 0, value 0

### Event 18

**Trigger**

- Object event: subject 797, op 14, value 20
- Object event: subject 798, op 14, value 20

**Action**

- Play dialog: PLAYER.SCR, line/variant 32

### Event 19

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 29

**Action**

- Object spawn/action: Crate_5_Special_Placehold (object 8, id 1019), subtype 14
- Object spawn/action: Crate_5_Special_Placehold (object 9, id 1020), subtype 14

### Event 20

**Trigger**

- Object event: subject 797, op 6, value 0

**Action**

- Object spawn/action: Crate_5_Special_Placehold (object 8, id 1019), subtype 15

### Event 21

**Trigger**

- Object event: subject 798, op 6, value 0

**Action**

- Object spawn/action: Crate_5_Special_Placehold (object 9, id 1020), subtype 15
- Object spawn/action: Crate_5_Special_Placehold (object 10, id 1031), subtype 14
- Object spawn/action: Crate_5_Special_Placehold (object 11, id 1032), subtype 14

### Event 22

**Trigger**

- Object event: subject 146, op 6, value 0

**Action**

- Object spawn/action: Crate_5_Special_Placehold (object 10, id 1031), subtype 15

### Event 23

**Trigger**

- Object event: subject 162, op 6, value 0

**Action**

- Object spawn/action: Crate_5_Special_Placehold (object 11, id 1032), subtype 15

## Waypoints

### Waypoint 0

- Tag: `104`
- Members: `GalSpan_Destroyer (object 14, id 1006, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1206.65, -607.52, 2033.90) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 1

- Tag: `103`
- Members: `GalSpan_Cruiser (object 12, id 768, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2530.91, -195.37, 1568.70) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 2

- Tag: `101`
- Members: `Laser_Core (object 0, id 777, starts at point 1)`, `GalSpan_Orion (object 1, id 773, starts at point 2)`, `GalSpan_Orion (object 2, id 774, starts at point 2)`, `GalSpan_Orion (object 3, id 775, starts at point 2)`, `GalSpan_Orion (object 4, id 776, starts at point 2)`, `GalSpan_Pegasus (object 5, id 977, starts at point 0)`, `GalSpan_Pegasus (object 6, id 978, starts at point 0)`, `GalSpan_Pegasus (object 7, id 979, starts at point 0)`, `Valiant (object 13, id 242, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (992.50, 510.08, -2632.61) | None |
| 1 | (1203.40, 206.00, -1301.68) | on arrival activate current object (raw param -1 ignored); listened by Event 5 for Valiant (object 13, id 242) |
| 2 | (1256.66, 118.37, -950.49) | None; listened by Event 7 for Valiant (object 13, id 242), Event 8 for Valiant (object 13, id 242) |
| 3 | (1568.14, -1.18, 874.12) | None; listened by Event 10 for Valiant (object 13, id 242) |
| 4 | (1698.75, 0.00, 1632.00) | on arrival activate current object (raw param -1 ignored); listened by Event 16 for Valiant (object 13, id 242) |

## Spawn Lists

### Spawn List 0

- ID: `41`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | Valiant (object 13, id 242) | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Laser_Core` | 777 | Interactive | 1536.49,96.82,873.69 | 0,0,0 | waypoint: Waypoint 2 (tag 101, 5 point(s)), starting point 1, arrival event value 6619137 |
| 1 | `GalSpan_Orion` | 773 | Interactive | 2053.17,0.00,2880.11 | 256,0,0 | group/role: FG_GEMINI / 1; waypoint: Waypoint 2 (tag 101, 5 point(s)), starting point 2, arrival event value 6619138 |
| 2 | `GalSpan_Orion` | 774 | Interactive | 2081.22,0.00,2806.26 | 256,0,0 | group/role: FG_GEMINI / 3; waypoint: Waypoint 2 (tag 101, 5 point(s)), starting point 2, arrival event value 6619138 |
| 3 | `GalSpan_Orion` | 775 | Interactive | 2127.30,0.00,2880.11 | 256,0,0 | group/role: FG_GEMINI / 2; waypoint: Waypoint 2 (tag 101, 5 point(s)), starting point 2, arrival event value 6619138 |
| 4 | `GalSpan_Orion` | 776 | Interactive | 2135.31,0.00,2817.12 | 256,0,0 | group/role: FG_GEMINI / 4; waypoint: Waypoint 2 (tag 101, 5 point(s)), starting point 2, arrival event value 6619138 |
| 5 | `GalSpan_Pegasus` | 977 | Interactive | 162.43,0.00,-3613.68 | 0,0,0 | group/role: FG_ARES / 1; waypoint: Waypoint 2 (tag 101, 5 point(s)), starting point 0, arrival event value 6619136 |
| 6 | `GalSpan_Pegasus` | 978 | Interactive | 210.42,0.00,-3613.68 | 0,0,0 | group/role: FG_ARES / 2; waypoint: Waypoint 2 (tag 101, 5 point(s)), starting point 0, arrival event value 6619136 |
| 7 | `GalSpan_Pegasus` | 979 | Interactive | 258.41,0.00,-3613.68 | 0,0,0 | group/role: FG_ARES / 3; waypoint: Waypoint 2 (tag 101, 5 point(s)), starting point 0, arrival event value 6619136 |
| 8 | `Crate_5_Special_Placehold` | 1019 | Interactive | 723.38,658.42,-809.25 | 0,0,0 | None |
| 9 | `Crate_5_Special_Placehold` | 1020 | Interactive | 544.90,-865.65,-527.72 | 0,0,0 | None |
| 10 | `Crate_5_Special_Placehold` | 1031 | Interactive | 687.93,658.91,846.41 | 0,0,0 | None |
| 11 | `Crate_5_Special_Placehold` | 1032 | Interactive | 687.93,-872.82,846.14 | 0,0,0 | None |
| 12 | `GalSpan_Cruiser` | 768 | Interactive | 2966.16,211.64,3208.94 | 270,498,0 | label: CEPHS; secondary groups: none, CEPHIUS; waypoint: Waypoint 1 (tag 103, 1 point(s)), starting point 0, arrival event value 6750208 |
| 13 | `Valiant` | 242 | Interactive | 929.16,595.60,-2947.78 | 16,491,0 | label: valnt; secondary groups: CONT_023, VALIANT; waypoint: Waypoint 2 (tag 101, 5 point(s)), starting point 0, arrival event value 6619136 |
| 14 | `GalSpan_Destroyer` | 1006 | Interactive | 1460.18,-598.68,3257.41 | 270,0,0 | label: dionysus; secondary groups: none, DIONYSUS; waypoint: Waypoint 0 (tag 104, 1 point(s)), starting point 0, arrival event value 6815744 |
