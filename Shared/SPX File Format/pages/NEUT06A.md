# Tachyon: The Fringe NEUT06A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT06A.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 5 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 11 |
| Events | 28 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Pegasus`, `1: Bora_Battleaxe`, `2: GalSpan_Poseidon` |
| Scripts | `G01BFA.SCR`, `G01GFA.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFNE_02`, `bfbe_08`, `BFNE_01`, `bfne_09`, `bfbe_01`, `BLACK`, `repar` |
| Aliases | `Todd08`, `Todd09`, `Todd10`, `oside`, `oside_1`, `oside_2`, `bagel`, `bagel_1`, `bagel_2`, `kwB10_01`, `kwB10_02`, `Todd13`, `Todd12`, `Todd02`, `Todd03`, `Todd04`, `Todd05`, `Todd06`, `Todd07`, `will_01`, `kevin01`, `SHIP1_HYPER`, `SHIP2_HYPER`, `SHIP3_HYPER`, `ohshit` |
| Groups | `FG_GEMINI`, `FG_SWORD`, `FG_PEGASI`, `FG_ATLAS` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0
- Gate state/action: param 4691, subtype 3, param 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 40
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Group/spawn-list action: spawn list/group 281, subtype 0
- Group/spawn-list action: spawn list/group 41, subtype 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Set runtime trigger variable: variable group 20, variable 2, subtype 0, value 0
- Gate state/action: param 4691, subtype 3, param 0
- Set/add variable: variable group 21, variable 20, subtype 0, value 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 0, variable 0, op 1, value 1
- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 39

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 18
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 18, subtype 0
- Group/spawn-list action: spawn list/group 41, subtype 0
- Group/spawn-list action: spawn list/group 281, subtype 0

### Event 5

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 1
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Group/spawn-list action: spawn list/group 56, subtype 3, param 4689

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 31, op 1, value 10 (join 2)
- Group/spawn-list event: subject 56, op 4, value 0 (flags 2)

**Action**

- Group/spawn-list action: spawn list/group 56, subtype 3, param 4689

### Event 7

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 0, variable 0, op 0, value 2

**Action**

- Play dialog: G01BFA.SCR, line/variant 0

### Event 8

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 0
- Variable comparison: subject variable group 20, variable 0, op 1, value 43

**Action**

- Play dialog: G01BFA.SCR, line/variant 1

### Event 9

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 58
- Sector/startup condition family: subject 0, op 0, value 1
- Variable comparison: subject variable group 21, variable 25, op 1, value 1

**Action**

- Play dialog: G01GFA.SCR, line/variant 0

### Event 10

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 1200 (extra 1, 4692; flags 2)
- Variable comparison: subject variable group 0, variable 0, op 1, value 2 (join 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 1200 (extra 1, 4695; flags 2)
- Variable comparison: subject variable group 0, variable 0, op 1, value 2 (join 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 1200 (extra 1, 4698; flags 2)
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Play dialog: PLAYER.SCR, line/variant 3

### Event 11

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 36

### Event 12

**Trigger**

- Sector/startup condition family: subject 2, op 0, value 36

**Action**

- Play dialog: G01GFA.SCR, line/variant 12
- Set runtime trigger variable: variable group 20, variable 31, subtype 0, value 0

### Event 13

**Trigger**

- Variable comparison: subject variable group 0, variable 0, op 1, value 1
- Variable comparison: subject variable group 21, variable 5, op 1, value 1
- Sector/startup condition family: subject 2, op 0, value 36

**Action**

- Play dialog: G01GFA.SCR, line/variant 14
- Mission objective/state: param 65542, subtype 0, param 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 39

### Event 14

**Trigger**

- Object event: subject Bora_Battleaxe (object 4, id 4704), op 7, value 0 (join 2)
- Object event: subject Bora_Battleaxe (object 4, id 4704), op 2, value 0 (join 2)
- Object event: subject Bora_Battleaxe (object 4, id 4704), op 6, value 0 (join 2)

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 15

**Trigger**

- Object event: subject Bora_Battleaxe (object 3, id 4705), op 7, value 0 (join 2)
- Object event: subject Bora_Battleaxe (object 3, id 4705), op 2, value 0 (join 2)
- Object event: subject Bora_Battleaxe (object 3, id 4705), op 6, value 0 (join 2)

**Action**

- Set/add variable: variable group 21, variable 20, subtype 1, value 1

### Event 16

**Trigger**

- Variable comparison: subject variable group 21, variable 5, op 1, value 0
- Group/spawn-list event: subject 281, op 2, value 65537 (Waypoint 0 (tag 1), point 1)
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 281, subtype 6

### Event 17

**Trigger**

- Variable comparison: subject variable group 21, variable 5, op 1, value 0
- Group/spawn-list event: subject 18, op 2, value 65537 (Waypoint 0 (tag 1), point 1)
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 18, subtype 6

### Event 18

**Trigger**

- Variable comparison: subject variable group 21, variable 5, op 1, value 0
- Group/spawn-list event: subject 41, op 2, value 65537 (Waypoint 0 (tag 1), point 1)
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 41, subtype 6

### Event 19

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 800 (extra 1, 4692; flags 2)
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Set/add variable: variable group 21, variable 5, subtype 0, value 1
- Group/spawn-list action: spawn list/group 18, subtype 2
- Group/spawn-list action: spawn list/group 41, subtype 2
- Group/spawn-list action: spawn list/group 281, subtype 2
- Group/spawn-list action: spawn list/group 18, subtype 8, param 65538 (Waypoint 0 (tag 1), point 2)
- Group/spawn-list action: spawn list/group 41, subtype 8, param 65538 (Waypoint 0 (tag 1), point 2)
- Group/spawn-list action: spawn list/group 281, subtype 8, param 65538 (Waypoint 0 (tag 1), point 2)

### Event 20

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 800 (extra 1, 4695; flags 2)
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Set/add variable: variable group 21, variable 5, subtype 0, value 1
- Group/spawn-list action: spawn list/group 18, subtype 2
- Group/spawn-list action: spawn list/group 41, subtype 2
- Group/spawn-list action: spawn list/group 281, subtype 2
- Group/spawn-list action: spawn list/group 18, subtype 8, param 65538 (Waypoint 0 (tag 1), point 2)
- Group/spawn-list action: spawn list/group 41, subtype 8, param 65538 (Waypoint 0 (tag 1), point 2)
- Group/spawn-list action: spawn list/group 281, subtype 8, param 65538 (Waypoint 0 (tag 1), point 2)

### Event 21

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 800 (extra 1, 4698; flags 2)
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Set/add variable: variable group 21, variable 5, subtype 0, value 1
- Group/spawn-list action: spawn list/group 18, subtype 2
- Group/spawn-list action: spawn list/group 41, subtype 2
- Group/spawn-list action: spawn list/group 281, subtype 2
- Group/spawn-list action: spawn list/group 18, subtype 8, param 65538 (Waypoint 0 (tag 1), point 2)
- Group/spawn-list action: spawn list/group 41, subtype 8, param 65538 (Waypoint 0 (tag 1), point 2)
- Group/spawn-list action: spawn list/group 281, subtype 8, param 65538 (Waypoint 0 (tag 1), point 2)

### Event 22

**Trigger**

- Variable comparison: subject variable group 21, variable 10, op 1, value 1
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Set/add variable: variable group 21, variable 5, subtype 0, value 1
- Group/spawn-list action: spawn list/group 18, subtype 2
- Group/spawn-list action: spawn list/group 41, subtype 2
- Group/spawn-list action: spawn list/group 281, subtype 2
- Group/spawn-list action: spawn list/group 18, subtype 8, param 65538 (Waypoint 0 (tag 1), point 2)
- Group/spawn-list action: spawn list/group 41, subtype 8, param 65538 (Waypoint 0 (tag 1), point 2)
- Group/spawn-list action: spawn list/group 281, subtype 8, param 65538 (Waypoint 0 (tag 1), point 2)

### Event 23

**Trigger**

- Group/spawn-list event: subject 56, op 0, value 0 (join 2)
- Group/spawn-list event: subject 56, op 6, value 0

**Action**

- Set/add variable: variable group 21, variable 6, subtype 0, value 1

### Event 24

**Trigger**

- Variable comparison: subject variable group 21, variable 35, op 1, value 0
- Group/spawn-list event: subject 281, op 2, value 65537 (Waypoint 0 (tag 1), point 1)
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Group/spawn-list action: spawn list/group 281, subtype 8, param 131072 (Waypoint 1 (tag 2), point 0)

### Event 25

**Trigger**

- Variable comparison: subject variable group 21, variable 35, op 1, value 0
- Group/spawn-list event: subject 18, op 2, value 65537 (Waypoint 0 (tag 1), point 1)
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Group/spawn-list action: spawn list/group 18, subtype 8, param 131072 (Waypoint 1 (tag 2), point 0)

### Event 26

**Trigger**

- Variable comparison: subject variable group 21, variable 35, op 1, value 0
- Group/spawn-list event: subject 41, op 2, value 65537 (Waypoint 0 (tag 1), point 1)
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Group/spawn-list action: spawn list/group 41, subtype 8, param 131072 (Waypoint 1 (tag 2), point 0)

### Event 27

**Trigger**

- Variable comparison: subject variable group 21, variable 35, op 1, value 1
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Group/spawn-list action: spawn list/group 281, subtype 8, param 65538 (Waypoint 0 (tag 1), point 2)
- Group/spawn-list action: spawn list/group 18, subtype 8, param 65538 (Waypoint 0 (tag 1), point 2)
- Group/spawn-list action: spawn list/group 41, subtype 8, param 65538 (Waypoint 0 (tag 1), point 2)

## Waypoints

### Waypoint 0

- Tag: `1`
- Members: `GalSpan_Poseidon (object 0, id 4698, starts at point 0)`, `GalSpan_Poseidon (object 1, id 4699, starts at point 0)`, `GalSpan_Poseidon (object 2, id 4700, starts at point 0)`, `GalSpan_Pegasus (object 5, id 4692, starts at point 0)`, `GalSpan_Pegasus (object 6, id 4693, starts at point 0)`, `GalSpan_Pegasus (object 7, id 4694, starts at point 0)`, `GalSpan_Poseidon (object 8, id 4695, starts at point 0)`, `GalSpan_Poseidon (object 9, id 4696, starts at point 0)`, `GalSpan_Poseidon (object 10, id 4697, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1699.49, 0.00, 541.82) | None |
| 1 | (-354.72, 0.00, 1874.76) | None |
| 2 | (-338.64, 0.00, 1889.94) | on arrival play dialog/script or enter gate, param 4689 |

### Waypoint 1

- Tag: `2`
- Members: `Bora_Battleaxe (object 3, id 4705, starts at point 0)`, `Bora_Battleaxe (object 4, id 4704, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-64.28, 0.00, 1642.17) | None |
| 1 | (-607.37, 0.00, 2107.52) | None |
| 2 | (26.86, 0.00, 2770.64) | None |
| 3 | (596.58, 0.00, 2150.62) | on arrival redirect to Waypoint 1 (tag 2), point 0 |

## Spawn Lists

### Spawn List 0

- ID: `41`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 1

- ID: `18`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 2

- ID: `56`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 5 | spawn list 18 | None |
| 1 | 5 | spawn list 281 | None |
| 2 | 5 | spawn list 41 | None |
| 3 | 9 | none | None |

### Spawn List 3

- ID: `281`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `GalSpan_Poseidon` | 4698 | Interactive | -1926.07,-97.80,314.11 | 48,0,0 | group/role: FG_GEMINI / 1; alias: Todd08; waypoint: Waypoint 0 (tag 1, 3 point(s)), starting point 0, arrival event value 65536 |
| 1 | `GalSpan_Poseidon` | 4699 | Interactive | -1895.89,-97.80,314.11 | 48,0,0 | group/role: FG_GEMINI / 2; alias: Todd09; waypoint: Waypoint 0 (tag 1, 3 point(s)), starting point 0, arrival event value 65536 |
| 2 | `GalSpan_Poseidon` | 4700 | Interactive | -1858.51,-97.80,317.58 | 48,0,0 | group/role: FG_GEMINI / 3; alias: Todd10; waypoint: Waypoint 0 (tag 1, 3 point(s)), starting point 0, arrival event value 65536 |
| 3 | `Bora_Battleaxe` | 4705 | Interactive | 25.04,0.00,2189.08 | 256,0,0 | group/role: FG_SWORD / 2; alias: Todd13; waypoint: Waypoint 1 (tag 2, 4 point(s)), starting point 0, arrival event value 131072 |
| 4 | `Bora_Battleaxe` | 4704 | Interactive | -31.02,0.00,2118.21 | 256,0,0 | group/role: FG_SWORD / 1; alias: Todd12; waypoint: Waypoint 1 (tag 2, 4 point(s)), starting point 0, arrival event value 131072 |
| 5 | `GalSpan_Pegasus` | 4692 | Interactive | -2197.83,-97.80,375.88 | 48,0,0 | group/role: FG_PEGASI / 1; alias: Todd02; waypoint: Waypoint 0 (tag 1, 3 point(s)), starting point 0, arrival event value 65536 |
| 6 | `GalSpan_Pegasus` | 4693 | Interactive | -2161.51,-97.80,375.28 | 48,0,0 | group/role: FG_PEGASI / 2; alias: Todd03; waypoint: Waypoint 0 (tag 1, 3 point(s)), starting point 0, arrival event value 65536 |
| 7 | `GalSpan_Pegasus` | 4694 | Interactive | -2121.27,-97.80,374.52 | 48,0,0 | group/role: FG_PEGASI / 3; alias: Todd04; waypoint: Waypoint 0 (tag 1, 3 point(s)), starting point 0, arrival event value 65536 |
| 8 | `GalSpan_Poseidon` | 4695 | Interactive | -2057.72,-97.80,237.77 | 48,0,0 | group/role: FG_ATLAS / 1; alias: Todd05; waypoint: Waypoint 0 (tag 1, 3 point(s)), starting point 0, arrival event value 65536 |
| 9 | `GalSpan_Poseidon` | 4696 | Interactive | -2027.53,-97.80,241.26 | 48,0,0 | group/role: FG_ATLAS / 2; alias: Todd06; waypoint: Waypoint 0 (tag 1, 3 point(s)), starting point 0, arrival event value 65536 |
| 10 | `GalSpan_Poseidon` | 4697 | Interactive | -1987.28,-97.80,239.52 | 48,0,0 | group/role: FG_ATLAS / 3; alias: Todd07; waypoint: Waypoint 0 (tag 1, 3 point(s)), starting point 0, arrival event value 65536 |
