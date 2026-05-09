# Tachyon: The Fringe FRON08D.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON08D.SPX` |
| Sector | `QUAD_08` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 7 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 0 |
| Entities | 0 |
| Events | 1 |
| Waypoints | 0 |
| Child Sectors | 0 |
| Scripts | 0 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | None |
| Scripts | None |
| Scenes | None |
| Labels | `bfne_03`, `bfne_01`, `HSLAV`, `BFGE_01`, `CHAPEL` |
| Aliases | `Jerome01`, `Jerome02`, `Jerome03`, `Jerome04`, `Jerome05`, `Jerome06`, `bc05_2`, `bc05_1`, `bc05_4`, `bc05_5`, `BC05_Sistine_Chapel` |
| Groups | None |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 2

**Action**

- Set/add variable: variable group 16, variable 420, subtype 0, value 1
- Set/add variable: variable group 16, variable 421, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 11, param 38
- Show/update HUD contact: contact/list 0, subtype 8, param 0

## Waypoints

None
## Spawn Lists

None

## Objects

None
