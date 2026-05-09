# Tachyon: The Fringe FRON02A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON02A.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 5 |
| Entities | 5 |
| Events | 7 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Armon_Patroli_Black_Market_Ship`, `1: Generic_Light_Freighter`, `2: Crate_6`, `3: Junk_03`, `4: Junk_06` |
| Scripts | `ARMAN.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `SPIKE`, `Arman` |
| Aliases | `Arman` |
| Groups | `CONT_016`, `BLANK`, `CONT_027`, `OPPORTUNITY`, `CONT_044` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 24, op 1, value 1

**Action**

- Set runtime trigger variable: variable group 20, variable 9, subtype 0, value 0
- Object spawn/action: Armon_Patroli_Black_Market_Ship (object 4, id 3), subtype 8, param 4
- Gate state/action: param 2, subtype 3, param 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 1500 (extra 1, 3; flags 2)

**Action**

- Object spawn/action: Armon_Patroli_Black_Market_Ship (object 4, id 3), subtype 6

### Event 2

**Trigger**

- Object event: subject Armon_Patroli_Black_Market_Ship (object 4, id 3), op 0, value 0 (flags 2)
- Variable comparison: subject variable group 21, variable 24, op 1, value 1

**Action**

- Object spawn/action: Armon_Patroli_Black_Market_Ship (object 4, id 3), subtype 5
- Play dialog: ARMAN.SCR, line/variant 4

### Event 3

**Trigger**

- Object event: subject Armon_Patroli_Black_Market_Ship (object 4, id 3), op 4, value 50 (join 2)

**Action**

- Object spawn/action: Armon_Patroli_Black_Market_Ship (object 4, id 3), subtype 4

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 8

**Action**

- Play scene: unknown index 0, param 0
- Play dialog: ARMAN.SCR, line/variant 0
- Mission objective/state: param 262153, subtype 0, param 0
- Set/add variable: variable group 21, variable 25, subtype 0, value 0
- Broadcast hide/remove contact: contact/list 0, subtype 0, param 47
- Broadcast hide/remove contact: contact/list 0, subtype 0, param 29

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 266; flags 2)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 500
- Play dialog: PLAYER.SCR, line/variant 145
- Show/update HUD contact: contact/list 0, subtype 9, param 41
- Set runtime trigger variable: variable group 20, variable 22, subtype 0, value 0

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 22, op 1, value 5

**Action**

- Set runtime trigger variable: variable group 20, variable 23, subtype 1, value 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 41

## Waypoints

### Waypoint 0

- Tag: `1`
- Members: `Armon_Patroli_Black_Market_Ship (object 4, id 3, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1218.13, -330.33, 2217.37) | None |
| 1 | (160.26, -330.33, 2628.08) | None |
| 2 | (-1476.51, -330.33, 2658.21) | None |
| 3 | (-2492.15, -330.33, 1295.51) | None |
| 4 | (-2174.76, 0.00, -647.93) | on arrival redirect to Waypoint 0 (tag 1), point 0 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Junk_06` | 257 | Object | 3429.64,4203.20,-3018.63 | 256,0,0 | Scale/Radius: 1.00 |
| 1 | `Junk_03` | 261 | Object | 3451.05,4203.20,-3038.27 | 0,0,0 | Scale/Radius: 1.00 |
| 2 | `Crate_6` | 266 | Interactive | 3439.57,4200.99,-3043.73 | 0,0,0 | secondary groups: CONT_016, none |
| 3 | `Generic_Light_Freighter` | 256 | Interactive | 3443.80,4203.23,-3038.65 | 0,0,0 | label: SPIKE; secondary groups: CONT_027, BLANK |
| 4 | `Armon_Patroli_Black_Market_Ship` | 3 | Interactive | 1992.18,-330.33,1637.48 | 448,0,0 | label: Arman; group/role: none / 1; alias: Arman; secondary groups: CONT_044, OPPORTUNITY; waypoint: Waypoint 0 (tag 1, 5 point(s)), starting point 0, arrival event value 65536 |
