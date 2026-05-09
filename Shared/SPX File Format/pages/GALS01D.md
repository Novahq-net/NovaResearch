# Tachyon: The Fringe GALS01D.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `GALS01D.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 2 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 1 |
| Events | 1 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Shuttle_Medium` |
| Scripts | `TRISH.SCR` |
| Scenes | None |
| Labels | `bfge_02` |
| Aliases | `stocks01`, `Jerome10`, `Jerome11`, `Jerome09`, `Jerome08`, `Jerome07`, `Jerome12`, `frank05`, `frank06`, `frank07`, `frank08`, `wing_man`, `stocks02`, `stocks03`, `stocks04`, `frank10` |
| Groups | `CONT_033` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 9, value 0

**Action**

- Play dialog: TRISH.SCR, line/variant 7
- Object spawn/action: GalSpan_Shuttle_Medium (object 0, id 199), subtype 1, param 3

## Waypoints

### Waypoint 0

- Tag: `251`
- Members: `GalSpan_Shuttle_Medium (object 0, id 199, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (307.26, 34.14, 559.29) | None |
| 1 | (-181.52, 169.64, 388.72) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `GalSpan_Shuttle_Medium` | 199 | Interactive | 458.22,0.00,1063.92 | 302,0,0 | secondary groups: CONT_033, none; waypoint: Waypoint 0 (tag 251, 2 point(s)), starting point 0, arrival event value 16449536 |
