# Tachyon: The Fringe BORA04.SPX - Offline Mines

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `BORA04.SPX` |
| Sector | `QUAD_04` |
| Backdrop | `BORA4.BDF` |
| Region | 3 |
| Sector ID | 3 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 5 |
| Entities | 6 |
| Events | 6 |
| Waypoints | 1 |
| Child Sectors | 1 |
| Scripts | 0 |
| Scenes | 1 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Mad_Pirate_Platform`, `1: Medical_Facility`, `2: Bora_Warhammer`, `3: Bora_Shuttle_Medium`, `4: Hyper_Gate` |
| Scripts | None |
| Scenes | `B4BC060A.SEN` |
| Labels | `BFBE_09`, `BFBF_09`, `dummy` |
| Aliases | None |
| Groups | `FG_ROVER`, `CONT_002`, `CONT_041`, `FG_TRIDENT`, `MERCY_FACILITY` |
| Child Sectors | [bora04A.spx](BORA04A.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 354; flags 6)
- Variable comparison: subject variable group 8, variable 22, op 1, value 1 (flags 4)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 550
- Set/add variable: variable group 8, variable 22, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 21
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 354; flags 6)
- Variable comparison: subject variable group 8, variable 22, op 1, value 2 (flags 4)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 1100
- Set/add variable: variable group 8, variable 22, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 21
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 354; flags 6)
- Variable comparison: subject variable group 8, variable 22, op 1, value 3 (flags 4)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 1650
- Set/add variable: variable group 8, variable 22, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 21
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 354; flags 6)
- Variable comparison: subject variable group 8, variable 22, op 1, value 4 (flags 4)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 2200
- Set/add variable: variable group 8, variable 22, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 21
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 354; flags 6)
- Variable comparison: subject variable group 8, variable 22, op 2, value 4

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 2750
- Set/add variable: variable group 8, variable 22, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 21
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 32, op 2, value 10 (flags 4)

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 21
- Set/add variable: variable group 20, variable 32, subtype 0, value 0

## Waypoints

### Waypoint 0

- Tag: `104`
- Members: `Bora_Shuttle_Medium (object 1, id 170, starts at point 0)`, `Bora_Shuttle_Medium (object 2, id 171, starts at point 3)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1871.08, 542.04, 3829.28) | None |
| 1 | (-2033.82, 542.04, 2170.17) | None |
| 2 | (-434.80, 0.00, 3029.88) | None |
| 3 | (1135.04, 0.00, 2248.84) | None |
| 4 | (1071.86, 0.00, 3921.55) | on arrival activate current object (raw param -1 ignored) |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 4 | Gate | -153.22,-1215.13,6008.16 | 256,38,0 | Gate SPX: [bora01.spx](BORA01.md) |
| 1 | `Bora_Shuttle_Medium` | 170 | Interactive | -497.47,0.00,4715.93 | 128,0,0 | label: BFBF_09; group/role: FG_ROVER / 0; secondary groups: CONT_002, none; waypoint: Waypoint 0 (tag 104, 5 point(s)), starting point 0, arrival event value 6815744 |
| 2 | `Bora_Shuttle_Medium` | 171 | Interactive | 921.38,0.00,2200.33 | 0,0,0 | group/role: FG_ROVER / 0; secondary groups: CONT_041, none; waypoint: Waypoint 0 (tag 104, 5 point(s)), starting point 3, arrival event value 6815747 |
| 3 | `Bora_Warhammer` | 172 | Interactive | -876.36,0.00,5365.47 | 256,0,0 | group/role: FG_TRIDENT / 0 |
| 4 | `Medical_Facility` | 352 | Interactive | 555.27,-142.00,5169.61 | 0,0,0 | secondary groups: none, MERCY_FACILITY |
| 5 | `Mad_Pirate_Platform` | 354 | Interactive | 555.42,-142.15,5169.96 | 0,0,0 | None |
