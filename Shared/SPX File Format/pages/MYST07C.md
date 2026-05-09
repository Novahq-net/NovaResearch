# Tachyon: The Fringe MYST07C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST07C.SPX` |
| Sector | `QUAD_07` |
| Backdrop | `(none)` |
| Region | 5 |
| Sector ID | 6 |
| SectorHazardFlags | Twilight fog / fog-radar impairment (0x00000002) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 8 |
| Events | 33 |
| Waypoints | 0 |
| Child Sectors | 0 |
| Scripts | 4 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Demon_Pirate_Fighter` |
| Scripts | `DRCAS.SCR`, `B41DPB.SCR`, `B41DP.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `pisce`, `minotaur`, `cerbs`, `hydras`, `MPP1` |
| Aliases | `PISCES1`, `PISCES2`, `PISCES3`, `PISCES4`, `stocks02` |
| Groups | `FG_LURKER`, `FG_SPECTER`, `FG_SHADE`, `FG_GHOST` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 8, variable 7, op 1, value 1

**Action**

- Play dialog: DRCAS.SCR, line/variant 7

### Event 1

**Trigger**

- Group/spawn-list event: subject 126, op 4, value 0 (join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1622; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1626; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1630; flags 2)

**Action**

- Group/spawn-list action: spawn list/group 126, subtype 7

### Event 2

**Trigger**

- Group/spawn-list event: subject 126, op 0, value 0
- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1622; join 2; flags 2)
- Group/spawn-list event: subject 126, op 0, value 0
- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1626; join 2; flags 2)
- Group/spawn-list event: subject 126, op 0, value 0
- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1630; flags 2)

**Action**

- Group/spawn-list action: spawn list/group 77, subtype 1, param 1630

### Event 3

**Trigger**

- Group/spawn-list event: subject 77, op 1, value 50
- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1622; join 2; flags 2)
- Group/spawn-list event: subject 77, op 1, value 50
- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1626; flags 2)

**Action**

- Group/spawn-list action: spawn list/group 78, subtype 1, param 1626
- Play dialog: B41DPB.SCR, line/variant 3

### Event 4

**Trigger**

- Group/spawn-list event: subject 78, op 0, value 0
- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1626; join 2; flags 2)
- Group/spawn-list event: subject 78, op 0, value 0
- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1630; flags 2)

**Action**

- Group/spawn-list action: spawn list/group 79, subtype 1, param 1622

### Event 5

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 7
- Variable comparison: subject variable group 8, variable 7, op 1, value 1

**Action**

- Play dialog: B41DP.SCR, line/variant 3

### Event 6

**Trigger**

- Group/spawn-list event: subject 77, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 78, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 79, op 4, value 0 (flags 2)

**Action**

- Play dialog: B41DP.SCR, line/variant 4

### Event 7

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 10500 (extra 4, 0; flags 2)

**Action**

- Play dialog: B41DP.SCR, line/variant 5

### Event 8

**Trigger**

- None

**Action**

- None

### Event 9

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 40

**Action**

- Play dialog: PLAYER.SCR, line/variant 25

### Event 10

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 7000 (extra 1, 770; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 7000 (extra 1, 894; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 7000 (extra 1, 893; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 7000 (extra 1, 900; flags 2)

**Action**

- Play dialog: B41DP.SCR, line/variant 6

### Event 11

**Trigger**

- Object event: subject 1537, op 0, value 0 (flags 2)

**Action**

- Play dialog: B41DPB.SCR, line/variant 2

### Event 12

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 0
- Variable comparison: subject variable group 8, variable 7, op 1, value 1
- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1622; flags 2)

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1
- Set/add variable: variable group 21, variable 30, subtype 1, value 1
- Object spawn/action: id 1622, subtype 15

### Event 13

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1626; flags 2)
- Variable comparison: subject variable group 21, variable 21, op 1, value 0
- Variable comparison: subject variable group 8, variable 7, op 1, value 1

**Action**

- Set/add variable: variable group 21, variable 21, subtype 1, value 1
- Set/add variable: variable group 21, variable 30, subtype 1, value 1
- Object spawn/action: id 1626, subtype 15

### Event 14

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1630; flags 2)
- Variable comparison: subject variable group 21, variable 22, op 1, value 0
- Variable comparison: subject variable group 8, variable 7, op 1, value 1

**Action**

- Set/add variable: variable group 21, variable 22, subtype 1, value 1
- Set/add variable: variable group 21, variable 30, subtype 1, value 1
- Object spawn/action: id 1630, subtype 15

### Event 15

**Trigger**

- Variable comparison: subject variable group 21, variable 30, op 1, value 3

**Action**

- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 17, variable 402, subtype 0, value 1
- Set/add variable: variable group 17, variable 403, subtype 0, value 2
- Play dialog: DRCAS.SCR, line/variant 5
- Show/update HUD contact: contact/list 0, subtype 12, param 28
- Set/add variable: variable group 38, variable 2, subtype 0, value 1

### Event 16

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 5

**Action**

- Play dialog: DRCAS.SCR, line/variant 6

### Event 17

**Trigger**

- Object event: subject 766, op 3, value 90 (join 2)
- Object event: subject Demon_Pirate_Fighter (object 0, id 770), op 3, value 90 (join 2)
- Object event: subject Demon_Pirate_Fighter (object 5, id 894), op 3, value 90

**Action**

- Play dialog: B41DPB.SCR, line/variant 5

### Event 18

**Trigger**

- Object event: subject 767, op 4, value 100 (join 2)
- Object event: subject Demon_Pirate_Fighter (object 4, id 893), op 6, value 0 (join 2)
- Object event: subject Demon_Pirate_Fighter (object 3, id 890), op 4, value 20

**Action**

- Play dialog: B41DPB.SCR, line/variant 4

### Event 19

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 50

**Action**

- Play dialog: PLAYER.SCR, line/variant 34

### Event 20

**Trigger**

- Group/spawn-list event: subject 78, op 3, value 0
- Group/spawn-list event: subject 79, op 3, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 33

### Event 21

**Trigger**

- Group/spawn-list event: subject 77, op 3, value 0
- Group/spawn-list event: subject 78, op 3, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 32

### Event 22

**Trigger**

- Object event: subject 766, op 3, value 10 (join 2)
- Object event: subject Demon_Pirate_Fighter (object 0, id 770), op 3, value 10 (join 2)
- Object event: subject Demon_Pirate_Fighter (object 5, id 894), op 3, value 10

**Action**

- Play dialog: B41DPB.SCR, line/variant 5

### Event 23

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1622; flags 2)

**Action**

- Play dialog: DRCAS.SCR, line/variant 8

### Event 24

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 1
- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1626; flags 2)

**Action**

- Play dialog: DRCAS.SCR, line/variant 8

### Event 25

**Trigger**

- Variable comparison: subject variable group 21, variable 22, op 1, value 1
- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1630; flags 2)

**Action**

- Play dialog: DRCAS.SCR, line/variant 8

### Event 26

**Trigger**

- Variable comparison: subject variable group 21, variable 30, op 1, value 0
- Sector/startup condition family: subject 0, op 0, value 7

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 19
- Object spawn/action: id 1622, subtype 14
- Object spawn/action: id 1626, subtype 14
- Object spawn/action: id 1630, subtype 14

### Event 27

**Trigger**

- Variable comparison: subject variable group 21, variable 30, op 1, value 1

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 19
- Show/update HUD contact: contact/list 0, subtype 9, param 20

### Event 28

**Trigger**

- Variable comparison: subject variable group 21, variable 30, op 1, value 2

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 21
- Hide/remove HUD contact: contact/list 0, subtype 9, param 20

### Event 29

**Trigger**

- Variable comparison: subject variable group 21, variable 30, op 1, value 3

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 21

### Event 30

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Variable comparison: subject variable group 21, variable 30, op 1, value 1

**Action**

- Play dialog: DRCAS.SCR, line/variant 4

### Event 31

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 1
- Variable comparison: subject variable group 21, variable 30, op 1, value 1

**Action**

- Play dialog: DRCAS.SCR, line/variant 4

### Event 32

**Trigger**

- Variable comparison: subject variable group 21, variable 22, op 1, value 1
- Variable comparison: subject variable group 21, variable 30, op 1, value 1

**Action**

- Play dialog: DRCAS.SCR, line/variant 4

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Demon_Pirate_Fighter` | 770 | Interactive | -1262.26,637.77,434.08 | 189,0,128 | group/role: FG_LURKER / 2 |
| 1 | `Demon_Pirate_Fighter` | 771 | Interactive | -1172.22,637.77,364.59 | 183,0,135 | group/role: FG_LURKER / 4 |
| 2 | `Demon_Pirate_Fighter` | 889 | Interactive | 2594.88,0.00,-1149.52 | 0,0,0 | group/role: FG_SPECTER / 1 |
| 3 | `Demon_Pirate_Fighter` | 890 | Interactive | 2761.90,0.00,-1149.52 | 0,0,0 | group/role: FG_SPECTER / 2 |
| 4 | `Demon_Pirate_Fighter` | 893 | Interactive | 2548.30,0.00,-492.84 | 0,0,0 | group/role: FG_SHADE / 1 |
| 5 | `Demon_Pirate_Fighter` | 894 | Interactive | 2830.95,0.00,-506.77 | 0,0,0 | group/role: FG_SHADE / 2 |
| 6 | `Demon_Pirate_Fighter` | 899 | Interactive | 2651.53,0.00,-899.51 | 0,0,0 | group/role: FG_GHOST / 1 |
| 7 | `Demon_Pirate_Fighter` | 900 | Interactive | 2831.39,0.00,-885.58 | 0,0,0 | group/role: FG_GHOST / 2 |
