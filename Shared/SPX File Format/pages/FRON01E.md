# Tachyon: The Fringe FRON01E.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON01E.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 3 |
| Events | 3 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Cruiser`, `1: Generic_Light_Freighter`, `2: Bora_Shuttle_Medium` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFGF_05`, `BFNE_03`, `BFNF_03`, `BFGE_01`, `BFGF_01`, `bfne_05` |
| Aliases | `Python 4`, `Python 3`, `Python 1`, `Python 2`, `Kimodo 1`, `Jerome02`, `Jerome03`, `Jerome04`, `Jerome05`, `Jerome06`, `Jerome01`, `BC05_sistine_chapel`, `bc05_1`, `bc05_2`, `bc05_4`, `bc05_5`, `Mantis1`, `Mantis2`, `Mantis3`, `Mantis4`, `Aphid1`, `Aphid2`, `Aphid3`, `Aphid4`, `Python1`, `Python2`, `Python3`, `Python4`, `Komodo1`, `Komodo2`, `Komodo3`, `Komodo4`, `Kimodo 2`, `Kimodo 3`, `Kimodo 4`, `Cephius`, `Stocks01` |
| Groups | `CONT_033`, `CONT_020` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 19, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 20

**Action**

- Play dialog: PLAYER.SCR, line/variant 25
- Set runtime trigger variable: variable group 20, variable 19, subtype 1, value 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 0 (extra 2, 4; flags 2)

**Action**

- Object spawn/action: GalSpan_Cruiser (object 2, id 566), subtype 0

## Waypoints

### Waypoint 0

- Tag: `302`
- Members: `Bora_Shuttle_Medium (object 0, id 477, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2389.72, 0.00, 1316.82) | None |
| 1 | (-8758.52, 0.00, -12899.88) | None |

### Waypoint 1

- Tag: `301`
- Members: `Generic_Light_Freighter (object 1, id 318, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1095.93, 0.00, -2080.26) | None |
| 1 | (1074.58, 0.00, -331.84) | None |
| 2 | (1468.34, 0.00, 1056.92) | on arrival activate current object (raw param -1 ignored) |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Bora_Shuttle_Medium` | 477 | Interactive | -2112.47,0.00,2089.52 | 0,0,0 | secondary groups: CONT_033, none; waypoint: Waypoint 0 (tag 302, 2 point(s)), starting point 0, arrival event value 19791872 |
| 1 | `Generic_Light_Freighter` | 318 | Interactive | 1095.93,0.00,-2913.95 | 0,0,0 | label: bfne_05; secondary groups: CONT_020, none; waypoint: Waypoint 1 (tag 301, 3 point(s)), starting point 0, arrival event value 19726336 |
| 2 | `GalSpan_Cruiser` | 566 | Interactive | 2102.46,0.00,-2325.12 | 0,0,0 | None |
