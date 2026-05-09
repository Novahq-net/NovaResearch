# Tachyon: The Fringe DISP08.SPX - The Final Assault on GalSpan

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP08.SPX` |
| Sector | `QUAD_08` |
| Backdrop | `DISPUT8.BDF` |
| Region | 6 |
| Sector ID | 7 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 5 |
| Events | 7 |
| Waypoints | 0 |
| Child Sectors | 5 |
| Scripts | 2 |
| Scenes | 2 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: DisputG_StarBase`, `1: Navigational_Bouy`, `2: Mega_Gate`, `3: Hyper_Gate` |
| Scripts | `TRISH.SCR`, `PLAYER.SCR` |
| Scenes | `RIP2GAL.SEN`, `RIP2MYS.SEN` |
| Labels | `SPIKE` |
| Aliases | `spy_1`, `SPIKE` |
| Groups | `HELLAS_STARBASE` |
| Child Sectors | [disp08B.spx](DISP08B.md), [disp08C.spx](DISP08C.md), [disp08D.spx](DISP08D.md), [disp08E.spx](DISP08E.md), [disp08F.spx](DISP08F.md) |

## Events

### Event 0

**Trigger**

- Variable comparison: subject variable group 0, variable 4, op 1, value 3005

**Action**

- Mission objective/state: param 393218, subtype 0, param 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 0, variable 4, op 1, value 3005
- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 9, subtype 0, value 0
- Gate state/action: param 2, subtype 3, param 0

### Event 2

**Trigger**

- Variable comparison: subject variable group 0, variable 4, op 1, value 3005
- Variable comparison: subject variable group 20, variable 9, op 1, value 15

**Action**

- Play dialog: TRISH.SCR, line/variant 0
- Set runtime trigger variable: variable group 20, variable 9, subtype 1, value 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 0, variable 4, op 1, value 3008

**Action**

- Mission objective/state: param 393221, subtype 0, param 0

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 3010

**Action**

- Mission objective/state: param 393222, subtype 0, param 0
- Gate state/action: param 2, subtype 3, param 0

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4031

**Action**

- Gate state/action: param 2, subtype 3, param 0
- Mission objective/state: param 393217, subtype 0, param 0

### Event 6

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 0, op 0, value 1
- Variable comparison: subject variable group 0, variable 4, op 1, value 4018

**Action**

- Mission objective/state: param 393216, subtype 0, param 0
- Gate state/action: param 2, subtype 3, param 0
- Play dialog: PLAYER.SCR, line/variant 97

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | -1234.78,131.99,-2623.06 | 0,0,0 | Gate SPX: [disp04.spx](DISP04.md) |
| 1 | `Mega_Gate` | 2 | Gate | 479.81,-684.80,-423.24 | 0,0,0 | Gate SPX: [gals06.spx](GALS06.md) |
| 2 | `none` | 6 | Marker | -1211.51,-200.00,-1493.62 | 0,0,0 | None |
| 3 | `Navigational_Bouy` | 10 | Interactive | -1143.03,-111.64,-1237.73 | 0,0,0 | secondary groups: none, HELLAS_STARBASE |
| 4 | `DisputG_StarBase` | 3 | Interactive | -644.69,0.00,-736.67 | 64,0,0 | None |
