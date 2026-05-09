# Tachyon: The Fringe MYST02C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST02C.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `(none)` |
| Region | 5 |
| Sector ID | 1 |
| SectorHazardFlags | Radiation hazard (0x00000001) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 0 |
| Entities | 0 |
| Events | 3 |
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
| Aliases | `Will_02` |
| Groups | None |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Variable comparison: subject variable group 20, variable 13, op 1, value 3
- Variable comparison: subject variable group 37, variable 4, op 1, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 37

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 13, op 1, value 2
- Variable comparison: subject variable group 37, variable 4, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 38

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 13, subtype 0, value 0

## Waypoints

None
## Spawn Lists

None

## Objects

None
