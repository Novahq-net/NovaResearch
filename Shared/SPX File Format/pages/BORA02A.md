# Tachyon: The Fringe BORA02A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `BORA02A.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `(none)` |
| Region | 3 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 5 |
| Entities | 10 |
| Events | 7 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Hvy_Freighter`, `1: Bora_Battleaxe`, `2: Bora_Mace`, `3: Bora_Shuttle_Medium`, `4: Bora_Cutlass` |
| Scripts | `CHAAS.SCR` |
| Scenes | None |
| Labels | `chaas`, `bfbf_01`, `BFBE_05`, `BFGE_05`, `BFBF_05` |
| Aliases | `frank01`, `frank02`, `frank03`, `frank04`, `stocks06` |
| Groups | `FG_CLAW`, `CONT_026`, `FG_GOLDRUSH` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 30, subtype 1, param 6

### Event 1

**Trigger**

- Group/spawn-list event: subject 30, op 3, value 0
- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Play dialog: CHAAS.SCR, line/variant 2

### Event 2

**Trigger**

- Group/spawn-list event: subject 30, op 2, value 6619136 (Waypoint 2 (tag 101), point 0)

**Action**

- Object spawn/action: Bora_Shuttle_Medium (object 1, id 201), subtype 12
- Group/spawn-list action: spawn list/group 101, subtype 7

### Event 3

**Trigger**

- Object arrival: Bora_Shuttle_Medium (object 1, id 201) reached Waypoint 0 (tag 103), point 0 (raw value 6750208)

**Action**

- Object spawn/action: Bora_Shuttle_Medium (object 1, id 201), subtype 2, param 6
- Group/spawn-list action: spawn list/group 101, subtype 3, param 6

### Event 4

**Trigger**

- Object event: subject Bora_Cutlass (object 0, id 7), op 7, value 0
- Object event: subject Bora_Battleaxe (object 6, id 8), op 7, value 0
- Object event: subject Bora_Battleaxe (object 7, id 9), op 7, value 0
- Object event: subject Bora_Battleaxe (object 8, id 10), op 7, value 0

**Action**

- Set/add variable: variable group 21, variable 21, subtype 1, value 1

### Event 5

**Trigger**

- Object event: subject Bora_Hvy_Freighter (object 9, id 349), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Bora_Hvy_Freighter (object 9, id 349), subtype 12
- Object spawn/action: Bora_Hvy_Freighter (object 9, id 349), subtype 5

### Event 6

**Trigger**

- Object arrival: Bora_Hvy_Freighter (object 9, id 349) reached Waypoint 0 (tag 103), point 0 (raw value 6750208)

**Action**

- Object spawn/action: Bora_Hvy_Freighter (object 9, id 349), subtype 4

## Waypoints

### Waypoint 0

- Tag: `103`
- Members: `Bora_Shuttle_Medium (object 1, id 201, starts at point 0)`, `Bora_Mace (object 2, id 202, starts at point 0)`, `Bora_Mace (object 3, id 203, starts at point 0)`, `Bora_Hvy_Freighter (object 9, id 349, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-523.98, -232.35, 1538.90) | on arrival activate current object (raw param -1 ignored); listened by Event 3 for Bora_Shuttle_Medium (object 1, id 201), Event 6 for Bora_Hvy_Freighter (object 9, id 349) |

### Waypoint 1

- Tag: `102`
- Members: `Bora_Mace (object 4, id 204, starts at point 0)`, `Bora_Mace (object 5, id 205, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1198.73, 0.00, -681.93) | None |
| 1 | (2258.37, 0.00, 1271.30) | None |
| 2 | (154.23, 0.00, 2110.46) | None |
| 3 | (-2335.92, 0.00, 754.07) | None |
| 4 | (-2131.56, 0.00, -304.62) | None |
| 5 | (192.07, 0.00, -1182.76) | on arrival redirect to Waypoint 1 (tag 102), point 0 |

### Waypoint 2

- Tag: `101`
- Members: `Bora_Cutlass (object 0, id 7, starts at point 0)`, `Bora_Battleaxe (object 6, id 8, starts at point 0)`, `Bora_Battleaxe (object 7, id 9, starts at point 0)`, `Bora_Battleaxe (object 8, id 10, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2141.32, 0.00, 351.81) | None |
| 1 | (964.04, -144.63, -499.72) | None |
| 2 | (-442.06, -209.90, -847.41) | on arrival play dialog/script or enter gate, param 5 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Bora_Cutlass` | 7 | Interactive | 2181.83,-209.90,376.98 | 330,0,0 | label: chaas; group/role: FG_CLAW / 1; alias: frank01; waypoint: Waypoint 2 (tag 101, 3 point(s)), starting point 0, arrival event value 6619136 |
| 1 | `Bora_Shuttle_Medium` | 201 | Interactive | -474.96,-275.32,610.46 | 462,0,0 | label: bfbf_01; secondary groups: CONT_026, none; waypoint: Waypoint 0 (tag 103, 1 point(s)), starting point 0, arrival event value 6750208 |
| 2 | `Bora_Mace` | 202 | Interactive | -462.09,-278.41,513.27 | 448,0,0 | label: bfbf_01; group/role: FG_GOLDRUSH / 0; waypoint: Waypoint 0 (tag 103, 1 point(s)), starting point 0, arrival event value 6750208 |
| 3 | `Bora_Mace` | 203 | Interactive | -377.51,-278.41,567.10 | 448,0,0 | group/role: FG_GOLDRUSH / 0; waypoint: Waypoint 0 (tag 103, 1 point(s)), starting point 0, arrival event value 6750208 |
| 4 | `Bora_Mace` | 204 | Interactive | 668.91,0.00,-1174.34 | 0,0,0 | label: bfbf_01; group/role: FG_GOLDRUSH / 0; waypoint: Waypoint 1 (tag 102, 6 point(s)), starting point 0, arrival event value 6684672 |
| 5 | `Bora_Mace` | 205 | Interactive | 737.03,0.00,-1174.34 | 0,0,0 | group/role: FG_GOLDRUSH / 0; waypoint: Waypoint 1 (tag 102, 6 point(s)), starting point 0, arrival event value 6684672 |
| 6 | `Bora_Battleaxe` | 8 | Interactive | 2185.61,-209.90,426.08 | 330,0,0 | group/role: FG_CLAW / 2; alias: frank02; waypoint: Waypoint 2 (tag 101, 3 point(s)), starting point 0, arrival event value 6619136 |
| 7 | `Bora_Battleaxe` | 9 | Interactive | 2252.12,-209.90,388.36 | 330,0,0 | group/role: FG_CLAW / 3; alias: frank03; waypoint: Waypoint 2 (tag 101, 3 point(s)), starting point 0, arrival event value 6619136 |
| 8 | `Bora_Battleaxe` | 10 | Interactive | 2249.82,-209.90,452.05 | 337,0,0 | group/role: FG_CLAW / 4; alias: frank04; waypoint: Waypoint 2 (tag 101, 3 point(s)), starting point 0, arrival event value 6619136 |
| 9 | `Bora_Hvy_Freighter` | 349 | Interactive | -1187.87,396.36,-26.63 | 455,0,0 | waypoint: Waypoint 0 (tag 103, 1 point(s)), starting point 0, arrival event value 6750208 |
