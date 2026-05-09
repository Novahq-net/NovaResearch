# Tachyon: The Fringe MYST01.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST01.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `MYSTER1.BDF` |
| Region | 5 |
| Sector ID | 0 |
| SectorHazardFlags | Twilight fog / fog-radar impairment (0x00000002) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 5 |
| Events | 10 |
| Waypoints | 0 |
| Child Sectors | 5 |
| Scripts | 2 |
| Scenes | 2 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Outworlds_StarBase`, `1: Spcargo_Credits`, `2: Navigational_Bouy`, `3: Hyper_Gate` |
| Scripts | `TRISH.SCR`, `PLAYER.SCR` |
| Scenes | `MYS2FRON.SEN`, `MYS2RIP.SEN` |
| Labels | `bfne_07`, `bfbf_07`, `bfgf_05` |
| Aliases | None |
| Groups | `DEEP_FRINGE_ARRAY_STARBASE`, `CONT_071` |
| Child Sectors | [myst01A.spx](MYST01A.md), [myst01B.spx](MYST01B.md), [myst01C.spx](MYST01C.md), [myst01D.spx](MYST01D.md), [myst01E.spx](MYST01E.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 2009

**Action**

- Mission objective/state: param 327684, subtype 0, param 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 3009

**Action**

- Mission objective/state: param 327686, subtype 0, param 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4019

**Action**

- Mission objective/state: param 327685, subtype 0, param 0

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4024

**Action**

- Mission objective/state: param 327682, subtype 0, param 0

### Event 4

**Trigger**

- Variable comparison: subject variable group 0, variable 4, op 0, value 4028
- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Mission objective/state: param 327681, subtype 0, param 0

### Event 5

**Trigger**

- Variable comparison: subject variable group 0, variable 4, op 1, value 3007

**Action**

- Mission objective/state: param 327683, subtype 0, param 0

### Event 6

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 9, value 0
- Variable comparison: subject variable group 0, variable 4, op 0, value 3007

**Action**

- Play dialog: TRISH.SCR, line/variant 0

### Event 7

**Trigger**

- Variable comparison: subject variable group 17, variable 403, op 0, value 2

**Action**

- Set/add variable: variable group 22, variable 23, subtype 0, value 1

### Event 8

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 223; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 130
- Set/add variable: variable group 0, variable 2, subtype 1, value 5000
- Show/update HUD contact: contact/list 0, subtype 9, param 31
- Set/add variable: variable group 17, variable 804, subtype 0, value 1
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 9

**Trigger**

- Variable comparison: subject variable group 20, variable 32, op 2, value 10

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 31
- Set/add variable: variable group 20, variable 32, subtype 0, value 0

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 60 | Gate | -446.90,2085.70,1183.17 | 0,0,0 | Gate SPX: [myst06.spx](MYST06.md) |
| 1 | `none` | 211 | Marker | 93.38,0.00,1242.98 | 0,0,0 | None |
| 2 | `Navigational_Bouy` | 217 | Interactive | 0.23,367.16,1099.12 | 0,0,0 | secondary groups: none, DEEP_FRINGE_ARRAY_STARBASE |
| 3 | `Spcargo_Credits` | 223 | Interactive | -1428.51,75.93,291.22 | 50,434,85 | secondary groups: CONT_071, none |
| 4 | `Outworlds_StarBase` | 59 | Interactive | 4.17,0.00,-53.00 | 0,0,0 | None |
