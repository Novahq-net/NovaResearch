# Tachyon: The Fringe FRON11J.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON11J.SPX` |
| Sector | `QUAD_11` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 10 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 4 |
| Events | 9 |
| Waypoints | 4 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Independent_Merc_Piranha` |
| Scripts | `ARENA.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `bfne_05`, `BFBE_04`, `bfne_01`, `bfne_03`, `bfne_02`, `bfne_04`, `bfne_06`, `bfne_08`, `bfne_07`, `bfne_09` |
| Aliases | `BC05_sistine_chapel`, `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1`, `bc05_2`, `bc05_3`, `bc05_5`, `bc05_4`, `Stocks01` |
| Groups | `ARENA_CHALLENGER` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 21, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 44

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 21, op 1, value 5

**Action**

- Play dialog: ARENA.SCR, line/variant 8
- Play scene: unknown index 0, param 2

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 21, op 1, value 25

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 35
- Hide/remove HUD contact: contact/list 0, subtype 9, param 44
- Gate state/action: param 1, subtype 3, param 0
- Gate state/action: param 2, subtype 3, param 0
- Gate state/action: param 3, subtype 3, param 0

### Event 3

**Trigger**

- Object event: subject Independent_Merc_Piranha (object 0, id 591), op 2, value 0 (join 2)
- Object event: subject Independent_Merc_Piranha (object 1, id 592), op 2, value 0 (join 2)
- Object event: subject Independent_Merc_Piranha (object 3, id 594), op 2, value 0 (join 2)
- Object event: subject Independent_Merc_Piranha (object 2, id 593), op 2, value 0 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 185

### Event 4

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 185

**Action**

- Play dialog: ARENA.SCR, line/variant 35

### Event 5

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 25

**Action**

- Play dialog: ARENA.SCR, line/variant 24

### Event 6

**Trigger**

- Object event: subject Independent_Merc_Piranha (object 0, id 591), op 2, value 0
- Object event: subject Independent_Merc_Piranha (object 1, id 592), op 2, value 0
- Object event: subject Independent_Merc_Piranha (object 2, id 593), op 2, value 0
- Object event: subject Independent_Merc_Piranha (object 3, id 594), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 35
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 16, variable 438, subtype 0, value 1
- Set/add variable: variable group 16, variable 439, subtype 0, value 2
- Gate state/action: param 1, subtype 0, param 0
- Gate state/action: param 2, subtype 2, param 0
- Gate state/action: param 3, subtype 2, param 0
- Play dialog: ARENA.SCR, line/variant 29

### Event 7

**Trigger**

- Object event: subject Independent_Merc_Piranha (object 0, id 591), op 2, value 0
- Object event: subject Independent_Merc_Piranha (object 1, id 592), op 2, value 0
- Object event: subject Independent_Merc_Piranha (object 2, id 593), op 2, value 0
- Object event: subject Independent_Merc_Piranha (object 3, id 594), op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 12, param 39

### Event 8

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 29

**Action**

- Play dialog: ARENA.SCR, line/variant 33

## Waypoints

### Waypoint 0

- Tag: `554`
- Members: `Independent_Merc_Piranha (object 3, id 594, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2961.50, -1615.34, 7198.57) | None |
| 1 | (-711.27, -1040.99, 6264.82) | None |

### Waypoint 1

- Tag: `553`
- Members: `Independent_Merc_Piranha (object 2, id 593, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2922.22, 520.50, 7058.10) | None |
| 1 | (623.28, -71.79, 6245.43) | None |

### Waypoint 2

- Tag: `552`
- Members: `Independent_Merc_Piranha (object 1, id 592, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (300.82, -592.29, 8515.12) | None |
| 1 | (1746.09, -592.29, 6918.55) | None |
| 2 | (264.46, -592.29, 5558.33) | None |

### Waypoint 3

- Tag: `551`
- Members: `Independent_Merc_Piranha (object 0, id 591, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-395.43, -592.29, 8509.91) | None |
| 1 | (-1695.31, -592.29, 6922.62) | None |
| 2 | (-335.34, -592.29, 5576.04) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Independent_Merc_Piranha` | 591 | Interactive | -440.17,0.00,9693.44 | 257,0,0 | secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 3 (tag 551, 3 point(s)), starting point 0, arrival event value 36110336 |
| 1 | `Independent_Merc_Piranha` | 592 | Interactive | 370.82,0.00,9718.93 | 257,0,0 | label: bfne_06; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 2 (tag 552, 3 point(s)), starting point 0, arrival event value 36175872 |
| 2 | `Independent_Merc_Piranha` | 593 | Interactive | 4554.72,0.00,7535.05 | 351,0,0 | secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 1 (tag 553, 2 point(s)), starting point 0, arrival event value 36241408 |
| 3 | `Independent_Merc_Piranha` | 594 | Interactive | -4327.13,0.00,7826.66 | 185,0,0 | label: bfne_05; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 0 (tag 554, 2 point(s)), starting point 0, arrival event value 36306944 |
