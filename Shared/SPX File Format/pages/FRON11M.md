# Tachyon: The Fringe FRON11M.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON11M.SPX` |
| Sector | `QUAD_11` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 10 |
| SectorHazardFlags | Twilight fog / fog-radar impairment (0x00000002) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 6 |
| Events | 11 |
| Waypoints | 4 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Skav_Pirate_Manta` |
| Scripts | `ARENA.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `bfne_05`, `BFBE_04`, `bfne_01`, `bfne_03`, `bfne_02`, `bfne_04`, `bfne_06`, `bfne_08`, `bfne_07`, `bfne_09` |
| Aliases | `BC05_sistine_chapel`, `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1`, `bc05_2`, `bc05_3`, `bc05_5`, `bc05_4`, `Stocks01` |
| Groups | `ARENA_CHALLENGER`, `FG_WRAITH`, `FG_WYRM` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 24, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 44

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 24, op 1, value 8

**Action**

- Play dialog: ARENA.SCR, line/variant 48
- Play scene: unknown index 0, param 2

### Event 2

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 8

**Action**

- Play dialog: PLAYER.SCR, line/variant 183

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 24, op 1, value 20

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 35
- Hide/remove HUD contact: contact/list 0, subtype 9, param 44
- Gate state/action: param 1, subtype 3, param 0
- Gate state/action: param 2, subtype 3, param 0
- Gate state/action: param 3, subtype 3, param 0

### Event 4

**Trigger**

- Object event: subject Skav_Pirate_Manta (object 0, id 654), op 2, value 0 (join 2)
- Object event: subject Skav_Pirate_Manta (object 5, id 659), op 2, value 0 (join 2)

**Action**

- Play dialog: ARENA.SCR, line/variant 24

### Event 5

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 24

**Action**

- Play dialog: PLAYER.SCR, line/variant 146

### Event 6

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 40

**Action**

- Play dialog: PLAYER.SCR, line/variant 188

### Event 7

**Trigger**

- Group/spawn-list event: subject 81, op 0, value 0
- Group/spawn-list event: subject 251, op 0, value 0
- Object event: subject Skav_Pirate_Manta (object 0, id 654), op 2, value 0
- Object event: subject Skav_Pirate_Manta (object 5, id 659), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 35
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 16, variable 444, subtype 0, value 1
- Set/add variable: variable group 16, variable 445, subtype 0, value 2
- Gate state/action: param 1, subtype 0, param 0
- Gate state/action: param 2, subtype 2, param 0
- Gate state/action: param 3, subtype 2, param 0
- Play dialog: ARENA.SCR, line/variant 27

### Event 8

**Trigger**

- Group/spawn-list event: subject 81, op 0, value 0 (join 2)
- Group/spawn-list event: subject 251, op 0, value 0 (join 2)

**Action**

- Play dialog: ARENA.SCR, line/variant 47

### Event 9

**Trigger**

- Group/spawn-list event: subject 81, op 0, value 0
- Group/spawn-list event: subject 251, op 0, value 0
- Object event: subject Skav_Pirate_Manta (object 0, id 654), op 2, value 0
- Object event: subject Skav_Pirate_Manta (object 5, id 659), op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 12, param 39

### Event 10

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 47

**Action**

- Play dialog: ARENA.SCR, line/variant 60

## Waypoints

### Waypoint 0

- Tag: `704`
- Members: `Skav_Pirate_Manta (object 5, id 659, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1348.89, -551.48, 8983.01) | None |
| 1 | (968.16, -570.50, 6255.81) | None |

### Waypoint 1

- Tag: `703`
- Members: `Skav_Pirate_Manta (object 3, id 657, starts at point 0)`, `Skav_Pirate_Manta (object 4, id 658, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (535.98, -570.50, 9491.47) | None |
| 1 | (381.63, -570.50, 6311.60) | None |

### Waypoint 2

- Tag: `702`
- Members: `Skav_Pirate_Manta (object 1, id 655, starts at point 0)`, `Skav_Pirate_Manta (object 2, id 656, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-637.09, -570.50, 9480.32) | None |
| 1 | (-410.70, -570.50, 6356.23) | None |

### Waypoint 3

- Tag: `701`
- Members: `Skav_Pirate_Manta (object 0, id 654, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1357.39, -570.50, 9106.54) | None |
| 1 | (-966.37, -570.50, 6395.28) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Skav_Pirate_Manta` | 654 | Interactive | -1447.47,-570.50,9358.28 | 260,0,0 | secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 3 (tag 701, 2 point(s)), starting point 0, arrival event value 45940736 |
| 1 | `Skav_Pirate_Manta` | 655 | Interactive | -737.10,-570.50,9719.83 | 260,0,0 | group/role: FG_WRAITH / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 2 (tag 702, 2 point(s)), starting point 0, arrival event value 46006272 |
| 2 | `Skav_Pirate_Manta` | 656 | Interactive | -635.62,-570.50,9735.55 | 260,0,0 | label: bfne_03; group/role: FG_WRAITH / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 2 (tag 702, 2 point(s)), starting point 0, arrival event value 46006272 |
| 3 | `Skav_Pirate_Manta` | 657 | Interactive | 466.18,-570.50,9704.11 | 260,0,0 | group/role: FG_WYRM / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 1 (tag 703, 2 point(s)), starting point 0, arrival event value 46071808 |
| 4 | `Skav_Pirate_Manta` | 658 | Interactive | 553.17,-570.50,9672.67 | 260,0,0 | label: bfne_07; group/role: FG_WYRM / 0; secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 1 (tag 703, 2 point(s)), starting point 0, arrival event value 46071808 |
| 5 | `Skav_Pirate_Manta` | 659 | Interactive | 1394.01,-570.50,9216.80 | 260,0,0 | secondary groups: none, ARENA_CHALLENGER; waypoint: Waypoint 0 (tag 704, 2 point(s)), starting point 0, arrival event value 46137344 |
