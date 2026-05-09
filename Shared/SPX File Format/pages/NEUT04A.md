# Tachyon: The Fringe NEUT04A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT04A.SPX` |
| Sector | `QUAD_04` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 3 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 11 |
| Events | 17 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Heavy_Freighter`, `1: Pirate_Mine_HvyLaser` |
| Scripts | `PLAYER.SCR`, `MERCH.SCR`, `DRAKE.SCR` |
| Scenes | None |
| Labels | `bfne_06`, `BFBE_03`, `MISHK`, `HESPE`, `Merch` |
| Aliases | `Courage`, `kwI03_02`, `kwI03_03`, `kwi03_7`, `Jerome24`, `Jerome25`, `Jerome26`, `Jerome22`, `Jerome21`, `Jerome20`, `Intrepid`, `Artemis`, `KWi03_10`, `Hermes` |
| Groups | `FG_DORADO`, `CONT_045`, `CONT_046`, `GAUSS`, `CONT_028` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 2

**Action**

- Play scene: unknown index 0, param 0

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 3

**Action**

- Play dialog: PLAYER.SCR, line/variant 20
- Set runtime trigger variable: variable group 20, variable 0, subtype 1, value 0

### Event 3

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 20

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 5

**Action**

- Play dialog: PLAYER.SCR, line/variant 21
- Set runtime trigger variable: variable group 20, variable 0, subtype 1, value 0

### Event 5

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 21 (join 1)
- Object event: subject Pirate_Mine_HvyLaser (object 0, id 721), op 2, value 0 (flags 1)

**Action**

- Show/update HUD contact: contact/list 0, subtype 1, param 166

### Event 6

**Trigger**

- Group/spawn-list event: subject 166, op 1, value 10
- Variable comparison: subject variable group 21, variable 31, op 1, value 0

**Action**

- Play dialog: MERCH.SCR, line/variant 3

### Event 7

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 3
- Variable comparison: subject variable group 21, variable 31, op 1, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 18
- Hide/remove HUD contact: contact/list 0, subtype 1, param 166

### Event 8

**Trigger**

- Group/spawn-list event: subject 166, op 1, value 30
- Variable comparison: subject variable group 21, variable 31, op 1, value 0

**Action**

- Play dialog: MERCH.SCR, line/variant 4

### Event 9

**Trigger**

- Object event: subject Pirate_Mine_HvyLaser (object 0, id 721), op 10, value 0 (flags 1)
- Sector/startup condition family: subject 1, op 0, value 3

**Action**

- Play dialog: PLAYER.SCR, line/variant 24

### Event 10

**Trigger**

- Object event: subject Pirate_Mine_HvyLaser (object 0, id 721), op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0
- Hide/remove HUD contact: contact/list 0, subtype 1, param 166
- Hide/remove HUD contact: contact/list 0, subtype 9, param 18
- Set/add variable: variable group 21, variable 31, subtype 0, value 1

### Event 11

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 7

**Action**

- Play dialog: DRAKE.SCR, line/variant 4
- Hide/remove HUD contact: contact/list 0, subtype 9, param 18
- Show/update HUD contact: contact/list 0, subtype 9, param 20
- Object spawn/action: id 1552, subtype 14

### Event 12

**Trigger**

- Object event: subject Pirate_Mine_HvyLaser (object 0, id 721), op 2, value 0

**Action**

- Group/spawn-list action: spawn list/group 166, subtype 6
- Group/spawn-list action: spawn list/group 166, subtype 4, param 4

### Event 13

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1552; flags 2)

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 18

### Event 14

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 6, value 1 (extra 1, 1552; flags 2)

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 20
- Set/add variable: variable group 8, variable 2, subtype 0, value 1
- Mission objective/state: param 65541, subtype 0, param 0
- Play dialog: DRAKE.SCR, line/variant 6
- Object spawn/action: id 1552, subtype 15

### Event 15

**Trigger**

- Sector/startup condition family: subject 2, op 0, value 4

**Action**

- Object spawn/action: Generic_Heavy_Freighter (object 10, id 713), subtype 13, param 65541
- Set runtime trigger variable: variable group 20, variable 0, subtype 1, value 0

### Event 16

**Trigger**

- Object event: subject Generic_Heavy_Freighter (object 10, id 713), op 0, value 0 (flags 3)
- Sector/startup condition family: subject 2, op 0, value 4

**Action**

- Object spawn/action: Generic_Heavy_Freighter (object 10, id 713), subtype 4

## Waypoints

### Waypoint 0

- Tag: `1`
- Members: `Generic_Heavy_Freighter (object 10, id 713, starts at point 6)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1101.19, 436.08, 1011.61) | None |
| 1 | (1398.05, 436.08, 1057.05) | None |
| 2 | (-1181.26, 436.08, 883.81) | None |
| 3 | (-1219.77, 436.08, -896.57) | None |
| 4 | (-1232.56, 436.08, 395.40) | on arrival redirect to Waypoint 0 (tag 1), point 0 |
| 5 | (-2118.00, 436.08, 2516.50) | on arrival action 1, param -1 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Pirate_Mine_HvyLaser` | 721 | Interactive | 28.98,667.51,238.41 | 284,0,0 | group/role: FG_DORADO / 0; secondary groups: CONT_045, none |
| 1 | `Pirate_Mine_HvyLaser` | 722 | Interactive | 638.22,666.20,-130.33 | 320,0,0 | group/role: FG_DORADO / 0; secondary groups: CONT_046, none |
| 2 | `Pirate_Mine_HvyLaser` | 725 | Interactive | -916.97,-132.78,-789.23 | 128,0,0 | group/role: FG_DORADO / 0; secondary groups: CONT_046, none |
| 3 | `Pirate_Mine_HvyLaser` | 726 | Interactive | 905.54,104.74,-764.96 | 384,0,0 | group/role: FG_DORADO / 0; secondary groups: CONT_046, none |
| 4 | `Pirate_Mine_HvyLaser` | 727 | Interactive | -411.24,629.76,-13.34 | 228,0,0 | group/role: FG_DORADO / 0; secondary groups: CONT_046, none |
| 5 | `Pirate_Mine_HvyLaser` | 728 | Interactive | -246.50,892.86,-315.30 | 0,0,0 | group/role: FG_DORADO / 0; secondary groups: CONT_046, none |
| 6 | `Pirate_Mine_HvyLaser` | 967 | Interactive | 947.27,-97.66,152.74 | 384,0,0 | group/role: FG_DORADO / 0; secondary groups: CONT_046, none |
| 7 | `Pirate_Mine_HvyLaser` | 969 | Interactive | 376.98,732.28,-381.77 | 0,0,0 | group/role: FG_DORADO / 0; secondary groups: CONT_046, none |
| 8 | `Pirate_Mine_HvyLaser` | 970 | Interactive | -834.67,757.07,215.31 | 0,0,0 | group/role: FG_DORADO / 0; secondary groups: CONT_046, none |
| 9 | `Pirate_Mine_HvyLaser` | 971 | Interactive | -1068.32,164.41,-184.94 | 128,0,0 | group/role: FG_DORADO / 0; secondary groups: CONT_046, none |
| 10 | `Generic_Heavy_Freighter` | 713 | Interactive | -1435.60,436.08,-2361.91 | 7,0,0 | label: Merch; group/role: none / 1; secondary groups: CONT_028, GAUSS; waypoint: Waypoint 0 (tag 1, 6 point(s)), starting point 6 |
