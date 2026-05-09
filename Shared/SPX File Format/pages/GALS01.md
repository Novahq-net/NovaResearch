# Tachyon: The Fringe GALS01.SPX - The Review; Final Payment

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `GALS01.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `GALSPA1.BDF` |
| Region | 2 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 7 |
| Events | 8 |
| Waypoints | 0 |
| Child Sectors | 9 |
| Scripts | 1 |
| Scenes | 4 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_StarBase`, `1: Navigational_Bouy`, `2: Mega_Gate`, `3: Hyper_Gate` |
| Scripts | `PLAYER.SCR` |
| Scenes | `GAL_INT1.SEN`, `GAL2HUB.SEN`, `GAL2RIP.SEN`, `GAL2FRON.SEN` |
| Labels | `bfge_02` |
| Aliases | `stocks01`, `Jerome10`, `Jerome11`, `Jerome09`, `Jerome08`, `Jerome07`, `Jerome12`, `frank05`, `frank06`, `frank07`, `frank08`, `wing_man`, `stocks02`, `stocks03`, `stocks04`, `frank10` |
| Groups | `OLYMPUS_STARBASE` |
| Child Sectors | [gals01B.spx](GALS01B.md), [gals01C.spx](GALS01C.md), [gals01D.spx](GALS01D.md), [gals01E.spx](GALS01E.md), [gals01F.spx](GALS01F.md), [gals01G.spx](GALS01G.md), [gals01H.spx](GALS01H.md), [gals01I.spx](GALS01I.md), [gals01J.spx](GALS01J.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 3004

**Action**

- Mission objective/state: param 131074, subtype 0, param 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 9, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 3004

**Action**

- Play dialog: PLAYER.SCR, line/variant 0

### Event 2

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 3004

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 1, value 0

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4021

**Action**

- Mission objective/state: param 131073, subtype 0, param 0

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4016

**Action**

- Mission objective/state: param 131076, subtype 0, param 0

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4006

**Action**

- Mission objective/state: param 131077, subtype 0, param 0

### Event 6

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 14, variable 600, op 0, value 0

**Action**

- Play scene: GAL_INT1.SEN, param 0
- Set/add variable: variable group 14, variable 600, subtype 0, value 1

### Event 7

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4015

**Action**

- Mission objective/state: param 131075, subtype 0, param 0

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | -280.12,0.00,1091.36 | 252,0,0 | Gate SPX: [Gals02.spx](GALS02.md) |
| 1 | `Hyper_Gate` | 2 | Gate | 380.87,0.00,942.71 | 307,0,0 | Gate SPX: [Gals04.spx](GALS04.md) |
| 2 | `Hyper_Gate` | 3 | Gate | 761.04,0.00,403.64 | 356,0,0 | Gate SPX: [Gals05.spx](GALS05.md) |
| 3 | `Mega_Gate` | 4 | Gate | 743.06,0.00,-433.43 | 431,0,0 | Gate SPX: [Neut08.spx](NEUT08.md) |
| 4 | `none` | 262 | Marker | 317.40,308.46,443.26 | 57,0,0 | None |
| 5 | `Navigational_Bouy` | 289 | Interactive | 266.46,357.52,534.57 | 0,0,0 | secondary groups: none, OLYMPUS_STARBASE |
| 6 | `GalSpan_StarBase` | 5 | Interactive | -259.74,0.00,25.00 | 321,0,0 | None |
