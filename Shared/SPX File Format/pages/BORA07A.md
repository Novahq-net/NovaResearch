# Tachyon: The Fringe BORA07A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `BORA07A.SPX` |
| Sector | `QUAD_07` |
| Backdrop | `(none)` |
| Region | 3 |
| Sector ID | 6 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 0 |
| Entities | 0 |
| Events | 3 |
| Waypoints | 0 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | None |
| Scripts | `ANNAH.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | None |
| Aliases | None |
| Groups | None |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Play dialog: ANNAH.SCR, line/variant 3

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 29, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 16

### Event 2

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 16

**Action**

- Play dialog: PLAYER.SCR, line/variant 115

## Waypoints

None
## Spawn Lists

None

## Objects

None
