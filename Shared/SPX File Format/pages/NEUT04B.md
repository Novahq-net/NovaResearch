# Tachyon: The Fringe NEUT04B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT04B.SPX` |
| Sector | `QUAD_04` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 3 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 13 |
| Events | 17 |
| Waypoints | 4 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Light_Freighter`, `1: Leoff_Coward_Indestructable`, `2: Independent_Merc_Piranha` |
| Scripts | `CLEON.SCR`, `MAGEL.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `bfne_06`, `BFBE_03`, `MISHK`, `HESPE`, `Merch` |
| Aliases | `Courage`, `kwI03_02`, `kwI03_03`, `kwi03_7`, `Jerome24`, `Jerome25`, `Jerome26`, `Jerome22`, `Jerome21`, `Jerome20`, `Intrepid`, `Artemis`, `KWi03_10`, `Hermes` |
| Groups | `FG_JADE`, `FG_AMBER`, `LEON`, `FG_MAGELLAN` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 135, subtype 2
- Object spawn/action: Generic_Light_Freighter (object 7, id 1221), subtype 3
- Object spawn/action: Generic_Light_Freighter (object 8, id 1222), subtype 3
- Object spawn/action: Generic_Light_Freighter (object 9, id 1223), subtype 3
- Group/spawn-list action: spawn list/group 147, subtype 2
- Object spawn/action: Generic_Light_Freighter (object 10, id 1225), subtype 3
- Object spawn/action: Generic_Light_Freighter (object 11, id 1226), subtype 3
- Object spawn/action: Generic_Light_Freighter (object 12, id 1227), subtype 3

### Event 1

**Trigger**

- Group/spawn-list event: subject 181, op 3, value 0

**Action**

- Object spawn/action: Generic_Light_Freighter (object 7, id 1221), subtype 14
- Show/update HUD contact: contact/list 0, subtype 7, param 181

### Event 2

**Trigger**

- Group/spawn-list event: subject 147, op 2, value 10027009 (Waypoint 1 (tag 153), point 1) (join 2)
- Group/spawn-list event: subject 135, op 2, value 10092545 (Waypoint 0 (tag 154), point 1) (join 2)

**Action**

- Play dialog: CLEON.SCR, line/variant 0
- Object spawn/action: Leoff_Coward_Indestructable (object 6, id 1771), subtype 8, param 9
- Group/spawn-list action: spawn list/group 135, subtype 4, param 9
- Group/spawn-list action: spawn list/group 147, subtype 4, param 9

### Event 3

**Trigger**

- Group/spawn-list event: subject 181, op 4, value 0 (extra 5, 135; join 2; flags 2)
- Group/spawn-list event: subject 181, op 4, value 0 (extra 5, 147; join 2; flags 2)

**Action**

- Show/update HUD contact: contact/list 0, subtype 3, param 181
- Hide/remove HUD contact: contact/list 0, subtype 7, param 181
- Play dialog: MAGEL.SCR, line/variant 1

### Event 4

**Trigger**

- Group/spawn-list event: subject 181, op 1, value 40

**Action**

- Set/add variable: variable group 13, variable 417, subtype 0, value 1
- Play dialog: PLAYER.SCR, line/variant 97
- Set/add variable: variable group 13, variable 416, subtype 0, value 1
- Mark/flash contact: contact/list 0, subtype 3, param 181
- Show/update HUD contact: contact/list 0, subtype 11, param 34
- Set/add variable: variable group 21, variable 18, subtype 0, value 1

### Event 5

**Trigger**

- Object event: subject Independent_Merc_Piranha (object 0, id 1246), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 19, subtype 1, value 1

### Event 6

**Trigger**

- Object event: subject Independent_Merc_Piranha (object 1, id 1247), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 19, subtype 1, value 1

### Event 7

**Trigger**

- Object event: subject Independent_Merc_Piranha (object 2, id 1248), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 19, subtype 1, value 1

### Event 8

**Trigger**

- Object event: subject Independent_Merc_Piranha (object 4, id 1553), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 19, subtype 1, value 1

### Event 9

**Trigger**

- Object event: subject Independent_Merc_Piranha (object 3, id 1575), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 19, subtype 1, value 1

### Event 10

**Trigger**

- Object event: subject 1748, op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 19, subtype 1, value 1

### Event 11

**Trigger**

- Object event: subject Independent_Merc_Piranha (object 5, id 1770), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 19, subtype 1, value 1

### Event 12

**Trigger**

- Variable comparison: subject variable group 21, variable 19, op 1, value 1 (join 2)
- Object event: subject Leoff_Coward_Indestructable (object 6, id 1771), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Leoff_Coward_Indestructable (object 6, id 1771), subtype 2, param 8
- Play dialog: CLEON.SCR, line/variant 1

### Event 13

**Trigger**

- Object event: subject Generic_Light_Freighter (object 7, id 1221), op 8, value 0 (join 2)
- Object event: subject Generic_Light_Freighter (object 8, id 1222), op 8, value 0 (join 2)
- Object event: subject Generic_Light_Freighter (object 9, id 1223), op 8, value 0 (join 2)
- Object event: subject Generic_Light_Freighter (object 10, id 1225), op 8, value 0 (join 2)
- Object event: subject Generic_Light_Freighter (object 11, id 1226), op 8, value 0 (join 2)
- Object event: subject Generic_Light_Freighter (object 12, id 1227), op 8, value 0 (join 2)

**Action**

- Set/add variable: variable group 21, variable 20, subtype 0, value 2
- Hide/remove HUD contact: contact/list 0, subtype 3, param 181
- Mission objective/state: param 65543, subtype 0, param 0

### Event 14

**Trigger**

- Group/spawn-list event: subject 181, op 2, value 9895939 (Waypoint 3 (tag 151), point 3)

**Action**

- Play dialog: MAGEL.SCR, line/variant 2

### Event 15

**Trigger**

- Object event: subject Generic_Light_Freighter (object 9, id 1223), op 2, value 0

**Action**

- Play dialog: MAGEL.SCR, line/variant 3

### Event 16

**Trigger**

- None

**Action**

- None

## Waypoints

### Waypoint 0

- Tag: `154`
- Members: `Independent_Merc_Piranha (object 3, id 1575, starts at point 0)`, `Independent_Merc_Piranha (object 4, id 1553, starts at point 0)`, `Independent_Merc_Piranha (object 5, id 1770, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (520.83, -191.39, 924.00) | None |
| 1 | (-53.64, -341.81, -287.65) | None |
| 2 | (-615.76, 96.97, -1578.43) | None |

### Waypoint 1

- Tag: `153`
- Members: `Independent_Merc_Piranha (object 0, id 1246, starts at point 0)`, `Independent_Merc_Piranha (object 1, id 1247, starts at point 0)`, `Independent_Merc_Piranha (object 2, id 1248, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (321.90, -191.39, 281.20) | None |
| 1 | (-7.06, -341.81, -479.55) | None |
| 2 | (-630.84, 96.97, -1668.30) | None |

### Waypoint 2

- Tag: `152`
- Members: `Generic_Light_Freighter (object 10, id 1225, starts at point 0)`, `Generic_Light_Freighter (object 11, id 1226, starts at point 0)`, `Generic_Light_Freighter (object 12, id 1227, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-877.98, 103.21, -1758.50) | None |
| 1 | (-1747.24, 243.27, -784.80) | None |
| 2 | (-1494.49, 368.60, 520.85) | None |
| 3 | (-451.34, 479.17, 1327.37) | None |
| 4 | (-174.10, 497.77, 1872.01) | on arrival action 1, param -1 |

### Waypoint 3

- Tag: `151`
- Members: `Generic_Light_Freighter (object 7, id 1221, starts at point 0)`, `Generic_Light_Freighter (object 8, id 1222, starts at point 0)`, `Generic_Light_Freighter (object 9, id 1223, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-724.59, 103.21, -1764.91) | None |
| 1 | (-1609.90, 243.27, -784.63) | None |
| 2 | (-1359.09, 368.60, 520.85) | None |
| 3 | (-323.91, 479.17, 1318.73) | None |
| 4 | (-69.72, 497.77, 1873.08) | on arrival action 1, param -1 |

## Spawn Lists

### Spawn List 0

- ID: `147`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 9 | none | None |
| 1 | 2 | Generic_Light_Freighter (object 9, id 1223) | None |
| 2 | 2 | Generic_Light_Freighter (object 10, id 1225) | None |

### Spawn List 1

- ID: `135`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 9 | none | None |
| 1 | 2 | Generic_Light_Freighter (object 9, id 1223) | None |
| 2 | 2 | Generic_Light_Freighter (object 10, id 1225) | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Independent_Merc_Piranha` | 1246 | Interactive | 412.56,-191.39,425.19 | 311,0,0 | label: bfne_06; group/role: FG_JADE / 1; waypoint: Waypoint 1 (tag 153, 3 point(s)), starting point 0, arrival event value 10027008 |
| 1 | `Independent_Merc_Piranha` | 1247 | Interactive | 483.40,-191.39,497.99 | 311,0,0 | group/role: FG_JADE / 2; waypoint: Waypoint 1 (tag 153, 3 point(s)), starting point 0, arrival event value 10027008 |
| 2 | `Independent_Merc_Piranha` | 1248 | Interactive | 544.28,-191.39,574.79 | 311,0,0 | group/role: FG_JADE / 3; waypoint: Waypoint 1 (tag 153, 3 point(s)), starting point 0, arrival event value 10027008 |
| 3 | `Independent_Merc_Piranha` | 1575 | Interactive | 655.19,-191.39,1140.66 | 303,0,0 | group/role: FG_AMBER / 3; waypoint: Waypoint 0 (tag 154, 3 point(s)), starting point 0, arrival event value 10092544 |
| 4 | `Independent_Merc_Piranha` | 1553 | Interactive | 718.49,-191.40,1207.75 | 304,0,0 | label: bfne_06; group/role: FG_AMBER / 1; waypoint: Waypoint 0 (tag 154, 3 point(s)), starting point 0, arrival event value 10092544 |
| 5 | `Independent_Merc_Piranha` | 1770 | Interactive | 759.56,-191.40,1272.44 | 304,0,0 | group/role: FG_AMBER / 1; waypoint: Waypoint 0 (tag 154, 3 point(s)), starting point 0, arrival event value 10092544 |
| 6 | `Leoff_Coward_Indestructable` | 1771 | Interactive | 1527.99,0.00,372.41 | 286,0,0 | secondary groups: none, LEON |
| 7 | `Generic_Light_Freighter` | 1221 | Interactive | 211.56,35.46,-2049.17 | 401,0,0 | group/role: FG_MAGELLAN / 0; alias: Jerome24; waypoint: Waypoint 3 (tag 151, 5 point(s)), starting point 0, arrival event value 9895936 |
| 8 | `Generic_Light_Freighter` | 1222 | Interactive | 343.35,35.46,-2175.53 | 401,0,0 | group/role: FG_MAGELLAN / 0; alias: Jerome25; waypoint: Waypoint 3 (tag 151, 5 point(s)), starting point 0, arrival event value 9895936 |
| 9 | `Generic_Light_Freighter` | 1223 | Interactive | 554.43,35.46,-2170.68 | 401,0,0 | group/role: FG_MAGELLAN / 0; alias: Jerome26; waypoint: Waypoint 3 (tag 151, 5 point(s)), starting point 0, arrival event value 9895936 |
| 10 | `Generic_Light_Freighter` | 1225 | Interactive | 448.94,35.46,-2292.34 | 401,0,0 | group/role: FG_MAGELLAN / 0; alias: Jerome22; waypoint: Waypoint 2 (tag 152, 5 point(s)), starting point 0, arrival event value 9961472 |
| 11 | `Generic_Light_Freighter` | 1226 | Interactive | 237.94,35.46,-2311.27 | 401,0,0 | group/role: FG_MAGELLAN / 0; alias: Jerome21; waypoint: Waypoint 2 (tag 152, 5 point(s)), starting point 0, arrival event value 9961472 |
| 12 | `Generic_Light_Freighter` | 1227 | Interactive | 118.67,35.46,-2169.81 | 401,0,0 | group/role: FG_MAGELLAN / 0; alias: Jerome20; waypoint: Waypoint 2 (tag 152, 5 point(s)), starting point 0, arrival event value 9961472 |
