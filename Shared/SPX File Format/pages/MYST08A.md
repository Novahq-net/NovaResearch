# Tachyon: The Fringe MYST08A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST08A.SPX` |
| Sector | `QUAD_08` |
| Backdrop | `(none)` |
| Region | 5 |
| Sector ID | 7 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 4 |
| Events | 6 |
| Waypoints | 0 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Demon_Pirate_Fighter` |
| Scripts | `PLAYER.SCR`, `B41DP.SCR` |
| Scenes | None |
| Labels | `OPAL` |
| Aliases | `stocks02` |
| Groups | `FG_SHADE`, `FG_LURKER` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Play scene: unknown index 0, param 0
- Set/add variable: variable group 21, variable 21, subtype 1, value 1
- Show/update HUD contact: contact/list 0, subtype 9, param 14
- Play dialog: PLAYER.SCR, line/variant 11

### Event 1

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 11 (join 1)
- Area/player/sector/dock/time event: subject 0, op 1, value 300 (extra 1, 2118; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 12
- Set runtime trigger variable: variable group 20, variable 30, subtype 0, value 0

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 30, op 1, value 10

**Action**

- Group/spawn-list action: spawn list/group 78, subtype 1, param 1
- Play dialog: B41DP.SCR, line/variant 7
- Set runtime trigger variable: variable group 20, variable 30, subtype 1, value 0

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 150 (extra 1, 2118; flags 2)
- Sector/startup condition family: subject 0, op 0, value 12

**Action**

- Play dialog: PLAYER.SCR, line/variant 13
- Play scene: unknown index 0, param 1

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 100

**Action**

- Play dialog: PLAYER.SCR, line/variant 16

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 2118; flags 2)

**Action**

- Show/update HUD contact: contact/list 0, subtype 12, param 28
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 14
- Set/add variable: variable group 17, variable 400, subtype 0, value 1
- Set/add variable: variable group 17, variable 401, subtype 0, value 2
- Play dialog: PLAYER.SCR, line/variant 14
- Group/spawn-list action: spawn list/group 126, subtype 1, param 1

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Demon_Pirate_Fighter` | 4041 | Interactive | -1216.76,-238.84,-1134.11 | 0,0,0 | group/role: FG_SHADE / 1 |
| 1 | `Demon_Pirate_Fighter` | 4042 | Interactive | -1179.98,-238.84,-1134.11 | 0,0,0 | group/role: FG_SHADE / 2 |
| 2 | `Demon_Pirate_Fighter` | 4043 | Interactive | -1100.29,-238.84,-1147.40 | 0,0,0 | group/role: FG_LURKER / 1 |
| 3 | `Demon_Pirate_Fighter` | 4044 | Interactive | -1063.50,-238.84,-1147.40 | 0,0,0 | group/role: FG_LURKER / 2 |
