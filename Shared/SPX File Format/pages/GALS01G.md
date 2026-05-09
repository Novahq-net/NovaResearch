# Tachyon: The Fringe GALS01G.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `GALS01G.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 2 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 15 |
| Events | 20 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Frigate`, `1: GalSpan_Poseidon`, `2: GalSpan_Pegasus`, `3: GalSpan_Orion` |
| Scripts | `MARTE.SCR`, `ADHAG.SCR` |
| Scenes | None |
| Labels | `bfge_02` |
| Aliases | `stocks01`, `Jerome10`, `Jerome11`, `Jerome09`, `Jerome08`, `Jerome07`, `Jerome12`, `frank05`, `frank06`, `frank07`, `frank08`, `wing_man`, `stocks02`, `stocks03`, `stocks04`, `frank10` |
| Groups | `FG_GRUS`, `FG_ATLAS`, `FG_ARES`, `FG_LEPUS`, `DEMETER`, `CONT_026` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Gate state/action: param 1, subtype 3, param 0
- Gate state/action: param 2, subtype 3, param 0
- Gate state/action: param 3, subtype 3, param 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Area/player/sector/dock/time event: subject 0, op 9, value 0
- Variable comparison: subject variable group 0, variable 7, op 1, value 13

**Action**

- Set runtime trigger variable: variable group 20, variable 1, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 13

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 4

**Action**

- Play dialog: MARTE.SCR, line/variant 0

### Event 3

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 0

**Action**

- Gate state/action: param 1, subtype 2, param 0
- Gate state/action: param 2, subtype 2, param 0
- Gate state/action: param 3, subtype 2, param 0

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Area/player/sector/dock/time event: subject 0, op 9, value 0 (join 1)
- Variable comparison: subject variable group 0, variable 7, op 1, value 13

**Action**

- Set runtime trigger variable: variable group 20, variable 3, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 13

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 3, op 1, value 4

**Action**

- Play dialog: MARTE.SCR, line/variant 1

### Event 6

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 1

**Action**

- Group/spawn-list action: spawn list/group 241, subtype 0

### Event 7

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 1 (join 2)
- Group/spawn-list event: subject 241, op 2, value 26279937 (Waypoint 1 (tag 401), point 1)

**Action**

- Gate state/action: param 1, subtype 2, param 0
- Gate state/action: param 2, subtype 2, param 0
- Gate state/action: param 3, subtype 2, param 0

### Event 8

**Trigger**

- Object event: subject GalSpan_Orion (object 0, id 214), op 7, value 0
- Object event: subject GalSpan_Orion (object 1, id 215), op 7, value 0
- Object event: subject GalSpan_Orion (object 2, id 216), op 7, value 0
- Object event: subject GalSpan_Orion (object 3, id 217), op 7, value 0

**Action**

- Set/add variable: variable group 21, variable 21, subtype 1, value 1

### Event 9

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 13

### Event 10

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 5

**Action**

- Group/spawn-list action: spawn list/group 16, subtype 0
- Group/spawn-list action: spawn list/group 18, subtype 0
- Group/spawn-list action: spawn list/group 176, subtype 0
- Object spawn/action: GalSpan_Frigate (object 14, id 213), subtype 8, param 1
- Show/update HUD contact: contact/list 0, subtype 9, param 19

### Event 11

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 20, variable 0, op 1, value 5

**Action**

- Object spawn/action: GalSpan_Frigate (object 14, id 213), subtype 5

### Event 12

**Trigger**

- Object event: subject GalSpan_Frigate (object 14, id 213), op 14, value 21
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Play dialog: ADHAG.SCR, line/variant 5
- Set/add variable: variable group 14, variable 412, subtype 0, value 1
- Set/add variable: variable group 14, variable 413, subtype 0, value 2
- Hide/remove HUD contact: contact/list 0, subtype 9, param 19
- Show/update HUD contact: contact/list 0, subtype 12, param 20
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 13

**Trigger**

- Object event: subject GalSpan_Frigate (object 14, id 213), op 14, value 21
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Object spawn/action: GalSpan_Frigate (object 14, id 213), subtype 6
- Object spawn/action: GalSpan_Frigate (object 14, id 213), subtype 8, param 2

### Event 14

**Trigger**

- Object event: subject GalSpan_Frigate (object 14, id 213), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Set/add variable: variable group 21, variable 22, subtype 1, value 1

### Event 15

**Trigger**

- Variable comparison: subject variable group 21, variable 22, op 1, value 1
- Object event: subject GalSpan_Frigate (object 14, id 213), op 16, value 0

**Action**

- Play dialog: ADHAG.SCR, line/variant 4
- Set/add variable: variable group 14, variable 412, subtype 0, value 1
- Set/add variable: variable group 14, variable 413, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 19
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 21

### Event 16

**Trigger**

- Object event: subject GalSpan_Frigate (object 14, id 213), op 8, value 0
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Play dialog: ADHAG.SCR, line/variant 6
- Set/add variable: variable group 14, variable 800, subtype 0, value 1
- Set/add variable: variable group 14, variable 413, subtype 0, value 3
- Set/add variable: variable group 14, variable 412, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 19

### Event 17

**Trigger**

- Object event: subject GalSpan_Frigate (object 14, id 213), op 8, value 0
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 12, param 20
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 18

**Trigger**

- Object event: subject GalSpan_Frigate (object 14, id 213), op 0, value 0 (flags 2)
- Variable comparison: subject variable group 21, variable 20, op 3, value 0

**Action**

- Object spawn/action: GalSpan_Frigate (object 14, id 213), subtype 8, param 1
- Group/spawn-list action: spawn list/group 241, subtype 4, param 1
- Group/spawn-list action: spawn list/group 241, subtype 2

### Event 19

**Trigger**

- Group/spawn-list event: subject 241, op 0, value 0

**Action**

- Set/add variable: variable group 21, variable 24, subtype 1, value 1

## Waypoints

### Waypoint 0

- Tag: `402`
- Members: `GalSpan_Frigate (object 14, id 213, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (913.78, 310.93, 1683.03) | None |
| 1 | (1674.50, 309.96, 2172.46) | on arrival action 1, param -1 |

### Waypoint 1

- Tag: `401`
- Members: `GalSpan_Orion (object 0, id 214, starts at point 0)`, `GalSpan_Orion (object 1, id 215, starts at point 0)`, `GalSpan_Orion (object 2, id 216, starts at point 0)`, `GalSpan_Orion (object 3, id 217, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (736.38, 155.93, 1701.16) | None |
| 1 | (577.54, 12.08, 1151.01) | on arrival play dialog/script or enter gate, param 2 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `GalSpan_Orion` | 214 | Interactive | 781.04,315.22,1749.26 | 306,0,0 | group/role: FG_GRUS / 1; alias: frank05; waypoint: Waypoint 1 (tag 401, 2 point(s)), starting point 0, arrival event value 26279936 |
| 1 | `GalSpan_Orion` | 215 | Interactive | 832.58,315.22,1755.47 | 306,0,0 | group/role: FG_GRUS / 2; alias: frank06; waypoint: Waypoint 1 (tag 401, 2 point(s)), starting point 0, arrival event value 26279936 |
| 2 | `GalSpan_Orion` | 216 | Interactive | 770.05,315.22,1812.19 | 306,0,0 | group/role: FG_GRUS / 3; alias: frank07; waypoint: Waypoint 1 (tag 401, 2 point(s)), starting point 0, arrival event value 26279936 |
| 3 | `GalSpan_Orion` | 217 | Interactive | 840.04,315.22,1841.96 | 306,0,0 | group/role: FG_GRUS / 4; alias: frank08; waypoint: Waypoint 1 (tag 401, 2 point(s)), starting point 0, arrival event value 26279936 |
| 4 | `GalSpan_Orion` | 268 | Interactive | 1418.41,0.00,2174.80 | 306,0,0 | group/role: FG_ATLAS / 1 |
| 5 | `GalSpan_Orion` | 269 | Interactive | 1410.66,0.00,2229.51 | 299,0,0 | group/role: FG_ATLAS / 2 |
| 6 | `GalSpan_Orion` | 270 | Interactive | 1467.52,0.00,2184.44 | 306,0,0 | group/role: FG_ATLAS / 3 |
| 7 | `GalSpan_Pegasus` | 274 | Interactive | 450.35,0.00,597.50 | 0,0,0 | group/role: FG_ARES / 1 |
| 8 | `GalSpan_Pegasus` | 275 | Interactive | 433.72,0.00,598.47 | 0,0,0 | group/role: FG_ARES / 2 |
| 9 | `GalSpan_Pegasus` | 276 | Interactive | 408.78,0.00,565.31 | 0,0,0 | group/role: FG_ARES / 3 |
| 10 | `GalSpan_Pegasus` | 277 | Interactive | 468.16,0.00,552.43 | 0,0,0 | group/role: FG_ARES / 4 |
| 11 | `GalSpan_Poseidon` | 271 | Interactive | -438.48,0.00,1695.59 | 149,0,0 | group/role: FG_LEPUS / 1 |
| 12 | `GalSpan_Poseidon` | 272 | Interactive | -478.41,0.00,1668.07 | 156,0,0 | group/role: FG_LEPUS / 2 |
| 13 | `GalSpan_Poseidon` | 273 | Interactive | -465.85,0.00,1732.06 | 164,0,0 | group/role: FG_LEPUS / 3 |
| 14 | `GalSpan_Frigate` | 213 | Interactive | 575.88,310.43,1487.46 | 85,0,0 | alias: frank10; secondary groups: CONT_026, DEMETER; waypoint: Waypoint 0 (tag 402, 2 point(s)), starting point 0, arrival event value 26345472 |
