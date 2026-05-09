# Tachyon: The Fringe GALS01E.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `GALS01E.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 2 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 4 |
| Events | 5 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 0 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Minelayer`, `1: GalSpan_Heavy_Freighter`, `2: GalSpan_Poseidon` |
| Scripts | None |
| Scenes | None |
| Labels | `bfge_02` |
| Aliases | `stocks01`, `Jerome10`, `Jerome11`, `Jerome09`, `Jerome08`, `Jerome07`, `Jerome12`, `frank05`, `frank06`, `frank07`, `frank08`, `wing_man`, `stocks02`, `stocks03`, `stocks04`, `frank10` |
| Groups | `FG_BELUS`, `CONT_017` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Object arrival: GalSpan_Heavy_Freighter (object 2, id 204) reached Waypoint 1 (tag 301), point 1 (raw value 19726337)

**Action**

- Object spawn/action: GalSpan_Heavy_Freighter (object 2, id 204), subtype 4

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Gate state/action: param 4, subtype 3, param 0
- Set runtime trigger variable: variable group 20, variable 26, subtype 0, value 0

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 26, op 1, value 13

**Action**

- Group/spawn-list action: spawn list/group 150, subtype 1, param 2
- Set runtime trigger variable: variable group 20, variable 26, subtype 1, value 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 14, variable 402, op 1, value 1
- Variable comparison: subject variable group 14, variable 403, op 1, value 2

**Action**

- Object spawn/action: GalSpan_Poseidon (object 0, id 231), subtype 16
- Object spawn/action: GalSpan_Poseidon (object 1, id 232), subtype 16
- Object spawn/action: GalSpan_Minelayer (object 3, id 235), subtype 0

### Event 4

**Trigger**

- Object event: subject GalSpan_Minelayer (object 3, id 235), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: GalSpan_Minelayer (object 3, id 235), subtype 5

## Waypoints

### Waypoint 0

- Tag: `302`
- Members: `GalSpan_Poseidon (object 0, id 231, starts at point 0)`, `GalSpan_Poseidon (object 1, id 232, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-88.46, 6.12, 152.18) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 1

- Tag: `301`
- Members: `GalSpan_Heavy_Freighter (object 2, id 204, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (481.97, -113.22, 64.41) | None |
| 1 | (1103.14, -208.76, 22.59) | None; listened by Event 0 for GalSpan_Heavy_Freighter (object 2, id 204) |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `GalSpan_Poseidon` | 231 | Interactive | 473.37,0.00,1096.00 | 313,0,0 | group/role: FG_BELUS / 1; waypoint: Waypoint 0 (tag 302, 1 point(s)), starting point 0, arrival event value 19791872 |
| 1 | `GalSpan_Poseidon` | 232 | Interactive | 520.05,0.00,1089.20 | 306,0,0 | group/role: FG_BELUS / 2; waypoint: Waypoint 0 (tag 302, 1 point(s)), starting point 0, arrival event value 19791872 |
| 2 | `GalSpan_Heavy_Freighter` | 204 | Interactive | 70.11,-106.15,77.76 | 134,0,0 | secondary groups: CONT_017, none; waypoint: Waypoint 1 (tag 301, 2 point(s)), starting point 0, arrival event value 19726336 |
| 3 | `GalSpan_Minelayer` | 235 | Interactive | 317.48,-47.52,559.91 | 348,0,50 | None |
