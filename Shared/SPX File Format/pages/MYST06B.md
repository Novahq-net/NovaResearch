# Tachyon: The Fringe MYST06B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST06B.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `(none)` |
| Region | 5 |
| Sector ID | 5 |
| SectorHazardFlags | Twilight fog / fog-radar impairment (0x00000002) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 4 |
| Events | 2 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Archangel` |
| Scripts | `PISCE.SCR` |
| Scenes | None |
| Labels | `PISCE`, `RALPH` |
| Aliases | `PISCES1`, `PISCES2`, `pisces3`, `pisces4`, `stocks02` |
| Groups | `FG_PISCES` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Gate state/action: param 4, subtype 3, param 0
- Set runtime trigger variable: variable group 20, variable 10, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 10, op 1, value 5

**Action**

- Play dialog: PISCE.SCR, line/variant 0
- Set runtime trigger variable: variable group 20, variable 10, subtype 1, value 0

## Waypoints

### Waypoint 0

- Tag: `151`
- Members: `GalSpan_Archangel (object 0, id 5, starts at point 0)`, `GalSpan_Archangel (object 1, id 6, starts at point 0)`, `GalSpan_Archangel (object 2, id 43, starts at point 0)`, `GalSpan_Archangel (object 3, id 44, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (70.22, -54.36, -203.08) | None |
| 1 | (278.93, -195.61, -179.01) | None |
| 2 | (636.47, -295.61, -527.40) | on arrival play dialog/script or enter gate, param 3 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `GalSpan_Archangel` | 5 | Interactive | 15.97,-54.33,-198.66 | 108,0,0 | label: PISCE; group/role: FG_PISCES / 1; alias: PISCES1; waypoint: Waypoint 0 (tag 151, 3 point(s)), starting point 0, arrival event value 9895936 |
| 1 | `GalSpan_Archangel` | 6 | Interactive | -8.50,-54.33,-240.92 | 107,0,0 | group/role: FG_PISCES / 2; alias: PISCES2; waypoint: Waypoint 0 (tag 151, 3 point(s)), starting point 0, arrival event value 9895936 |
| 2 | `GalSpan_Archangel` | 43 | Interactive | -80.63,-54.33,-226.34 | 108,0,0 | group/role: FG_PISCES / 3; alias: pisces3; waypoint: Waypoint 0 (tag 151, 3 point(s)), starting point 0, arrival event value 9895936 |
| 3 | `GalSpan_Archangel` | 44 | Interactive | -93.55,-54.33,-284.73 | 108,0,0 | group/role: FG_PISCES / 4; alias: pisces4; waypoint: Waypoint 0 (tag 151, 3 point(s)), starting point 0, arrival event value 9895936 |
