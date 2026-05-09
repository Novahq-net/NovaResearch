# Tachyon: The Fringe FRON03B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON03B.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 5 |
| Entities | 16 |
| Events | 6 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Crate_6`, `1: Junk_10`, `2: Junk_05`, `3: Junk_04`, `4: Void_Pirate_Fighter` |
| Scripts | `VOIDR.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFGF_01` |
| Aliases | `Komodo1`, `Komodo2`, `Komodo3`, `Komodo4` |
| Groups | `FG_KOMODO`, `CONT_029` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 24, op 1, value 1

**Action**

- Set runtime trigger variable: variable group 20, variable 4, subtype 0, value 0
- Set/add variable: variable group 21, variable 26, subtype 0, value 1
- Set/add variable: variable group 21, variable 25, subtype 0, value 1

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 4, op 1, value 6

**Action**

- Play dialog: VOIDR.SCR, line/variant 0

### Event 2

**Trigger**

- Group/spawn-list event: subject 228, op 4, value 0 (flags 2)

**Action**

- Play dialog: VOIDR.SCR, line/variant 2

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 4, op 1, value 45

**Action**

- Group/spawn-list action: spawn list/group 228, subtype 3, param 1
- Group/spawn-list action: spawn list/group 229, subtype 3, param 1

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 25; flags 2)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 3500
- Play dialog: PLAYER.SCR, line/variant 145

### Event 5

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 0

**Action**

- None

## Waypoints

### Waypoint 0

- Tag: `151`
- Members: `Void_Pirate_Fighter (object 0, id 2, starts at point -1)`, `Void_Pirate_Fighter (object 1, id 3, starts at point -1)`, `Void_Pirate_Fighter (object 2, id 4, starts at point -1)`, `Void_Pirate_Fighter (object 3, id 5, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-601.01, 0.00, 1110.17) | None |
| 1 | (-592.26, 0.00, 22.18) | None |
| 2 | (1154.44, 0.00, 17.15) | None |
| 3 | (1579.68, 0.00, 1079.05) | None |
| 4 | (1207.65, 0.00, 1394.90) | on arrival redirect to Waypoint 0 (tag 151), point 0 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Void_Pirate_Fighter` | 2 | Interactive | -40.02,222.74,805.71 | 0,0,0 | group/role: FG_KOMODO / 0; alias: Komodo1; waypoint: Waypoint 0 (tag 151, 5 point(s)), starting point -1 |
| 1 | `Void_Pirate_Fighter` | 3 | Interactive | -4.51,222.74,805.71 | 0,0,0 | group/role: FG_KOMODO / 0; alias: Komodo2; waypoint: Waypoint 0 (tag 151, 5 point(s)), starting point -1 |
| 2 | `Void_Pirate_Fighter` | 4 | Interactive | 40.70,222.74,805.71 | 0,0,0 | group/role: FG_KOMODO / 0; alias: Komodo3; waypoint: Waypoint 0 (tag 151, 5 point(s)), starting point -1 |
| 3 | `Void_Pirate_Fighter` | 5 | Interactive | 76.23,222.74,805.71 | 0,0,0 | label: BFGF_01; group/role: FG_KOMODO / 0; alias: Komodo4; waypoint: Waypoint 0 (tag 151, 5 point(s)), starting point -1 |
| 4 | `Junk_04` | 9 | Object | 1166.50,40.66,1071.21 | 65,0,0 | Scale/Radius: 1.00 |
| 5 | `Junk_04` | 10 | Object | 1255.26,25.62,1054.83 | 0,0,441 | Scale/Radius: 1.00 |
| 6 | `Junk_05` | 11 | Object | 1295.89,58.18,1109.05 | 65,0,441 | Scale/Radius: 1.00 |
| 7 | `Junk_10` | 19 | Object | 1184.70,-26.36,1033.81 | 65,0,441 | Scale/Radius: 1.71 |
| 8 | `Crate_6` | 25 | Interactive | 1233.38,0.00,1008.79 | 0,0,0 | secondary groups: CONT_029, none |
| 9 | `Junk_10` | 18 | Object | 1221.97,93.31,1043.40 | 65,0,46 | Scale/Radius: 3.60 |
| 10 | `Junk_10` | 14 | Object | 1207.53,16.78,1087.09 | 388,0,441 | Scale/Radius: 1.00 |
| 11 | `Junk_04` | 16 | Object | 1254.21,-15.21,996.13 | 0,0,0 | Scale/Radius: 5.12 |
| 12 | `Junk_05` | 15 | Object | 1170.35,89.59,969.65 | 453,0,0 | Scale/Radius: 3.89 |
| 13 | `Junk_04` | 13 | Object | 1209.59,93.31,1102.11 | 65,0,441 | Scale/Radius: 1.00 |
| 14 | `Junk_05` | 12 | Object | 1252.96,25.62,1010.01 | 0,0,0 | Scale/Radius: 1.00 |
| 15 | `Junk_04` | 17 | Object | 1257.53,25.62,1088.23 | 388,0,0 | Scale/Radius: 1.77 |
