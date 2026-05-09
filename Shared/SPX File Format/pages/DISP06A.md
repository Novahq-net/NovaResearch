# Tachyon: The Fringe DISP06A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP06A.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 5 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 8 |
| Entities | 17 |
| Events | 49 |
| Waypoints | 4 |
| Child Sectors | 0 |
| Scripts | 5 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Battleaxe`, `1: Bora_Warhammer`, `2: Crate_7`, `3: Crate_6`, `4: Crate_5`, `5: Independent_Merc_Piranha`, `6: Independent_Merc_Gar`, `7: Bora_Mace` |
| Scripts | `CINDER.SCR`, `PLAYER.SCR`, `SPY3R.SCR`, `SPY2W.SCR`, `SPY1W.SCR` |
| Scenes | None |
| Labels | `obsidian`, `killer`, `BFGE_02`, `greyhound`, `quasar` |
| Aliases | `fake_2`, `fake_1`, `spy_1` |
| Groups | `FG_REVOLUTION`, `OBSIDIAN`, `FG_SHALE`, `FG_AMBER`, `FG_JADE`, `FG_BLOODSTONE`, `FG_GARNET`, `LAUREN`, `CONT_054`, `STARD`, `KILLIAN`, `FG_VALOR`, `GREYHOUND`, `FG_HONOR`, `QUASAR` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Object spawn/action: Bora_Warhammer (object 15, id 389), subtype 8, param 4
- Object spawn/action: Bora_Battleaxe (object 16, id 388), subtype 8, param 4
- Object spawn/action: Bora_Mace (object 0, id 387), subtype 8, param 4
- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0
- Broadcast hide/remove contact: contact/list 0, subtype 0, param 16
- Show/update HUD contact: contact/list 0, subtype 9, param 17
- Object spawn/action: id 405, subtype 8, param 4

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 5

**Action**

- Play dialog: CINDER.SCR, line/variant 0
- Set runtime trigger variable: variable group 20, variable 0, subtype 1, value 0
- Play scene: unknown index 0, param 0

### Event 2

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 10

**Action**

- Play dialog: PLAYER.SCR, line/variant 52
- Set runtime trigger variable: variable group 20, variable 0, subtype 1, value 0

### Event 4

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 52

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 20

**Action**

- Play dialog: PLAYER.SCR, line/variant 53
- Set runtime trigger variable: variable group 20, variable 0, subtype 1, value 0
- Set runtime trigger variable: variable group 20, variable 1, subtype 0, value 0

### Event 6

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 401; flags 2)

**Action**

- Object spawn/action: Bora_Warhammer (object 15, id 389), subtype 8, param 2
- Show/update HUD contact: contact/list 0, subtype 9, param 21
- Mission objective/state: param 393218, subtype 0, param 0
- Object spawn/action: Bora_Warhammer (object 15, id 389), subtype 2, param 1
- Play dialog: PLAYER.SCR, line/variant 215
- Hide/remove HUD contact: contact/list 0, subtype 9, param 17
- Set/add variable: variable group 21, variable 21, subtype 0, value 1

### Event 7

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 402; flags 2)

**Action**

- Object spawn/action: Bora_Battleaxe (object 16, id 388), subtype 8, param 2
- Object spawn/action: Bora_Battleaxe (object 16, id 388), subtype 2, param 1
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Play dialog: PLAYER.SCR, line/variant 216
- Hide/remove HUD contact: contact/list 0, subtype 9, param 17
- Set/add variable: variable group 21, variable 20, subtype 0, value 1

### Event 8

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 403; flags 2)

**Action**

- Object spawn/action: Bora_Mace (object 0, id 387), subtype 8, param 2
- Show/update HUD contact: contact/list 0, subtype 9, param 21
- Mission objective/state: param 393218, subtype 0, param 0
- Object spawn/action: Bora_Mace (object 0, id 387), subtype 2, param 1
- Play dialog: PLAYER.SCR, line/variant 214
- Hide/remove HUD contact: contact/list 0, subtype 9, param 17
- Set/add variable: variable group 21, variable 22, subtype 0, value 1

### Event 9

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 401; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 402; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 403; join 2; flags 2)

**Action**

- Group/spawn-list action: spawn list/group 130, subtype 2
- Group/spawn-list action: spawn list/group 128, subtype 2
- Group/spawn-list action: spawn list/group 127, subtype 2
- Object spawn/action: id 405, subtype 8, param 6
- Set/add variable: variable group 21, variable 28, subtype 0, value 1
- Object spawn/action: id 405, subtype 6

### Event 10

**Trigger**

- Variable comparison: subject variable group 21, variable 28, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 127, subtype 4, param 6
- Group/spawn-list action: spawn list/group 128, subtype 4, param 6
- Group/spawn-list action: spawn list/group 130, subtype 4, param 6
- Group/spawn-list action: spawn list/group 128, subtype 3, param 1

### Event 11

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1 (join 2)
- Variable comparison: subject variable group 21, variable 23, op 1, value 1 (join 2)
- Variable comparison: subject variable group 21, variable 32, op 1, value 1 (join 2)

**Action**

- Object spawn/action: Bora_Warhammer (object 15, id 389), subtype 5
- Object spawn/action: Bora_Mace (object 0, id 387), subtype 5
- Object spawn/action: Crate_5 (object 10, id 401), subtype 16
- Object spawn/action: Crate_7 (object 12, id 403), subtype 16

### Event 12

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 0, value 1 (join 2)
- Variable comparison: subject variable group 21, variable 23, op 0, value 1 (join 2)
- Variable comparison: subject variable group 21, variable 32, op 0, value 1 (join 2)

**Action**

- Object spawn/action: Bora_Mace (object 0, id 387), subtype 5
- Object spawn/action: Bora_Battleaxe (object 16, id 388), subtype 5
- Object spawn/action: Crate_6 (object 11, id 402), subtype 16
- Object spawn/action: Crate_7 (object 12, id 403), subtype 16

### Event 13

**Trigger**

- Variable comparison: subject variable group 21, variable 22, op 1, value 1 (join 2)
- Variable comparison: subject variable group 21, variable 23, op 1, value 1 (join 2)
- Variable comparison: subject variable group 21, variable 32, op 1, value 1 (join 2)

**Action**

- Object spawn/action: Bora_Battleaxe (object 16, id 388), subtype 5
- Object spawn/action: Bora_Warhammer (object 15, id 389), subtype 5
- Object spawn/action: Crate_5 (object 10, id 401), subtype 16
- Object spawn/action: Crate_6 (object 11, id 402), subtype 16

### Event 14

**Trigger**

- Object event: subject Bora_Warhammer (object 15, id 389), op 0, value 0 (join 2; flags 2)
- Object event: subject Bora_Battleaxe (object 16, id 388), op 0, value 0 (join 2; flags 2)
- Object event: subject Bora_Mace (object 0, id 387), op 0, value 0 (join 1; flags 2)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1 (join 1)
- Variable comparison: subject variable group 21, variable 21, op 1, value 1 (join 1)
- Variable comparison: subject variable group 21, variable 22, op 1, value 1 (join 1)

**Action**

- Object spawn/action: Crate_5 (object 10, id 401), subtype 16
- Object spawn/action: Crate_6 (object 11, id 402), subtype 16
- Object spawn/action: Crate_7 (object 12, id 403), subtype 16
- Object spawn/action: Bora_Warhammer (object 15, id 389), subtype 5
- Object spawn/action: Bora_Battleaxe (object 16, id 388), subtype 5
- Object spawn/action: Bora_Mace (object 0, id 387), subtype 5
- Set/add variable: variable group 21, variable 32, subtype 0, value 1

### Event 15

**Trigger**

- Group/spawn-list event: subject 135, op 4, value 0 (join 2; flags 2)
- Variable comparison: subject variable group 21, variable 32, op 1, value 1 (join 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1 (join 1)
- Variable comparison: subject variable group 21, variable 21, op 1, value 1 (join 1)
- Variable comparison: subject variable group 21, variable 22, op 1, value 1 (join 1)

**Action**

- Group/spawn-list action: spawn list/group 135, subtype 1, param 405
- Set/add variable: variable group 21, variable 23, subtype 0, value 1
- Broadcast hide/remove contact: contact/list 0, subtype 0, param 17
- Play dialog: CINDER.SCR, line/variant 1

### Event 16

**Trigger**

- Group/spawn-list event: subject 127, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 130, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 128, op 4, value 0 (join 2; flags 2)
- Variable comparison: subject variable group 21, variable 23, op 1, value 1 (join 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1 (join 1)
- Variable comparison: subject variable group 21, variable 21, op 1, value 1 (join 1)
- Variable comparison: subject variable group 21, variable 22, op 1, value 1 (join 1)

**Action**

- Group/spawn-list action: spawn list/group 127, subtype 2
- Group/spawn-list action: spawn list/group 128, subtype 2
- Group/spawn-list action: spawn list/group 130, subtype 2
- Group/spawn-list action: spawn list/group 127, subtype 4, param 9
- Group/spawn-list action: spawn list/group 128, subtype 4, param 9
- Group/spawn-list action: spawn list/group 130, subtype 4, param 9
- Set/add variable: variable group 21, variable 32, subtype 0, value 1
- Object spawn/action: id 405, subtype 8, param 9

### Event 17

**Trigger**

- Variable comparison: subject variable group 21, variable 32, op 1, value 1
- Group/spawn-list event: subject 135, op 0, value 0
- Group/spawn-list event: subject 128, op 0, value 0
- Group/spawn-list event: subject 127, op 0, value 0
- Group/spawn-list event: subject 130, op 0, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 0, value 1
- Object spawn/action: Bora_Battleaxe (object 16, id 388), subtype 2, param 1
- Hide/remove HUD contact: contact/list 0, subtype 2, param 388
- Hide/remove HUD contact: contact/list 0, subtype 2, param 389
- Hide/remove HUD contact: contact/list 0, subtype 2, param 387
- Show/update HUD contact: contact/list 0, subtype 9, param 21
- Object spawn/action: Bora_Warhammer (object 15, id 389), subtype 7
- Object spawn/action: Bora_Mace (object 0, id 387), subtype 7

### Event 18

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 24, op 1, value 1
- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Set/add variable: variable group 21, variable 20, subtype 0, value 1
- Set/add variable: variable group 21, variable 23, subtype 0, value 1
- Play dialog: PLAYER.SCR, line/variant 72
- Set runtime trigger variable: variable group 20, variable 16, subtype 0, value 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 21
- Show/update HUD contact: contact/list 0, subtype 9, param 22
- Hide/remove HUD contact: contact/list 0, subtype 11, param 0

### Event 19

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 24, op 1, value 1
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Set/add variable: variable group 21, variable 20, subtype 0, value 1
- Set/add variable: variable group 21, variable 23, subtype 0, value 1
- Play dialog: PLAYER.SCR, line/variant 72
- Set runtime trigger variable: variable group 20, variable 16, subtype 0, value 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 21
- Show/update HUD contact: contact/list 0, subtype 9, param 22
- Hide/remove HUD contact: contact/list 0, subtype 11, param 0

### Event 20

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 72

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 22
- Show/update HUD contact: contact/list 0, subtype 1, param 127
- Show/update HUD contact: contact/list 0, subtype 1, param 147
- Show/update HUD contact: contact/list 0, subtype 1, param 130
- Group/spawn-list action: spawn list/group 147, subtype 1, param 405
- Group/spawn-list action: spawn list/group 127, subtype 4, param 9
- Group/spawn-list action: spawn list/group 130, subtype 4, param 9
- Object spawn/action: id 405, subtype 8, param 9

### Event 21

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 24, op 1, value 1
- Variable comparison: subject variable group 21, variable 21, op 1, value 1
- Object event: subject Bora_Mace (object 0, id 387), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 29, subtype 0, value 1

### Event 22

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 24, op 1, value 1
- Variable comparison: subject variable group 21, variable 22, op 1, value 1
- Object event: subject Bora_Warhammer (object 15, id 389), op 2, value 0

**Action**

- Set/add variable: variable group 21, variable 29, subtype 0, value 1

### Event 23

**Trigger**

- Object event: subject Bora_Battleaxe (object 16, id 388), op 2, value 0
- Variable comparison: subject variable group 21, variable 23, op 1, value 1

**Action**

- Set/add variable: variable group 18, variable 408, subtype 0, value 1
- Set/add variable: variable group 18, variable 409, subtype 0, value 1
- Broadcast mark/flash contact: contact/list 0, subtype 0, param 15
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 25
- Hide/remove HUD contact: contact/list 0, subtype 2, param 388
- Hide/remove HUD contact: contact/list 0, subtype 2, param 387
- Hide/remove HUD contact: contact/list 0, subtype 2, param 389

### Event 24

**Trigger**

- Variable comparison: subject variable group 21, variable 24, op 1, value 1
- Variable comparison: subject variable group 21, variable 23, op 1, value 1
- Group/spawn-list event: subject 147, op 0, value 0
- Group/spawn-list event: subject 127, op 0, value 0
- Group/spawn-list event: subject 130, op 0, value 0 (join 1)
- Object event: subject Bora_Battleaxe (object 16, id 388), op 2, value 0 (join 1)

**Action**

- Object spawn/action: Bora_Battleaxe (object 16, id 388), subtype 2, param 1
- Play dialog: SPY3R.SCR, line/variant 6
- Broadcast HUD contact action: contact/list 0, subtype 0, param 15
- Object spawn/action: Bora_Battleaxe (object 16, id 388), subtype 14

### Event 25

**Trigger**

- Object event: subject Bora_Battleaxe (object 16, id 388), op 4, value 100

**Action**

- Play dialog: SPY3R.SCR, line/variant 10

### Event 26

**Trigger**

- Object event: subject Bora_Warhammer (object 15, id 389), op 4, value 80

**Action**

- Play dialog: SPY2W.SCR, line/variant 7

### Event 27

**Trigger**

- Object event: subject Bora_Mace (object 0, id 387), op 4, value 90

**Action**

- Play dialog: SPY1W.SCR, line/variant 10

### Event 28

**Trigger**

- Object event: subject Bora_Battleaxe (object 16, id 388), op 3, value 50

**Action**

- Play dialog: SPY3R.SCR, line/variant 11

### Event 29

**Trigger**

- Object event: subject Bora_Warhammer (object 15, id 389), op 3, value 70

**Action**

- Play dialog: SPY2W.SCR, line/variant 8

### Event 30

**Trigger**

- Object event: subject Bora_Mace (object 0, id 387), op 3, value 80

**Action**

- Play dialog: SPY1W.SCR, line/variant 11

### Event 31

**Trigger**

- Object event: subject Bora_Warhammer (object 15, id 389), op 2, value 0 (join 2)
- Object event: subject Bora_Battleaxe (object 16, id 388), op 2, value 0 (join 2)
- Object event: subject Bora_Mace (object 0, id 387), op 2, value 0 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 73

### Event 32

**Trigger**

- Variable comparison: subject variable group 20, variable 16, op 1, value 30 (join 1)
- Object event: subject Bora_Mace (object 0, id 387), op 2, value 0 (join 1)
- Variable comparison: subject variable group 21, variable 22, op 1, value 1 (join 1)

**Action**

- Play dialog: SPY1W.SCR, line/variant 9

### Event 33

**Trigger**

- Variable comparison: subject variable group 20, variable 16, op 1, value 90 (join 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1 (join 1)
- Object event: subject Bora_Battleaxe (object 16, id 388), op 2, value 0 (join 1)

**Action**

- Play dialog: SPY3R.SCR, line/variant 5

### Event 34

**Trigger**

- Variable comparison: subject variable group 20, variable 16, op 1, value 90 (join 1)
- Variable comparison: subject variable group 21, variable 21, op 1, value 1 (join 1)
- Object event: subject Bora_Warhammer (object 15, id 389), op 2, value 0 (join 1)

**Action**

- Play dialog: SPY2W.SCR, line/variant 6

### Event 35

**Trigger**

- Group/spawn-list event: subject 135, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 135

### Event 36

**Trigger**

- Group/spawn-list event: subject 127, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 127

### Event 37

**Trigger**

- Group/spawn-list event: subject 130, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 130

### Event 38

**Trigger**

- Group/spawn-list event: subject 128, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 128

### Event 39

**Trigger**

- Group/spawn-list event: subject 147, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 147

### Event 40

**Trigger**

- Variable comparison: subject variable group 21, variable 32, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 2, param 388
- Show/update HUD contact: contact/list 0, subtype 2, param 387
- Show/update HUD contact: contact/list 0, subtype 2, param 389

### Event 41

**Trigger**

- Object event: subject Bora_Battleaxe (object 16, id 388), op 2, value 0

**Action**

- Mark/flash contact: contact/list 0, subtype 2, param 388

### Event 42

**Trigger**

- Object event: subject Bora_Mace (object 0, id 387), op 2, value 0

**Action**

- Mark/flash contact: contact/list 0, subtype 2, param 387

### Event 43

**Trigger**

- Object event: subject Bora_Warhammer (object 15, id 389), op 2, value 0

**Action**

- Mark/flash contact: contact/list 0, subtype 2, param 389

### Event 44

**Trigger**

- Object event: subject Bora_Battleaxe (object 16, id 388), op 2, value 0
- Object event: subject Bora_Mace (object 0, id 387), op 2, value 0
- Object event: subject Bora_Warhammer (object 15, id 389), op 2, value 0

**Action**

- Set/add variable: variable group 18, variable 408, subtype 0, value 1
- Set/add variable: variable group 18, variable 407, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Broadcast HUD contact action: contact/list 0, subtype 0, param 25

### Event 45

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 12

**Action**

- Object spawn/action: Crate_5 (object 10, id 401), subtype 0
- Object spawn/action: Crate_6 (object 11, id 402), subtype 0
- Object spawn/action: Crate_7 (object 12, id 403), subtype 0
- Set runtime trigger variable: variable group 20, variable 1, subtype 1, value 0

### Event 46

**Trigger**

- Object event: subject Bora_Battleaxe (object 16, id 388), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 1, param 135
- Hide/remove HUD contact: contact/list 0, subtype 1, param 127
- Hide/remove HUD contact: contact/list 0, subtype 1, param 147
- Hide/remove HUD contact: contact/list 0, subtype 1, param 130

### Event 47

**Trigger**

- Runtime condition family: subject 0, op 0, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 197

### Event 48

**Trigger**

- Variable comparison: subject variable group 20, variable 16, op 1, value 95

**Action**

- Object spawn/action: Bora_Mace (object 0, id 387), subtype 7
- Object spawn/action: Bora_Warhammer (object 15, id 389), subtype 7
- Set runtime trigger variable: variable group 20, variable 16, subtype 1, value 0

## Waypoints

### Waypoint 0

- Tag: `9`
- Members: `Independent_Merc_Piranha (object 6, id 397, starts at point 0)`, `Independent_Merc_Piranha (object 7, id 398, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1344.10, 0.00, 480.25) | None |
| 1 | (-832.62, 0.00, -628.18) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 1

- Tag: `7`
- Members: `Independent_Merc_Gar (object 1, id 392, starts at point 0)`, `Independent_Merc_Gar (object 2, id 393, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1279.28, 0.00, -1842.53) | None |
| 1 | (-675.15, 0.00, -1316.72) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 2

- Tag: `6`
- Members: `Independent_Merc_Piranha (object 8, id 399, starts at point 0)`, `Independent_Merc_Piranha (object 13, id 406, starts at point 0)`, `Independent_Merc_Piranha (object 14, id 408, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (729.31, 0.00, 288.16) | None |
| 1 | (164.67, 0.00, -367.06) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 3

- Tag: `4`
- Members: `Independent_Merc_Gar (object 3, id 394, starts at point 0)`, `Independent_Merc_Gar (object 4, id 395, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (68.22, 402.04, 2975.34) | None |
| 1 | (-771.41, 0.00, 2999.24) | None |
| 2 | (-1484.21, -616.11, 1406.59) | None |
| 3 | (-668.24, -616.11, 656.44) | None |
| 4 | (635.86, 0.00, 1204.24) | None |
| 5 | (1026.12, 402.04, 2452.92) | on arrival redirect to Waypoint 3 (tag 4), point 0 |

## Spawn Lists

### Spawn List 0

- ID: `85`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 5 | spawn list 147 | None |
| 2 | 5 | spawn list 130 | None |
| 3 | 5 | spawn list 127 | None |

### Spawn List 1

- ID: `106`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 5 | spawn list 130 | None |
| 2 | 5 | spawn list 147 | None |
| 3 | 5 | spawn list 127 | None |

### Spawn List 2

- ID: `109`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 5 | spawn list 147 | None |
| 2 | 5 | spawn list 130 | None |
| 3 | 5 | spawn list 127 | None |

### Spawn List 3

- ID: `130`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 6 | Bora_Battleaxe (object 16, id 388) | None |
| 2 | 6 | Bora_Mace (object 0, id 387) | None |
| 3 | 6 | Bora_Warhammer (object 15, id 389) | None |

### Spawn List 4

- ID: `127`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 6 | Bora_Battleaxe (object 16, id 388) | None |
| 2 | 6 | Bora_Mace (object 0, id 387) | None |
| 3 | 6 | Bora_Warhammer (object 15, id 389) | None |

### Spawn List 5

- ID: `147`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 6 | Bora_Battleaxe (object 16, id 388) | None |
| 2 | 6 | Bora_Mace (object 0, id 387) | None |
| 3 | 6 | Bora_Warhammer (object 15, id 389) | None |

### Spawn List 6

- ID: `128`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | Bora_Battleaxe (object 16, id 388) | None |

### Spawn List 7

- ID: `135`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | Bora_Battleaxe (object 16, id 388) | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Bora_Mace` | 387 | Interactive | -229.98,0.00,-909.22 | 125,0,0 | label: obsidian; group/role: FG_REVOLUTION / 0; alias: fake_2; secondary groups: none, OBSIDIAN |
| 1 | `Independent_Merc_Gar` | 392 | Interactive | -1420.02,0.00,-2093.10 | 37,0,0 | label: killer; group/role: FG_SHALE / 0; waypoint: Waypoint 1 (tag 7, 2 point(s)), starting point 0, arrival event value 458752 |
| 2 | `Independent_Merc_Gar` | 393 | Interactive | -1455.34,0.00,-1899.74 | 90,0,0 | group/role: FG_SHALE / 0; waypoint: Waypoint 1 (tag 7, 2 point(s)), starting point 0, arrival event value 458752 |
| 3 | `Independent_Merc_Gar` | 394 | Interactive | 267.90,400.91,2939.12 | 391,0,0 | group/role: FG_AMBER / 0; waypoint: Waypoint 3 (tag 4, 6 point(s)), starting point 0, arrival event value 262144 |
| 4 | `Independent_Merc_Gar` | 395 | Interactive | 265.26,400.91,2997.10 | 371,0,0 | label: BFGE_02; group/role: FG_AMBER / 0; waypoint: Waypoint 3 (tag 4, 6 point(s)), starting point 0, arrival event value 262144 |
| 5 | `Independent_Merc_Piranha` | 396 | Interactive | -429.50,0.00,879.23 | 449,0,0 | group/role: FG_JADE / 0 |
| 6 | `Independent_Merc_Piranha` | 397 | Interactive | -1417.37,0.00,688.35 | 203,0,0 | label: BFGE_02; group/role: FG_BLOODSTONE / 0; waypoint: Waypoint 0 (tag 9, 2 point(s)), starting point 0, arrival event value 589824 |
| 7 | `Independent_Merc_Piranha` | 398 | Interactive | -1494.25,0.00,630.57 | 212,0,0 | group/role: FG_BLOODSTONE / 0; waypoint: Waypoint 0 (tag 9, 2 point(s)), starting point 0, arrival event value 589824 |
| 8 | `Independent_Merc_Piranha` | 399 | Interactive | 1034.65,0.00,704.79 | 337,0,0 | label: BFGE_02; group/role: FG_GARNET / 0; secondary groups: none, LAUREN; waypoint: Waypoint 2 (tag 6, 2 point(s)), starting point 0, arrival event value 393216 |
| 9 | `Independent_Merc_Piranha` | 400 | Interactive | -394.10,0.00,921.03 | 455,0,0 | label: BFGE_02; group/role: FG_JADE / 0 |
| 10 | `Crate_5` | 401 | Interactive | -209.93,0.00,-782.34 | 129,0,0 | secondary groups: CONT_054, none |
| 11 | `Crate_6` | 402 | Interactive | -217.56,0.00,-672.56 | 129,0,0 | secondary groups: CONT_054, none |
| 12 | `Crate_7` | 403 | Interactive | -216.02,0.00,-909.73 | 134,0,0 | secondary groups: CONT_054, none |
| 13 | `Independent_Merc_Piranha` | 406 | Interactive | 1060.61,0.00,640.88 | 319,0,0 | group/role: FG_GARNET / 0; secondary groups: none, STARD; waypoint: Waypoint 2 (tag 6, 2 point(s)), starting point 0, arrival event value 393216 |
| 14 | `Independent_Merc_Piranha` | 408 | Interactive | 1082.14,0.00,609.00 | 319,0,0 | group/role: FG_GARNET / 0; secondary groups: none, KILLIAN; waypoint: Waypoint 2 (tag 6, 2 point(s)), starting point 0, arrival event value 393216 |
| 15 | `Bora_Warhammer` | 389 | Interactive | -229.41,0.00,-782.77 | 124,0,0 | label: greyhound; group/role: FG_VALOR / 0; alias: fake_1; secondary groups: none, GREYHOUND |
| 16 | `Bora_Battleaxe` | 388 | Interactive | -230.22,0.00,-673.27 | 127,0,0 | label: quasar; group/role: FG_HONOR / 0; alias: spy_1; secondary groups: none, QUASAR |
