# Tachyon: The Fringe NEUT02A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT02A.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 4 |
| Events | 10 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Hvy_Freighter`, `1: Bora_Cutlass` |
| Scripts | `G02BRA.SCR`, `PLAYER.SCR`, `BFIGH.SCR` |
| Scenes | None |
| Labels | `G02BFA`, `BFIGH` |
| Aliases | `fred_fighter2`, `fred_fighter1`, `fred_freighter1`, `fred_freighter2` |
| Groups | `FG_MUTINY`, `CAMEL_47`, `CONT_018`, `EXEMPTION`, `CONT_020` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 11
- Set runtime trigger variable: variable group 20, variable 25, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 25, op 1, value 3

**Action**

- Play dialog: G02BRA.SCR, line/variant 0
- Set runtime trigger variable: variable group 20, variable 25, subtype 1, value 0

### Event 2

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 29, subtype 0, value 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 29, op 1, value 2

**Action**

- Play dialog: PLAYER.SCR, line/variant 51
- Set runtime trigger variable: variable group 20, variable 29, subtype 1, value 0

### Event 4

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 51

**Action**

- Set runtime trigger variable: variable group 20, variable 29, subtype 0, value 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 11
- Mission objective/state: param 65538, subtype 0, param 0

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 29, op 1, value 4

**Action**

- Play dialog: BFIGH.SCR, line/variant 0
- Set runtime trigger variable: variable group 20, variable 29, subtype 1, value 0

### Event 6

**Trigger**

- Object event: subject Bora_Hvy_Freighter (object 2, id 3), op 8, value 0

**Action**

- Set/add variable: variable group 21, variable 2, subtype 0, value 1

### Event 7

**Trigger**

- Object event: subject Bora_Hvy_Freighter (object 3, id 11), op 8, value 0

**Action**

- Set/add variable: variable group 21, variable 3, subtype 0, value 1

### Event 8

**Trigger**

- Object event: subject Bora_Cutlass (object 0, id 34), op 2, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 53

### Event 9

**Trigger**

- Group/spawn-list event: subject 83, op 0, value 0 (join 2)
- Group/spawn-list event: subject 83, op 6, value 0 (join 2)

**Action**

- Set/add variable: variable group 21, variable 34, subtype 0, value 1

## Waypoints

### Waypoint 0

- Tag: `4`
- Members: `Bora_Cutlass (object 0, id 34, starts at point 0)`, `Bora_Cutlass (object 1, id 1474, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1608.86, 0.00, 858.16) | None |
| 1 | (-1256.44, 0.00, -254.79) | None |
| 2 | (-1949.08, 0.00, 2397.25) | on arrival redirect to Waypoint 0 (tag 4), point 1 |

### Waypoint 1

- Tag: `2`
- Members: `Bora_Hvy_Freighter (object 3, id 11, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1273.75, 0.00, 2464.62) | None |
| 1 | (-1274.73, 0.00, 2537.01) | on arrival action 1, param -1 |

### Waypoint 2

- Tag: `1`
- Members: `Bora_Hvy_Freighter (object 2, id 3, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1598.73, 0.00, 2451.22) | None |
| 1 | (-1598.89, 0.00, 2520.51) | on arrival action 1, param -1 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Bora_Cutlass` | 34 | Interactive | -2131.92,0.00,1959.32 | 0,0,0 | label: G02BFA; group/role: FG_MUTINY / 1; alias: fred_fighter2; waypoint: Waypoint 0 (tag 4, 3 point(s)), starting point 0, arrival event value 262144 |
| 1 | `Bora_Cutlass` | 1474 | Interactive | -1861.33,0.00,2068.27 | 0,0,0 | label: BFIGH; group/role: FG_MUTINY / 0; alias: fred_fighter1; waypoint: Waypoint 0 (tag 4, 3 point(s)), starting point 0, arrival event value 262144 |
| 2 | `Bora_Hvy_Freighter` | 3 | Interactive | -1599.36,0.00,2267.48 | 0,0,0 | alias: fred_freighter1; secondary groups: CONT_018, CAMEL_47; waypoint: Waypoint 2 (tag 1, 2 point(s)), starting point 0, arrival event value 65536 |
| 3 | `Bora_Hvy_Freighter` | 11 | Interactive | -1270.11,0.00,2266.54 | 0,0,0 | alias: fred_freighter2; secondary groups: CONT_020, EXEMPTION; waypoint: Waypoint 1 (tag 2, 2 point(s)), starting point 0, arrival event value 131072 |
