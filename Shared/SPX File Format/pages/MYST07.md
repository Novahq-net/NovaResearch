# Tachyon: The Fringe MYST07.SPX - Extraordinary Hunt; The Sightseer

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST07.SPX` |
| Sector | `QUAD_07` |
| Backdrop | `MYSTER7.BDF` |
| Region | 5 |
| Sector ID | 6 |
| SectorHazardFlags | Twilight fog / fog-radar impairment (0x00000002) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 12 |
| Entities | 480 |
| Events | 4 |
| Waypoints | 1 |
| Child Sectors | 4 |
| Scripts | 2 |
| Scenes | 1 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Mad_Pirate_Platform`, `1: Vacuum_Translucency_Module`, `2: Mad_Pirate_Station`, `3: Spcargo_Contraband`, `4: Asteroid_2`, `5: Roid_Sm_Grey`, `6: Roid_Lrg_Grey`, `7: Roid_SM_Grey_Points`, `8: Asteroid_1`, `9: Demon_Pirate_Fighter`, `10: Ice_Roid_2`, `11: Hyper_Gate` |
| Scripts | `B41DP.SCR`, `PLAYER.SCR` |
| Scenes | `M7GC080A.SEN` |
| Labels | `pisce`, `minotaur`, `cerbs`, `hydras`, `MPP1` |
| Aliases | `PISCES1`, `PISCES2`, `PISCES3`, `PISCES4`, `stocks02` |
| Groups | `FG_WRAITH`, `CONT_031`, `DEMON_STATION`, `CONT_UNKNOWN` |
| Child Sectors | [myst07A.spx](MYST07A.md), [myst07B.spx](MYST07B.md), [myst07C.spx](MYST07C.md), [myst07D.spx](MYST07D.md) |

## Events

### Event 0

**Trigger**

- Group/spawn-list event: subject 81, op 4, value 0 (flags 2)

**Action**

- Play dialog: B41DP.SCR, line/variant 4

### Event 1

**Trigger**

- Object event: subject Mad_Pirate_Platform (object 479, id 1630), op 2, value 0

**Action**

- Set/add variable: variable group 17, variable 800, subtype 0, value 1

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 1738; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 129
- Set/add variable: variable group 17, variable 801, subtype 0, value 1

### Event 3

**Trigger**

- Variable comparison: subject variable group 0, variable 4, op 1, value 3009
- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Object spawn/action: Demon_Pirate_Fighter (object 139, id 766), subtype 7
- Object spawn/action: Demon_Pirate_Fighter (object 140, id 767), subtype 7

## Waypoints

### Waypoint 0

- Tag: `51`
- Members: `Demon_Pirate_Fighter (object 139, id 766, starts at point 2)`, `Demon_Pirate_Fighter (object 140, id 767, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (12.14, 0.00, 1571.61) | on arrival redirect to waypoint tag 1, point 0 |
| 1 | (-997.89, 0.00, 760.90) | None |
| 2 | (-540.80, 0.00, -1730.71) | None |
| 3 | (1757.20, 0.00, -1110.90) | on arrival redirect to Waypoint 0 (tag 51), point 0 |

## Spawn Lists

### Spawn List 0

- ID: `81`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | -737.36,200.00,1343.08 | 263,498,14 | Gate SPX: [myst06.spx](MYST06.md) |
| 1 | `Hyper_Gate` | 2 | Gate | 675.71,-300.00,-1927.99 | 468,7,0 | Gate SPX: [myst08.spx](MYST08.md) |
| 2 | `Ice_Roid_2` | 304 | Object | -1691.20,-57.74,362.02 | 475,481,218 | Scale/Radius: 6.00 |
| 3 | `Ice_Roid_2` | 306 | Object | -1597.66,-654.38,777.75 | 196,171,307 | Scale/Radius: 3.00 |
| 4 | `Ice_Roid_2` | 308 | Object | -1070.81,-846.85,2446.26 | 484,461,149 | Scale/Radius: 5.00 |
| 5 | `Ice_Roid_2` | 310 | Object | -1483.33,558.15,604.53 | 446,162,20 | Scale/Radius: 1.00 |
| 6 | `Ice_Roid_2` | 312 | Object | -1081.20,-346.44,1926.61 | 333,294,262 | Scale/Radius: 1.00 |
| 7 | `Ice_Roid_2` | 314 | Object | -1275.47,923.83,881.68 | 487,464,407 | Scale/Radius: 4.00 |
| 8 | `Ice_Roid_2` | 316 | Object | -1320.25,-461.92,2307.69 | 408,15,463 | Scale/Radius: 4.00 |
| 9 | `Ice_Roid_2` | 318 | Object | -1639.23,-750.61,-261.57 | 473,403,131 | Scale/Radius: 1.00 |
| 10 | `Ice_Roid_2` | 320 | Object | -1537.43,-76.99,-466.40 | 244,433,178 | Scale/Radius: 2.00 |
| 11 | `Ice_Roid_2` | 322 | Object | -935.70,-365.68,2203.76 | 118,375,307 | Scale/Radius: 3.00 |
| 12 | `Ice_Roid_2` | 324 | Object | -927.32,346.44,-1495.57 | 384,89,457 | Scale/Radius: 6.00 |
| 13 | `Ice_Roid_2` | 326 | Object | -1951.02,-38.49,50.23 | 465,114,496 | Scale/Radius: 3.00 |
| 14 | `Ice_Roid_2` | 328 | Object | -1589.40,673.63,-1124.64 | 222,212,259 | Scale/Radius: 6.00 |
| 15 | `Ice_Roid_2` | 330 | Object | -1389.80,731.37,1401.33 | 368,409,366 | Scale/Radius: 4.00 |
| 16 | `Ice_Roid_2` | 332 | Object | -1608.05,-577.40,223.45 | 83,184,331 | Scale/Radius: 2.00 |
| 17 | `Ice_Roid_2` | 334 | Object | -1641.36,-538.90,-1089.99 | 488,243,209 | Scale/Radius: 1.00 |
| 18 | `Ice_Roid_2` | 336 | Object | -1547.23,-461.92,1509.11 | 130,271,238 | Scale/Radius: 5.00 |
| 19 | `Ice_Roid_2` | 338 | Object | -1576.87,38.49,-157.63 | 128,154,49 | Scale/Radius: 6.00 |
| 20 | `Ice_Roid_2` | 340 | Object | -1672.54,-134.73,-1159.28 | 277,350,494 | Scale/Radius: 6.00 |
| 21 | `Ice_Roid_2` | 342 | Object | -1181.93,115.48,1297.40 | 346,156,437 | Scale/Radius: 5.00 |
| 22 | `Ice_Roid_2` | 344 | Object | -1247.49,654.38,2273.05 | 94,312,338 | Scale/Radius: 6.00 |
| 23 | `Ice_Roid_2` | 346 | Object | -1216.31,-481.16,1788.03 | 511,372,63 | Scale/Radius: 1.00 |
| 24 | `Ice_Roid_2` | 348 | Object | -1472.94,808.35,1782.41 | 164,488,492 | Scale/Radius: 1.00 |
| 25 | `Ice_Roid_2` | 350 | Object | -1722.38,-500.41,-192.28 | 297,459,474 | Scale/Radius: 6.00 |
| 26 | `Ice_Roid_2` | 352 | Object | -1483.33,904.59,812.39 | 117,199,36 | Scale/Radius: 5.00 |
| 27 | `Ice_Roid_2` | 358 | Object | -1104.00,-673.63,-1599.51 | 162,224,179 | Scale/Radius: 3.00 |
| 28 | `Ice_Roid_2` | 362 | Object | -1296.26,230.96,1435.98 | 317,502,66 | Scale/Radius: 1.00 |
| 29 | `Ice_Roid_2` | 364 | Object | -1319.18,-230.96,-501.05 | 318,430,269 | Scale/Radius: 1.00 |
| 30 | `Ice_Roid_2` | 366 | Object | -894.13,558.15,1649.46 | 394,33,486 | Scale/Radius: 3.00 |
| 31 | `Ice_Roid_2` | 370 | Object | -1493.73,789.11,1782.41 | 286,21,297 | Scale/Radius: 2.00 |
| 32 | `Ice_Roid_2` | 372 | Object | -1566.48,923.83,-261.57 | 118,201,68 | Scale/Radius: 3.00 |
| 33 | `Ice_Roid_2` | 374 | Object | -1213.11,384.93,1332.05 | 275,262,494 | Scale/Radius: 3.00 |
| 34 | `Ice_Roid_2` | 376 | Object | -1247.49,38.49,2134.47 | 373,6,340 | Scale/Radius: 6.00 |
| 35 | `Ice_Roid_2` | 378 | Object | -1732.77,-384.93,15.58 | 258,365,345 | Scale/Radius: 3.00 |
| 36 | `Ice_Roid_2` | 380 | Object | -2034.17,558.15,-53.70 | 287,305,442 | Scale/Radius: 4.00 |
| 37 | `Ice_Roid_2` | 382 | Object | -1008.45,866.09,1718.75 | 284,343,408 | Scale/Radius: 2.00 |
| 38 | `Ice_Roid_2` | 384 | Object | -1692.73,-519.66,1335.89 | 148,85,467 | Scale/Radius: 1.00 |
| 39 | `Ice_Roid_2` | 386 | Object | -1547.82,-519.66,-708.91 | 27,134,510 | Scale/Radius: 3.00 |
| 40 | `Ice_Roid_2` | 388 | Object | -1129.97,-519.66,708.46 | 371,57,266 | Scale/Radius: 5.00 |
| 41 | `Ice_Roid_2` | 390 | Object | -1070.81,-827.60,1857.32 | 253,139,460 | Scale/Radius: 5.00 |
| 42 | `Ice_Roid_2` | 392 | Object | -1692.73,-558.15,1405.18 | 251,222,451 | Scale/Radius: 1.00 |
| 43 | `Ice_Roid_2` | 394 | Object | -1847.09,-230.96,-400.14 | 104,244,88 | Scale/Radius: 4.00 |
| 44 | `Ice_Roid_2` | 398 | Object | -1505.65,423.42,1509.11 | 276,72,127 | Scale/Radius: 1.00 |
| 45 | `Ice_Roid_2` | 400 | Object | -1443.89,307.94,-639.62 | 477,323,274 | Scale/Radius: 6.00 |
| 46 | `Ice_Roid_2` | 402 | Object | -1441.76,750.61,777.75 | 220,469,142 | Scale/Radius: 1.00 |
| 47 | `Ice_Roid_2` | 404 | Object | -2158.89,76.99,327.38 | 16,461,497 | Scale/Radius: 1.00 |
| 48 | `Ice_Roid_2` | 407 | Object | -1073.09,192.47,-1764.68 | 342,26,106 | Scale/Radius: 3.00 |
| 49 | `Ice_Roid_2` | 409 | Object | -1980.90,-943.08,46.99 | 198,404,336 | Scale/Radius: 6.00 |
| 50 | `Ice_Roid_2` | 411 | Object | -2090.61,-904.59,539.70 | 388,26,34 | Scale/Radius: 6.00 |
| 51 | `Ice_Roid_2` | 415 | Object | -1179.47,-442.67,-1719.66 | 44,398,443 | Scale/Radius: 4.00 |
| 52 | `Ice_Roid_2` | 417 | Object | -1834.65,-250.20,-777.59 | 425,298,68 | Scale/Radius: 6.00 |
| 53 | `Ice_Roid_2` | 419 | Object | -1182.80,-346.44,-1857.06 | 404,375,141 | Scale/Radius: 5.00 |
| 54 | `Ice_Roid_2` | 423 | Object | -2255.17,769.86,170.17 | 369,108,472 | Scale/Radius: 5.00 |
| 55 | `Ice_Roid_2` | 427 | Object | -1406.80,827.60,-1270.30 | 137,202,211 | Scale/Radius: 4.00 |
| 56 | `Ice_Roid_2` | 429 | Object | -2079.64,962.33,108.58 | 20,145,448 | Scale/Radius: 6.00 |
| 57 | `Ice_Roid_2` | 433 | Object | -2112.55,-789.11,108.58 | 174,409,382 | Scale/Radius: 1.00 |
| 58 | `Ice_Roid_2` | 441 | Object | -1794.41,-519.66,-414.93 | 37,70,321 | Scale/Radius: 5.00 |
| 59 | `Ice_Roid_2` | 443 | Object | -1958.96,750.61,-291.75 | 280,479,504 | Scale/Radius: 6.00 |
| 60 | `Ice_Roid_2` | 449 | Object | -672.45,-327.19,-2434.55 | 413,115,488 | Scale/Radius: 3.00 |
| 61 | `Ice_Roid_2` | 451 | Object | -1838.29,-866.09,-76.19 | 172,98,320 | Scale/Radius: 2.00 |
| 62 | `Ice_Roid_2` | 453 | Object | -1593.29,-307.94,-1147.12 | 152,285,67 | Scale/Radius: 4.00 |
| 63 | `Ice_Roid_2` | 455 | Object | -595.65,-558.15,-2311.37 | 266,116,475 | Scale/Radius: 6.00 |
| 64 | `Ice_Roid_2` | 461 | Object | -1505.53,0.00,-1239.51 | 101,270,487 | Scale/Radius: 1.00 |
| 65 | `Ice_Roid_2` | 465 | Object | -847.97,-500.41,-2372.96 | 469,474,496 | Scale/Radius: 1.00 |
| 66 | `Ice_Roid_2` | 471 | Object | -1417.77,250.20,-623.62 | 45,123,82 | Scale/Radius: 6.00 |
| 67 | `Ice_Roid_2` | 475 | Object | -2178.37,19.25,-353.34 | 71,424,479 | Scale/Radius: 5.00 |
| 68 | `Ice_Roid_2` | 477 | Object | -1915.08,-442.67,601.29 | 152,439,479 | Scale/Radius: 3.00 |
| 69 | `Ice_Roid_2` | 479 | Object | -1007.27,-134.73,-1826.27 | 135,486,63 | Scale/Radius: 1.00 |
| 70 | `Ice_Roid_2` | 483 | Object | -1670.09,519.66,-900.77 | 127,353,361 | Scale/Radius: 2.00 |
| 71 | `Ice_Roid_2` | 485 | Object | -1051.15,885.34,-1826.27 | 191,194,403 | Scale/Radius: 6.00 |
| 72 | `Ice_Roid_2` | 487 | Object | -1958.96,577.40,293.34 | 269,199,36 | Scale/Radius: 4.00 |
| 73 | `Ice_Roid_2` | 489 | Object | -1373.63,19.25,-1256.08 | 19,456,57 | Scale/Radius: 6.00 |
| 74 | `Ice_Roid_2` | 491 | Object | -2024.79,789.11,539.70 | 312,105,494 | Scale/Radius: 3.00 |
| 75 | `Ice_Roid_2` | 493 | Object | -913.80,0.00,-2034.22 | 98,98,65 | Scale/Radius: 1.00 |
| 76 | `Ice_Roid_2` | 495 | Object | -1713.97,230.96,-1085.53 | 442,109,201 | Scale/Radius: 6.00 |
| 77 | `Ice_Roid_2` | 497 | Object | -639.53,-538.90,-2095.81 | 130,329,153 | Scale/Radius: 3.00 |
| 78 | `Ice_Roid_2` | 499 | Object | -1582.32,-461.92,-808.38 | 149,186,409 | Scale/Radius: 3.00 |
| 79 | `Ice_Roid_2` | 503 | Object | -1146.56,808.35,-2119.99 | 212,289,491 | Scale/Radius: 2.00 |
| 80 | `Ice_Roid_2` | 507 | Object | -1201.41,115.48,-2273.96 | 163,268,319 | Scale/Radius: 1.00 |
| 81 | `Ice_Roid_2` | 511 | Object | -1362.66,-846.85,-917.34 | 175,357,152 | Scale/Radius: 5.00 |
| 82 | `Ice_Roid_2` | 513 | Object | -2222.26,846.85,-353.34 | 348,246,160 | Scale/Radius: 4.00 |
| 83 | `Ice_Roid_2` | 521 | Object | 589.71,199.59,2138.52 | 441,411,77 | Scale/Radius: 1.00 |
| 84 | `Ice_Roid_2` | 523 | Object | -1558.20,117.40,1981.28 | 399,305,286 | Scale/Radius: 2.00 |
| 85 | `Ice_Roid_2` | 525 | Object | -103.17,-399.17,1733.00 | 462,351,349 | Scale/Radius: 5.00 |
| 86 | `Ice_Roid_2` | 527 | Object | -622.82,446.13,1724.72 | 173,33,317 | Scale/Radius: 3.00 |
| 87 | `Ice_Roid_2` | 529 | Object | -241.74,-140.88,2229.56 | 78,216,414 | Scale/Radius: 3.00 |
| 88 | `Ice_Roid_2` | 531 | Object | -1073.19,-340.47,2312.32 | 130,164,467 | Scale/Radius: 6.00 |
| 89 | `Ice_Roid_2` | 533 | Object | -518.89,422.65,2378.52 | 421,344,135 | Scale/Radius: 2.00 |
| 90 | `Ice_Roid_2` | 535 | Object | 173.98,187.85,2022.66 | 243,501,34 | Scale/Radius: 2.00 |
| 91 | `Ice_Roid_2` | 537 | Object | 1225.23,70.44,1862.88 | 504,481,29 | Scale/Radius: 1.00 |
| 92 | `Ice_Roid_2` | 539 | Object | -1488.92,-493.10,1832.31 | 370,368,93 | Scale/Radius: 3.00 |
| 93 | `Ice_Roid_2` | 541 | Object | -553.54,316.99,2436.46 | 228,372,56 | Scale/Radius: 5.00 |
| 94 | `Ice_Roid_2` | 543 | Object | 693.64,-211.33,1733.00 | 89,395,157 | Scale/Radius: 2.00 |
| 95 | `Ice_Roid_2` | 545 | Object | 1422.91,-575.28,993.61 | 439,1,7 | Scale/Radius: 4.00 |
| 96 | `Ice_Roid_2` | 547 | Object | -899.97,457.87,1881.96 | 505,240,345 | Scale/Radius: 6.00 |
| 97 | `Ice_Roid_2` | 549 | Object | -1454.27,-187.85,2246.11 | 75,122,1 | Scale/Radius: 6.00 |
| 98 | `Ice_Roid_2` | 551 | Object | -622.82,129.14,1890.24 | 17,318,286 | Scale/Radius: 4.00 |
| 99 | `Ice_Roid_2` | 553 | Object | 520.42,211.33,2444.73 | 179,108,113 | Scale/Radius: 3.00 |
| 100 | `Ice_Roid_2` | 555 | Object | -622.82,-223.07,1981.28 | 214,500,214 | Scale/Radius: 5.00 |
| 101 | `Ice_Roid_2` | 557 | Object | -68.52,-340.47,1683.34 | 472,304,145 | Scale/Radius: 6.00 |
| 102 | `Ice_Roid_2` | 559 | Object | 659.00,-129.14,2155.07 | 320,84,267 | Scale/Radius: 1.00 |
| 103 | `Ice_Roid_2` | 561 | Object | -33.88,-176.11,1923.34 | 2,25,55 | Scale/Radius: 3.00 |
| 104 | `Ice_Roid_2` | 563 | Object | -137.81,422.65,2295.76 | 106,387,454 | Scale/Radius: 4.00 |
| 105 | `Ice_Roid_2` | 565 | Object | 693.64,93.92,1799.20 | 258,166,345 | Scale/Radius: 5.00 |
| 106 | `Ice_Roid_2` | 567 | Object | 589.71,-504.84,1906.79 | 18,438,301 | Scale/Radius: 5.00 |
| 107 | `Ice_Roid_2` | 569 | Object | 485.78,-129.14,2411.63 | 279,177,176 | Scale/Radius: 1.00 |
| 108 | `Ice_Roid_2` | 571 | Object | 712.47,316.99,1496.60 | 490,57,302 | Scale/Radius: 4.00 |
| 109 | `Ice_Roid_2` | 573 | Object | -311.03,129.14,2196.45 | 184,77,500 | Scale/Radius: 6.00 |
| 110 | `Ice_Roid_2` | 575 | Object | 693.64,-540.06,2370.25 | 363,339,377 | Scale/Radius: 5.00 |
| 111 | `Ice_Roid_2` | 577 | Object | 208.63,211.33,2055.76 | 74,216,68 | Scale/Radius: 2.00 |
| 112 | `Ice_Roid_2` | 579 | Object | -1246.41,422.65,2403.35 | 108,465,327 | Scale/Radius: 2.00 |
| 113 | `Ice_Roid_2` | 581 | Object | 624.35,-305.25,1716.44 | 313,393,308 | Scale/Radius: 4.00 |
| 114 | `Ice_Roid_2` | 583 | Object | -1350.34,-328.73,2353.70 | 286,273,194 | Scale/Radius: 6.00 |
| 115 | `Ice_Roid_2` | 585 | Object | 347.20,-293.51,1824.03 | 386,218,471 | Scale/Radius: 5.00 |
| 116 | `Ice_Roid_2` | 587 | Object | 1388.27,-35.22,1647.41 | 345,124,477 | Scale/Radius: 6.00 |
| 117 | `Ice_Roid_2` | 589 | Object | 589.71,-23.48,1964.72 | 238,221,420 | Scale/Radius: 4.00 |
| 118 | `Ice_Roid_2` | 591 | Object | 624.35,-176.11,1890.24 | 184,303,415 | Scale/Radius: 1.00 |
| 119 | `Ice_Roid_2` | 593 | Object | -969.26,305.25,1815.76 | 82,390,356 | Scale/Radius: 1.00 |
| 120 | `Ice_Roid_2` | 595 | Object | -1038.55,352.21,1824.03 | 502,491,431 | Scale/Radius: 6.00 |
| 121 | `Ice_Roid_2` | 597 | Object | -414.96,270.03,2254.38 | 6,317,95 | Scale/Radius: 1.00 |
| 122 | `Ice_Roid_2` | 599 | Object | 1007.19,340.47,1316.37 | 270,311,337 | Scale/Radius: 2.00 |
| 123 | `Ice_Roid_2` | 601 | Object | 312.56,58.70,2287.49 | 50,461,393 | Scale/Radius: 3.00 |
| 124 | `Ice_Roid_2` | 603 | Object | -1835.35,481.36,1766.10 | 234,130,261 | Scale/Radius: 1.00 |
| 125 | `Ice_Roid_2` | 605 | Object | -1488.92,410.91,2146.80 | 145,442,284 | Scale/Radius: 6.00 |
| 126 | `Ice_Roid_2` | 607 | Object | -414.96,528.32,2444.73 | 113,448,130 | Scale/Radius: 5.00 |
| 127 | `Ice_Roid_2` | 609 | Object | -276.39,23.48,1865.41 | 151,17,405 | Scale/Radius: 5.00 |
| 128 | `Ice_Roid_2` | 611 | Object | 1041.83,328.73,993.61 | 55,403,24 | Scale/Radius: 1.00 |
| 129 | `Ice_Roid_2` | 613 | Object | 1422.91,340.47,1349.47 | 9,377,424 | Scale/Radius: 5.00 |
| 130 | `Ice_Roid_2` | 615 | Object | -1142.48,246.55,2213.00 | 331,427,314 | Scale/Radius: 2.00 |
| 131 | `Ice_Roid_2` | 617 | Object | 702.65,270.03,1618.41 | 233,221,314 | Scale/Radius: 4.00 |
| 132 | `Ice_Roid_2` | 619 | Object | -1211.77,-234.81,2146.80 | 337,138,193 | Scale/Radius: 2.00 |
| 133 | `Ice_Roid_2` | 621 | Object | 693.64,199.59,1807.48 | 219,317,162 | Scale/Radius: 5.00 |
| 134 | `Ice_Roid_2` | 623 | Object | -345.67,-35.22,1931.62 | 469,504,313 | Scale/Radius: 5.00 |
| 135 | `Ice_Roid_2` | 625 | Object | 948.08,305.25,2144.26 | 134,412,60 | Scale/Radius: 3.00 |
| 136 | `Ice_Roid_2` | 627 | Object | 982.73,23.48,2078.05 | 204,399,11 | Scale/Radius: 2.00 |
| 137 | `Ice_Roid_2` | 629 | Object | -726.75,140.88,2262.66 | 39,297,43 | Scale/Radius: 3.00 |
| 138 | `Ice_Roid_2` | 631 | Object | -241.74,23.48,1881.96 | 72,386,235 | Scale/Radius: 5.00 |
| 139 | `Demon_Pirate_Fighter` | 766 | Interactive | 1784.03,0.00,-986.73 | 0,0,0 | group/role: FG_WRAITH / 1; waypoint: Waypoint 0 (tag 51, 4 point(s)), starting point 2, arrival event value 3342338 |
| 140 | `Demon_Pirate_Fighter` | 767 | Interactive | -664.08,0.00,-1729.15 | 0,0,0 | group/role: FG_WRAITH / 2; waypoint: Waypoint 0 (tag 51, 4 point(s)), starting point 0, arrival event value 3342336 |
| 141 | `Ice_Roid_2` | 773 | Object | 2826.75,33.10,72.40 | 349,339,232 | Scale/Radius: 3.00 |
| 142 | `Ice_Roid_2` | 775 | Object | 1748.86,496.56,513.86 | 152,378,398 | Scale/Radius: 3.00 |
| 143 | `Ice_Roid_2` | 779 | Object | 2024.09,-49.66,417.62 | 381,36,503 | Scale/Radius: 3.00 |
| 144 | `Ice_Roid_2` | 781 | Object | 2236.76,463.46,1206.73 | 27,158,339 | Scale/Radius: 3.00 |
| 145 | `Ice_Roid_2` | 783 | Object | 2461.94,66.21,687.08 | 135,229,241 | Scale/Radius: 2.00 |
| 146 | `Ice_Roid_2` | 785 | Object | 1848.94,-678.63,1418.44 | 264,52,242 | Scale/Radius: 5.00 |
| 147 | `Ice_Roid_2` | 787 | Object | 1397.04,-297.94,692.04 | 484,91,187 | Scale/Radius: 6.00 |
| 148 | `Ice_Roid_2` | 789 | Object | 2311.82,811.05,1245.22 | 197,263,256 | Scale/Radius: 6.00 |
| 149 | `Ice_Roid_2` | 791 | Object | 2174.21,-529.66,1283.72 | 251,132,217 | Scale/Radius: 5.00 |
| 150 | `Ice_Roid_2` | 793 | Object | 2136.68,-546.22,533.10 | 334,460,250 | Scale/Radius: 1.00 |
| 151 | `Ice_Roid_2` | 795 | Object | 2149.19,-513.11,359.89 | 85,247,365 | Scale/Radius: 2.00 |
| 152 | `Ice_Roid_2` | 797 | Object | 2311.82,297.94,321.39 | 146,106,350 | Scale/Radius: 1.00 |
| 153 | `Ice_Roid_2` | 801 | Object | 2325.49,66.21,132.32 | 316,400,368 | Scale/Radius: 4.00 |
| 154 | `Ice_Roid_2` | 805 | Object | 2461.94,546.22,956.53 | 421,460,39 | Scale/Radius: 2.00 |
| 155 | `Ice_Roid_2` | 807 | Object | 1534.65,-546.22,403.34 | 414,155,145 | Scale/Radius: 1.00 |
| 156 | `Ice_Roid_2` | 811 | Object | 2500.63,827.60,16.84 | 261,470,262 | Scale/Radius: 6.00 |
| 157 | `Ice_Roid_2` | 813 | Object | 2363.02,811.05,-21.65 | 133,60,44 | Scale/Radius: 6.00 |
| 158 | `Ice_Roid_2` | 815 | Object | 2213.75,777.94,264.87 | 111,139,146 | Scale/Radius: 1.00 |
| 159 | `Ice_Roid_2` | 817 | Object | 2149.19,-16.55,379.13 | 298,92,208 | Scale/Radius: 6.00 |
| 160 | `Ice_Roid_2` | 821 | Object | 2424.41,115.86,898.79 | 455,385,444 | Scale/Radius: 2.00 |
| 161 | `Ice_Roid_2` | 827 | Object | 1974.05,264.83,1110.50 | 374,127,246 | Scale/Radius: 4.00 |
| 162 | `Ice_Roid_2` | 831 | Object | 2588.21,-446.90,55.34 | 306,186,23 | Scale/Radius: 3.00 |
| 163 | `Ice_Roid_2` | 835 | Object | 2562.03,-281.38,552.35 | 177,374,508 | Scale/Radius: 2.00 |
| 164 | `Ice_Roid_2` | 837 | Object | 1861.45,-182.07,456.12 | 387,452,43 | Scale/Radius: 6.00 |
| 165 | `Ice_Roid_2` | 841 | Object | 2199.23,82.76,744.82 | 356,477,480 | Scale/Radius: 4.00 |
| 166 | `Ice_Roid_2` | 843 | Object | 2524.50,662.08,898.79 | 310,477,223 | Scale/Radius: 3.00 |
| 167 | `Ice_Roid_2` | 845 | Object | 2486.97,331.04,494.61 | 63,239,496 | Scale/Radius: 6.00 |
| 168 | `Ice_Roid_2` | 847 | Object | 1898.98,744.84,359.89 | 270,242,13 | Scale/Radius: 3.00 |
| 169 | `Ice_Roid_2` | 849 | Object | 2199.23,-231.73,379.13 | 396,126,365 | Scale/Radius: 5.00 |
| 170 | `Ice_Roid_2` | 851 | Object | 2713.31,711.74,55.34 | 477,99,63 | Scale/Radius: 3.00 |
| 171 | `Ice_Roid_2` | 853 | Object | 2086.64,-496.56,1052.76 | 409,447,478 | Scale/Radius: 5.00 |
| 172 | `Ice_Roid_2` | 855 | Object | 1588.67,-82.76,1702.58 | 158,368,125 | Scale/Radius: 2.00 |
| 173 | `Ice_Roid_2` | 861 | Object | 1711.33,413.80,1187.49 | 163,132,77 | Scale/Radius: 3.00 |
| 174 | `Ice_Roid_2` | 863 | Object | 1911.49,16.55,1110.50 | 384,399,365 | Scale/Radius: 1.00 |
| 175 | `Ice_Roid_2` | 865 | Object | 1798.90,595.87,379.13 | 31,352,291 | Scale/Radius: 2.00 |
| 176 | `Ice_Roid_2` | 867 | Object | 2450.59,165.52,93.83 | 137,436,492 | Scale/Radius: 5.00 |
| 177 | `Ice_Roid_2` | 869 | Object | 2486.97,463.46,513.86 | 320,289,70 | Scale/Radius: 3.00 |
| 178 | `Ice_Roid_2` | 871 | Object | 2149.19,198.62,1379.95 | 64,279,295 | Scale/Radius: 4.00 |
| 179 | `Ice_Roid_2` | 873 | Object | 2599.56,546.22,513.86 | 483,510,266 | Scale/Radius: 4.00 |
| 180 | `Asteroid_1` | 917 | Object | -1973.43,475.83,848.20 | 181,442,293 | Scale/Radius: 3.00 |
| 181 | `Ice_Roid_2` | 923 | Object | -1950.33,-127.03,1456.39 | 419,420,167 | Scale/Radius: 3.00 |
| 182 | `Asteroid_1` | 925 | Object | -1842.55,134.73,1202.33 | 287,222,160 | Scale/Radius: 7.00 |
| 183 | `Roid_SM_Grey_Points` | 926 | Object | -1819.46,-88.53,748.11 | 253,103,91 | Scale/Radius: 1.00 |
| 184 | `Ice_Roid_2` | 931 | Object | -1934.94,-73.14,863.59 | 139,33,496 | Scale/Radius: 3.00 |
| 185 | `Asteroid_1` | 933 | Object | -1906.79,-338.44,909.78 | 35,10,5 | Scale/Radius: 1.00 |
| 186 | `Roid_SM_Grey_Points` | 934 | Object | -1719.37,0.00,1086.85 | 122,24,75 | Scale/Radius: 2.00 |
| 187 | `Asteroid_1` | 937 | Object | -1780.96,-50.04,825.10 | 333,119,71 | Scale/Radius: 5.00 |
| 188 | `Ice_Roid_2` | 939 | Object | -1750.17,533.57,1040.66 | 431,13,142 | Scale/Radius: 3.00 |
| 189 | `Asteroid_1` | 941 | Object | -1919.54,157.82,1448.69 | 458,110,96 | Scale/Radius: 1.00 |
| 190 | `Roid_SM_Grey_Points` | 942 | Object | -1842.55,150.12,817.40 | 320,75,322 | Scale/Radius: 5.00 |
| 191 | `Asteroid_1` | 945 | Object | -1973.43,42.34,932.88 | 450,101,25 | Scale/Radius: 9.00 |
| 192 | `Ice_Roid_2` | 947 | Object | -2004.22,-53.89,1009.87 | 385,102,359 | Scale/Radius: 2.00 |
| 193 | `Roid_SM_Grey_Points` | 950 | Object | -1919.54,-73.14,1186.93 | 453,24,278 | Scale/Radius: 3.00 |
| 194 | `Ice_Roid_2` | 955 | Object | -1850.25,-119.33,1310.11 | 188,26,45 | Scale/Radius: 1.00 |
| 195 | `Asteroid_1` | 957 | Object | -1942.63,-138.57,1210.03 | 498,54,97 | Scale/Radius: 1.00 |
| 196 | `Ice_Roid_2` | 959 | Object | -1696.28,-84.68,1317.81 | 129,216,506 | Scale/Radius: 2.00 |
| 197 | `Ice_Roid_2` | 963 | Object | -1958.03,7.70,994.47 | 184,235,234 | Scale/Radius: 4.00 |
| 198 | `Asteroid_1` | 965 | Object | -1958.03,180.92,979.07 | 274,134,381 | Scale/Radius: 9.00 |
| 199 | `Asteroid_1` | 969 | Object | -1896.44,-88.53,1086.85 | 11,28,510 | Scale/Radius: 2.00 |
| 200 | `Roid_SM_Grey_Points` | 970 | Object | -1727.07,-150.12,963.68 | 444,113,449 | Scale/Radius: 3.00 |
| 201 | `Ice_Roid_2` | 971 | Object | -1827.15,-161.67,1171.54 | 99,244,467 | Scale/Radius: 5.00 |
| 202 | `Asteroid_1` | 973 | Object | -1896.44,-100.08,1233.13 | 162,184,110 | Scale/Radius: 6.00 |
| 203 | `Roid_SM_Grey_Points` | 974 | Object | -1922.19,-342.29,1102.25 | 266,372,250 | Scale/Radius: 9.00 |
| 204 | `Asteroid_1` | 981 | Object | -1765.57,545.12,802.00 | 61,38,123 | Scale/Radius: 7.00 |
| 205 | `Asteroid_1` | 989 | Object | -1834.85,-103.93,778.91 | 137,68,0 | Scale/Radius: 7.00 |
| 206 | `Roid_SM_Grey_Points` | 994 | Object | -1934.94,42.34,848.20 | 225,87,213 | Scale/Radius: 7.00 |
| 207 | `Asteroid_1` | 997 | Object | -1703.98,115.48,1387.10 | 69,510,303 | Scale/Radius: 1.00 |
| 208 | `Roid_SM_Grey_Points` | 998 | Object | -1873.35,471.99,755.81 | 180,77,151 | Scale/Radius: 5.00 |
| 209 | `Ice_Roid_2` | 999 | Object | -1719.37,-184.77,1387.10 | 127,366,348 | Scale/Radius: 6.00 |
| 210 | `Roid_SM_Grey_Points` | 1002 | Object | -2011.92,169.37,1333.21 | 344,358,27 | Scale/Radius: 4.00 |
| 211 | `Asteroid_1` | 1009 | Object | -1804.06,177.07,1364.00 | 8,290,187 | Scale/Radius: 1.00 |
| 212 | `Ice_Roid_2` | 1011 | Object | -1850.25,-46.19,1387.10 | 29,216,50 | Scale/Radius: 3.00 |
| 213 | `Asteroid_1` | 1013 | Object | -1750.17,-73.14,1171.54 | 269,447,46 | Scale/Radius: 3.00 |
| 214 | `Roid_SM_Grey_Points` | 1014 | Object | -1981.13,23.10,840.50 | 420,80,16 | Scale/Radius: 5.00 |
| 215 | `Ice_Roid_2` | 1015 | Object | -1750.17,57.74,979.07 | 31,195,499 | Scale/Radius: 1.00 |
| 216 | `Roid_Lrg_Grey` | 1292 | Object | 2341.76,459.99,780.96 | 169,410,351 | Scale/Radius: 8.00 |
| 217 | `Roid_Sm_Grey` | 1293 | Object | 2303.26,540.82,349.84 | 4,202,486 | Scale/Radius: 2.00 |
| 218 | `Roid_SM_Grey_Points` | 1294 | Object | 1972.22,-336.82,981.12 | 13,331,218 | Scale/Radius: 1.00 |
| 219 | `Asteroid_2` | 1295 | Object | 2357.15,425.34,650.08 | 437,380,259 | Scale/Radius: 9.00 |
| 220 | `Asteroid_1` | 1296 | Object | 2203.18,-429.20,981.12 | 424,193,368 | Scale/Radius: 3.00 |
| 221 | `Roid_Lrg_Grey` | 1297 | Object | 2280.17,552.37,865.64 | 294,380,350 | Scale/Radius: 5.00 |
| 222 | `Roid_Sm_Grey` | 1298 | Object | 2241.68,-325.27,311.34 | 503,54,427 | Scale/Radius: 5.00 |
| 223 | `Roid_SM_Grey_Points` | 1299 | Object | 2434.14,-313.72,403.73 | 132,397,60 | Scale/Radius: 8.00 |
| 224 | `Asteroid_2` | 1300 | Object | 2595.81,390.70,303.65 | 220,489,287 | Scale/Radius: 1.00 |
| 225 | `Asteroid_1` | 1301 | Object | 2164.69,332.96,642.38 | 282,272,129 | Scale/Radius: 9.00 |
| 226 | `Roid_Lrg_Grey` | 1302 | Object | 2395.65,-267.53,719.37 | 101,164,401 | Scale/Radius: 7.00 |
| 227 | `Roid_Sm_Grey` | 1303 | Object | 2156.99,-13.48,727.07 | 344,371,324 | Scale/Radius: 7.00 |
| 228 | `Roid_SM_Grey_Points` | 1304 | Object | 2110.80,483.08,342.14 | 117,48,117 | Scale/Radius: 3.00 |
| 229 | `Asteroid_2` | 1305 | Object | 2003.02,517.73,973.42 | 449,127,206 | Scale/Radius: 8.00 |
| 230 | `Asteroid_1` | 1306 | Object | 2364.85,-510.04,419.12 | 58,274,40 | Scale/Radius: 3.00 |
| 231 | `Roid_Lrg_Grey` | 1307 | Object | 2703.59,67.36,403.73 | 58,371,166 | Scale/Radius: 2.00 |
| 232 | `Roid_Sm_Grey` | 1308 | Object | 2634.30,-556.23,349.84 | 218,68,417 | Scale/Radius: 7.00 |
| 233 | `Roid_SM_Grey_Points` | 1309 | Object | 2634.30,90.46,950.33 | 16,92,338 | Scale/Radius: 4.00 |
| 234 | `Asteroid_2` | 1310 | Object | 2003.02,-510.04,249.76 | 249,10,338 | Scale/Radius: 3.00 |
| 235 | `Asteroid_1` | 1311 | Object | 2580.41,240.58,588.49 | 245,54,495 | Scale/Radius: 3.00 |
| 236 | `Roid_Lrg_Grey` | 1312 | Object | 2511.13,-394.56,603.89 | 270,36,476 | Scale/Radius: 4.00 |
| 237 | `Roid_Sm_Grey` | 1313 | Object | 2280.17,298.32,349.84 | 284,257,395 | Scale/Radius: 4.00 |
| 238 | `Roid_SM_Grey_Points` | 1314 | Object | 2310.96,459.99,896.44 | 65,302,432 | Scale/Radius: 3.00 |
| 239 | `Asteroid_1` | 1316 | Object | 2457.24,205.93,434.52 | 380,432,134 | Scale/Radius: 8.00 |
| 240 | `Roid_Lrg_Grey` | 1317 | Object | 2665.10,390.70,465.32 | 88,203,166 | Scale/Radius: 2.00 |
| 241 | `Roid_Sm_Grey` | 1318 | Object | 2534.22,229.03,303.65 | 373,341,156 | Scale/Radius: 1.00 |
| 242 | `Roid_SM_Grey_Points` | 1319 | Object | 2418.74,390.70,419.12 | 235,162,377 | Scale/Radius: 8.00 |
| 243 | `Asteroid_2` | 1320 | Object | 2688.19,413.80,857.95 | 333,283,471 | Scale/Radius: 7.00 |
| 244 | `Asteroid_1` | 1321 | Object | 2010.72,275.22,665.48 | 71,6,145 | Scale/Radius: 3.00 |
| 245 | `Roid_Lrg_Grey` | 1322 | Object | 2172.39,321.41,357.54 | 401,0,255 | Scale/Radius: 9.00 |
| 246 | `Roid_Sm_Grey` | 1323 | Object | 2364.85,-117.41,703.97 | 141,459,58 | Scale/Radius: 5.00 |
| 247 | `Roid_SM_Grey_Points` | 1324 | Object | 2118.50,-348.37,303.65 | 402,85,11 | Scale/Radius: 2.00 |
| 248 | `Asteroid_2` | 1325 | Object | 2264.77,-94.31,280.55 | 146,360,331 | Scale/Radius: 9.00 |
| 249 | `Asteroid_1` | 1326 | Object | 2495.73,67.36,342.14 | 324,348,459 | Scale/Radius: 8.00 |
| 250 | `Roid_Lrg_Grey` | 1327 | Object | 2418.74,-152.05,873.34 | 439,465,307 | Scale/Radius: 4.00 |
| 251 | `Roid_Sm_Grey` | 1328 | Object | 2264.77,148.19,326.74 | 375,50,151 | Scale/Radius: 3.00 |
| 252 | `Roid_SM_Grey_Points` | 1329 | Object | 2503.43,-105.86,449.92 | 282,183,16 | Scale/Radius: 7.00 |
| 253 | `Asteroid_2` | 1330 | Object | 1949.13,67.36,257.45 | 223,267,181 | Scale/Radius: 5.00 |
| 254 | `Asteroid_1` | 1331 | Object | 2203.18,-1.93,888.74 | 245,412,465 | Scale/Radius: 3.00 |
| 255 | `Roid_Lrg_Grey` | 1332 | Object | 2072.31,-232.89,865.64 | 100,65,326 | Scale/Radius: 2.00 |
| 256 | `Roid_Sm_Grey` | 1333 | Object | 2418.74,-452.30,834.85 | 391,155,309 | Scale/Radius: 5.00 |
| 257 | `Roid_SM_Grey_Points` | 1334 | Object | 2357.15,-325.27,542.30 | 186,511,0 | Scale/Radius: 1.00 |
| 258 | `Asteroid_2` | 1335 | Object | 1949.13,-544.68,326.74 | 71,238,452 | Scale/Radius: 7.00 |
| 259 | `Asteroid_1` | 1336 | Object | 2241.68,-255.98,557.70 | 459,368,44 | Scale/Radius: 5.00 |
| 260 | `Roid_Lrg_Grey` | 1337 | Object | 2434.14,-232.89,896.44 | 459,63,9 | Scale/Radius: 5.00 |
| 261 | `Roid_Sm_Grey` | 1338 | Object | 2434.14,-117.41,611.59 | 212,455,438 | Scale/Radius: 7.00 |
| 262 | `Roid_SM_Grey_Points` | 1339 | Object | 2072.31,136.65,480.71 | 9,391,156 | Scale/Radius: 1.00 |
| 263 | `Asteroid_2` | 1340 | Object | 2318.66,-440.75,234.36 | 337,267,188 | Scale/Radius: 9.00 |
| 264 | `Asteroid_1` | 1341 | Object | 2272.47,-510.04,242.06 | 10,303,18 | Scale/Radius: 6.00 |
| 265 | `Roid_Lrg_Grey` | 1342 | Object | 2233.98,-302.17,850.25 | 46,146,218 | Scale/Radius: 7.00 |
| 266 | `Roid_Sm_Grey` | 1343 | Object | 2534.22,-336.82,950.33 | 299,119,377 | Scale/Radius: 5.00 |
| 267 | `Roid_SM_Grey_Points` | 1344 | Object | 2087.70,113.55,272.85 | 481,431,1 | Scale/Radius: 1.00 |
| 268 | `Asteroid_2` | 1345 | Object | 1979.92,-82.76,650.08 | 393,437,243 | Scale/Radius: 9.00 |
| 269 | `Asteroid_1` | 1346 | Object | 2195.48,-348.37,634.69 | 290,377,412 | Scale/Radius: 9.00 |
| 270 | `Roid_Lrg_Grey` | 1347 | Object | 2072.31,-290.63,719.37 | 269,475,343 | Scale/Radius: 2.00 |
| 271 | `Roid_Sm_Grey` | 1348 | Object | 2195.48,136.65,272.85 | 256,235,161 | Scale/Radius: 8.00 |
| 272 | `Roid_SM_Grey_Points` | 1349 | Object | 2018.42,-13.48,419.12 | 381,330,253 | Scale/Radius: 6.00 |
| 273 | `Asteroid_2` | 1350 | Object | 2387.95,448.44,942.63 | 478,235,252 | Scale/Radius: 3.00 |
| 274 | `Asteroid_1` | 1351 | Object | 1964.53,332.96,303.65 | 88,159,102 | Scale/Radius: 7.00 |
| 275 | `Roid_Lrg_Grey` | 1352 | Object | 2118.50,-544.68,734.77 | 448,65,202 | Scale/Radius: 3.00 |
| 276 | `Roid_Sm_Grey` | 1353 | Object | 2141.59,436.89,904.14 | 0,366,432 | Scale/Radius: 9.00 |
| 277 | `Roid_SM_Grey_Points` | 1354 | Object | 2387.95,517.73,850.25 | 54,415,137 | Scale/Radius: 6.00 |
| 278 | `Asteroid_2` | 1355 | Object | 1941.43,9.62,657.78 | 263,3,466 | Scale/Radius: 4.00 |
| 279 | `Asteroid_1` | 1356 | Object | 2318.66,-371.46,288.25 | 341,385,139 | Scale/Radius: 5.00 |
| 280 | `Roid_Lrg_Grey` | 1357 | Object | 2264.77,-544.68,396.03 | 292,321,353 | Scale/Radius: 5.00 |
| 281 | `Roid_Sm_Grey` | 1358 | Object | 1979.92,67.36,634.69 | 36,142,410 | Scale/Radius: 1.00 |
| 282 | `Asteroid_2` | 1360 | Object | 2403.35,136.65,757.86 | 395,324,256 | Scale/Radius: 1.00 |
| 283 | `Asteroid_1` | 1361 | Object | 2387.95,55.81,396.03 | 260,375,186 | Scale/Radius: 1.00 |
| 284 | `Roid_Lrg_Grey` | 1362 | Object | 2180.09,-463.84,311.34 | 107,47,149 | Scale/Radius: 1.00 |
| 285 | `Roid_Sm_Grey` | 826 | Object | 2800.88,480.01,-40.90 | 260,265,368 | Scale/Radius: 10.00 |
| 286 | `Roid_Sm_Grey` | 305 | Object | -1493.73,-115.48,1262.76 | 424,494,110 | Scale/Radius: 10.00 |
| 287 | `Roid_Sm_Grey` | 307 | Object | -1164.35,-615.89,1926.61 | 369,6,339 | Scale/Radius: 10.00 |
| 288 | `Roid_Sm_Grey` | 309 | Object | -1389.80,-789.11,1713.13 | 470,39,151 | Scale/Radius: 10.00 |
| 289 | `Roid_Sm_Grey` | 311 | Object | -1254.68,-38.49,881.68 | 188,25,252 | Scale/Radius: 10.00 |
| 290 | `Roid_Sm_Grey` | 315 | Object | -1202.72,-76.99,1332.05 | 313,457,28 | Scale/Radius: 10.00 |
| 291 | `Roid_Sm_Grey` | 317 | Object | -1826.31,134.73,604.53 | 300,497,199 | Scale/Radius: 10.00 |
| 292 | `Roid_Sm_Grey` | 319 | Object | -885.75,-904.59,-1668.79 | 41,70,216 | Scale/Radius: 10.00 |
| 293 | `Roid_Sm_Grey` | 321 | Object | -1348.22,-461.92,950.96 | 13,58,347 | Scale/Radius: 10.00 |
| 294 | `Roid_Sm_Grey` | 323 | Object | -1992.60,654.38,-296.21 | 424,301,355 | Scale/Radius: 10.00 |
| 295 | `Roid_Sm_Grey` | 325 | Object | -2138.10,-577.40,535.24 | 176,39,148 | Scale/Radius: 10.00 |
| 296 | `Roid_Sm_Grey` | 329 | Object | -1680.80,-635.14,154.16 | 92,350,142 | Scale/Radius: 10.00 |
| 297 | `Roid_Sm_Grey` | 333 | Object | -1753.55,-481.16,-400.14 | 309,396,315 | Scale/Radius: 10.00 |
| 298 | `Roid_Sm_Grey` | 335 | Object | -1587.26,173.22,15.58 | 49,53,144 | Scale/Radius: 10.00 |
| 299 | `Roid_Sm_Grey` | 337 | Object | -1140.36,192.47,1643.84 | 176,495,504 | Scale/Radius: 10.00 |
| 300 | `Roid_Sm_Grey` | 339 | Object | -1524.91,-365.68,292.73 | 332,383,82 | Scale/Radius: 10.00 |
| 301 | `Roid_Sm_Grey` | 341 | Object | -1216.31,-538.90,2099.83 | 205,7,418 | Scale/Radius: 10.00 |
| 302 | `Roid_Sm_Grey` | 343 | Object | -2075.74,-173.22,-19.06 | 356,261,74 | Scale/Radius: 10.00 |
| 303 | `Roid_Sm_Grey` | 345 | Object | -1306.65,115.48,1332.05 | 304,337,296 | Scale/Radius: 10.00 |
| 304 | `Roid_Sm_Grey` | 347 | Object | -1774.34,750.61,188.80 | 440,155,506 | Scale/Radius: 10.00 |
| 305 | `Roid_Sm_Grey` | 349 | Object | -1412.71,-76.99,-604.98 | 231,502,461 | Scale/Radius: 10.00 |
| 306 | `Roid_Sm_Grey` | 351 | Object | -1112.38,0.00,2273.05 | 155,241,481 | Scale/Radius: 10.00 |
| 307 | `Roid_Sm_Grey` | 353 | Object | -1660.02,-731.37,-400.14 | 88,477,433 | Scale/Radius: 10.00 |
| 308 | `Roid_Sm_Grey` | 355 | Object | -1150.75,288.70,1262.76 | 358,329,24 | Scale/Radius: 10.00 |
| 309 | `Roid_Sm_Grey` | 357 | Object | -1795.13,-635.14,673.81 | 394,94,322 | Scale/Radius: 10.00 |
| 310 | `Roid_Sm_Grey` | 359 | Object | -2096.53,750.61,-296.21 | 308,356,47 | Scale/Radius: 10.00 |
| 311 | `Roid_Sm_Grey` | 361 | Object | -1233.90,904.59,465.95 | 376,213,370 | Scale/Radius: 10.00 |
| 312 | `Roid_Sm_Grey` | 363 | Object | -1576.87,153.97,1990.28 | 372,139,306 | Scale/Radius: 10.00 |
| 313 | `Roid_Sm_Grey` | 365 | Object | -1202.72,-731.37,362.02 | 477,191,469 | Scale/Radius: 10.00 |
| 314 | `Roid_Sm_Grey` | 367 | Object | -1701.59,-673.63,-434.78 | 380,490,425 | Scale/Radius: 10.00 |
| 315 | `Roid_Sm_Grey` | 369 | Object | -1472.94,-827.60,-192.28 | 5,487,288 | Scale/Radius: 10.00 |
| 316 | `Roid_Sm_Grey` | 371 | Object | -935.70,-288.70,2203.76 | 410,5,235 | Scale/Radius: 10.00 |
| 317 | `Roid_Sm_Grey` | 373 | Object | -1888.66,211.71,396.67 | 83,202,186 | Scale/Radius: 10.00 |
| 318 | `Roid_Sm_Grey` | 375 | Object | -1161.15,692.87,1609.20 | 427,405,172 | Scale/Radius: 10.00 |
| 319 | `Roid_Sm_Grey` | 377 | Object | -1630.97,-827.60,-951.42 | 357,221,222 | Scale/Radius: 10.00 |
| 320 | `Roid_Sm_Grey` | 379 | Object | -1982.20,-288.70,569.88 | 510,506,497 | Scale/Radius: 10.00 |
| 321 | `Roid_Sm_Grey` | 381 | Object | -1410.58,-885.34,396.67 | 96,391,256 | Scale/Radius: 10.00 |
| 322 | `Roid_Sm_Grey` | 383 | Object | -792.21,173.22,-1876.66 | 152,211,477 | Scale/Radius: 10.00 |
| 323 | `Roid_Sm_Grey` | 385 | Object | -1556.08,-19.25,743.10 | 250,470,137 | Scale/Radius: 10.00 |
| 324 | `Roid_Sm_Grey` | 387 | Object | -2002.99,615.89,431.31 | 335,372,218 | Scale/Radius: 10.00 |
| 325 | `Roid_Sm_Grey` | 389 | Object | -1680.80,-500.41,950.96 | 169,493,397 | Scale/Radius: 10.00 |
| 326 | `Roid_Sm_Grey` | 393 | Object | -925.31,-269.45,1753.39 | 384,418,221 | Scale/Radius: 10.00 |
| 327 | `Roid_Sm_Grey` | 395 | Object | -1317.04,808.35,1193.47 | 508,269,478 | Scale/Radius: 10.00 |
| 328 | `Roid_Sm_Grey` | 399 | Object | -1774.34,712.12,50.23 | 396,94,338 | Scale/Radius: 10.00 |
| 329 | `Roid_Sm_Grey` | 401 | Object | -2117.31,327.19,-88.35 | 363,494,383 | Scale/Radius: 10.00 |
| 330 | `Roid_Sm_Grey` | 403 | Object | -1475.07,-615.89,-1020.70 | 139,319,66 | Scale/Radius: 10.00 |
| 331 | `Roid_Sm_Grey` | 405 | Object | -1576.87,-404.18,881.68 | 60,404,447 | Scale/Radius: 10.00 |
| 332 | `Roid_Sm_Grey` | 410 | Object | -1439.71,-808.35,-1455.07 | 11,419,191 | Scale/Radius: 10.00 |
| 333 | `Roid_Sm_Grey` | 412 | Object | 1717.89,57.74,1413.99 | 265,356,366 | Scale/Radius: 10.00 |
| 334 | `Roid_Sm_Grey` | 414 | Object | -1406.80,-96.23,-1208.71 | 36,196,106 | Scale/Radius: 10.00 |
| 335 | `Roid_Sm_Grey` | 416 | Object | -1768.82,461.92,-500.44 | 233,220,196 | Scale/Radius: 10.00 |
| 336 | `Roid_Sm_Grey` | 424 | Object | -1915.08,750.61,-322.55 | 81,235,452 | Scale/Radius: 10.00 |
| 337 | `Roid_Sm_Grey` | 428 | Object | -1168.50,-134.73,-1534.89 | 179,212,240 | Scale/Radius: 10.00 |
| 338 | `Roid_Sm_Grey` | 430 | Object | -2024.79,-461.92,-168.57 | 420,355,259 | Scale/Radius: 10.00 |
| 339 | `Roid_Sm_Grey` | 432 | Object | -1029.21,115.48,-1795.47 | 395,466,439 | Scale/Radius: 10.00 |
| 340 | `Roid_Sm_Grey` | 436 | Object | -2134.49,-750.61,447.31 | 381,230,228 | Scale/Radius: 10.00 |
| 341 | `Roid_Sm_Grey` | 438 | Object | -815.06,789.11,-2065.02 | 55,354,257 | Scale/Radius: 10.00 |
| 342 | `Roid_Sm_Grey` | 440 | Object | -946.71,134.73,-1972.63 | 127,494,503 | Scale/Radius: 10.00 |
| 343 | `Roid_Sm_Grey` | 442 | Object | -1384.60,-904.59,-732.57 | 447,494,2 | Scale/Radius: 10.00 |
| 344 | `Roid_Sm_Grey` | 448 | Object | -1980.90,173.22,-168.57 | 62,254,100 | Scale/Radius: 10.00 |
| 345 | `Roid_Sm_Grey` | 450 | Object | -880.89,-519.66,-2280.58 | 35,394,355 | Scale/Radius: 10.00 |
| 346 | `Roid_Sm_Grey` | 452 | Object | -617.59,789.11,-1880.25 | 29,170,323 | Scale/Radius: 10.00 |
| 347 | `Roid_Sm_Grey` | 456 | Object | -1604.27,-76.99,-1393.48 | 252,68,94 | Scale/Radius: 10.00 |
| 348 | `Roid_Sm_Grey` | 458 | Object | -1062.12,-673.63,-1918.65 | 79,400,481 | Scale/Radius: 10.00 |
| 349 | `Roid_Sm_Grey` | 464 | Object | -1160.86,269.45,-2072.62 | 485,382,287 | Scale/Radius: 10.00 |
| 350 | `Roid_Sm_Grey` | 466 | Object | -1373.88,-423.42,-500.44 | 11,442,337 | Scale/Radius: 10.00 |
| 351 | `Roid_Sm_Grey` | 474 | Object | -968.65,307.94,-2372.96 | 104,85,301 | Scale/Radius: 10.00 |
| 352 | `Roid_Sm_Grey` | 478 | Object | 1717.89,134.73,1321.61 | 266,143,429 | Scale/Radius: 10.00 |
| 353 | `Roid_Sm_Grey` | 482 | Object | -1757.85,712.12,-623.62 | 36,250,196 | Scale/Radius: 10.00 |
| 354 | `Roid_Sm_Grey` | 484 | Object | -1904.11,-577.40,-291.75 | 352,28,35 | Scale/Radius: 10.00 |
| 355 | `Roid_Sm_Grey` | 486 | Object | -2200.31,-134.73,139.37 | 390,50,288 | Scale/Radius: 10.00 |
| 356 | `Roid_Sm_Grey` | 488 | Object | -749.24,57.74,-2311.37 | 487,459,56 | Scale/Radius: 10.00 |
| 357 | `Roid_Sm_Grey` | 490 | Object | -1538.44,558.15,-1239.51 | 273,275,485 | Scale/Radius: 10.00 |
| 358 | `Roid_Sm_Grey` | 492 | Object | -1713.97,-192.47,-808.38 | 380,2,114 | Scale/Radius: 10.00 |
| 359 | `Roid_Sm_Grey` | 494 | Object | -2013.82,-57.74,-230.16 | 237,230,109 | Scale/Radius: 10.00 |
| 360 | `Roid_Sm_Grey` | 496 | Object | -1783.43,-712.12,-106.98 | 431,136,0 | Scale/Radius: 10.00 |
| 361 | `Roid_Sm_Grey` | 502 | Object | -1330.00,-904.59,-1301.09 | 51,49,466 | Scale/Radius: 10.00 |
| 362 | `Roid_Sm_Grey` | 506 | Object | -1812.71,-134.73,-1085.53 | 297,103,460 | Scale/Radius: 10.00 |
| 363 | `Roid_Sm_Grey` | 512 | Object | -628.56,712.12,-2065.02 | 179,88,32 | Scale/Radius: 10.00 |
| 364 | `Roid_Sm_Grey` | 518 | Object | -1593.29,76.99,-685.21 | 66,461,325 | Scale/Radius: 10.00 |
| 365 | `Roid_Sm_Grey` | 520 | Object | 589.71,-352.21,2304.04 | 160,375,18 | Scale/Radius: 10.00 |
| 366 | `Roid_Sm_Grey` | 522 | Object | -588.18,-35.22,1799.20 | 42,474,205 | Scale/Radius: 10.00 |
| 367 | `Roid_Sm_Grey` | 524 | Object | 277.91,-457.87,2403.35 | 264,368,420 | Scale/Radius: 10.00 |
| 368 | `Roid_Sm_Grey` | 526 | Object | 972.54,-11.74,1274.99 | 82,64,273 | Scale/Radius: 10.00 |
| 369 | `Roid_Sm_Grey` | 528 | Object | 35.41,-575.28,1716.44 | 314,164,346 | Scale/Radius: 10.00 |
| 370 | `Roid_Sm_Grey` | 530 | Object | 1388.27,293.51,968.78 | 312,431,72 | Scale/Radius: 10.00 |
| 371 | `Roid_Sm_Grey` | 532 | Object | 1353.62,23.48,1043.26 | 18,160,423 | Scale/Radius: 10.00 |
| 372 | `Roid_Sm_Grey` | 534 | Object | -241.74,-82.18,1799.20 | 198,409,30 | Scale/Radius: 10.00 |
| 373 | `Roid_Sm_Grey` | 536 | Object | -830.69,281.77,2179.90 | 410,242,258 | Scale/Radius: 10.00 |
| 374 | `Roid_Sm_Grey` | 538 | Object | -241.74,316.99,2469.56 | 483,94,281 | Scale/Radius: 10.00 |
| 375 | `Roid_Sm_Grey` | 540 | Object | -207.10,481.36,2378.52 | 237,496,398 | Scale/Radius: 10.00 |
| 376 | `Roid_Sm_Grey` | 542 | Object | 1318.98,-352.21,993.61 | 267,423,353 | Scale/Radius: 10.00 |
| 377 | `Roid_Sm_Grey` | 544 | Object | -899.97,363.95,2320.59 | 167,142,220 | Scale/Radius: 10.00 |
| 378 | `Roid_Sm_Grey` | 546 | Object | 208.63,352.21,1865.41 | 279,440,422 | Scale/Radius: 10.00 |
| 379 | `Roid_Sm_Grey` | 548 | Object | -207.10,-93.92,1733.00 | 3,404,208 | Scale/Radius: 10.00 |
| 380 | `Roid_Sm_Grey` | 550 | Object | -33.88,-234.81,1799.20 | 2,401,291 | Scale/Radius: 10.00 |
| 381 | `Roid_Sm_Grey` | 552 | Object | 1121.30,434.39,1978.74 | 193,175,365 | Scale/Radius: 10.00 |
| 382 | `Roid_Sm_Grey` | 554 | Object | 573.90,-70.44,1612.46 | 316,483,316 | Scale/Radius: 10.00 |
| 383 | `Roid_Sm_Grey` | 556 | Object | -103.17,-82.18,2130.24 | 315,359,142 | Scale/Radius: 10.00 |
| 384 | `Roid_Sm_Grey` | 558 | Object | -207.10,58.70,1757.82 | 125,240,292 | Scale/Radius: 10.00 |
| 385 | `Roid_Sm_Grey` | 560 | Object | 1086.66,293.51,2119.43 | 11,480,324 | Scale/Radius: 10.00 |
| 386 | `Roid_Sm_Grey` | 562 | Object | 485.78,328.73,2494.39 | 273,64,320 | Scale/Radius: 10.00 |
| 387 | `Roid_Sm_Grey` | 564 | Object | 1155.95,340.47,2003.57 | 27,138,231 | Scale/Radius: 10.00 |
| 388 | `Roid_Sm_Grey` | 566 | Object | 1007.19,-516.58,977.05 | 244,396,352 | Scale/Radius: 10.00 |
| 389 | `Roid_Sm_Grey` | 568 | Object | -1627.49,-387.43,2030.93 | 413,256,351 | Scale/Radius: 10.00 |
| 390 | `Roid_Sm_Grey` | 570 | Object | 70.05,-363.95,2221.28 | 244,327,392 | Scale/Radius: 10.00 |
| 391 | `Roid_Sm_Grey` | 572 | Object | -657.47,270.03,1790.93 | 234,268,302 | Scale/Radius: 10.00 |
| 392 | `Roid_Sm_Grey` | 574 | Object | 485.78,-516.58,1716.44 | 481,75,198 | Scale/Radius: 10.00 |
| 393 | `Roid_Sm_Grey` | 576 | Object | -622.82,387.43,1923.34 | 44,21,108 | Scale/Radius: 10.00 |
| 394 | `Roid_Sm_Grey` | 578 | Object | 347.20,-328.73,2064.04 | 242,407,484 | Scale/Radius: 10.00 |
| 395 | `Roid_Sm_Grey` | 580 | Object | -692.11,-446.13,2213.00 | 242,315,391 | Scale/Radius: 10.00 |
| 396 | `Roid_Sm_Grey` | 582 | Object | 416.49,-105.66,2262.66 | 296,83,306 | Scale/Radius: 10.00 |
| 397 | `Roid_Sm_Grey` | 584 | Object | 1086.66,117.40,1780.12 | 502,256,103 | Scale/Radius: 10.00 |
| 398 | `Roid_Sm_Grey` | 586 | Object | -1662.13,481.36,2030.93 | 487,388,479 | Scale/Radius: 10.00 |
| 399 | `Roid_Sm_Grey` | 588 | Object | 35.41,-575.28,2312.32 | 291,341,57 | Scale/Radius: 10.00 |
| 400 | `Roid_Sm_Grey` | 590 | Object | -1142.48,-281.77,1774.38 | 292,384,148 | Scale/Radius: 10.00 |
| 401 | `Roid_Sm_Grey` | 592 | Object | 173.98,129.14,2411.63 | 94,312,298 | Scale/Radius: 10.00 |
| 402 | `Roid_Sm_Grey` | 594 | Object | 1180.41,-316.99,968.78 | 458,175,337 | Scale/Radius: 10.00 |
| 403 | `Roid_Sm_Grey` | 596 | Object | -1800.71,199.59,1939.90 | 150,395,358 | Scale/Radius: 10.00 |
| 404 | `Roid_Sm_Grey` | 598 | Object | -172.45,-70.44,2304.04 | 392,320,33 | Scale/Radius: 10.00 |
| 405 | `Roid_Sm_Grey` | 600 | Object | 903.26,-199.59,1324.65 | 419,420,455 | Scale/Radius: 10.00 |
| 406 | `Roid_Sm_Grey` | 602 | Object | 1225.23,-11.74,1978.74 | 380,501,384 | Scale/Radius: 10.00 |
| 407 | `Roid_Sm_Grey` | 604 | Object | -726.75,82.18,1840.58 | 510,254,500 | Scale/Radius: 10.00 |
| 408 | `Roid_Sm_Grey` | 606 | Object | -207.10,93.92,2039.21 | 249,430,267 | Scale/Radius: 10.00 |
| 409 | `Roid_Sm_Grey` | 608 | Object | 1284.34,23.48,1672.24 | 478,36,197 | Scale/Radius: 10.00 |
| 410 | `Roid_Sm_Grey` | 610 | Object | 903.26,234.81,1150.85 | 450,211,94 | Scale/Radius: 10.00 |
| 411 | `Roid_Sm_Grey` | 612 | Object | 624.35,152.62,2155.07 | 183,192,85 | Scale/Radius: 10.00 |
| 412 | `Roid_Sm_Grey` | 614 | Object | -1454.27,211.33,2130.24 | 465,254,413 | Scale/Radius: 10.00 |
| 413 | `Roid_Sm_Grey` | 616 | Object | -1454.27,35.22,1989.55 | 47,272,444 | Scale/Radius: 10.00 |
| 414 | `Roid_Sm_Grey` | 618 | Object | 728.28,-211.33,2188.18 | 67,138,399 | Scale/Radius: 10.00 |
| 415 | `Roid_Sm_Grey` | 620 | Object | 1007.19,587.02,977.05 | 219,389,367 | Scale/Radius: 10.00 |
| 416 | `Roid_Sm_Grey` | 622 | Object | 1249.69,199.59,1034.99 | 400,191,221 | Scale/Radius: 10.00 |
| 417 | `Roid_Sm_Grey` | 624 | Object | 624.35,387.43,1848.86 | 169,386,279 | Scale/Radius: 10.00 |
| 418 | `Roid_Sm_Grey` | 626 | Object | 693.64,258.29,2345.42 | 152,169,268 | Scale/Radius: 10.00 |
| 419 | `Roid_Sm_Grey` | 628 | Object | -276.39,363.95,1906.79 | 401,343,179 | Scale/Radius: 10.00 |
| 420 | `Roid_Sm_Grey` | 630 | Object | 1052.01,234.81,1846.33 | 498,315,185 | Scale/Radius: 10.00 |
| 421 | `Roid_Sm_Grey` | 774 | Object | 1611.25,529.66,610.09 | 127,461,55 | Scale/Radius: 10.00 |
| 422 | `Roid_Sm_Grey` | 776 | Object | 1359.51,430.35,769.03 | 316,131,503 | Scale/Radius: 10.00 |
| 423 | `Roid_Sm_Grey` | 778 | Object | 2161.70,-430.35,802.55 | 331,79,210 | Scale/Radius: 10.00 |
| 424 | `Roid_Sm_Grey` | 780 | Object | 1911.49,-99.31,610.09 | 459,461,335 | Scale/Radius: 10.00 |
| 425 | `Roid_Sm_Grey` | 782 | Object | 1974.05,-132.42,1206.73 | 180,88,388 | Scale/Radius: 10.00 |
| 426 | `Roid_Sm_Grey` | 784 | Object | 2311.82,794.50,417.62 | 265,257,395 | Scale/Radius: 10.00 |
| 427 | `Roid_Sm_Grey` | 786 | Object | 2550.68,-711.74,16.84 | 100,346,377 | Scale/Radius: 10.00 |
| 428 | `Roid_Sm_Grey` | 792 | Object | 1723.84,-364.14,975.77 | 384,19,498 | Scale/Radius: 10.00 |
| 429 | `Roid_Sm_Grey` | 794 | Object | 2713.31,331.04,55.34 | 41,84,147 | Scale/Radius: 10.00 |
| 430 | `Roid_Sm_Grey` | 796 | Object | 2789.22,331.04,303.36 | 491,318,131 | Scale/Radius: 10.00 |
| 431 | `Roid_Sm_Grey` | 798 | Object | 2261.78,-331.04,340.64 | 493,289,72 | Scale/Radius: 10.00 |
| 432 | `Roid_Sm_Grey` | 800 | Object | 1472.10,-82.76,345.61 | 93,6,281 | Scale/Radius: 10.00 |
| 433 | `Roid_Sm_Grey` | 802 | Object | 2388.04,-165.52,132.32 | 142,227,505 | Scale/Radius: 10.00 |
| 434 | `Roid_Sm_Grey` | 804 | Object | 2713.31,-231.73,-117.88 | 440,6,466 | Scale/Radius: 10.00 |
| 435 | `Roid_Sm_Grey` | 806 | Object | 2361.86,-430.35,764.06 | 400,143,47 | Scale/Radius: 10.00 |
| 436 | `Roid_Sm_Grey` | 808 | Object | 2211.74,-811.05,802.55 | 26,240,169 | Scale/Radius: 10.00 |
| 437 | `Roid_Sm_Grey` | 810 | Object | 2650.76,480.01,151.57 | 506,48,407 | Scale/Radius: 10.00 |
| 438 | `Roid_Sm_Grey` | 812 | Object | 2275.45,-248.28,170.81 | 94,270,425 | Scale/Radius: 10.00 |
| 439 | `Roid_Sm_Grey` | 814 | Object | 1811.41,-33.10,879.54 | 361,37,67 | Scale/Radius: 10.00 |
| 440 | `Roid_Sm_Grey` | 818 | Object | 2388.04,480.01,267.05 | 469,472,82 | Scale/Radius: 10.00 |
| 441 | `Roid_Sm_Grey` | 822 | Object | 1873.96,66.21,1091.25 | 400,478,174 | Scale/Radius: 10.00 |
| 442 | `Roid_Sm_Grey` | 824 | Object | 2299.31,-115.86,841.05 | 359,4,306 | Scale/Radius: 10.00 |
| 443 | `Roid_Sm_Grey` | 828 | Object | 1636.27,364.14,1341.46 | 295,146,241 | Scale/Radius: 10.00 |
| 444 | `Roid_Sm_Grey` | 830 | Object | 2099.15,827.60,552.35 | 168,460,487 | Scale/Radius: 10.00 |
| 445 | `Roid_Sm_Grey` | 834 | Object | 2236.76,-794.50,667.83 | 373,67,296 | Scale/Radius: 10.00 |
| 446 | `Roid_Sm_Grey` | 836 | Object | 1661.29,-678.63,1110.50 | 344,88,68 | Scale/Radius: 10.00 |
| 447 | `Roid_Sm_Grey` | 838 | Object | 1673.80,612.42,1014.27 | 37,169,103 | Scale/Radius: 10.00 |
| 448 | `Roid_Sm_Grey` | 840 | Object | 1648.78,-777.94,1360.70 | 333,487,308 | Scale/Radius: 10.00 |
| 449 | `Roid_Sm_Grey` | 844 | Object | 2488.12,49.66,-194.87 | 328,19,15 | Scale/Radius: 10.00 |
| 450 | `Roid_Sm_Grey` | 846 | Object | 2024.09,413.80,1072.01 | 44,28,43 | Scale/Radius: 10.00 |
| 451 | `Roid_Sm_Grey` | 848 | Object | 2564.04,628.98,303.36 | 371,142,363 | Scale/Radius: 10.00 |
| 452 | `Roid_Sm_Grey` | 852 | Object | 2174.21,678.63,1379.95 | 491,411,177 | Scale/Radius: 10.00 |
| 453 | `Roid_Sm_Grey` | 854 | Object | 2161.70,-16.55,590.84 | 254,468,41 | Scale/Radius: 10.00 |
| 454 | `Roid_Sm_Grey` | 856 | Object | 1798.90,281.38,475.36 | 478,293,44 | Scale/Radius: 10.00 |
| 455 | `Roid_Sm_Grey` | 858 | Object | 1296.96,-148.97,769.03 | 76,294,237 | Scale/Radius: 10.00 |
| 456 | `Roid_Sm_Grey` | 862 | Object | 2136.68,-480.01,533.10 | 17,219,237 | Scale/Radius: 10.00 |
| 457 | `Roid_Sm_Grey` | 864 | Object | 2049.11,380.70,648.58 | 137,378,421 | Scale/Radius: 10.00 |
| 458 | `Roid_Sm_Grey` | 866 | Object | 1898.98,-645.53,359.89 | 148,465,110 | Scale/Radius: 10.00 |
| 459 | `Roid_Sm_Grey` | 868 | Object | 1736.35,529.66,379.13 | 447,154,497 | Scale/Radius: 10.00 |
| 460 | `Roid_Sm_Grey` | 870 | Object | 2211.74,480.01,1014.27 | 442,86,119 | Scale/Radius: 10.00 |
| 461 | `Roid_Sm_Grey` | 872 | Object | 1472.10,347.59,576.56 | 268,72,93 | Scale/Radius: 10.00 |
| 462 | `Roid_Sm_Grey` | 874 | Object | 2411.90,-148.97,918.03 | 380,427,374 | Scale/Radius: 10.00 |
| 463 | `Roid_Sm_Grey` | 920 | Object | -1927.24,165.52,1394.80 | 61,161,47 | Scale/Radius: 10.00 |
| 464 | `Roid_Sm_Grey` | 924 | Object | -1904.14,-84.68,1325.51 | 478,412,209 | Scale/Radius: 10.00 |
| 465 | `Roid_Sm_Grey` | 928 | Object | -2019.62,157.82,1163.84 | 296,362,101 | Scale/Radius: 10.00 |
| 466 | `Roid_Sm_Grey` | 932 | Object | -1873.35,100.08,1271.62 | 424,383,348 | Scale/Radius: 10.00 |
| 467 | `Roid_Sm_Grey` | 940 | Object | -1950.33,-153.97,986.77 | 511,286,316 | Scale/Radius: 10.00 |
| 468 | `Roid_Sm_Grey` | 948 | Object | -1929.89,-326.90,1202.33 | 55,124,478 | Scale/Radius: 10.00 |
| 469 | `Roid_Sm_Grey` | 960 | Object | -1927.24,130.88,1125.35 | 46,43,156 | Scale/Radius: 10.00 |
| 470 | `Roid_Sm_Grey` | 964 | Object | -1719.37,11.55,1471.78 | 421,177,234 | Scale/Radius: 10.00 |
| 471 | `Roid_Sm_Grey` | 976 | Object | -1696.28,73.14,1402.50 | 329,403,286 | Scale/Radius: 10.00 |
| 472 | `Roid_Sm_Grey` | 996 | Object | -1773.26,-123.18,871.29 | 194,303,263 | Scale/Radius: 10.00 |
| 473 | `Roid_Sm_Grey` | 1016 | Object | -1965.73,-134.73,1479.48 | 331,508,451 | Scale/Radius: 10.00 |
| 474 | `Spcargo_Contraband` | 1738 | Interactive | 168.40,0.00,-926.40 | 469,78,341 | secondary groups: CONT_031, none |
| 475 | `Mad_Pirate_Station` | 1537 | Interactive | 20.61,0.00,-653.15 | 437,0,0 | secondary groups: none, DEMON_STATION |
| 476 | `Vacuum_Translucency_Module` | 1612 | Interactive | -911.78,-797.52,-1144.20 | 0,0,0 | secondary groups: CONT_UNKNOWN, none |
| 477 | `Mad_Pirate_Platform` | 1622 | Interactive | -1677.39,850.97,566.75 | 438,0,0 | None |
| 478 | `Mad_Pirate_Platform` | 1626 | Interactive | -1354.12,83.97,392.81 | 437,0,0 | None |
| 479 | `Mad_Pirate_Platform` | 1630 | Interactive | 1397.64,86.25,-1696.33 | 437,0,0 | label: MPP1 |
