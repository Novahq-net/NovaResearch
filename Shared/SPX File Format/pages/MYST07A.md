# Tachyon: The Fringe MYST07A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST07A.SPX` |
| Sector | `QUAD_07` |
| Backdrop | `(none)` |
| Region | 5 |
| Sector ID | 6 |
| SectorHazardFlags | Twilight fog / fog-radar impairment (0x00000002) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 12 |
| Events | 14 |
| Waypoints | 0 |
| Child Sectors | 0 |
| Scripts | 4 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Demon_Pirate_Fighter` |
| Scripts | `PLAYER.SCR`, `B41DP.SCR`, `B41DPB.SCR`, `B41DPA.SCR` |
| Scenes | None |
| Labels | `pisce`, `minotaur`, `cerbs`, `hydras`, `MPP1` |
| Aliases | `PISCES1`, `PISCES2`, `PISCES3`, `PISCES4`, `stocks02` |
| Groups | `FG_SHADE`, `FG_GHOST`, `FG_PHANTOM`, `FG_SPECTER`, `FG_SPOOK`, `FG_LURKER` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 31, subtype 0, value 0
- Set/add variable: variable group 21, variable 20, subtype 1, value 1
- Group/spawn-list action: spawn list/group 79, subtype 1, param 1623

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 31, op 1, value 3

**Action**

- Play dialog: PLAYER.SCR, line/variant 8

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 31, op 1, value 15

**Action**

- Group/spawn-list action: spawn list/group 77, subtype 7
- Set runtime trigger variable: variable group 20, variable 31, subtype 1, value 0

### Event 3

**Trigger**

- Group/spawn-list event: subject 77, op 5, value 0

**Action**

- Play dialog: B41DP.SCR, line/variant 0

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 70

**Action**

- Play dialog: B41DP.SCR, line/variant 2

### Event 5

**Trigger**

- Object event: subject 1537, op 0, value 0 (flags 2)

**Action**

- Play dialog: B41DPB.SCR, line/variant 0

### Event 6

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 500 (extra 1, 2; flags 2)

**Action**

- Play dialog: B41DPB.SCR, line/variant 1

### Event 7

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 21, op 1, value 1
- Group/spawn-list event: subject 79, op 0, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 31, subtype 0, value 0
- Group/spawn-list action: spawn list/group 153, subtype 1, param 1626

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 31, op 1, value 17

**Action**

- Play dialog: B41DPA.SCR, line/variant 0

### Event 9

**Trigger**

- Sector/startup condition family: subject 3, op 0, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 15

### Event 10

**Trigger**

- Group/spawn-list event: subject 153, op 0, value 0

**Action**

- Group/spawn-list action: spawn list/group 78, subtype 1, param 1626

### Event 11

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 1
- Global enemy/object-count event: subject 0, op 1, value 80

**Action**

- Group/spawn-list action: spawn list/group 80, subtype 1, param 2

### Event 12

**Trigger**

- Group/spawn-list event: subject 80, op 0, value 0

**Action**

- Group/spawn-list action: spawn list/group 126, subtype 1, param 1623

### Event 13

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 1
- Area/player/sector/dock/time event: subject 0, op 0, value 70

**Action**

- Play dialog: PLAYER.SCR, line/variant 16

## Waypoints

None
## Spawn Lists

### Spawn List 0

- ID: `78`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Demon_Pirate_Fighter` | 902 | Interactive | -250.21,0.00,-2794.85 | 0,0,0 | group/role: FG_SHADE / 1 |
| 1 | `Demon_Pirate_Fighter` | 903 | Interactive | -66.57,0.00,-2794.85 | 0,0,0 | group/role: FG_SHADE / 2 |
| 2 | `Demon_Pirate_Fighter` | 906 | Interactive | 1341.77,125.41,-1786.31 | 0,0,0 | group/role: FG_GHOST / 1 |
| 3 | `Demon_Pirate_Fighter` | 907 | Interactive | 1413.15,125.41,-1755.63 | 0,0,0 | group/role: FG_GHOST / 2 |
| 4 | `Demon_Pirate_Fighter` | 908 | Interactive | 236.34,0.00,-2775.49 | 0,0,0 | group/role: FG_PHANTOM / 0 |
| 5 | `Demon_Pirate_Fighter` | 909 | Interactive | 472.45,0.00,-2775.49 | 0,0,0 | group/role: FG_PHANTOM / 0 |
| 6 | `Demon_Pirate_Fighter` | 1217 | Interactive | 813.38,0.00,-2773.86 | 0,0,0 | group/role: FG_SPECTER / 1 |
| 7 | `Demon_Pirate_Fighter` | 1218 | Interactive | 1021.64,0.00,-2779.00 | 0,0,0 | group/role: FG_SPECTER / 2 |
| 8 | `Demon_Pirate_Fighter` | 1221 | Interactive | 1371.89,0.00,-2778.99 | 0,0,0 | group/role: FG_SPOOK / 1 |
| 9 | `Demon_Pirate_Fighter` | 1223 | Interactive | 1556.48,0.00,-2789.26 | 0,0,0 | group/role: FG_SPOOK / 2 |
| 10 | `Demon_Pirate_Fighter` | 1225 | Interactive | 1883.07,0.00,-2789.26 | 0,0,0 | group/role: FG_LURKER / 1 |
| 11 | `Demon_Pirate_Fighter` | 1226 | Interactive | 2086.59,0.00,-2789.26 | 0,0,0 | group/role: FG_LURKER / 2 |
