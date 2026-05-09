# Tachyon: The Fringe MYST07B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST07B.SPX` |
| Sector | `QUAD_07` |
| Backdrop | `(none)` |
| Region | 5 |
| Sector ID | 6 |
| SectorHazardFlags | Twilight fog / fog-radar impairment (0x00000002) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 30 |
| Events | 36 |
| Waypoints | 4 |
| Child Sectors | 0 |
| Scripts | 4 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Destroyer`, `1: Navigational_Bouy`, `2: GalSpan_Archangel`, `3: Demon_Pirate_Fighter` |
| Scripts | `PLAYER.SCR`, `CERBS.SCR`, `PISCE.SCR`, `B41DP.SCR` |
| Scenes | None |
| Labels | `pisce`, `minotaur`, `cerbs`, `hydras`, `MPP1` |
| Aliases | `PISCES1`, `PISCES2`, `PISCES3`, `PISCES4`, `stocks02` |
| Groups | `FG_SPOOK`, `FG_PISCES`, `FG_SPECTER`, `FG_GHOST`, `FG_WISP`, `FG_BANSHEE`, `CONT_004`, `FG_LURKER`, `FG_PHANTOM`, `MINOTAUR`, `CEREBUS`, `HYDRAS` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 11, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 25
- Show/update HUD contact: contact/list 0, subtype 9, param 26
- Show/update HUD contact: contact/list 0, subtype 9, param 27

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 11, op 1, value 5

**Action**

- Play dialog: PLAYER.SCR, line/variant 48
- Set runtime trigger variable: variable group 20, variable 11, subtype 1, value 0

### Event 2

**Trigger**

- Group/spawn-list event: subject 50, op 3, value 0
- Sector/startup condition family: subject 0, op 0, value 48

**Action**

- Play dialog: CERBS.SCR, line/variant 0

### Event 3

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 11, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 15
- Hide/remove HUD contact: contact/list 0, subtype 9, param 25
- Hide/remove HUD contact: contact/list 0, subtype 9, param 26
- Hide/remove HUD contact: contact/list 0, subtype 9, param 27

### Event 4

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 0

**Action**

- Object spawn/action: Navigational_Bouy (object 13, id 1602), subtype 14
- Object spawn/action: Navigational_Bouy (object 14, id 639), subtype 14
- Object spawn/action: Navigational_Bouy (object 12, id 640), subtype 14

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 11, op 1, value 8

**Action**

- Play dialog: PISCE.SCR, line/variant 1
- Group/spawn-list action: spawn list/group 80, subtype 0

### Event 6

**Trigger**

- Variable comparison: subject variable group 21, variable 23, op 1, value 0
- Area/player/sector/dock/time event: subject 0, op 1, value 100 (extra 1, 1602; flags 2)

**Action**

- Set/add variable: variable group 21, variable 23, subtype 1, value 1
- Set/add variable: variable group 21, variable 21, subtype 1, value 1
- Object spawn/action: Navigational_Bouy (object 13, id 1602), subtype 15

### Event 7

**Trigger**

- Variable comparison: subject variable group 21, variable 24, op 1, value 0
- Area/player/sector/dock/time event: subject 0, op 1, value 100 (extra 1, 639; flags 2)

**Action**

- Set/add variable: variable group 21, variable 24, subtype 1, value 1
- Set/add variable: variable group 21, variable 21, subtype 1, value 1
- Object spawn/action: Navigational_Bouy (object 14, id 639), subtype 15

### Event 8

**Trigger**

- Variable comparison: subject variable group 21, variable 25, op 1, value 0
- Area/player/sector/dock/time event: subject 0, op 1, value 100 (extra 1, 640; flags 2)

**Action**

- Set/add variable: variable group 21, variable 25, subtype 1, value 1
- Set/add variable: variable group 21, variable 21, subtype 1, value 1
- Object spawn/action: Navigational_Bouy (object 12, id 640), subtype 15

### Event 9

**Trigger**

- Group/spawn-list event: subject 80, op 0, value 0

**Action**

- Group/spawn-list action: spawn list/group 79, subtype 1, param 1630
- Play dialog: B41DP.SCR, line/variant 7

### Event 10

**Trigger**

- Group/spawn-list event: subject 80, op 0, value 0
- Group/spawn-list event: subject 79, op 1, value 50

**Action**

- Group/spawn-list action: spawn list/group 77, subtype 1, param 1622

### Event 11

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 51

### Event 12

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 2

**Action**

- Play dialog: PLAYER.SCR, line/variant 52

### Event 13

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 3

**Action**

- Play dialog: PLAYER.SCR, line/variant 54
- Hide/remove HUD contact: contact/list 0, subtype 9, param 15

### Event 14

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 54

**Action**

- Object spawn/action: GalSpan_Destroyer (object 27, id 1538), subtype 3
- Object spawn/action: GalSpan_Destroyer (object 28, id 1555), subtype 3
- Object spawn/action: GalSpan_Destroyer (object 29, id 1572), subtype 3
- Group/spawn-list action: spawn list/group 186, subtype 1, param 1630

### Event 15

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 54

**Action**

- Object spawn/action: GalSpan_Destroyer (object 27, id 1538), subtype 14
- Object spawn/action: GalSpan_Destroyer (object 28, id 1555), subtype 14
- Object spawn/action: GalSpan_Destroyer (object 29, id 1572), subtype 14
- Show/update HUD contact: contact/list 0, subtype 2, param 1538
- Show/update HUD contact: contact/list 0, subtype 2, param 1555
- Show/update HUD contact: contact/list 0, subtype 2, param 1572

### Event 16

**Trigger**

- Object arrival: GalSpan_Destroyer (object 29, id 1572) reached Waypoint 3 (tag 151), point 1 (raw value 9895937)

**Action**

- Play dialog: CERBS.SCR, line/variant 3
- Play scene: unknown index 0, param 0

### Event 17

**Trigger**

- Object arrival: GalSpan_Destroyer (object 29, id 1572) reached Waypoint 3 (tag 151), point 2 (raw value 9895938)

**Action**

- Object spawn/action: GalSpan_Destroyer (object 29, id 1572), subtype 21, param 7
- Set runtime trigger variable: variable group 20, variable 8, subtype 0, value 0
- Group/spawn-list action: spawn list/group 185, subtype 1, param 1626

### Event 18

**Trigger**

- Variable comparison: subject variable group 20, variable 8, op 1, value 4

**Action**

- Object spawn/action: id 1630, subtype 21, param 3

### Event 19

**Trigger**

- Runtime condition family: subject 0, op 0, value 0

**Action**

- Play dialog: CERBS.SCR, line/variant 4

### Event 20

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 4

**Action**

- Play dialog: B41DP.SCR, line/variant 8
- Hide/remove HUD contact: contact/list 0, subtype 2, param 1572
- Object spawn/action: GalSpan_Destroyer (object 29, id 1572), subtype 15

### Event 21

**Trigger**

- Object event: subject GalSpan_Destroyer (object 27, id 1538), op 4, value 80

**Action**

- Play dialog: CERBS.SCR, line/variant 6

### Event 22

**Trigger**

- Object event: subject GalSpan_Destroyer (object 28, id 1555), op 4, value 60

**Action**

- Play dialog: CERBS.SCR, line/variant 7

### Event 23

**Trigger**

- Object event: subject GalSpan_Destroyer (object 28, id 1555), op 3, value 90

**Action**

- Play dialog: CERBS.SCR, line/variant 9

### Event 24

**Trigger**

- Object arrival: GalSpan_Destroyer (object 27, id 1538) reached Waypoint 1 (tag 153), point 2 (raw value 10027010)
- Variable comparison: subject variable group 21, variable 20, op 1, value 0

**Action**

- Object spawn/action: GalSpan_Destroyer (object 27, id 1538), subtype 5

### Event 25

**Trigger**

- Object arrival: GalSpan_Destroyer (object 27, id 1538) reached Waypoint 1 (tag 153), point 2 (raw value 10027010)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Object spawn/action: GalSpan_Destroyer (object 27, id 1538), subtype 4
- Object spawn/action: GalSpan_Destroyer (object 27, id 1538), subtype 15
- Hide/remove HUD contact: contact/list 0, subtype 2, param 1538

### Event 26

**Trigger**

- Object arrival: GalSpan_Destroyer (object 27, id 1538) reached Waypoint 1 (tag 153), point 4 (raw value 10027012)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Object spawn/action: GalSpan_Destroyer (object 27, id 1538), subtype 4
- Object spawn/action: GalSpan_Destroyer (object 27, id 1538), subtype 15
- Hide/remove HUD contact: contact/list 0, subtype 2, param 1538

### Event 27

**Trigger**

- Object arrival: GalSpan_Destroyer (object 28, id 1555) reached Waypoint 2 (tag 152), point 2 (raw value 9961474)
- Variable comparison: subject variable group 21, variable 20, op 1, value 0

**Action**

- Object spawn/action: id 1612, subtype 19
- Set/add variable: variable group 21, variable 20, subtype 1, value 1
- Object spawn/action: GalSpan_Destroyer (object 28, id 1555), subtype 5

### Event 28

**Trigger**

- Object arrival: GalSpan_Destroyer (object 28, id 1555) reached Waypoint 2 (tag 152), point 3 (raw value 9961475)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Set/add variable: variable group 17, variable 406, subtype 0, value 1
- Set/add variable: variable group 17, variable 407, subtype 0, value 2
- Play dialog: CERBS.SCR, line/variant 10
- Show/update HUD contact: contact/list 0, subtype 12, param 28
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 38, variable 8, subtype 0, value 1

### Event 29

**Trigger**

- Object event: subject Navigational_Bouy (object 13, id 1602), op 2, value 0 (join 2)
- Object event: subject Navigational_Bouy (object 14, id 639), op 2, value 0 (join 2)
- Object event: subject Navigational_Bouy (object 12, id 640), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 22, subtype 1, value 1

### Event 30

**Trigger**

- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Set/add variable: variable group 17, variable 406, subtype 0, value 0
- Set/add variable: variable group 17, variable 407, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 15
- Play dialog: PISCE.SCR, line/variant 4
- Show/update HUD contact: contact/list 0, subtype 11, param 29
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 31

**Trigger**

- Sector/startup condition family: subject 2, op 0, value 4

**Action**

- Play dialog: PLAYER.SCR, line/variant 57

### Event 32

**Trigger**

- Object event: subject 1612, op 0, value 0 (flags 3)
- Object event: subject 1612, op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 2

### Event 33

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 2

**Action**

- Play dialog: CERBS.SCR, line/variant 11
- Hide/remove HUD contact: contact/list 0, subtype 9, param 15
- Set/add variable: variable group 17, variable 406, subtype 0, value 0
- Set/add variable: variable group 17, variable 407, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 11, param 29
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 34

**Trigger**

- Object event: subject GalSpan_Destroyer (object 28, id 1555), op 8, value 0

**Action**

- Group/spawn-list action: spawn list/group 126, subtype 1, param 1
- Group/spawn-list action: spawn list/group 50, subtype 3, param 1
- Hide/remove HUD contact: contact/list 0, subtype 2, param 1555
- Object spawn/action: GalSpan_Destroyer (object 28, id 1555), subtype 15

### Event 35

**Trigger**

- Group/spawn-list event: subject 126, op 0, value 0

**Action**

- Group/spawn-list action: spawn list/group 153, subtype 1, param 1

## Waypoints

### Waypoint 0

- Tag: `154`
- Members: `GalSpan_Archangel (object 2, id 641, starts at point 0)`, `GalSpan_Archangel (object 3, id 642, starts at point 0)`, `GalSpan_Archangel (object 25, id 1726, starts at point 0)`, `GalSpan_Archangel (object 26, id 1727, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-538.75, 194.50, 1249.90) | None |
| 1 | (-562.29, 179.09, 482.32) | None |

### Waypoint 1

- Tag: `153`
- Members: `GalSpan_Destroyer (object 27, id 1538, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2778.17, 287.72, -658.82) | None |
| 1 | (1872.54, 198.16, -1831.22) | None |
| 2 | (1095.78, 174.84, -3015.82) | on arrival activate current object (raw param -1 ignored); listened by Event 24 for GalSpan_Destroyer (object 27, id 1538), Event 25 for GalSpan_Destroyer (object 27, id 1538) |
| 3 | (-238.45, -768.26, -1956.60) | None |
| 4 | (-1039.04, 0.00, -1295.23) | on arrival activate current object (raw param -1 ignored); listened by Event 26 for GalSpan_Destroyer (object 27, id 1538) |

### Waypoint 2

- Tag: `152`
- Members: `GalSpan_Destroyer (object 28, id 1555, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1254.77, -851.48, 129.62) | None |
| 1 | (151.52, -940.01, -392.07) | None |
| 2 | (-1000.61, -978.34, -838.70) | on arrival activate current object (raw param -1 ignored); listened by Event 27 for GalSpan_Destroyer (object 28, id 1555) |
| 3 | (-1666.82, -997.78, -1770.48) | on arrival action 1, param -1; listened by Event 28 for GalSpan_Destroyer (object 28, id 1555) |

### Waypoint 3

- Tag: `151`
- Members: `GalSpan_Destroyer (object 29, id 1572, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1634.45, -889.63, -498.68) | None |
| 1 | (1494.63, -392.93, -1145.41) | None; listened by Event 16 for GalSpan_Destroyer (object 29, id 1572) |
| 2 | (1420.05, -167.50, -1450.93) | on arrival activate current object (raw param -1 ignored); listened by Event 17 for GalSpan_Destroyer (object 29, id 1572) |

## Spawn Lists

### Spawn List 0

- ID: `80`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | GalSpan_Destroyer (object 27, id 1538) | None |
| 1 | 2 | GalSpan_Destroyer (object 28, id 1555) | None |
| 2 | 2 | GalSpan_Destroyer (object 29, id 1572) | None |

### Spawn List 1

- ID: `77`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | GalSpan_Destroyer (object 27, id 1538) | None |
| 1 | 2 | GalSpan_Destroyer (object 28, id 1555) | None |
| 2 | 2 | GalSpan_Destroyer (object 29, id 1572) | None |
| 3 | 5 | spawn list 50 | None |

### Spawn List 2

- ID: `79`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | GalSpan_Destroyer (object 27, id 1538) | None |
| 1 | 2 | GalSpan_Destroyer (object 28, id 1555) | None |
| 2 | 2 | GalSpan_Destroyer (object 29, id 1572) | None |
| 3 | 5 | spawn list 50 | None |

### Spawn List 3

- ID: `50`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 4

- ID: `185`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | GalSpan_Destroyer (object 28, id 1555) | None |
| 1 | 5 | spawn list 50 | None |

### Spawn List 5

- ID: `186`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | GalSpan_Destroyer (object 28, id 1555) | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Demon_Pirate_Fighter` | 645 | Interactive | -1198.93,0.00,-219.05 | 0,0,0 | group/role: FG_SPOOK / 2 |
| 1 | `Demon_Pirate_Fighter` | 646 | Interactive | -1155.72,0.00,-137.06 | 0,0,0 | group/role: FG_SPOOK / 1 |
| 2 | `GalSpan_Archangel` | 641 | Interactive | -626.33,194.50,1259.08 | 128,0,0 | label: pisce; group/role: FG_PISCES / 1; alias: PISCES1; waypoint: Waypoint 0 (tag 154, 2 point(s)), starting point 0, arrival event value 10092544 |
| 3 | `GalSpan_Archangel` | 642 | Interactive | -571.52,194.50,1303.37 | 128,0,0 | group/role: FG_PISCES / 2; alias: PISCES2; waypoint: Waypoint 0 (tag 154, 2 point(s)), starting point 0, arrival event value 10092544 |
| 4 | `Demon_Pirate_Fighter` | 1635 | Interactive | 620.24,0.00,-2022.51 | 0,0,0 | group/role: FG_SPECTER / 1 |
| 5 | `Demon_Pirate_Fighter` | 1636 | Interactive | 662.62,0.00,-2026.33 | 0,0,0 | group/role: FG_SPECTER / 2 |
| 6 | `Demon_Pirate_Fighter` | 1637 | Interactive | 94.43,0.00,-2023.75 | 0,0,0 | group/role: FG_GHOST / 1 |
| 7 | `Demon_Pirate_Fighter` | 1638 | Interactive | 147.41,0.00,-2031.41 | 0,0,0 | group/role: FG_GHOST / 2 |
| 8 | `Demon_Pirate_Fighter` | 1682 | Interactive | 864.91,0.00,-2019.13 | 0,0,0 | group/role: FG_WISP / 1 |
| 9 | `Demon_Pirate_Fighter` | 1683 | Interactive | 930.17,0.00,-2023.29 | 0,0,0 | group/role: FG_WISP / 2 |
| 10 | `Demon_Pirate_Fighter` | 1684 | Interactive | 1116.33,0.00,-2019.13 | 0,0,0 | group/role: FG_BANSHEE / 1 |
| 11 | `Demon_Pirate_Fighter` | 1685 | Interactive | 1183.51,0.00,-2019.13 | 0,0,0 | group/role: FG_BANSHEE / 2 |
| 12 | `Navigational_Bouy` | 640 | Interactive | -1662.14,-900.00,1674.12 | 0,0,0 | group/role: none / 1; secondary groups: CONT_004, none |
| 13 | `Navigational_Bouy` | 1602 | Interactive | 1544.93,0.00,1506.90 | 0,0,0 | group/role: none / 3; secondary groups: CONT_004, none |
| 14 | `Navigational_Bouy` | 639 | Interactive | -1218.04,600.00,-1416.71 | 0,0,0 | group/role: none / 2; secondary groups: CONT_004, none |
| 15 | `Demon_Pirate_Fighter` | 1696 | Interactive | 97.57,0.00,-2091.28 | 0,0,0 | group/role: FG_GHOST / 3 |
| 16 | `Demon_Pirate_Fighter` | 1697 | Interactive | 145.56,0.00,-2097.52 | 0,0,0 | group/role: FG_GHOST / 4 |
| 17 | `Demon_Pirate_Fighter` | 1698 | Interactive | 871.03,0.00,-2087.12 | 0,0,0 | group/role: FG_WISP / 3 |
| 18 | `Demon_Pirate_Fighter` | 1699 | Interactive | 913.25,0.00,-2087.12 | 0,0,0 | group/role: FG_WISP / 4 |
| 19 | `Demon_Pirate_Fighter` | 1710 | Interactive | -989.10,0.00,1567.46 | 0,0,0 | group/role: FG_LURKER / 1 |
| 20 | `Demon_Pirate_Fighter` | 1711 | Interactive | -952.44,0.00,1566.04 | 0,0,0 | group/role: FG_LURKER / 2 |
| 21 | `Demon_Pirate_Fighter` | 1712 | Interactive | -934.11,0.00,1566.04 | 0,0,0 | group/role: FG_LURKER / 3 |
| 22 | `Demon_Pirate_Fighter` | 1713 | Interactive | -746.85,0.00,1567.46 | 0,0,0 | group/role: FG_PHANTOM / 1 |
| 23 | `Demon_Pirate_Fighter` | 1714 | Interactive | -716.73,0.00,1567.46 | 0,0,0 | group/role: FG_PHANTOM / 2 |
| 24 | `Demon_Pirate_Fighter` | 1715 | Interactive | -694.47,0.00,1567.46 | 0,0,0 | group/role: FG_PHANTOM / 3 |
| 25 | `GalSpan_Archangel` | 1726 | Interactive | -659.40,0.00,1333.88 | 128,0,0 | group/role: FG_PISCES / 3; alias: PISCES3; waypoint: Waypoint 0 (tag 154, 2 point(s)), starting point 0, arrival event value 10092544 |
| 26 | `GalSpan_Archangel` | 1727 | Interactive | -700.18,0.00,1262.39 | 128,0,0 | group/role: FG_PISCES / 4; alias: PISCES4; waypoint: Waypoint 0 (tag 154, 2 point(s)), starting point 0, arrival event value 10092544 |
| 27 | `GalSpan_Destroyer` | 1538 | Interactive | 3028.85,336.24,-217.18 | 297,505,0 | label: minotaur; secondary groups: none, MINOTAUR; waypoint: Waypoint 1 (tag 153, 5 point(s)), starting point 0, arrival event value 10027008 |
| 28 | `GalSpan_Destroyer` | 1555 | Interactive | 1555.33,-877.38,295.77 | 341,0,0 | label: cerbs; secondary groups: none, CEREBUS; waypoint: Waypoint 2 (tag 152, 4 point(s)), starting point 0, arrival event value 9961472 |
| 29 | `GalSpan_Destroyer` | 1572 | Interactive | 1706.38,-1111.11,-202.82 | 276,43,0 | label: hydras; secondary groups: none, HYDRAS; waypoint: Waypoint 3 (tag 151, 3 point(s)), starting point 0, arrival event value 9895936 |
