# Tachyon: The Fringe DISP07A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP07A.SPX` |
| Sector | `QUAD_07` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 6 |
| SectorHazardFlags | Twilight fog / fog-radar impairment (0x00000002) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 13 |
| Entities | 41 |
| Events | 40 |
| Waypoints | 9 |
| Child Sectors | 0 |
| Scripts | 8 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Cruiser`, `1: GalSpan_Singularity_Platform`, `2: Bora_Destroyer`, `3: Bora_Frigate`, `4: GalSpan_Archangel`, `5: Cassitor_Advanced_Drone`, `6: Bora_Claymore`, `7: Bora_Mace`, `8: GalSpan_Pegasus`, `9: TNS_Inquirer`, `10: Bora_Battleaxe`, `11: Bora_Warhammer`, `12: GalSpan_Orion` |
| Scripts | `TNSA.SCR`, `G10GPA.SCR`, `CRGUS.SCR`, `HEPHA.SCR`, `INTEG.SCR`, `SUSAN.SCR`, `PLAYER.SCR`, `GDRON.SCR` |
| Scenes | None |
| Labels | `TNSA`, `gdron`, `CRGUS`, `INTEG`, `HEPHA` |
| Aliases | `tnsa` |
| Groups | `FG_VIRGO`, `FG_TRIDENT`, `FG_MAUL`, `TNS_INQUIRER`, `CONT_005`, `FG_CANCER`, `FG_SWORD`, `FG_CATAPULT`, `FG_MUSCA`, `FG_CYCNUS`, `FG_LYNX`, `COURAGEOUS`, `CONT_023`, `INTEGRITY`, `HEPH_MINING`, `LAZARUS` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Variable comparison: subject variable group 21, variable 24, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 275, subtype 1, param 2

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 2, param 1323

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 4

**Action**

- Play dialog: TNSA.SCR, line/variant 0
- Set runtime trigger variable: variable group 20, variable 0, subtype 1, value 0

### Event 3

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 8

**Action**

- Play dialog: G10GPA.SCR, line/variant 1

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 12

**Action**

- Object spawn/action: Bora_Destroyer (object 38, id 738), subtype 3
- Object spawn/action: Bora_Frigate (object 37, id 708), subtype 3
- Group/spawn-list action: spawn list/group 28, subtype 1, param 2

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 13

**Action**

- Group/spawn-list action: spawn list/group 57, subtype 1, param 2
- Group/spawn-list action: spawn list/group 56, subtype 1, param 2

### Event 7

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 30

**Action**

- Play dialog: CRGUS.SCR, line/variant 0
- Set runtime trigger variable: variable group 20, variable 0, subtype 1, value 0

### Event 8

**Trigger**

- Object arrival: Bora_Frigate (object 37, id 708) reached Waypoint 8 (tag 101), point 1 (raw value 6619137)

**Action**

- Play dialog: HEPHA.SCR, line/variant 3
- Show/update HUD contact: contact/list 0, subtype 0, param 708

### Event 9

**Trigger**

- Object event: subject GalSpan_Singularity_Platform (object 39, id 1323), op 4, value 50

**Action**

- Play dialog: HEPHA.SCR, line/variant 4

### Event 10

**Trigger**

- Object event: subject Bora_Frigate (object 37, id 708), op 4, value 10

**Action**

- Play dialog: CRGUS.SCR, line/variant 2

### Event 11

**Trigger**

- Object arrival: Bora_Frigate (object 37, id 708) reached Waypoint 8 (tag 101), point 2 (raw value 6619138)

**Action**

- Play dialog: CRGUS.SCR, line/variant 1

### Event 12

**Trigger**

- Sector/startup condition family: subject 2, op 0, value 1

**Action**

- Object spawn/action: Bora_Frigate (object 37, id 708), subtype 7

### Event 13

**Trigger**

- Object event: subject Bora_Frigate (object 37, id 708), op 16, value 0

**Action**

- Play dialog: INTEG.SCR, line/variant 1
- Set/add variable: variable group 21, variable 25, subtype 1, value 1
- Hide/remove HUD contact: contact/list 0, subtype 0, param 708

### Event 14

**Trigger**

- Variable comparison: subject variable group 21, variable 25, op 1, value 1
- Object arrival: Bora_Destroyer (object 38, id 738) reached Waypoint 7 (tag 104), point 0 (raw value 6815744)

**Action**

- Play dialog: SUSAN.SCR, line/variant 27
- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0

### Event 15

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 54

**Action**

- Object spawn/action: Bora_Destroyer (object 38, id 738), subtype 4
- Group/spawn-list action: spawn list/group 57, subtype 3, param 2
- Group/spawn-list action: spawn list/group 56, subtype 3, param 2
- Group/spawn-list action: spawn list/group 28, subtype 3, param 2
- Group/spawn-list action: spawn list/group 46, subtype 0
- Set runtime trigger variable: variable group 20, variable 0, subtype 1, value 0

### Event 16

**Trigger**

- Sector/startup condition family: subject 5, op 0, value 27

**Action**

- Play dialog: TNSA.SCR, line/variant 3

### Event 17

**Trigger**

- Object event: subject Bora_Warhammer (object 4, id 504), op 2, value 0 (join 2)
- Object event: subject Bora_Warhammer (object 4, id 504), op 7, value 0

**Action**

- Set/add variable: variable group 21, variable 22, subtype 1, value 1

### Event 18

**Trigger**

- Object event: subject Bora_Warhammer (object 5, id 505), op 2, value 0 (join 2)
- Object event: subject Bora_Warhammer (object 5, id 505), op 7, value 0

**Action**

- Set/add variable: variable group 21, variable 22, subtype 1, value 1

### Event 19

**Trigger**

- Object event: subject Bora_Warhammer (object 6, id 506), op 2, value 0 (join 2)
- Object event: subject Bora_Warhammer (object 6, id 506), op 7, value 0

**Action**

- Set/add variable: variable group 21, variable 22, subtype 1, value 1

### Event 20

**Trigger**

- Object event: subject Bora_Warhammer (object 7, id 507), op 2, value 0 (join 2)
- Object event: subject Bora_Warhammer (object 7, id 507), op 7, value 0

**Action**

- Set/add variable: variable group 21, variable 22, subtype 1, value 1

### Event 21

**Trigger**

- Object event: subject Bora_Mace (object 17, id 509), op 2, value 0 (join 2)
- Object event: subject Bora_Mace (object 17, id 509), op 7, value 0

**Action**

- Set/add variable: variable group 21, variable 22, subtype 1, value 1

### Event 22

**Trigger**

- Object event: subject Bora_Mace (object 18, id 510), op 2, value 0 (join 2)
- Object event: subject Bora_Mace (object 18, id 510), op 7, value 0

**Action**

- Set/add variable: variable group 21, variable 22, subtype 1, value 1

### Event 23

**Trigger**

- Object event: subject Bora_Mace (object 31, id 511), op 2, value 0 (join 2)
- Object event: subject Bora_Mace (object 31, id 511), op 7, value 0

**Action**

- Set/add variable: variable group 21, variable 22, subtype 1, value 1

### Event 24

**Trigger**

- Object event: subject Bora_Mace (object 32, id 512), op 2, value 0 (join 2)
- Object event: subject Bora_Mace (object 32, id 512), op 7, value 0

**Action**

- Set/add variable: variable group 21, variable 22, subtype 1, value 1

### Event 25

**Trigger**

- Object event: subject Bora_Battleaxe (object 8, id 513), op 2, value 0 (join 2)
- Object event: subject Bora_Battleaxe (object 8, id 513), op 7, value 0

**Action**

- Set/add variable: variable group 21, variable 22, subtype 1, value 1

### Event 26

**Trigger**

- Object event: subject Bora_Battleaxe (object 9, id 514), op 2, value 0 (join 2)
- Object event: subject Bora_Battleaxe (object 9, id 514), op 7, value 0

**Action**

- Set/add variable: variable group 21, variable 22, subtype 1, value 1

### Event 27

**Trigger**

- Object event: subject Bora_Battleaxe (object 10, id 515), op 2, value 0 (join 2)
- Object event: subject Bora_Battleaxe (object 10, id 515), op 7, value 0

**Action**

- Set/add variable: variable group 21, variable 22, subtype 1, value 1

### Event 28

**Trigger**

- Object event: subject Bora_Battleaxe (object 11, id 516), op 2, value 0 (join 2)
- Object event: subject Bora_Battleaxe (object 11, id 516), op 7, value 0

**Action**

- Set/add variable: variable group 21, variable 22, subtype 1, value 1

### Event 29

**Trigger**

- Object event: subject Bora_Claymore (object 19, id 517), op 2, value 0 (join 2)
- Object event: subject Bora_Claymore (object 19, id 517), op 7, value 0

**Action**

- Set/add variable: variable group 21, variable 22, subtype 1, value 1

### Event 30

**Trigger**

- Object event: subject Bora_Claymore (object 20, id 518), op 2, value 0 (join 2)
- Object event: subject Bora_Claymore (object 20, id 518), op 7, value 0

**Action**

- Set/add variable: variable group 21, variable 22, subtype 1, value 1

### Event 31

**Trigger**

- Object event: subject Bora_Claymore (object 21, id 519), op 2, value 0 (join 2)
- Object event: subject Bora_Claymore (object 21, id 519), op 7, value 0

**Action**

- Set/add variable: variable group 21, variable 22, subtype 1, value 1

### Event 32

**Trigger**

- Object event: subject Bora_Claymore (object 30, id 520), op 2, value 0 (join 2)
- Object event: subject Bora_Claymore (object 30, id 520), op 7, value 0

**Action**

- Set/add variable: variable group 21, variable 22, subtype 1, value 1

### Event 33

**Trigger**

- Variable comparison: subject variable group 21, variable 22, op 1, value 8

**Action**

- Play dialog: PLAYER.SCR, line/variant 82

### Event 34

**Trigger**

- Variable comparison: subject variable group 21, variable 22, op 1, value 16

**Action**

- Play dialog: PLAYER.SCR, line/variant 83
- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0

### Event 35

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 130

**Action**

- Mission objective/state: param 393216, subtype 0, param 0
- Set runtime trigger variable: variable group 20, variable 0, subtype 1, value 0
- Hide/remove HUD contact: contact/list 0, subtype 2, param 1323
- Set/add variable: variable group 21, variable 21, subtype 1, value 1

### Event 36

**Trigger**

- Sector/startup condition family: subject 6, op 0, value 83

**Action**

- Play dialog: TNSA.SCR, line/variant 4

### Event 37

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 4

**Action**

- Object spawn/action: TNS_Inquirer (object 12, id 1458), subtype 5

### Event 38

**Trigger**

- Object event: subject Cassitor_Advanced_Drone (object 26, id 1540), op 4, value 30 (join 2)
- Object event: subject Cassitor_Advanced_Drone (object 27, id 1541), op 4, value 30 (join 2)
- Object event: subject Cassitor_Advanced_Drone (object 28, id 1543), op 4, value 30 (join 2)
- Object event: subject Cassitor_Advanced_Drone (object 29, id 1544), op 4, value 30

**Action**

- Play dialog: GDRON.SCR, line/variant 1

### Event 39

**Trigger**

- Object event: subject Cassitor_Advanced_Drone (object 26, id 1540), op 3, value 10 (join 2)
- Object event: subject Cassitor_Advanced_Drone (object 27, id 1541), op 3, value 10 (join 2)
- Object event: subject Cassitor_Advanced_Drone (object 28, id 1543), op 3, value 10 (join 2)
- Object event: subject Cassitor_Advanced_Drone (object 29, id 1544), op 3, value 10

**Action**

- Play dialog: GDRON.SCR, line/variant 2

## Waypoints

### Waypoint 0

- Tag: `109`
- Members: `Bora_Warhammer (object 4, id 504, starts at point 0)`, `Bora_Warhammer (object 5, id 505, starts at point 0)`, `Bora_Warhammer (object 6, id 506, starts at point 0)`, `Bora_Warhammer (object 7, id 507, starts at point 0)`, `Bora_Mace (object 17, id 509, starts at point 0)`, `Bora_Mace (object 18, id 510, starts at point 0)`, `Bora_Claymore (object 19, id 517, starts at point 0)`, `Bora_Claymore (object 20, id 518, starts at point 0)`, `Bora_Claymore (object 21, id 519, starts at point 0)`, `GalSpan_Orion (object 22, id 1523, starts at point 0)`, `GalSpan_Orion (object 23, id 1524, starts at point 0)`, `GalSpan_Orion (object 24, id 1525, starts at point 0)`, `GalSpan_Orion (object 25, id 1526, starts at point 0)`, `Bora_Claymore (object 30, id 520, starts at point 0)`, `Bora_Mace (object 31, id 511, starts at point 0)`, `Bora_Mace (object 32, id 512, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2952.97, 0.00, -2794.19) | on arrival redirect to Waypoint 1 (tag 108), point 2 |

### Waypoint 1

- Tag: `108`
- Members: `GalSpan_Orion (object 0, id 454, starts at point 0)`, `GalSpan_Orion (object 1, id 456, starts at point 0)`, `GalSpan_Orion (object 2, id 457, starts at point 0)`, `GalSpan_Orion (object 3, id 458, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (929.99, 0.00, -3356.08) | None |
| 1 | (2564.32, 0.00, -4080.04) | None |
| 2 | (3829.93, 0.00, -4717.57) | on arrival redirect to Waypoint 1 (tag 108), point 1 |

### Waypoint 2

- Tag: `107`
- Members: `GalSpan_Pegasus (object 13, id 521, starts at point 1)`, `GalSpan_Pegasus (object 14, id 522, starts at point 1)`, `GalSpan_Pegasus (object 15, id 524, starts at point 1)`, `GalSpan_Pegasus (object 16, id 523, starts at point 1)`, `GalSpan_Archangel (object 33, id 1487, starts at point 0)`, `GalSpan_Archangel (object 34, id 1485, starts at point 0)`, `GalSpan_Archangel (object 35, id 1486, starts at point 0)`, `GalSpan_Archangel (object 36, id 1484, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2913.11, 0.00, -1789.28) | None |
| 1 | (5215.12, 0.00, -2329.56) | None |
| 2 | (4706.88, 0.00, -4847.23) | on arrival redirect to Waypoint 2 (tag 107), point 1 |

### Waypoint 3

- Tag: `149`
- Members: `Cassitor_Advanced_Drone (object 26, id 1540, starts at point 0)`, `Cassitor_Advanced_Drone (object 27, id 1541, starts at point 5)`, `Cassitor_Advanced_Drone (object 28, id 1543, starts at point 9)`, `Cassitor_Advanced_Drone (object 29, id 1544, starts at point 3)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1694.51, 0.00, -1027.81) | None |
| 1 | (1308.31, 486.97, -1287.93) | None |
| 2 | (993.01, 469.52, -1100.90) | None |
| 3 | (572.71, 465.23, -1365.28) | None |
| 4 | (159.26, 0.00, -1591.83) | None |
| 5 | (-35.16, 355.89, -1618.38) | None |
| 6 | (-90.29, 227.26, -2025.95) | None |
| 7 | (-164.63, 458.80, -2080.26) | None |
| 8 | (69.83, 471.66, -2342.08) | None |
| 9 | (269.97, 0.00, -2648.78) | on arrival redirect to Waypoint 3 (tag 149), point 0 |

### Waypoint 4

- Tag: `106`
- Members: `TNS_Inquirer (object 12, id 1458, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (4475.75, 685.67, -5863.88) | on arrival play dialog/script or enter gate, param 2 |

### Waypoint 5

- Tag: `150`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1158.64, 21.89, -1866.73) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 6

- Tag: `105`
- Members: `GalSpan_Cruiser (object 40, id 762, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2428.77, 0.00, -4297.23) | on arrival activate current object (raw param -1 ignored) |
| 1 | (2830.72, 0.00, -2365.49) | on arrival redirect to Waypoint 6 (tag 105), point 0 |

### Waypoint 7

- Tag: `104`
- Members: `Bora_Destroyer (object 38, id 738, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1993.22, 0.00, -4611.78) | None; listened by Event 14 for Bora_Destroyer (object 38, id 738) |

### Waypoint 8

- Tag: `101`
- Members: `Bora_Frigate (object 37, id 708, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (3462.29, -919.58, -5815.41) | None |
| 1 | (2729.51, -919.58, -3816.87) | None; listened by Event 8 for Bora_Frigate (object 37, id 708) |
| 2 | (2194.48, -919.58, -2300.71) | on arrival activate current object (raw param -1 ignored); listened by Event 11 for Bora_Frigate (object 37, id 708) |

## Spawn Lists

### Spawn List 0

- ID: `46`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 5 | id 59 | None |
| 1 | 5 | id 43 | None |
| 2 | 5 | spawn list 44 | None |
| 3 | 5 | id 27 | None |
| 4 | 9 | none | None |
| 5 | 6 | GalSpan_Cruiser (object 40, id 762) | None |
| 6 | 6 | id 774 | None |

### Spawn List 1

- ID: `44`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Bora_Destroyer (object 38, id 738) | None |
| 1 | 2 | Bora_Frigate (object 37, id 708) | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `GalSpan_Orion` | 454 | Interactive | 760.17,-319.46,-2979.80 | 164,0,0 | group/role: FG_VIRGO / 1; waypoint: Waypoint 1 (tag 108, 3 point(s)), starting point 0, arrival event value 7077888 |
| 1 | `GalSpan_Orion` | 456 | Interactive | 706.34,-319.46,-3045.79 | 164,0,0 | group/role: FG_VIRGO / 2; waypoint: Waypoint 1 (tag 108, 3 point(s)), starting point 0, arrival event value 7077888 |
| 2 | `GalSpan_Orion` | 457 | Interactive | 642.22,-319.46,-3125.26 | 164,0,0 | group/role: FG_VIRGO / 3; waypoint: Waypoint 1 (tag 108, 3 point(s)), starting point 0, arrival event value 7077888 |
| 3 | `GalSpan_Orion` | 458 | Interactive | 559.48,-319.46,-3200.24 | 164,0,0 | group/role: FG_VIRGO / 4; waypoint: Waypoint 1 (tag 108, 3 point(s)), starting point 0, arrival event value 7077888 |
| 4 | `Bora_Warhammer` | 504 | Interactive | 4491.56,0.00,-6824.99 | 0,0,0 | group/role: FG_TRIDENT / 1; waypoint: Waypoint 0 (tag 109, 1 point(s)), starting point 0, arrival event value 7143424 |
| 5 | `Bora_Warhammer` | 505 | Interactive | 4587.11,0.00,-6827.91 | 0,0,0 | group/role: FG_TRIDENT / 2; waypoint: Waypoint 0 (tag 109, 1 point(s)), starting point 0, arrival event value 7143424 |
| 6 | `Bora_Warhammer` | 506 | Interactive | 4724.22,0.00,-6814.08 | 0,0,0 | group/role: FG_TRIDENT / 3; waypoint: Waypoint 0 (tag 109, 1 point(s)), starting point 0, arrival event value 7143424 |
| 7 | `Bora_Warhammer` | 507 | Interactive | 4855.83,0.00,-6825.49 | 0,0,0 | group/role: FG_TRIDENT / 4; waypoint: Waypoint 0 (tag 109, 1 point(s)), starting point 0, arrival event value 7143424 |
| 8 | `Bora_Battleaxe` | 513 | Interactive | 1727.05,0.00,-2879.02 | 448,0,0 | group/role: FG_MAUL / 1 |
| 9 | `Bora_Battleaxe` | 514 | Interactive | 2042.88,0.00,-3095.50 | 434,0,0 | group/role: FG_MAUL / 2 |
| 10 | `Bora_Battleaxe` | 515 | Interactive | 2416.49,0.00,-2956.39 | 427,0,0 | group/role: FG_MAUL / 3 |
| 11 | `Bora_Battleaxe` | 516 | Interactive | 2224.71,0.00,-611.78 | 384,0,0 | group/role: FG_MAUL / 4 |
| 12 | `TNS_Inquirer` | 1458 | Interactive | 4517.88,1444.19,-6230.39 | 28,0,0 | label: TNSA; alias: tnsa; secondary groups: CONT_005, TNS_INQUIRER; waypoint: Waypoint 4 (tag 106, 1 point(s)), starting point 0, arrival event value 6946816 |
| 13 | `GalSpan_Pegasus` | 521 | Interactive | 5344.99,0.00,-3641.20 | 256,0,0 | group/role: FG_CANCER / 1; waypoint: Waypoint 2 (tag 107, 3 point(s)), starting point 1, arrival event value 7012353 |
| 14 | `GalSpan_Pegasus` | 522 | Interactive | 5454.93,0.00,-3641.19 | 256,0,0 | group/role: FG_CANCER / 2; waypoint: Waypoint 2 (tag 107, 3 point(s)), starting point 1, arrival event value 7012353 |
| 15 | `GalSpan_Pegasus` | 524 | Interactive | 5540.42,0.00,-3641.19 | 256,0,0 | group/role: FG_CANCER / 3; waypoint: Waypoint 2 (tag 107, 3 point(s)), starting point 1, arrival event value 7012353 |
| 16 | `GalSpan_Pegasus` | 523 | Interactive | 5638.13,0.00,-3641.19 | 256,0,0 | group/role: FG_CANCER / 4; waypoint: Waypoint 2 (tag 107, 3 point(s)), starting point 1, arrival event value 7012353 |
| 17 | `Bora_Mace` | 509 | Interactive | 4655.12,0.00,-7142.35 | 0,0,0 | group/role: FG_SWORD / 1; waypoint: Waypoint 0 (tag 109, 1 point(s)), starting point 0, arrival event value 7143424 |
| 18 | `Bora_Mace` | 510 | Interactive | 4774.65,0.00,-7142.35 | 0,0,0 | group/role: FG_SWORD / 2; waypoint: Waypoint 0 (tag 109, 1 point(s)), starting point 0, arrival event value 7143424 |
| 19 | `Bora_Claymore` | 517 | Interactive | 4980.22,0.00,-7577.98 | 0,0,0 | group/role: FG_CATAPULT / 1; waypoint: Waypoint 0 (tag 109, 1 point(s)), starting point 0, arrival event value 7143424 |
| 20 | `Bora_Claymore` | 518 | Interactive | 5102.35,0.00,-7577.98 | 0,0,0 | group/role: FG_CATAPULT / 2; waypoint: Waypoint 0 (tag 109, 1 point(s)), starting point 0, arrival event value 7143424 |
| 21 | `Bora_Claymore` | 519 | Interactive | 5261.13,0.00,-7605.65 | 0,0,0 | group/role: FG_CATAPULT / 3; waypoint: Waypoint 0 (tag 109, 1 point(s)), starting point 0, arrival event value 7143424 |
| 22 | `GalSpan_Orion` | 1523 | Interactive | 4382.78,0.00,-5607.64 | 455,0,0 | group/role: FG_MUSCA / 1; waypoint: Waypoint 0 (tag 109, 1 point(s)), starting point 0, arrival event value 7143424 |
| 23 | `GalSpan_Orion` | 1524 | Interactive | 4377.76,0.00,-5665.62 | 455,0,0 | group/role: FG_MUSCA / 2; waypoint: Waypoint 0 (tag 109, 1 point(s)), starting point 0, arrival event value 7143424 |
| 24 | `GalSpan_Orion` | 1525 | Interactive | 4446.56,0.00,-5622.19 | 455,0,0 | group/role: FG_MUSCA / 3; waypoint: Waypoint 0 (tag 109, 1 point(s)), starting point 0, arrival event value 7143424 |
| 25 | `GalSpan_Orion` | 1526 | Interactive | 4504.07,0.00,-5622.23 | 455,0,0 | group/role: FG_MUSCA / 4; waypoint: Waypoint 0 (tag 109, 1 point(s)), starting point 0, arrival event value 7143424 |
| 26 | `Cassitor_Advanced_Drone` | 1540 | Interactive | 1720.28,-9.82,-1027.09 | 0,0,0 | label: gdron; group/role: FG_CYCNUS / 0; waypoint: Waypoint 3 (tag 149, 10 point(s)), starting point 0, arrival event value 9764864 |
| 27 | `Cassitor_Advanced_Drone` | 1541 | Interactive | -72.21,357.35,-1604.26 | 0,0,0 | label: gdron; group/role: FG_CYCNUS / 0; waypoint: Waypoint 3 (tag 149, 10 point(s)), starting point 5, arrival event value 9764869 |
| 28 | `Cassitor_Advanced_Drone` | 1543 | Interactive | 294.11,0.00,-2646.64 | 0,0,0 | label: gdron; group/role: FG_CYCNUS / 0; waypoint: Waypoint 3 (tag 149, 10 point(s)), starting point 9, arrival event value 9764873 |
| 29 | `Cassitor_Advanced_Drone` | 1544 | Interactive | 544.08,483.01,-1352.68 | 0,0,0 | label: gdron; group/role: FG_CYCNUS / 0; waypoint: Waypoint 3 (tag 149, 10 point(s)), starting point 3, arrival event value 9764867 |
| 30 | `Bora_Claymore` | 520 | Interactive | 5392.60,0.00,-7606.31 | 0,0,0 | group/role: FG_CATAPULT / 4; waypoint: Waypoint 0 (tag 109, 1 point(s)), starting point 0, arrival event value 7143424 |
| 31 | `Bora_Mace` | 511 | Interactive | 4889.20,0.00,-7147.54 | 0,0,0 | group/role: FG_SWORD / 3; waypoint: Waypoint 0 (tag 109, 1 point(s)), starting point 0, arrival event value 7143424 |
| 32 | `Bora_Mace` | 512 | Interactive | 5032.63,0.00,-7120.46 | 0,0,0 | group/role: FG_SWORD / 4; waypoint: Waypoint 0 (tag 109, 1 point(s)), starting point 0, arrival event value 7143424 |
| 33 | `GalSpan_Archangel` | 1487 | Interactive | 2323.00,612.83,-1736.24 | 192,0,0 | group/role: FG_LYNX / 1; waypoint: Waypoint 2 (tag 107, 3 point(s)), starting point 0, arrival event value 7012352 |
| 34 | `GalSpan_Archangel` | 1485 | Interactive | 2451.66,612.83,-1610.02 | 192,0,0 | group/role: FG_LYNX / 3; waypoint: Waypoint 2 (tag 107, 3 point(s)), starting point 0, arrival event value 7012352 |
| 35 | `GalSpan_Archangel` | 1486 | Interactive | 2390.40,612.83,-1663.17 | 192,0,0 | group/role: FG_LYNX / 2; waypoint: Waypoint 2 (tag 107, 3 point(s)), starting point 0, arrival event value 7012352 |
| 36 | `GalSpan_Archangel` | 1484 | Interactive | 2543.56,612.83,-1530.31 | 192,0,0 | group/role: FG_LYNX / 4; waypoint: Waypoint 2 (tag 107, 3 point(s)), starting point 0, arrival event value 7012352 |
| 37 | `Bora_Frigate` | 708 | Interactive | 3636.36,-985.27,-6313.26 | 485,0,0 | label: CRGUS; secondary groups: CONT_023, COURAGEOUS; waypoint: Waypoint 8 (tag 101, 3 point(s)), starting point 0, arrival event value 6619136 |
| 38 | `Bora_Destroyer` | 738 | Interactive | 6828.40,-525.47,-3970.72 | 364,0,0 | label: INTEG; secondary groups: CONT_023, INTEGRITY; waypoint: Waypoint 7 (tag 104, 1 point(s)), starting point 0, arrival event value 6815744 |
| 39 | `GalSpan_Singularity_Platform` | 1323 | Interactive | 564.89,0.00,-1769.84 | 57,0,0 | label: HEPHA; secondary groups: none, HEPH_MINING |
| 40 | `GalSpan_Cruiser` | 762 | Interactive | 1376.67,-1329.05,-3135.32 | 193,0,0 | secondary groups: none, LAZARUS; waypoint: Waypoint 6 (tag 105, 2 point(s)), starting point 0, arrival event value 6881280 |
