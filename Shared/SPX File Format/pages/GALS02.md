# Tachyon: The Fringe GALS02.SPX - Prometheus Patrol

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `GALS02.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `GALSPA2.BDF` |
| Region | 2 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 13 |
| Entities | 43 |
| Events | 2 |
| Waypoints | 0 |
| Child Sectors | 3 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Outpost`, `1: GalSpan_Construction_Facility`, `2: Spcargo_Parts`, `3: Junk_10`, `4: Junk_09`, `5: Junk_08`, `6: Junk_07`, `7: Junk_06`, `8: Junk_05`, `9: Junk_04`, `10: Junk_03`, `11: Mega_Gate`, `12: Hyper_Gate` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `bfge_02`, `BFGF_03`, `BFGE_03` |
| Aliases | `stocks04`, `Jerome07`, `Jerome08`, `Jerome09`, `Jerome10`, `Jerome11`, `Jerome12`, `stocks03`, `stocks02`, `stocks01` |
| Groups | `CONT_060`, `CERIPHILON` |
| Child Sectors | [gals02A.spx](GALS02A.md), [gals02B.spx](GALS02B.md), [gals02C.spx](GALS02C.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 445; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 47
- Set/add variable: variable group 14, variable 805, subtype 0, value 1

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 444; flags 2)

**Action**

- Set/add variable: variable group 14, variable 804, subtype 0, value 1

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | -1819.73,0.00,417.88 | 85,0,0 | Gate SPX: [Gals03.spx](GALS03.md) |
| 1 | `Hyper_Gate` | 2 | Gate | -280.51,0.00,72.60 | 51,0,0 | Gate SPX: [Gals01.spx](GALS01.md) |
| 2 | `Mega_Gate` | 3 | Gate | 1318.40,0.00,-50.26 | 449,0,0 | Gate SPX: [Fron01.spx](FRON01.md) |
| 3 | `Junk_03` | 316 | Object | 1012.60,-77.00,3032.59 | 0,475,0 | Scale/Radius: 1.00 |
| 4 | `Junk_03` | 318 | Object | 1114.28,0.00,2890.69 | 0,0,479 | Scale/Radius: 1.00 |
| 5 | `Junk_03` | 320 | Object | 1337.52,0.00,2832.26 | 0,0,0 | Scale/Radius: 1.00 |
| 6 | `Junk_04` | 321 | Object | 1314.43,0.00,3149.45 | 453,0,0 | Scale/Radius: 1.00 |
| 7 | `Junk_04` | 322 | Object | 1222.05,0.00,3057.63 | 0,0,0 | Scale/Radius: 1.00 |
| 8 | `Junk_04` | 323 | Object | 1198.96,-32.00,2832.26 | 256,0,479 | Scale/Radius: 1.00 |
| 9 | `Junk_04` | 324 | Object | 909.43,-54.00,3174.49 | 0,202,47 | Scale/Radius: 1.00 |
| 10 | `Junk_05` | 327 | Object | 1414.50,0.00,3149.45 | 0,0,0 | Scale/Radius: 1.00 |
| 11 | `Junk_05` | 328 | Object | 1368.31,0.00,3358.12 | 453,0,0 | Scale/Radius: 1.00 |
| 12 | `Junk_05` | 329 | Object | 852.85,38.00,2857.30 | 453,0,0 | Scale/Radius: 1.00 |
| 13 | `Junk_05` | 331 | Object | 1445.29,0.00,2949.12 | 256,0,0 | Scale/Radius: 1.00 |
| 14 | `Junk_06` | 332 | Object | 1113.88,67.00,3349.77 | 12,0,0 | Scale/Radius: 1.00 |
| 15 | `Junk_06` | 333 | Object | 951.62,34.00,3333.08 | 0,0,0 | Scale/Radius: 1.00 |
| 16 | `Junk_07` | 334 | Object | 943.92,34.00,3558.45 | 0,475,0 | Scale/Radius: 1.00 |
| 17 | `Junk_07` | 335 | Object | 806.36,54.00,3366.47 | 453,0,0 | Scale/Radius: 1.00 |
| 18 | `Junk_07` | 336 | Object | 595.51,47.00,3583.49 | 0,202,0 | Scale/Radius: 1.00 |
| 19 | `Junk_07` | 337 | Object | 775.57,54.00,3591.83 | 453,124,0 | Scale/Radius: 1.00 |
| 20 | `Junk_07` | 338 | Object | 579.12,72.00,3850.59 | 100,475,47 | Scale/Radius: 1.00 |
| 21 | `Junk_07` | 339 | Object | 537.93,-79.00,3658.61 | 0,0,47 | Scale/Radius: 1.00 |
| 22 | `Junk_08` | 341 | Object | 637.00,0.00,3992.49 | 0,0,479 | Scale/Radius: 1.00 |
| 23 | `Junk_08` | 342 | Object | 469.65,-54.00,4000.83 | 0,0,0 | Scale/Radius: 1.00 |
| 24 | `Junk_08` | 343 | Object | 452.25,0.00,3833.89 | 0,305,0 | Scale/Radius: 1.00 |
| 25 | `Junk_08` | 344 | Object | 661.10,-79.00,3650.26 | 256,0,479 | Scale/Radius: 1.00 |
| 26 | `Junk_08` | 346 | Object | 167.42,-63.00,4034.22 | 0,33,185 | Scale/Radius: 1.00 |
| 27 | `Junk_09` | 347 | Object | 388.97,71.00,4075.95 | 453,0,0 | Scale/Radius: 1.00 |
| 28 | `Junk_09` | 348 | Object | 338.78,-54.00,3909.02 | 256,0,47 | Scale/Radius: 1.00 |
| 29 | `Junk_10` | 351 | Object | 252.10,0.00,4234.55 | 0,475,0 | Scale/Radius: 1.00 |
| 30 | `Junk_10` | 352 | Object | -32.72,0.00,4301.32 | 0,0,0 | Scale/Radius: 1.00 |
| 31 | `Junk_10` | 353 | Object | 180.82,38.00,4121.11 | 0,488,0 | Scale/Radius: 1.00 |
| 32 | `Junk_10` | 354 | Object | 115.61,66.00,3917.36 | 100,0,47 | Scale/Radius: 1.00 |
| 33 | `Junk_10` | 355 | Object | -81.21,-73.00,4109.34 | 453,475,0 | Scale/Radius: 1.00 |
| 34 | `Junk_10` | 356 | Object | 1083.09,67.00,3249.61 | 0,0,47 | Scale/Radius: 1.00 |
| 35 | `Junk_10` | 358 | Object | 971.02,-54.00,2890.69 | 0,475,0 | Scale/Radius: 1.00 |
| 36 | `Junk_03` | 361 | Object | -133.10,56.00,4217.85 | 256,0,47 | Scale/Radius: 1.00 |
| 37 | `Junk_03` | 362 | Object | -237.57,65.00,4226.20 | 100,0,0 | Scale/Radius: 1.00 |
| 38 | `Spcargo_Parts` | 444 | Interactive | 2182.03,-63.12,2792.87 | 0,0,0 | secondary groups: CONT_060, none |
| 39 | `Spcargo_Parts` | 445 | Interactive | -860.52,106.21,2398.34 | 36,441,78 | secondary groups: CONT_060, none |
| 40 | `GalSpan_Construction_Facility` | 313 | Interactive | -674.13,0.00,1650.42 | 0,0,0 | secondary groups: none, CERIPHILON |
| 41 | `GalSpan_Outpost` | 407 | Interactive | 718.74,0.00,2048.57 | 0,0,0 | None |
| 42 | `GalSpan_Construction_Facility` | 408 | Interactive | 2058.33,0.00,1624.51 | 0,0,0 | None |
