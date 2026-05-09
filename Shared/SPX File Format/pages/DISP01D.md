# Tachyon: The Fringe DISP01D.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP01D.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 2 |
| Events | 3 |
| Waypoints | 0 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Minelayer`, `1: Luxury_Liner` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `TNSA`, `SPIKE`, `capb` |
| Aliases | `BC10_Claymore4`, `BC10_Claymore1`, `BC10_Claymore3`, `BC10_Claymore2`, `BC10_Waraxe`, `tnsa`, `BC10_Mace4`, `BC10_Mace2`, `BC10_Mace1`, `BC10_Mace3`, `BC10_Warhammer3`, `BC10_Warhammer2`, `BC10_Warhammer4`, `BC10_Warhammer1`, `SPIKE`, `Stocks01` |
| Groups | `STAR_PRINCESS`, `CONT_032`, `COBALT_SPIKE` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Object event: subject Luxury_Liner (object 0, id 489), op 4, value 50

**Action**

- Object spawn/action: Luxury_Liner (object 0, id 489), subtype 4

### Event 1

**Trigger**

- Variable comparison: subject variable group 21, variable 2, op 1, value 4
- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Object spawn/action: Generic_Minelayer (object 1, id 499), subtype 3
- Play dialog: PLAYER.SCR, line/variant 104

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 9, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 97

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Luxury_Liner` | 489 | Interactive | -615.38,0.00,3166.26 | 0,0,0 | secondary groups: CONT_032, STAR_PRINCESS |
| 1 | `Generic_Minelayer` | 499 | Interactive | -302.95,180.15,-2521.33 | 85,0,0 | label: SPIKE; alias: SPIKE; secondary groups: none, COBALT_SPIKE |
