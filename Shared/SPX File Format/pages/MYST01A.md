# Tachyon: The Fringe MYST01A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST01A.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 5 |
| Sector ID | 0 |
| SectorHazardFlags | Twilight fog / fog-radar impairment (0x00000002) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 3 |
| Events | 2 |
| Waypoints | 4 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Light_Freighter`, `1: Bora_Hvy_Freighter`, `2: Shuttle_Medium` |
| Scripts | `ANNAH.SCR` |
| Scenes | None |
| Labels | `bfne_07`, `bfbf_07`, `bfgf_05` |
| Aliases | None |
| Groups | `CONT_027`, `CONT_004` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Group/spawn-list event: subject 78, op 2, value 196609 (Waypoint 1 (tag 3), point 1)

**Action**

- Object spawn/action: Bora_Light_Freighter (object 2, id 192), subtype 12

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 9, value 0

**Action**

- Mission objective/state: param 327685, subtype 0, param 0
- Play dialog: ANNAH.SCR, line/variant 0

## Waypoints

### Waypoint 0

- Tag: `4`
- Members: `Bora_Light_Freighter (object 2, id 192, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-671.25, -145.36, 1881.10) | on arrival action 1, param -1 |

### Waypoint 1

- Tag: `3`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (680.77, 318.02, -768.00) | None |
| 1 | (968.24, 318.02, 316.30) | None |
| 2 | (222.59, 318.02, 887.97) | None |
| 3 | (-1049.21, 318.02, 303.89) | None |
| 4 | (-600.88, 318.02, -977.36) | on arrival redirect to Waypoint 1 (tag 3), point 0 |

### Waypoint 2

- Tag: `2`
- Members: `Shuttle_Medium (object 0, id 82, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1206.05, 1335.67, -81.32) | None |
| 1 | (1692.61, 1266.93, 496.50) | None |
| 2 | (764.21, 1179.06, 1501.40) | on arrival play dialog/script or enter gate, param 60 |

### Waypoint 3

- Tag: `1`
- Members: `Bora_Hvy_Freighter (object 1, id 69, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1897.12, 1371.11, 2852.00) | on arrival action 1, param -1 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Shuttle_Medium` | 82 | Interactive | 1151.99,1335.67,-156.69 | 55,0,0 | label: bfne_07; waypoint: Waypoint 2 (tag 2, 3 point(s)), starting point 0, arrival event value 131072 |
| 1 | `Bora_Hvy_Freighter` | 69 | Interactive | -340.31,1208.08,-893.61 | 457,0,0 | label: bfbf_07; secondary groups: CONT_027, none; waypoint: Waypoint 3 (tag 1, 1 point(s)), starting point 0, arrival event value 65536 |
| 2 | `Bora_Light_Freighter` | 192 | Interactive | -1122.25,-145.36,1622.12 | 91,0,0 | label: bfbf_07; secondary groups: CONT_004, none; waypoint: Waypoint 0 (tag 4, 1 point(s)), starting point 0, arrival event value 262144 |
