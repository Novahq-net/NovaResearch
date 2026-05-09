# Tachyon: The Fringe FRON11G.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON11G.SPX` |
| Sector | `QUAD_11` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 10 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 1 |
| Events | 4 |
| Waypoints | 0 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Cruiser` |
| Scripts | `PRSPH.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `bfne_05`, `BFBE_04`, `bfne_01`, `bfne_03`, `bfne_02`, `bfne_04`, `bfne_06`, `bfne_08`, `bfne_07`, `bfne_09` |
| Aliases | `BC05_sistine_chapel`, `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1`, `bc05_2`, `bc05_3`, `bc05_5`, `bc05_4`, `Stocks01` |
| Groups | `PERSEPHONE` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 29, op 1, value 1

**Action**

- Object spawn/action: GalSpan_Cruiser (object 0, id 431), subtype 3
- Set runtime trigger variable: variable group 20, variable 11, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 2, param 431

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 11, op 1, value 5

**Action**

- Play dialog: PRSPH.SCR, line/variant 15

### Event 2

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 15

**Action**

- Object spawn/action: GalSpan_Cruiser (object 0, id 431), subtype 4
- Set/add variable: variable group 21, variable 29, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 16, variable 426, subtype 0, value 1
- Set/add variable: variable group 16, variable 427, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 12, param 37
- Hide/remove HUD contact: contact/list 0, subtype 2, param 431

### Event 3

**Trigger**

- Object event: subject GalSpan_Cruiser (object 0, id 431), op 2, value 0

**Action**

- Set/add variable: variable group 16, variable 426, subtype 0, value 1
- Set/add variable: variable group 16, variable 427, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 11, param 38
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Play dialog: PLAYER.SCR, line/variant 129

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `GalSpan_Cruiser` | 431 | Interactive | 315.96,0.00,2070.25 | 390,0,0 | alias: Stocks01; secondary groups: none, PERSEPHONE |
