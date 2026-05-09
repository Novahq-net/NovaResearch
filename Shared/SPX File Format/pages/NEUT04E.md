# Tachyon: The Fringe NEUT04E.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT04E.SPX` |
| Sector | `QUAD_04` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 3 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 6 |
| Events | 14 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Lt_Freighter`, `1: Wingman_Mishka`, `2: Red_Pirate_Shrike` |
| Scripts | `PLAYER.SCR`, `HESPE.SCR` |
| Scenes | None |
| Labels | `bfne_06`, `BFBE_03`, `MISHK`, `HESPE`, `Merch` |
| Aliases | `Courage`, `kwI03_02`, `kwI03_03`, `kwi03_7`, `Jerome24`, `Jerome25`, `Jerome26`, `Jerome22`, `Jerome21`, `Jerome20`, `Intrepid`, `Artemis`, `KWi03_10`, `Hermes` |
| Groups | `FG_SCORN`, `FG_DISDAIN`, `MISHKA_DWEATHERS`, `HESPERIDES`, `CONT_044` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 13, variable 412, op 1, value 1
- Variable comparison: subject variable group 13, variable 413, op 1, value 2

**Action**

- Group/spawn-list action: spawn list/group 167, subtype 0
- Group/spawn-list action: spawn list/group 168, subtype 0
- Object spawn/action: Wingman_Mishka (object 4, id 1617), subtype 0
- Set runtime trigger variable: variable group 20, variable 16, subtype 0, value 0

### Event 1

**Trigger**

- Group/spawn-list event: subject 167, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 168, op 4, value 0 (join 2; flags 2)

**Action**

- Group/spawn-list action: spawn list/group 167, subtype 4, param 9
- Group/spawn-list action: spawn list/group 168, subtype 4, param 9
- Set/add variable: variable group 21, variable 32, subtype 0, value 1
- Object spawn/action: Wingman_Mishka (object 4, id 1617), subtype 14

### Event 2

**Trigger**

- Group/spawn-list event: subject 167, op 0, value 0
- Group/spawn-list event: subject 168, op 0, value 0
- Variable comparison: subject variable group 21, variable 22, op 1, value 0
- Variable comparison: subject variable group 21, variable 32, op 1, value 1
- Variable comparison: subject variable group 21, variable 26, op 1, value 0

**Action**

- Object spawn/action: Wingman_Mishka (object 4, id 1617), subtype 13, param 21299200
- Set/add variable: variable group 21, variable 21, subtype 1, value 1
- Play dialog: PLAYER.SCR, line/variant 86
- Set/add variable: variable group 13, variable 801, subtype 0, value 1
- Set/add variable: variable group 13, variable 413, subtype 0, value 3
- Object spawn/action: Wingman_Mishka (object 4, id 1617), subtype 15

### Event 3

**Trigger**

- Object arrival: Wingman_Mishka (object 4, id 1617) reached Waypoint 1 (tag 325), point 1 (raw value 21299201)

**Action**

- Object spawn/action: Wingman_Mishka (object 4, id 1617), subtype 2, param 8

### Event 4

**Trigger**

- Object event: subject Wingman_Mishka (object 4, id 1617), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 22, subtype 0, value 1
- Set/add variable: variable group 13, variable 801, subtype 0, value 0
- Play dialog: PLAYER.SCR, line/variant 88
- Object spawn/action: Wingman_Mishka (object 4, id 1617), subtype 15

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 16, subtype 0, value 0

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 16, op 1, value 2

**Action**

- Object spawn/action: GalSpan_Lt_Freighter (object 5, id 1683), subtype 3
- Set runtime trigger variable: variable group 20, variable 16, subtype 1, value 0
- Show/update HUD contact: contact/list 0, subtype 6, param 1683
- Object spawn/action: GalSpan_Lt_Freighter (object 5, id 1683), subtype 14

### Event 7

**Trigger**

- Object arrival: GalSpan_Lt_Freighter (object 5, id 1683) reached Waypoint 0 (tag 326), point 0 (raw value 21364736)

**Action**

- Play dialog: HESPE.SCR, line/variant 1

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 16, op 1, value 5

**Action**

- Play dialog: PLAYER.SCR, line/variant 82
- Set runtime trigger variable: variable group 20, variable 16, subtype 1, value 0

### Event 9

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 23, subtype 0, value 1

### Event 10

**Trigger**

- Object event: subject GalSpan_Lt_Freighter (object 5, id 1683), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: GalSpan_Lt_Freighter (object 5, id 1683), subtype 4

### Event 11

**Trigger**

- Object event: subject Wingman_Mishka (object 4, id 1617), op 2, value 0 (flags 1)
- Variable comparison: subject variable group 13, variable 413, op 0, value 3

**Action**

- Set/add variable: variable group 13, variable 413, subtype 0, value 2
- Set/add variable: variable group 13, variable 801, subtype 0, value 0

### Event 12

**Trigger**

- Object event: subject GalSpan_Lt_Freighter (object 5, id 1683), op 8, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 6, param 1683
- Object spawn/action: GalSpan_Lt_Freighter (object 5, id 1683), subtype 15
- Mission objective/state: param 65543, subtype 0, param 0

### Event 13

**Trigger**

- Object event: subject GalSpan_Lt_Freighter (object 5, id 1683), op 14, value 27

**Action**

- Set/add variable: variable group 13, variable 412, subtype 0, value 1
- Set/add variable: variable group 13, variable 413, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 34

## Waypoints

### Waypoint 0

- Tag: `326`
- Members: `GalSpan_Lt_Freighter (object 5, id 1683, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (820.52, 264.65, -1486.12) | None; listened by Event 7 for GalSpan_Lt_Freighter (object 5, id 1683) |
| 1 | (825.23, 264.65, -1331.59) | on arrival action 1, param -1 |

### Waypoint 1

- Tag: `325`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1118.17, 253.88, -589.86) | None |
| 1 | (-183.31, 28.26, -2252.87) | None; listened by Event 3 for Wingman_Mishka (object 4, id 1617) |

## Spawn Lists

### Spawn List 0

- ID: `168`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Wingman_Mishka (object 4, id 1617) | None |

### Spawn List 1

- ID: `167`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Wingman_Mishka (object 4, id 1617) | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Red_Pirate_Shrike` | 1636 | Interactive | -65.85,129.20,1018.24 | 0,178,36 | group/role: FG_SCORN / 1 |
| 1 | `Red_Pirate_Shrike` | 1637 | Interactive | -467.07,-287.43,1704.60 | 0,185,107 | group/role: FG_SCORN / 2 |
| 2 | `Red_Pirate_Shrike` | 1639 | Interactive | 0.00,-690.77,1133.09 | 505,142,156 | group/role: FG_DISDAIN / 1; alias: kwI03_02 |
| 3 | `Red_Pirate_Shrike` | 1640 | Interactive | 505.79,-411.31,1876.68 | 7,149,370 | group/role: FG_DISDAIN / 2; alias: kwI03_03 |
| 4 | `Wingman_Mishka` | 1617 | Interactive | 52.34,646.54,892.58 | 0,164,135 | label: MISHK; alias: kwi03_7; secondary groups: none, MISHKA_DWEATHERS |
| 5 | `GalSpan_Lt_Freighter` | 1683 | Interactive | 820.47,253.24,-1600.97 | 0,0,0 | label: HESPE; alias: KWi03_10; secondary groups: CONT_044, HESPERIDES; waypoint: Waypoint 0 (tag 326, 2 point(s)), starting point 0, arrival event value 21364736 |
