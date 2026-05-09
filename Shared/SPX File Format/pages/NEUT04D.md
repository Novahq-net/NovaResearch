# Tachyon: The Fringe NEUT04D.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT04D.SPX` |
| Sector | `QUAD_04` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 3 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 4 |
| Events | 5 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Hvy_Freighter`, `1: Bora_Light_Freighter`, `2: Bora_Cruiser`, `3: Shuttle_Medium` |
| Scripts | `DRAKE.SCR` |
| Scenes | None |
| Labels | `bfne_06`, `BFBE_03`, `MISHK`, `HESPE`, `Merch` |
| Aliases | `Courage`, `kwI03_02`, `kwI03_03`, `kwi03_7`, `Jerome24`, `Jerome25`, `Jerome26`, `Jerome22`, `Jerome21`, `Jerome20`, `Intrepid`, `Artemis`, `KWi03_10`, `Hermes` |
| Groups | `CONT_018`, `CONT_019` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 20, op 1, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 15
- Object spawn/action: Bora_Cruiser (object 1, id 1401), subtype 5
- Object spawn/action: id 1552, subtype 14
- Set runtime trigger variable: variable group 20, variable 5, subtype 0, value 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1552; flags 2)
- Variable comparison: subject variable group 21, variable 20, op 1, value 0

**Action**

- Object spawn/action: Bora_Hvy_Freighter (object 3, id 1405), subtype 3
- Object spawn/action: id 1552, subtype 15

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 6, value 2 (extra 1, 1552; flags 2)
- Variable comparison: subject variable group 21, variable 20, op 1, value 0

**Action**

- Mission objective/state: param 65541, subtype 0, param 0
- Set/add variable: variable group 21, variable 20, subtype 1, value 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 15
- Set/add variable: variable group 8, variable 4, subtype 0, value 1
- Play dialog: DRAKE.SCR, line/variant 8

### Event 3

**Trigger**

- Object arrival: Bora_Cruiser (object 1, id 1401) reached Waypoint 2 (tag 251), point 1 (raw value 16449537)

**Action**

- Object spawn/action: Bora_Cruiser (object 1, id 1401), subtype 4

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 5, op 1, value 5

**Action**

- Set runtime trigger variable: variable group 20, variable 5, subtype 1, value 0
- Play dialog: DRAKE.SCR, line/variant 7

## Waypoints

### Waypoint 0

- Tag: `253`
- Members: `Shuttle_Medium (object 0, id 1594, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-949.68, 655.38, -133.92) | None |
| 1 | (46.17, 652.56, -104.32) | None |
| 2 | (203.43, -111.23, -91.76) | None |
| 3 | (-981.77, -114.73, 65.33) | on arrival redirect to Waypoint 0 (tag 253), point 0 |

### Waypoint 1

- Tag: `252`
- Members: `Bora_Hvy_Freighter (object 3, id 1405, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (666.20, 658.12, -1930.84) | None |
| 1 | (676.08, 679.74, -486.42) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 2

- Tag: `251`
- Members: `Bora_Cruiser (object 1, id 1401, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (80.73, -234.78, -2456.36) | None |
| 1 | (-1684.39, -181.27, -2430.45) | None; listened by Event 3 for Bora_Cruiser (object 1, id 1401) |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Shuttle_Medium` | 1594 | Interactive | -1332.15,-507.02,-168.70 | 21,128,36 | waypoint: Waypoint 0 (tag 253, 4 point(s)), starting point 0, arrival event value 16580608 |
| 1 | `Bora_Cruiser` | 1401 | Interactive | 1535.22,-195.32,-2479.92 | 380,0,14 | secondary groups: CONT_018, none; waypoint: Waypoint 2 (tag 251, 2 point(s)), starting point 0, arrival event value 16449536 |
| 2 | `Bora_Light_Freighter` | 1404 | Interactive | -895.34,789.76,-771.79 | 0,0,0 | None |
| 3 | `Bora_Hvy_Freighter` | 1405 | Interactive | -909.43,779.35,-2028.88 | 121,0,0 | secondary groups: CONT_019, none; waypoint: Waypoint 1 (tag 252, 2 point(s)), starting point 0, arrival event value 16515072 |
