# Tachyon: The Fringe FRON11E.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON11E.SPX` |
| Sector | `QUAD_11` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 10 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 6 |
| Events | 8 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Pirate_Mine_TRG`, `1: Baroness_Onrald_Champion` |
| Scripts | `PLAYER.SCR`, `ARENA.SCR` |
| Scenes | None |
| Labels | `bfne_05`, `BFBE_04`, `bfne_01`, `bfne_03`, `bfne_02`, `bfne_04`, `bfne_06`, `bfne_08`, `bfne_07`, `bfne_09` |
| Aliases | `BC05_sistine_chapel`, `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1`, `bc05_2`, `bc05_3`, `bc05_5`, `bc05_4`, `Stocks01` |
| Groups | `VLADIMIR_GRACZYK`, `ARENA_CHALLENGER` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Play scene: unknown index 0, param 1
- Set runtime trigger variable: variable group 20, variable 9, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 5

**Action**

- Play dialog: PLAYER.SCR, line/variant 123

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 20

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 35
- Gate state/action: param 1, subtype 3, param 0
- Gate state/action: param 2, subtype 3, param 0
- Gate state/action: param 3, subtype 3, param 0

### Event 3

**Trigger**

- Object event: subject Baroness_Onrald_Champion (object 0, id 193), op 2, value 0 (join 2)
- Object event: subject Baroness_Onrald_Champion (object 1, id 194), op 2, value 0 (join 2)

**Action**

- Play dialog: ARENA.SCR, line/variant 4

### Event 4

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 4

**Action**

- Play dialog: ARENA.SCR, line/variant 5

### Event 5

**Trigger**

- Object event: subject Baroness_Onrald_Champion (object 0, id 193), op 2, value 0
- Object event: subject Baroness_Onrald_Champion (object 1, id 194), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 35
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 16, variable 424, subtype 0, value 1
- Set/add variable: variable group 16, variable 425, subtype 0, value 2
- Gate state/action: param 1, subtype 0, param 0
- Gate state/action: param 2, subtype 2, param 0
- Gate state/action: param 3, subtype 2, param 0
- Play dialog: ARENA.SCR, line/variant 6

### Event 6

**Trigger**

- Object event: subject Baroness_Onrald_Champion (object 0, id 193), op 2, value 0
- Object event: subject Baroness_Onrald_Champion (object 1, id 194), op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 12, param 37
- Set/add variable: variable group 4, variable 11, subtype 1, value 1

### Event 7

**Trigger**

- Object event: subject Baroness_Onrald_Champion (object 0, id 193), op 2, value 0
- Object event: subject Baroness_Onrald_Champion (object 1, id 194), op 2, value 0

**Action**

- Object spawn/action: Pirate_Mine_TRG (object 2, id 458), subtype 8, param 4
- Object spawn/action: Pirate_Mine_TRG (object 3, id 459), subtype 8, param 4
- Object spawn/action: Pirate_Mine_TRG (object 4, id 460), subtype 8, param 4
- Object spawn/action: Pirate_Mine_TRG (object 5, id 461), subtype 8, param 4

## Waypoints

### Waypoint 0

- Tag: `302`
- Members: `Baroness_Onrald_Champion (object 1, id 194, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (383.12, -357.58, 8394.78) | None |
| 1 | (1621.23, -382.30, 6826.61) | None |
| 2 | (689.77, -681.10, 5725.98) | None |

### Waypoint 1

- Tag: `301`
- Members: `Baroness_Onrald_Champion (object 0, id 193, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-359.68, -681.10, 8362.72) | None |
| 1 | (-1701.10, -527.86, 6874.79) | None |
| 2 | (-869.27, -323.52, 5809.65) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Baroness_Onrald_Champion` | 193 | Interactive | -95.89,-575.91,8688.63 | 257,0,0 | secondary groups: none, VLADIMIR_GRACZYK; waypoint: Waypoint 1 (tag 301, 3 point(s)), starting point 0, arrival event value 19726336 |
| 1 | `Baroness_Onrald_Champion` | 194 | Interactive | 116.57,-357.58,8685.72 | 257,0,0 | label: bfne_05; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 0 (tag 302, 3 point(s)), starting point 0, arrival event value 19791872 |
| 2 | `Pirate_Mine_TRG` | 458 | Interactive | -205.46,-592.92,6458.61 | 339,0,0 | None |
| 3 | `Pirate_Mine_TRG` | 459 | Interactive | 180.04,-592.92,6821.92 | 59,0,0 | None |
| 4 | `Pirate_Mine_TRG` | 460 | Interactive | -317.52,-592.92,6948.29 | 461,0,0 | None |
| 5 | `Pirate_Mine_TRG` | 461 | Interactive | 278.65,-592.92,6355.33 | 197,0,0 | None |
