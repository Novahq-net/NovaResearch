# Tachyon: The Fringe MYST01B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST01B.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 5 |
| Sector ID | 0 |
| SectorHazardFlags | Twilight fog / fog-radar impairment (0x00000002) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 1 |
| Events | 3 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Lt_Freighter` |
| Scripts | `PLAYER.SCR`, `TRISH.SCR` |
| Scenes | None |
| Labels | `bfne_07`, `bfbf_07`, `bfgf_05` |
| Aliases | None |
| Groups | `CONT_UNKNOWN` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Object spawn/action: GalSpan_Lt_Freighter (object 0, id 193), subtype 12
- Set runtime trigger variable: variable group 20, variable 9, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 3

**Action**

- Play dialog: PLAYER.SCR, line/variant 45

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 9, value 0
- Sector/startup condition family: subject 0, op 0, value 45

**Action**

- Play dialog: TRISH.SCR, line/variant 4

## Waypoints

### Waypoint 0

- Tag: `151`
- Members: `GalSpan_Lt_Freighter (object 0, id 193, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1949.11, -145.44, 2397.90) | on arrival action 1, param -1 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `GalSpan_Lt_Freighter` | 193 | Interactive | 1157.82,-145.44,1609.36 | 63,0,0 | label: bfgf_05; secondary groups: CONT_UNKNOWN, none; waypoint: Waypoint 0 (tag 151, 1 point(s)), starting point 0, arrival event value 9895936 |
