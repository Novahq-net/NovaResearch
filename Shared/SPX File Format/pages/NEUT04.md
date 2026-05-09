# Tachyon: The Fringe NEUT04.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT04.SPX` |
| Sector | `QUAD_04` |
| Backdrop | `NEUTRA4.BDF` |
| Region | 1 |
| Sector ID | 3 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 5 |
| Events | 8 |
| Waypoints | 0 |
| Child Sectors | 5 |
| Scripts | 1 |
| Scenes | 1 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Mad_Pirate_Platform`, `1: Bora_Indep_Construc_Facility`, `2: Independent_Shipyard`, `3: Hyper_Gate` |
| Scripts | `DRAKE.SCR` |
| Scenes | `H4BC012A.SEN` |
| Labels | `bfne_06`, `BFBE_03`, `MISHK`, `HESPE`, `Merch` |
| Aliases | `Courage`, `kwI03_02`, `kwI03_03`, `kwi03_7`, `Jerome24`, `Jerome25`, `Jerome26`, `Jerome22`, `Jerome21`, `Jerome20`, `Intrepid`, `Artemis`, `KWi03_10`, `Hermes` |
| Groups | `LAREFF_REPAIR`, `DRAKE_FACILITY` |
| Child Sectors | [neut04A.spx](NEUT04A.md), [neut04B.spx](NEUT04B.md), [neut04C.spx](NEUT04C.md), [neut04D.spx](NEUT04D.md), [neut04E.spx](NEUT04E.md) |

## Events

### Event 0

**Trigger**

- Object event: subject Bora_Indep_Construc_Facility (object 3, id 1270), op 14, value 82

**Action**

- Set/add variable: variable group 21, variable 19, subtype 0, value 1

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 2000 (extra 1, 1552; flags 2)
- Variable comparison: subject variable group 8, variable 25, op 2, value 0

**Action**

- Play dialog: DRAKE.SCR, line/variant 9

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1552; flags 6)
- Variable comparison: subject variable group 8, variable 25, op 1, value 1 (flags 4)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 300
- Show/update HUD contact: contact/list 0, subtype 9, param 35
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1552; flags 6)
- Variable comparison: subject variable group 8, variable 25, op 1, value 2 (flags 4)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 600
- Show/update HUD contact: contact/list 0, subtype 9, param 35
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1552; flags 6)
- Variable comparison: subject variable group 8, variable 25, op 1, value 3 (flags 4)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 900
- Show/update HUD contact: contact/list 0, subtype 9, param 35
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1552; flags 6)
- Variable comparison: subject variable group 8, variable 25, op 1, value 4 (flags 4)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 1200
- Show/update HUD contact: contact/list 0, subtype 9, param 35
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 6

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1552; flags 6)
- Variable comparison: subject variable group 8, variable 25, op 2, value 4 (flags 4)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 1500
- Show/update HUD contact: contact/list 0, subtype 9, param 35
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 7

**Trigger**

- Variable comparison: subject variable group 20, variable 32, op 2, value 10 (flags 4)

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 35
- Set/add variable: variable group 20, variable 32, subtype 0, value 0

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 7 | Gate | 0.00,500.00,1709.45 | 256,0,0 | Gate SPX: [neut08.spx](NEUT08.md) |
| 1 | `Hyper_Gate` | 8 | Gate | -4.84,0.00,-2909.40 | 0,0,0 | Gate SPX: [neut01.spx](NEUT01.md) |
| 2 | `Independent_Shipyard` | 1219 | Interactive | 2619.17,150.00,-2011.49 | 128,0,0 | secondary groups: none, LAREFF_REPAIR |
| 3 | `Bora_Indep_Construc_Facility` | 1270 | Interactive | 0.00,0.00,0.00 | 0,0,0 | secondary groups: none, DRAKE_FACILITY |
| 4 | `Mad_Pirate_Platform` | 1552 | Interactive | -497.80,529.67,-121.03 | 0,0,0 | None |
