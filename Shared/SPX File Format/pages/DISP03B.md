# Tachyon: The Fringe DISP03B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP03B.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 6 |
| Entities | 38 |
| Events | 24 |
| Waypoints | 10 |
| Child Sectors | 0 |
| Scripts | 4 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Carrier`, `1: GalSpan_Frigate`, `2: Science_Vessel`, `3: GalSpan_Pegasus`, `4: Drone_Worker`, `5: Computer_Core` |
| Scripts | `PLAYER.SCR`, `CANDR.SCR`, `CANST.SCR`, `BINSD.SCR` |
| Scenes | None |
| Labels | `BFGE_02`, `BFBE_07`, `TNSA`, `BFBE_09`, `adder1`, `BFBF_07`, `ROSS`, `SPIKE`, `atkin`, `cruiser1` |
| Aliases | `fake_2`, `BC10_Waraxe`, `Coward`, `spy_1`, `fake_1`, `tnsa`, `BC10_Claymore4`, `BC10_Claymore3`, `BC10_Claymore2`, `BC10_Claymore1`, `BC10_Warhammer4`, `BC10_Warhammer3`, `BC10_Warhammer2`, `BC10_Warhammer1`, `BC10_Mace3`, `BC10_Mace4`, `BC10_Mace1`, `BC10_Mace2`, `Galileo`, `SPIKE`, `zeus`, `Stocks01` |
| Groups | `FG_CRUX`, `FG_MEDUSA`, `FG_CYCLOPS`, `FG_GORGONS`, `FG_CRONUS`, `FG_CETUS`, `FG_LUPUS`, `FG_CALLISTO`, `FG_NERGAL`, `GALILEO`, `CONT_036`, `URSA_MINOR`, `URSA_MAJOR` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 9, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 13
- Play dialog: PLAYER.SCR, line/variant 2

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Group/spawn-list action: spawn list/group 159, subtype 4, param 2
- Group/spawn-list action: spawn list/group 160, subtype 4, param 2
- Group/spawn-list action: spawn list/group 161, subtype 4, param 2

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 20 (join 1)
- Variable comparison: subject variable group 21, variable 34, op 1, value 1

**Action**

- Play dialog: CANDR.SCR, line/variant 8

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 8927; join 1; flags 2)
- Sector/startup condition family: subject 1, op 0, value 6

**Action**

- Play dialog: PLAYER.SCR, line/variant 3
- Set runtime trigger variable: variable group 20, variable 10, subtype 0, value 0
- Set/add variable: variable group 21, variable 21, subtype 0, value 1

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 10, op 1, value 25 (join 2)

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Object spawn/action: Computer_Core (object 0, id 8980), subtype 0
- Object spawn/action: Computer_Core (object 0, id 8980), subtype 14
- Show/update HUD contact: contact/list 0, subtype 9, param 14
- Play dialog: PLAYER.SCR, line/variant 5

### Event 5

**Trigger**

- Group/spawn-list event: subject 221, op 5, value 0 (join 2)
- Group/spawn-list event: subject 222, op 5, value 0 (join 2)
- Group/spawn-list event: subject 226, op 5, value 0 (join 2)
- Group/spawn-list event: subject 159, op 5, value 0 (join 2)
- Group/spawn-list event: subject 160, op 5, value 0 (join 2)
- Group/spawn-list event: subject 223, op 5, value 0 (join 2)
- Group/spawn-list event: subject 161, op 5, value 0 (join 2)

**Action**

- Set/add variable: variable group 21, variable 34, subtype 0, value 1

### Event 6

**Trigger**

- Variable comparison: subject variable group 21, variable 34, op 1, value 1 (join 1)
- Sector/startup condition family: subject 0, op 0, value 3

**Action**

- Play dialog: CANDR.SCR, line/variant 6

### Event 7

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 6

**Action**

- Play dialog: CANST.SCR, line/variant 4

### Event 8

**Trigger**

- Sector/startup condition family: subject 2, op 0, value 4

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Object spawn/action: Computer_Core (object 0, id 8980), subtype 0
- Object spawn/action: Computer_Core (object 0, id 8980), subtype 14
- Play dialog: PLAYER.SCR, line/variant 5
- Show/update HUD contact: contact/list 0, subtype 9, param 14

### Event 9

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 8980; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 9
- Hide/remove HUD contact: contact/list 0, subtype 9, param 14
- Mission objective/state: param 393216, subtype 0, param 0
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 21, variable 26, subtype 0, value 1
- Set/add variable: variable group 21, variable 27, subtype 0, value 1

### Event 10

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 90 (join 2)
- Object event: subject 8927, op 0, value 0 (join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 8980; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 300 (extra 1, 9011; join 2; flags 2)
- Group/spawn-list event: subject 160, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 161, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 159, op 4, value 0 (join 2; flags 2)

**Action**

- Group/spawn-list action: spawn list/group 221, subtype 0
- Group/spawn-list action: spawn list/group 222, subtype 0
- Group/spawn-list action: spawn list/group 223, subtype 0
- Group/spawn-list action: spawn list/group 226, subtype 8, param 10420224 (Waypoint 4 (tag 159), point 0)
- Group/spawn-list action: spawn list/group 221, subtype 4, param 2
- Group/spawn-list action: spawn list/group 222, subtype 4, param 2
- Group/spawn-list action: spawn list/group 223, subtype 4, param 2
- Group/spawn-list action: spawn list/group 226, subtype 4, param 2

### Event 11

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 0 (join 2)
- Object event: subject 8927, op 0, value 0 (join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 8980; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 300 (extra 1, 9011; join 2; flags 2)
- Group/spawn-list event: subject 160, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 161, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 159, op 4, value 0 (join 2; flags 2)

**Action**

- Play dialog: CANST.SCR, line/variant 1

### Event 12

**Trigger**

- Variable comparison: subject variable group 20, variable 10, op 1, value 45

**Action**

- Gate state/action: param 1, subtype 3, param 0
- Gate state/action: param 10203, subtype 3, param 0
- Gate state/action: param 2, subtype 3, param 0
- Gate state/action: param 3, subtype 3, param 0
- Gate state/action: param 6591, subtype 3, param 0
- Hide/remove HUD contact: contact/list 0, subtype 8, param 0

### Event 13

**Trigger**

- Variable comparison: subject variable group 20, variable 10, op 1, value 50

**Action**

- Play dialog: BINSD.SCR, line/variant 7
- Show/update HUD contact: contact/list 0, subtype 9, param 32

### Event 14

**Trigger**

- Sector/startup condition family: subject 3, op 0, value 7

**Action**

- Play dialog: PLAYER.SCR, line/variant 188

### Event 15

**Trigger**

- Variable comparison: subject variable group 20, variable 10, op 1, value 260

**Action**

- Play dialog: BINSD.SCR, line/variant 8

### Event 16

**Trigger**

- Variable comparison: subject variable group 20, variable 10, op 1, value 265

**Action**

- Gate state/action: param 1, subtype 2, param 0
- Gate state/action: param 10203, subtype 2, param 0
- Gate state/action: param 2, subtype 2, param 0
- Gate state/action: param 3, subtype 2, param 0
- Gate state/action: param 6591, subtype 2, param 0
- Group/spawn-list action: spawn list/group 224, subtype 1, param 3

### Event 17

**Trigger**

- Sector/startup condition family: subject 3, op 0, value 8

**Action**

- Play dialog: CANST.SCR, line/variant 2
- Hide/remove HUD contact: contact/list 0, subtype 9, param 32
- Show/update HUD contact: contact/list 0, subtype 12, param 24
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 38, variable 0, subtype 0, value 1

### Event 18

**Trigger**

- Variable comparison: subject variable group 20, variable 10, op 1, value 140
- Variable comparison: subject variable group 37, variable 12, op 1, value 0

**Action**

- Object spawn/action: GalSpan_Frigate (object 36, id 10215), subtype 3
- Object spawn/action: GalSpan_Carrier (object 37, id 11054), subtype 3
- Set runtime trigger variable: variable group 20, variable 8, subtype 0, value 0
- Play dialog: PLAYER.SCR, line/variant 187

### Event 19

**Trigger**

- Variable comparison: subject variable group 20, variable 10, op 1, value 90
- Variable comparison: subject variable group 37, variable 12, op 1, value 1

**Action**

- Object spawn/action: GalSpan_Frigate (object 36, id 10215), subtype 3
- Object spawn/action: GalSpan_Carrier (object 37, id 11054), subtype 3
- Set runtime trigger variable: variable group 20, variable 8, subtype 0, value 0
- Play dialog: PLAYER.SCR, line/variant 187

### Event 20

**Trigger**

- Variable comparison: subject variable group 20, variable 8, op 1, value 10

**Action**

- Group/spawn-list action: spawn list/group 227, subtype 1, param 11054

### Event 21

**Trigger**

- Group/spawn-list event: subject 224, op 1, value 20

**Action**

- Play dialog: PLAYER.SCR, line/variant 152

### Event 22

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 90 (join 1)
- Group/spawn-list event: subject 160, op 0, value 0

**Action**

- Play dialog: CANDR.SCR, line/variant 1

### Event 23

**Trigger**

- Group/spawn-list event: subject 221, op 1, value 30 (join 2)
- Group/spawn-list event: subject 222, op 1, value 30 (join 2)

**Action**

- Play dialog: CANDR.SCR, line/variant 5

## Waypoints

### Waypoint 0

- Tag: `162`
- Members: `GalSpan_Pegasus (object 23, id 10211, starts at point -1)`, `GalSpan_Pegasus (object 24, id 10212, starts at point -1)`, `GalSpan_Pegasus (object 25, id 10213, starts at point -1)`, `GalSpan_Pegasus (object 26, id 10214, starts at point -1)`, `GalSpan_Pegasus (object 27, id 11036, starts at point -1)`, `GalSpan_Pegasus (object 28, id 11037, starts at point -1)`, `GalSpan_Pegasus (object 29, id 11038, starts at point -1)`, `GalSpan_Pegasus (object 30, id 11039, starts at point -1)`, `GalSpan_Pegasus (object 31, id 11040, starts at point -1)`, `GalSpan_Pegasus (object 32, id 11041, starts at point -1)`, `GalSpan_Pegasus (object 33, id 11042, starts at point -1)`, `GalSpan_Pegasus (object 34, id 11043, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-750.09, 0.00, 2796.19) | None |
| 1 | (-1312.13, 0.00, 3708.26) | None |
| 2 | (-2480.81, 0.00, 3638.07) | None |
| 3 | (-2675.04, 0.00, 2709.96) | None |
| 4 | (-1377.38, 0.00, 1310.76) | on arrival redirect to Waypoint 0 (tag 162), point 0 |

### Waypoint 1

- Tag: `163`
- Members: `Computer_Core (object 0, id 8980, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-92.63, -152.46, 1088.73) | None |
| 1 | (-92.70, -265.03, 1088.55) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 2

- Tag: `161`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2594.64, 275.45, 878.18) | None |
| 1 | (-1109.06, 275.45, 4706.44) | on arrival action 1, param -1 |

### Waypoint 3

- Tag: `160`
- Members: `GalSpan_Frigate (object 36, id 10215, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (869.25, 275.45, -1492.15) | None |
| 1 | (-963.75, 275.45, 408.76) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 4

- Tag: `159`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-233.33, 0.00, -5129.19) | None |
| 1 | (-229.14, 0.00, -6091.42) | None |
| 2 | (1025.66, 0.00, -6099.02) | None |
| 3 | (1024.21, 0.00, -5121.01) | None |

### Waypoint 5

- Tag: `157`
- Members: `Drone_Worker (object 19, id 9001, starts at point 0)`, `Drone_Worker (object 20, id 9002, starts at point 0)`, `Drone_Worker (object 21, id 9003, starts at point 0)`, `Drone_Worker (object 22, id 9004, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (369.18, 0.00, -5180.34) | None |
| 1 | (370.92, 0.00, 198.90) | on arrival redirect to Waypoint 1 (tag 163), point 0 |

### Waypoint 6

- Tag: `156`
- Members: `Drone_Worker (object 15, id 8997, starts at point -1)`, `Drone_Worker (object 16, id 8998, starts at point -1)`, `Drone_Worker (object 17, id 8999, starts at point -1)`, `Drone_Worker (object 18, id 9000, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-285.88, 251.24, 740.69) | None |
| 1 | (-606.27, 161.74, 289.36) | on arrival redirect to Waypoint 0 (tag 162), point 2 |

### Waypoint 7

- Tag: `155`
- Members: `Drone_Worker (object 11, id 8993, starts at point 0)`, `Drone_Worker (object 12, id 8994, starts at point 0)`, `Drone_Worker (object 13, id 8995, starts at point 0)`, `Drone_Worker (object 14, id 8996, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (101.88, 256.93, 1421.43) | None |
| 1 | (441.21, 256.93, 1882.52) | on arrival redirect to Waypoint 0 (tag 162), point 0 |

### Waypoint 8

- Tag: `152`
- Members: `Drone_Worker (object 5, id 8949, starts at point 2)`, `Drone_Worker (object 6, id 8950, starts at point 2)`, `Drone_Worker (object 9, id 8948, starts at point 0)`, `Drone_Worker (object 10, id 8947, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-661.45, 0.00, 1022.98) | None |
| 1 | (-459.71, 0.00, 597.41) | None |
| 2 | (386.36, 0.00, 600.68) | None |
| 3 | (383.05, 0.00, 1561.04) | None |
| 4 | (-449.31, 0.00, 1565.04) | on arrival redirect to Waypoint 9 (tag 151), point 0 |

### Waypoint 9

- Tag: `151`
- Members: `Drone_Worker (object 7, id 8945, starts at point 3)`, `Drone_Worker (object 8, id 8946, starts at point 3)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-159.94, 385.05, 550.90) | None |
| 1 | (-127.58, -327.37, 554.42) | None |
| 2 | (6.02, -530.11, 1075.01) | None |
| 3 | (-147.71, -308.63, 1669.65) | None |
| 4 | (-84.10, 385.05, 1669.40) | on arrival redirect to Waypoint 8 (tag 152), point 0 |

## Spawn Lists

### Spawn List 0

- ID: `227`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 1

- ID: `224`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 2

- ID: `221`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 3

- ID: `222`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 4

- ID: `226`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 5

- ID: `159`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 6

- ID: `160`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 7

- ID: `223`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 8

- ID: `161`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Computer_Core` | 8980 | Interactive | -92.30,-145.94,1088.84 | 0,385,0 | waypoint: Waypoint 1 (tag 163, 2 point(s)), starting point -1 |
| 1 | `Drone_Worker` | 9015 | Interactive | 321.08,71.10,-5606.50 | 0,0,0 | group/role: FG_CRUX / 0 |
| 2 | `Drone_Worker` | 9016 | Interactive | 336.48,71.09,-5606.05 | 0,0,0 | group/role: FG_CRUX / 0 |
| 3 | `Drone_Worker` | 9017 | Interactive | 321.08,71.10,-5631.57 | 256,0,0 | group/role: FG_CRUX / 0 |
| 4 | `Drone_Worker` | 9018 | Interactive | 336.54,71.09,-5631.79 | 256,0,0 | group/role: FG_CRUX / 0 |
| 5 | `Drone_Worker` | 8949 | Interactive | 832.78,0.00,569.45 | 0,0,0 | group/role: FG_MEDUSA / 0; waypoint: Waypoint 8 (tag 152, 5 point(s)), starting point 2, arrival event value 9961474 |
| 6 | `Drone_Worker` | 8950 | Interactive | 850.30,0.00,453.06 | 0,0,0 | group/role: FG_MEDUSA / 0; waypoint: Waypoint 8 (tag 152, 5 point(s)), starting point 2, arrival event value 9961474 |
| 7 | `Drone_Worker` | 8945 | Interactive | -97.89,-152.07,1781.96 | 0,0,0 | group/role: FG_CYCLOPS / 0; waypoint: Waypoint 9 (tag 151, 5 point(s)), starting point 3, arrival event value 9895939 |
| 8 | `Drone_Worker` | 8946 | Interactive | 14.12,0.00,1729.06 | 0,0,0 | group/role: FG_CYCLOPS / 0; waypoint: Waypoint 9 (tag 151, 5 point(s)), starting point 3, arrival event value 9895939 |
| 9 | `Drone_Worker` | 8948 | Interactive | -821.55,0.00,1295.69 | 0,0,0 | group/role: FG_GORGONS / 0; waypoint: Waypoint 8 (tag 152, 5 point(s)), starting point 0, arrival event value 9961472 |
| 10 | `Drone_Worker` | 8947 | Interactive | -742.69,0.00,1390.92 | 0,0,0 | group/role: FG_GORGONS / 0; waypoint: Waypoint 8 (tag 152, 5 point(s)), starting point 0, arrival event value 9961472 |
| 11 | `Drone_Worker` | 8993 | Interactive | 32.68,256.93,1304.05 | 0,0,0 | group/role: FG_CRONUS / 0; waypoint: Waypoint 7 (tag 155, 2 point(s)), starting point 0, arrival event value 10158080 |
| 12 | `Drone_Worker` | 8994 | Interactive | 41.97,256.93,1290.42 | 0,0,0 | group/role: FG_CRONUS / 0; waypoint: Waypoint 7 (tag 155, 2 point(s)), starting point 0, arrival event value 10158080 |
| 13 | `Drone_Worker` | 8995 | Interactive | 48.70,256.93,1306.93 | 0,0,0 | group/role: FG_CRONUS / 0; waypoint: Waypoint 7 (tag 155, 2 point(s)), starting point 0, arrival event value 10158080 |
| 14 | `Drone_Worker` | 8996 | Interactive | 40.60,256.93,1319.36 | 0,0,0 | group/role: FG_CRONUS / 0; waypoint: Waypoint 7 (tag 155, 2 point(s)), starting point 0, arrival event value 10158080 |
| 15 | `Drone_Worker` | 8997 | Interactive | -237.43,253.37,866.44 | 0,0,0 | group/role: FG_CETUS / 0; waypoint: Waypoint 6 (tag 156, 2 point(s)), starting point -1 |
| 16 | `Drone_Worker` | 8998 | Interactive | -204.97,253.37,834.19 | 0,0,0 | group/role: FG_CETUS / 0; waypoint: Waypoint 6 (tag 156, 2 point(s)), starting point -1 |
| 17 | `Drone_Worker` | 8999 | Interactive | -221.40,253.37,856.50 | 0,0,0 | group/role: FG_CETUS / 0; waypoint: Waypoint 6 (tag 156, 2 point(s)), starting point -1 |
| 18 | `Drone_Worker` | 9000 | Interactive | -237.01,253.37,841.14 | 0,0,0 | group/role: FG_CETUS / 0; waypoint: Waypoint 6 (tag 156, 2 point(s)), starting point -1 |
| 19 | `Drone_Worker` | 9001 | Interactive | 304.88,0.00,-5532.87 | 0,0,0 | group/role: FG_LUPUS / 0; waypoint: Waypoint 5 (tag 157, 2 point(s)), starting point 0, arrival event value 10289152 |
| 20 | `Drone_Worker` | 9002 | Interactive | 320.25,0.00,-5530.53 | 0,0,0 | group/role: FG_LUPUS / 0; waypoint: Waypoint 5 (tag 157, 2 point(s)), starting point 0, arrival event value 10289152 |
| 21 | `Drone_Worker` | 9003 | Interactive | 316.83,0.00,-5555.37 | 0,0,0 | group/role: FG_LUPUS / 0; waypoint: Waypoint 5 (tag 157, 2 point(s)), starting point 0, arrival event value 10289152 |
| 22 | `Drone_Worker` | 9004 | Interactive | 333.58,0.00,-5514.49 | 0,0,0 | group/role: FG_LUPUS / 0; waypoint: Waypoint 5 (tag 157, 2 point(s)), starting point 0, arrival event value 10289152 |
| 23 | `GalSpan_Pegasus` | 10211 | Interactive | 908.84,0.00,-706.00 | 0,0,0 | label: BFBE_09; group/role: FG_CALLISTO / 0; waypoint: Waypoint 0 (tag 162, 5 point(s)), starting point -1 |
| 24 | `GalSpan_Pegasus` | 10212 | Interactive | 882.29,0.00,-746.81 | 0,0,0 | group/role: FG_CALLISTO / 0; waypoint: Waypoint 0 (tag 162, 5 point(s)), starting point -1 |
| 25 | `GalSpan_Pegasus` | 10213 | Interactive | 860.17,0.00,-777.27 | 0,0,0 | group/role: FG_CALLISTO / 0; waypoint: Waypoint 0 (tag 162, 5 point(s)), starting point -1 |
| 26 | `GalSpan_Pegasus` | 10214 | Interactive | 906.85,0.00,-773.20 | 0,0,0 | group/role: FG_CALLISTO / 0; waypoint: Waypoint 0 (tag 162, 5 point(s)), starting point -1 |
| 27 | `GalSpan_Pegasus` | 11036 | Interactive | 924.45,0.00,-740.34 | 0,0,0 | label: BFBE_09; group/role: FG_CALLISTO / 0; waypoint: Waypoint 0 (tag 162, 5 point(s)), starting point -1 |
| 28 | `GalSpan_Pegasus` | 11037 | Interactive | 949.50,0.00,-769.54 | 0,0,0 | label: BFBE_09; group/role: FG_CALLISTO / 0; waypoint: Waypoint 0 (tag 162, 5 point(s)), starting point -1 |
| 29 | `GalSpan_Pegasus` | 11038 | Interactive | 1192.39,0.00,-499.51 | 0,0,0 | label: BFBE_09; group/role: FG_NERGAL / 0; waypoint: Waypoint 0 (tag 162, 5 point(s)), starting point -1 |
| 30 | `GalSpan_Pegasus` | 11039 | Interactive | 1217.91,0.00,-539.48 | 0,0,0 | group/role: FG_NERGAL / 0; waypoint: Waypoint 0 (tag 162, 5 point(s)), starting point -1 |
| 31 | `GalSpan_Pegasus` | 11040 | Interactive | 1240.59,0.00,-567.15 | 0,0,0 | group/role: FG_NERGAL / 0; waypoint: Waypoint 0 (tag 162, 5 point(s)), starting point -1 |
| 32 | `GalSpan_Pegasus` | 11041 | Interactive | 1192.39,0.00,-564.07 | 0,0,0 | group/role: FG_NERGAL / 0; waypoint: Waypoint 0 (tag 162, 5 point(s)), starting point -1 |
| 33 | `GalSpan_Pegasus` | 11042 | Interactive | 1175.38,0.00,-533.33 | 0,0,0 | label: BFBE_09; group/role: FG_NERGAL / 0; waypoint: Waypoint 0 (tag 162, 5 point(s)), starting point -1 |
| 34 | `GalSpan_Pegasus` | 11043 | Interactive | 1152.70,0.00,-561.00 | 0,0,0 | label: BFBE_09; group/role: FG_NERGAL / 0; waypoint: Waypoint 0 (tag 162, 5 point(s)), starting point -1 |
| 35 | `Science_Vessel` | 9011 | Interactive | 321.84,0.00,-5618.82 | 128,0,0 | alias: Galileo; secondary groups: CONT_036, GALILEO |
| 36 | `GalSpan_Frigate` | 10215 | Interactive | 1404.11,266.03,-1967.28 | 449,0,0 | label: BFBE_09; secondary groups: none, URSA_MINOR; waypoint: Waypoint 3 (tag 160, 2 point(s)), starting point -1 |
| 37 | `GalSpan_Carrier` | 11054 | Interactive | 958.50,0.00,2519.97 | 449,0,0 | secondary groups: none, URSA_MAJOR |
