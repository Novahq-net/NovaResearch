# Tachyon: The Fringe EARTH03B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH03B.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `(none)` |
| Region | 0 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 0 |
| Entities | 0 |
| Events | 4 |
| Waypoints | 0 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | None |
| Scripts | `PLAYER.SCR`, `DILL.SCR` |
| Scenes | None |
| Labels | `SHUT`, `bfnf_03`, `PLAYER`, `ORION03`, `ORION02`, `ORION01`, `PEGASUS01`, `PEGASUS02`, `PEGASUS03`, `MAKO01`, `MAKO03`, `PIRANHA01`, `PIRANHA02`, `PIRANHA03`, `PIRANHA04`, `DART01`, `DART02`, `DART03`, `DART04`, `FRGT`, `CPSH`, `SAMA`, `FREIGHT01` |
| Aliases | `fred2`, `fred1`, `fred3` |
| Groups | None |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 25

**Action**

- Play dialog: PLAYER.SCR, line/variant 23
- Set runtime trigger variable: variable group 20, variable 0, subtype 1, value 0

### Event 2

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 23
- Variable comparison: subject variable group 5, variable 14, op 1, value 0

**Action**

- Play dialog: DILL.SCR, line/variant 27

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Mission objective/state: param 0, subtype 0, param 0

## Waypoints

None
## Spawn Lists

None

## Objects

None
