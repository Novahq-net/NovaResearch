# Tachyon: The Fringe GALS05.SPX - Missing Squadron; Bonus Incentive Program

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `GALS05.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `GALSPA5.BDF` |
| Region | 2 |
| Sector ID | 4 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 4 |
| Events | 6 |
| Waypoints | 0 |
| Child Sectors | 3 |
| Scripts | 0 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Medical_Facility`, `1: GalSpan_Research_Facility`, `2: Hyper_Gate` |
| Scripts | None |
| Scenes | None |
| Labels | `bfne_02`, `BFGE_04`, `bfne_03`, `bfgf_02`, `bfne_08`, `bfge_02` |
| Aliases | `wing_man` |
| Groups | `APOLLO_RESEARCH`, `THETIS_MEDICAL` |
| Child Sectors | [gals05A.spx](GALS05A.md), [gals05B.spx](GALS05B.md), [gals05C.spx](GALS05C.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 17; join 1; flags 6)
- Variable comparison: subject variable group 8, variable 23, op 1, value 1 (flags 4)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 650
- Set/add variable: variable group 8, variable 23, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 22
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 17; flags 6)
- Variable comparison: subject variable group 8, variable 23, op 1, value 2 (flags 4)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 1300
- Set/add variable: variable group 8, variable 23, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 22
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 17; flags 6)
- Variable comparison: subject variable group 8, variable 23, op 1, value 3 (flags 4)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 1950
- Set/add variable: variable group 8, variable 23, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 22
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 17; flags 6)
- Variable comparison: subject variable group 8, variable 23, op 1, value 4 (flags 4)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 2600
- Set/add variable: variable group 8, variable 23, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 22
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 17; flags 6)
- Variable comparison: subject variable group 8, variable 23, op 2, value 4 (flags 4)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 3250
- Set/add variable: variable group 8, variable 23, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 22
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 32, op 2, value 10 (flags 4)

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 22
- Set/add variable: variable group 20, variable 32, subtype 0, value 0

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | -596.90,83.49,80.56 | 0,0,0 | Gate SPX: [Gals01.spx](GALS01.md) |
| 1 | `Hyper_Gate` | 2 | Gate | 772.33,-145.66,140.85 | 491,0,0 | Gate SPX: [Gals06.spx](GALS06.md) |
| 2 | `GalSpan_Research_Facility` | 17 | Interactive | 1958.68,746.86,528.51 | 0,0,0 | secondary groups: none, APOLLO_RESEARCH |
| 3 | `Medical_Facility` | 18 | Interactive | -848.87,-308.70,1692.35 | 256,0,0 | secondary groups: none, THETIS_MEDICAL |
