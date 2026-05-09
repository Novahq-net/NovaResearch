# Tachyon: The Fringe DISP04D.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP04D.SPX` |
| Sector | `QUAD_04` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 3 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 0 |
| Entities | 0 |
| Events | 2 |
| Waypoints | 0 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | None |
| Scripts | `CANST.SCR` |
| Scenes | None |
| Labels | `BFNE_01`, `CLEON`, `SPIKE` |
| Aliases | `Coward`, `spy_1`, `SPIKE` |
| Groups | None |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 1, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 5

**Action**

- Play dialog: CANST.SCR, line/variant 6
- Set runtime trigger variable: variable group 20, variable 1, subtype 1, value 0

## Waypoints

None
## Spawn Lists

None

## Objects

None
