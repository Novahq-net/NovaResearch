# Tachyon: The Fringe NEUT06C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT06C.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 5 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 6 |
| Entities | 21 |
| Events | 29 |
| Waypoints | 10 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Light_Freighter`, `1: Bora_Hvy_Freighter`, `2: Medical_Frigate`, `3: GalSpan_Pegasus`, `4: GalSpan_Poseidon`, `5: Star_Patrol_Enforcer` |
| Scripts | `DROME.SCR`, `AOBUL.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFNE_02`, `bfbe_08`, `BFNE_01`, `bfne_09`, `bfbe_01`, `BLACK`, `repar` |
| Aliases | `Todd08`, `Todd09`, `Todd10`, `oside`, `oside_1`, `oside_2`, `bagel`, `bagel_1`, `bagel_2`, `kwB10_01`, `kwB10_02`, `Todd13`, `Todd12`, `Todd02`, `Todd03`, `Todd04`, `Todd05`, `Todd06`, `Todd07`, `will_01`, `kevin01`, `SHIP1_HYPER`, `SHIP2_HYPER`, `SHIP3_HYPER`, `ohshit` |
| Groups | `FG_QUAKE`, `FG_SIROCCO`, `FG_OCTANS`, `FG_MENSA`, `FG_PICTOR`, `FG_ARES`, `DROMEDARY`, `CONT_002`, `BOLD`, `CONT_004`, `TRAVELER`, `CONT_028`, `FINDER`, `CONT_030` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Variable comparison: subject variable group 21, variable 5, op 1, value 1

**Action**

- Object spawn/action: Medical_Frigate (object 17, id 4721), subtype 3

### Event 1

**Trigger**

- Variable comparison: subject variable group 21, variable 6, op 1, value 1

**Action**

- Object spawn/action: Bora_Hvy_Freighter (object 19, id 4729), subtype 3

### Event 2

**Trigger**

- Variable comparison: subject variable group 21, variable 7, op 1, value 1

**Action**

- Object spawn/action: Bora_Hvy_Freighter (object 18, id 4738), subtype 3

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Group/spawn-list action: spawn list/group 234, subtype 4, param 6
- Group/spawn-list action: spawn list/group 235, subtype 4, param 6
- Group/spawn-list action: spawn list/group 16, subtype 4, param 6
- Show/update HUD contact: contact/list 0, subtype 9, param 22
- Show/update HUD contact: contact/list 0, subtype 9, param 19
- Show/update HUD contact: contact/list 0, subtype 9, param 23
- Group/spawn-list action: spawn list/group 198, subtype 4, param 6
- Set runtime trigger variable: variable group 20, variable 4, subtype 0, value 0

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 4, op 1, value 3

**Action**

- Group/spawn-list action: spawn list/group 16, subtype 2
- Group/spawn-list action: spawn list/group 234, subtype 2
- Group/spawn-list action: spawn list/group 235, subtype 2
- Object spawn/action: Medical_Frigate (object 17, id 4721), subtype 5
- Object spawn/action: Bora_Hvy_Freighter (object 19, id 4729), subtype 5
- Object spawn/action: Bora_Hvy_Freighter (object 18, id 4738), subtype 5
- Group/spawn-list action: spawn list/group 198, subtype 2

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 4, op 1, value 7

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 19
- Hide/remove HUD contact: contact/list 0, subtype 9, param 22
- Hide/remove HUD contact: contact/list 0, subtype 9, param 23
- Show/update HUD contact: contact/list 0, subtype 2, param 4721
- Show/update HUD contact: contact/list 0, subtype 2, param 4729
- Show/update HUD contact: contact/list 0, subtype 2, param 4738
- Show/update HUD contact: contact/list 0, subtype 1, param 198

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 4, op 1, value 10

**Action**

- Set runtime trigger variable: variable group 20, variable 4, subtype 1, value 0
- Hide/remove HUD contact: contact/list 0, subtype 11, param 0
- Object spawn/action: Medical_Frigate (object 17, id 4721), subtype 14

### Event 7

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 3 (join 2)
- Sector/startup condition family: subject 0, op 0, value 2 (join 2)

**Action**

- Set/add variable: variable group 21, variable 20, subtype 0, value 1
- Play dialog: DROME.SCR, line/variant 1

### Event 8

**Trigger**

- Group/spawn-list event: subject 234, op 0, value 0
- Group/spawn-list event: subject 235, op 0, value 0
- Group/spawn-list event: subject 16, op 0, value 0

**Action**

- Play dialog: AOBUL.SCR, line/variant 19
- Group/spawn-list action: spawn list/group 141, subtype 3, param 4690
- Group/spawn-list action: spawn list/group 192, subtype 3, param 4690

### Event 9

**Trigger**

- Group/spawn-list event: subject 16, op 0, value 0
- Group/spawn-list event: subject 234, op 0, value 0
- Group/spawn-list event: subject 235, op 0, value 0
- Group/spawn-list event: subject 198, op 0, value 0 (join 1)
- Object event: subject Medical_Frigate (object 17, id 4721), op 2, value 0

**Action**

- Object spawn/action: Medical_Frigate (object 17, id 4721), subtype 4
- Object spawn/action: Bora_Hvy_Freighter (object 19, id 4729), subtype 4
- Object spawn/action: Bora_Hvy_Freighter (object 18, id 4738), subtype 4
- Hide/remove HUD contact: contact/list 0, subtype 2, param 4721
- Hide/remove HUD contact: contact/list 0, subtype 2, param 4738
- Hide/remove HUD contact: contact/list 0, subtype 2, param 4729
- Mission objective/state: param 65542, subtype 0, param 0
- Play dialog: PLAYER.SCR, line/variant 211

### Event 10

**Trigger**

- Object event: subject Medical_Frigate (object 17, id 4721), op 8, value 0

**Action**

- Set/add variable: variable group 21, variable 8, subtype 0, value 1
- Set/add variable: variable group 21, variable 34, subtype 0, value 1

### Event 11

**Trigger**

- Object event: subject Bora_Hvy_Freighter (object 19, id 4729), op 8, value 0

**Action**

- Set/add variable: variable group 21, variable 9, subtype 0, value 1

### Event 12

**Trigger**

- Object event: subject Bora_Hvy_Freighter (object 18, id 4738), op 8, value 0

**Action**

- Set/add variable: variable group 21, variable 10, subtype 0, value 1

### Event 13

**Trigger**

- Object event: subject Medical_Frigate (object 17, id 4721), op 2, value 0

**Action**

- Set/add variable: variable group 13, variable 410, subtype 0, value 1
- Set/add variable: variable group 13, variable 411, subtype 0, value 1
- Gate state/action: param 4689, subtype 3, param 0
- Play dialog: PLAYER.SCR, line/variant 75
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Mark/flash contact: contact/list 0, subtype 2, param 4721
- Show/update HUD contact: contact/list 0, subtype 11, param 34

### Event 14

**Trigger**

- Object event: subject Bora_Hvy_Freighter (object 19, id 4729), op 2, value 0

**Action**

- Mark/flash contact: contact/list 0, subtype 2, param 4729

### Event 15

**Trigger**

- Object event: subject Bora_Hvy_Freighter (object 18, id 4738), op 2, value 0

**Action**

- Mark/flash contact: contact/list 0, subtype 2, param 4738

### Event 16

**Trigger**

- Object event: subject Bora_Hvy_Freighter (object 19, id 4729), op 3, value 10

**Action**

- Play dialog: DROME.SCR, line/variant 2

### Event 17

**Trigger**

- Object event: subject Bora_Hvy_Freighter (object 18, id 4738), op 3, value 10

**Action**

- Play dialog: DROME.SCR, line/variant 3

### Event 18

**Trigger**

- Object event: subject Bora_Hvy_Freighter (object 19, id 4729), op 2, value 0
- Object event: subject Bora_Hvy_Freighter (object 18, id 4738), op 2, value 0 (join 1)
- Object event: subject Medical_Frigate (object 17, id 4721), op 2, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 74

### Event 19

**Trigger**

- Group/spawn-list event: subject 198, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 198

### Event 20

**Trigger**

- Group/spawn-list event: subject 16, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 16

### Event 21

**Trigger**

- Object event: subject GalSpan_Pegasus (object 12, id 6607), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: GalSpan_Pegasus (object 12, id 6607), subtype 7

### Event 22

**Trigger**

- Object event: subject GalSpan_Pegasus (object 13, id 6608), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: GalSpan_Pegasus (object 13, id 6608), subtype 7

### Event 23

**Trigger**

- Object event: subject GalSpan_Pegasus (object 14, id 6609), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: GalSpan_Pegasus (object 14, id 6609), subtype 7

### Event 24

**Trigger**

- Variable comparison: subject variable group 21, variable 34, op 1, value 1

**Action**

- Object spawn/action: Generic_Light_Freighter (object 20, id 6784), subtype 3

### Event 25

**Trigger**

- Object event: subject Generic_Light_Freighter (object 20, id 6784), op 8, value 0

**Action**

- Set/add variable: variable group 21, variable 30, subtype 0, value 1

### Event 26

**Trigger**

- Object event: subject GalSpan_Pegasus (object 12, id 6607), op 2, value 0
- Object event: subject GalSpan_Pegasus (object 13, id 6608), op 2, value 0
- Object event: subject GalSpan_Pegasus (object 14, id 6609), op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 1, param 16

### Event 27

**Trigger**

- Object event: subject Medical_Frigate (object 17, id 4721), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 16
- Hide/remove HUD contact: contact/list 0, subtype 1, param 198
- Hide/remove HUD contact: contact/list 0, subtype 2, param 4729
- Hide/remove HUD contact: contact/list 0, subtype 2, param 4738

### Event 28

**Trigger**

- Object event: subject Medical_Frigate (object 17, id 4721), op 14, value 4

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 34
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 13, variable 410, subtype 0, value 1
- Set/add variable: variable group 13, variable 411, subtype 0, value 1

## Waypoints

### Waypoint 0

- Tag: `210`
- Members: `Generic_Light_Freighter (object 20, id 6784, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (913.65, 0.00, -1410.64) | None |
| 1 | (899.63, 0.00, -847.82) | on arrival action 1, param -1 |

### Waypoint 1

- Tag: `209`
- Members: `GalSpan_Poseidon (object 15, id 6592, starts at point -1)`, `GalSpan_Poseidon (object 16, id 6593, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-67.88, -534.55, 920.57) | None |
| 1 | (-419.62, -534.55, 800.31) | None |
| 2 | (-474.46, -534.55, 73.48) | None |
| 3 | (250.71, -534.55, -164.39) | None |
| 4 | (707.75, -534.55, 344.39) | on arrival redirect to Waypoint 1 (tag 209), point 0 |

### Waypoint 2

- Tag: `208`
- Members: `Star_Patrol_Enforcer (object 0, id 4856, starts at point 0)`, `Star_Patrol_Enforcer (object 1, id 4857, starts at point 0)`, `Star_Patrol_Enforcer (object 2, id 4858, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-204.38, -534.55, -1573.46) | None |
| 1 | (-320.16, -534.55, -747.51) | None |
| 2 | (-344.54, -534.55, -93.36) | None |
| 3 | (-253.13, -534.55, 256.84) | None |

### Waypoint 3

- Tag: `204`
- Members: `Star_Patrol_Enforcer (object 3, id 4859, starts at point 1)`, `Star_Patrol_Enforcer (object 4, id 4860, starts at point 1)`, `Star_Patrol_Enforcer (object 5, id 4861, starts at point 1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (47.66, -534.55, -1547.69) | None |
| 1 | (23.29, -534.55, -411.19) | None |
| 2 | (35.48, -534.55, 282.61) | None |

### Waypoint 4

- Tag: `206`
- Members: `GalSpan_Pegasus (object 12, id 6607, starts at point -1)`, `GalSpan_Pegasus (object 13, id 6608, starts at point -1)`, `GalSpan_Pegasus (object 14, id 6609, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (181.73, -534.55, 705.82) | None |
| 1 | (-190.00, -534.55, 699.22) | None |
| 2 | (-305.78, -534.55, 190.43) | None |
| 3 | (267.04, -534.55, 104.53) | None |
| 4 | (590.02, -534.55, 527.42) | on arrival redirect to Waypoint 4 (tag 206), point 0 |

### Waypoint 5

- Tag: `203`
- Members: `GalSpan_Poseidon (object 8, id 6193, starts at point 0)`, `GalSpan_Poseidon (object 9, id 6199, starts at point 0)`, `GalSpan_Poseidon (object 10, id 6732, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1657.40, -534.55, -880.16) | None |
| 1 | (-1029.73, -534.55, -186.36) | None |
| 2 | (-542.22, -534.55, 77.94) | None |
| 3 | (-395.97, -534.55, 474.39) | None |
| 4 | (-5.96, -534.55, 454.57) | None |
| 5 | (-200.97, -534.55, -159.93) | None |

### Waypoint 6

- Tag: `205`
- Members: `GalSpan_Poseidon (object 6, id 6202, starts at point 0)`, `GalSpan_Poseidon (object 7, id 6203, starts at point 0)`, `GalSpan_Poseidon (object 11, id 6734, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1609.89, -534.55, -514.76) | None |
| 1 | (1055.35, -534.55, 27.06) | None |
| 2 | (683.62, -534.55, 416.91) | None |
| 3 | (354.55, -534.55, 449.95) | None |
| 4 | (305.80, -534.55, 159.21) | None |
| 5 | (616.59, -534.55, -157.95) | None |

### Waypoint 7

- Tag: `207`
- Members: `Medical_Frigate (object 17, id 4721, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (204.89, -534.55, -1394.89) | None |
| 1 | (204.89, -534.55, -502.87) | None |
| 2 | (180.51, -534.55, 309.86) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 8

- Tag: `202`
- Members: `Bora_Hvy_Freighter (object 19, id 4729, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (515.67, -534.55, -1468.57) | None |
| 1 | (546.14, -534.55, -536.90) | None |
| 2 | (473.02, -534.55, 302.27) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 9

- Tag: `201`
- Members: `Bora_Hvy_Freighter (object 18, id 4738, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-99.81, -534.55, -1409.10) | None |
| 1 | (-142.47, -534.55, -517.07) | None |
| 2 | (-142.47, -534.55, 322.09) | on arrival activate current object (raw param -1 ignored) |

## Spawn Lists

### Spawn List 0

- ID: `192`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 1 | spawn list 234 | None |
| 1 | 0 | none | None |
| 2 | 5 | spawn list 198 | None |

### Spawn List 1

- ID: `198`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 2

- ID: `16`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Medical_Frigate (object 17, id 4721) | None |
| 1 | 6 | Bora_Hvy_Freighter (object 18, id 4738) | None |
| 2 | 6 | Bora_Hvy_Freighter (object 19, id 4729) | None |

### Spawn List 3

- ID: `235`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Bora_Hvy_Freighter (object 19, id 4729) | None |
| 1 | 6 | Medical_Frigate (object 17, id 4721) | None |
| 2 | 2 | Bora_Hvy_Freighter (object 18, id 4738) | None |

### Spawn List 4

- ID: `234`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Bora_Hvy_Freighter (object 18, id 4738) | None |
| 1 | 6 | Medical_Frigate (object 17, id 4721) | None |
| 2 | 2 | Bora_Hvy_Freighter (object 19, id 4729) | None |

### Spawn List 5

- ID: `141`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 1 | spawn list 234 | None |
| 1 | 5 | spawn list 235 | None |
| 2 | 1 | spawn list 16 | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Star_Patrol_Enforcer` | 4856 | Interactive | -142.17,-714.05,-1913.45 | 0,0,0 | group/role: FG_QUAKE / 0; alias: oside; waypoint: Waypoint 2 (tag 208, 4 point(s)), starting point 0, arrival event value 13631488 |
| 1 | `Star_Patrol_Enforcer` | 4857 | Interactive | -121.29,-714.05,-2006.83 | 0,0,0 | group/role: FG_QUAKE / 0; alias: oside_1; waypoint: Waypoint 2 (tag 208, 4 point(s)), starting point 0, arrival event value 13631488 |
| 2 | `Star_Patrol_Enforcer` | 4858 | Interactive | -175.26,-714.05,-1996.95 | 0,0,0 | group/role: FG_QUAKE / 0; alias: oside_2; waypoint: Waypoint 2 (tag 208, 4 point(s)), starting point 0, arrival event value 13631488 |
| 3 | `Star_Patrol_Enforcer` | 4859 | Interactive | 10.78,-555.80,-1951.59 | 0,0,0 | group/role: FG_SIROCCO / 0; alias: bagel; waypoint: Waypoint 3 (tag 204, 3 point(s)), starting point 1, arrival event value 13369345 |
| 4 | `Star_Patrol_Enforcer` | 4860 | Interactive | -20.85,-555.80,-2014.41 | 0,0,0 | group/role: FG_SIROCCO / 0; alias: bagel_1; waypoint: Waypoint 3 (tag 204, 3 point(s)), starting point 1, arrival event value 13369345 |
| 5 | `Star_Patrol_Enforcer` | 4861 | Interactive | 37.30,-555.80,-2018.11 | 0,0,0 | group/role: FG_SIROCCO / 0; alias: bagel_2; waypoint: Waypoint 3 (tag 204, 3 point(s)), starting point 1, arrival event value 13369345 |
| 6 | `GalSpan_Poseidon` | 6202 | Interactive | 1632.68,-561.16,-661.49 | 486,0,0 | group/role: FG_OCTANS / 0; waypoint: Waypoint 6 (tag 205, 6 point(s)), starting point 0, arrival event value 13434880 |
| 7 | `GalSpan_Poseidon` | 6203 | Interactive | 1730.01,-561.16,-654.67 | 466,0,0 | label: BFNE_02; group/role: FG_OCTANS / 0; waypoint: Waypoint 6 (tag 205, 6 point(s)), starting point 0, arrival event value 13434880 |
| 8 | `GalSpan_Poseidon` | 6193 | Interactive | -2024.70,-538.40,-934.85 | 127,0,0 | label: BFNE_02; group/role: FG_MENSA / 0; waypoint: Waypoint 5 (tag 203, 6 point(s)), starting point 0, arrival event value 13303808 |
| 9 | `GalSpan_Poseidon` | 6199 | Interactive | -2096.80,-538.40,-987.18 | 127,0,0 | group/role: FG_MENSA / 0; waypoint: Waypoint 5 (tag 203, 6 point(s)), starting point 0, arrival event value 13303808 |
| 10 | `GalSpan_Poseidon` | 6732 | Interactive | -2058.56,0.00,-1069.38 | 92,0,0 | group/role: FG_MENSA / 0; waypoint: Waypoint 5 (tag 203, 6 point(s)), starting point 0, arrival event value 13303808 |
| 11 | `GalSpan_Poseidon` | 6734 | Interactive | 1745.35,0.00,-583.59 | 448,0,0 | group/role: FG_OCTANS / 0; waypoint: Waypoint 6 (tag 205, 6 point(s)), starting point 0, arrival event value 13434880 |
| 12 | `GalSpan_Pegasus` | 6607 | Interactive | 215.53,-532.39,1010.36 | 306,0,0 | group/role: FG_PICTOR / 0; waypoint: Waypoint 4 (tag 206, 5 point(s)), starting point -1 |
| 13 | `GalSpan_Pegasus` | 6608 | Interactive | 214.65,-532.39,972.49 | 306,0,0 | group/role: FG_PICTOR / 0; waypoint: Waypoint 4 (tag 206, 5 point(s)), starting point -1 |
| 14 | `GalSpan_Pegasus` | 6609 | Interactive | 244.31,-532.39,972.49 | 306,0,0 | group/role: FG_PICTOR / 0; waypoint: Waypoint 4 (tag 206, 5 point(s)), starting point -1 |
| 15 | `GalSpan_Poseidon` | 6592 | Interactive | -52.32,-515.64,1167.92 | 255,0,0 | group/role: FG_ARES / 0; waypoint: Waypoint 1 (tag 209, 5 point(s)), starting point -1 |
| 16 | `GalSpan_Poseidon` | 6593 | Interactive | 14.72,-515.64,1161.10 | 255,0,0 | label: BFNE_02; group/role: FG_ARES / 0; waypoint: Waypoint 1 (tag 209, 5 point(s)), starting point -1 |
| 17 | `Medical_Frigate` | 4721 | Interactive | 214.19,-555.80,-2091.61 | 0,0,0 | alias: SHIP1_HYPER; secondary groups: CONT_002, DROMEDARY; waypoint: Waypoint 7 (tag 207, 3 point(s)), starting point 0, arrival event value 13565952 |
| 18 | `Bora_Hvy_Freighter` | 4738 | Interactive | -80.26,-555.80,-1788.88 | 0,0,0 | alias: SHIP2_HYPER; secondary groups: CONT_004, BOLD; waypoint: Waypoint 9 (tag 201, 3 point(s)), starting point 0, arrival event value 13172736 |
| 19 | `Bora_Hvy_Freighter` | 4729 | Interactive | 515.08,-555.80,-1788.08 | 0,0,0 | alias: SHIP3_HYPER; secondary groups: CONT_028, TRAVELER; waypoint: Waypoint 8 (tag 202, 3 point(s)), starting point 0, arrival event value 13238272 |
| 20 | `Generic_Light_Freighter` | 6784 | Interactive | 917.84,0.00,-1760.34 | 0,0,0 | alias: ohshit; secondary groups: CONT_030, FINDER; waypoint: Waypoint 0 (tag 210, 2 point(s)), starting point -1 |
