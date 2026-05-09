# Tachyon: The Fringe FRON06.SPX - Core Weapon; Hajod’s Bargain

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON06.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `FRONTI6.BDF` |
| Region | 4 |
| Sector ID | 5 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 9 |
| Events | 4 |
| Waypoints | 0 |
| Child Sectors | 2 |
| Scripts | 1 |
| Scenes | 2 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Gun_Platform2`, `1: GalSpan_Space_Station`, `2: Spcargo_Medical`, `3: Hyper_Gate` |
| Scripts | `PLAYER.SCR` |
| Scenes | `F6BC030A.SEN`, `F6LAN01.SEN` |
| Labels | `CEPHS`, `valnt`, `dionysus` |
| Aliases | None |
| Groups | `CONT_002`, `ALEUS_STATION`, `CONT_026` |
| Child Sectors | [fron06A.spx](FRON06A.md), [fron06B.spx](FRON06B.md) |

## Events

### Event 0

**Trigger**

- Object event: subject Gun_Platform2 (object 8, id 797), op 14, value 7

**Action**

- Object spawn/action: Gun_Platform2 (object 8, id 797), subtype 6
- Set/add variable: variable group 21, variable 21, subtype 1, value 1

### Event 1

**Trigger**

- Object event: subject Gun_Platform2 (object 7, id 798), op 14, value 7

**Action**

- Object spawn/action: Gun_Platform2 (object 7, id 798), subtype 6
- Set/add variable: variable group 21, variable 22, subtype 1, value 1

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 990; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 145
- Set/add variable: variable group 16, variable 807, subtype 0, value 1

### Event 3

**Trigger**

- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Object spawn/action: Spcargo_Medical (object 1, id 990), subtype 0

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | 22.32,2604.87,-3767.95 | 0,447,0 | Gate SPX: [fron01.spx](FRON01.md) |
| 1 | `Spcargo_Medical` | 990 | Interactive | 5.78,320.55,6.84 | 0,0,0 | secondary groups: CONT_002, none |
| 2 | `GalSpan_Space_Station` | 891 | Interactive | 5.93,-86.62,5.84 | 0,0,0 | secondary groups: CONT_026, ALEUS_STATION |
| 3 | `Gun_Platform2` | 146 | Interactive | 687.90,659.16,846.69 | 107,0,0 | None |
| 4 | `Gun_Platform2` | 162 | Interactive | 688.12,-873.46,846.08 | 107,0,0 | None |
| 5 | `Gun_Platform2` | 194 | Interactive | -1067.47,654.56,-161.51 | 320,0,0 | None |
| 6 | `Gun_Platform2` | 178 | Interactive | -1067.96,-870.86,-161.92 | 320,1,0 | None |
| 7 | `Gun_Platform2` | 798 | Interactive | 544.88,-865.76,-527.63 | 18,0,0 | None |
| 8 | `Gun_Platform2` | 797 | Interactive | 723.61,654.55,-809.17 | 146,0,0 | None |
