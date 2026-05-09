# Tachyon: The Fringe BORA07B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `BORA07B.SPX` |
| Sector | `QUAD_07` |
| Backdrop | `(none)` |
| Region | 3 |
| Sector ID | 6 |
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
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | None |
| Aliases | None |
| Groups | None |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 0, variable 7, op 1, value 10

**Action**

- Play dialog: PLAYER.SCR, line/variant 49

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (join 1)
- Variable comparison: subject variable group 0, variable 7, op 1, value 10

**Action**

- Play dialog: PLAYER.SCR, line/variant 44

## Waypoints

None
## Spawn Lists

None

## Objects

None
