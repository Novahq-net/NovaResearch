# Tachyon: The Fringe MYST06C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST06C.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `(none)` |
| Region | 5 |
| Sector ID | 5 |
| SectorHazardFlags | Twilight fog / fog-radar impairment (0x00000002) |
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
| Scripts | `PLAYER.SCR`, `ANNAH.SCR` |
| Scenes | None |
| Labels | `PISCE`, `RALPH` |
| Aliases | `PISCES1`, `PISCES2`, `pisces3`, `pisces4`, `stocks02` |
| Groups | None |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 0, variable 4, op 1, value 2009

**Action**

- Gate state/action: param 4, subtype 3, param 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 8, variable 7, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 22

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 17, variable 402, op 1, value 1
- Variable comparison: subject variable group 17, variable 403, op 1, value 2

**Action**

- Play dialog: ANNAH.SCR, line/variant 1
- Play scene: unknown index 0, param 1

## Waypoints

None
## Spawn Lists

None

## Objects

None
