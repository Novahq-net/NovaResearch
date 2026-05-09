# Tachyon: The Fringe FRON11O.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON11O.SPX` |
| Sector | `QUAD_11` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 10 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 4 |
| Events | 16 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Demon_Pirate_Fighter` |
| Scripts | `ARENA.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `bfne_05`, `BFBE_04`, `bfne_01`, `bfne_03`, `bfne_02`, `bfne_04`, `bfne_06`, `bfne_08`, `bfne_07`, `bfne_09` |
| Aliases | `BC05_sistine_chapel`, `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1`, `bc05_2`, `bc05_3`, `bc05_5`, `bc05_4`, `Stocks01` |
| Groups | `FG_ELITE`, `ARENA_CHALLENGER`, `FG_ENVY` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 26, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 44

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 26, op 1, value 8

**Action**

- Play dialog: ARENA.SCR, line/variant 54
- Play scene: unknown index 0, param 2

### Event 2

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 54

**Action**

- Play dialog: PLAYER.SCR, line/variant 176

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 26, op 1, value 20

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 35
- Hide/remove HUD contact: contact/list 0, subtype 9, param 44
- Gate state/action: param 1, subtype 3, param 0
- Gate state/action: param 2, subtype 3, param 0
- Gate state/action: param 3, subtype 3, param 0

### Event 4

**Trigger**

- Object event: subject Demon_Pirate_Fighter (object 0, id 690), op 10, value 0 (join 2)
- Object event: subject Demon_Pirate_Fighter (object 1, id 691), op 10, value 0 (join 2)
- Object event: subject Demon_Pirate_Fighter (object 2, id 692), op 10, value 0 (join 2)
- Object event: subject Demon_Pirate_Fighter (object 3, id 693), op 10, value 0 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 147

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 80

**Action**

- Play dialog: PLAYER.SCR, line/variant 189

### Event 6

**Trigger**

- Object event: subject Demon_Pirate_Fighter (object 1, id 691), op 3, value 90 (join 2)
- Object event: subject Demon_Pirate_Fighter (object 3, id 693), op 3, value 90 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 186

### Event 7

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 40

**Action**

- Play dialog: PLAYER.SCR, line/variant 188

### Event 8

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 189

**Action**

- Play dialog: PLAYER.SCR, line/variant 167

### Event 9

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 167

**Action**

- Play dialog: ARENA.SCR, line/variant 21

### Event 10

**Trigger**

- Object event: subject Demon_Pirate_Fighter (object 0, id 690), op 2, value 0 (join 2)
- Object event: subject Demon_Pirate_Fighter (object 1, id 691), op 2, value 0 (join 2)
- Object event: subject Demon_Pirate_Fighter (object 2, id 692), op 2, value 0 (join 2)
- Object event: subject Demon_Pirate_Fighter (object 3, id 693), op 2, value 0 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 163

### Event 11

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 163

**Action**

- Play dialog: ARENA.SCR, line/variant 53

### Event 12

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 53

**Action**

- Play dialog: ARENA.SCR, line/variant 14

### Event 13

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 14

**Action**

- Play dialog: ARENA.SCR, line/variant 19

### Event 14

**Trigger**

- Group/spawn-list event: subject 271, op 0, value 0
- Group/spawn-list event: subject 152, op 0, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 35
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 16, variable 448, subtype 0, value 1
- Set/add variable: variable group 16, variable 449, subtype 0, value 2
- Gate state/action: param 1, subtype 0, param 0
- Gate state/action: param 2, subtype 2, param 0
- Gate state/action: param 3, subtype 2, param 0
- Play dialog: ARENA.SCR, line/variant 55

### Event 15

**Trigger**

- Group/spawn-list event: subject 271, op 0, value 0
- Group/spawn-list event: subject 152, op 0, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 12, param 39

## Waypoints

### Waypoint 0

- Tag: `802`
- Members: `Demon_Pirate_Fighter (object 2, id 692, starts at point 0)`, `Demon_Pirate_Fighter (object 3, id 693, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (703.91, -601.58, 9286.94) | None |
| 1 | (522.30, -601.58, 6239.89) | None |

### Waypoint 1

- Tag: `801`
- Members: `Demon_Pirate_Fighter (object 0, id 690, starts at point 0)`, `Demon_Pirate_Fighter (object 1, id 691, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-725.04, -601.58, 9270.68) | None |
| 1 | (-519.56, -601.58, 6291.71) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Demon_Pirate_Fighter` | 690 | Interactive | -749.08,-601.58,9336.22 | 247,0,0 | group/role: FG_ELITE / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 1 (tag 801, 2 point(s)), starting point 0, arrival event value 52494336 |
| 1 | `Demon_Pirate_Fighter` | 691 | Interactive | -720.40,-601.58,9346.58 | 247,0,0 | group/role: FG_ELITE / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 1 (tag 801, 2 point(s)), starting point 0, arrival event value 52494336 |
| 2 | `Demon_Pirate_Fighter` | 692 | Interactive | 684.90,-601.58,9355.65 | 266,0,0 | group/role: FG_ENVY / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 0 (tag 802, 2 point(s)), starting point 0, arrival event value 52559872 |
| 3 | `Demon_Pirate_Fighter` | 693 | Interactive | 732.64,-601.58,9351.24 | 266,0,0 | group/role: FG_ENVY / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 0 (tag 802, 2 point(s)), starting point 0, arrival event value 52559872 |
