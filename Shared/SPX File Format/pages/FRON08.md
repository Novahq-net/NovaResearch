# Tachyon: The Fringe FRON08.SPX - Strafing Run

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON08.SPX` |
| Sector | `QUAD_08` |
| Backdrop | `FRONTI8.BDF` |
| Region | 4 |
| Sector ID | 7 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 6 |
| Entities | 259 |
| Events | 4 |
| Waypoints | 0 |
| Child Sectors | 4 |
| Scripts | 1 |
| Scenes | 2 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Mad_Pirate_Platform`, `1: Baron_Hajod_Slave`, `2: Spcargo_Credits`, `3: Roid_Sm_Brown`, `4: Asteroid_2`, `5: Hyper_Gate` |
| Scripts | `PLAYER.SCR` |
| Scenes | `F8BC050A.SEN`, `F9GC030A.SEN` |
| Labels | `bfne_03`, `bfne_01`, `HSLAV`, `BFGE_01`, `CHAPEL` |
| Aliases | `Jerome01`, `Jerome02`, `Jerome03`, `Jerome04`, `Jerome05`, `Jerome06`, `bc05_2`, `bc05_1`, `bc05_4`, `bc05_5`, `BC05_Sistine_Chapel` |
| Groups | `CONT_065`, `IRONHAND_STATION` |
| Child Sectors | [fron08A.spx](FRON08A.md), [fron08B.spx](FRON08B.md), [fron08C.spx](FRON08C.md), [fron08D.spx](FRON08D.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 0, variable 4, op 1, value 4011
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Set/add variable: variable group 16, variable 414, subtype 0, value 1
- Set/add variable: variable group 16, variable 415, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 11, param 38
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 21, variable 20, subtype 0, value 2

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 0, variable 4, op 1, value 4011
- Variable comparison: subject variable group 21, variable 21, op 0, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 102

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 1111; flags 2)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 13
- Show/update HUD contact: contact/list 0, subtype 9, param 41
- Set/add variable: variable group 16, variable 810, subtype 0, value 1
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 32, op 2, value 10

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 41
- Set/add variable: variable group 20, variable 32, subtype 0, value 0

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | -1649.64,293.91,766.93 | 186,0,0 | Gate SPX: [fron01.spx](FRON01.md) |
| 1 | `Hyper_Gate` | 2 | Gate | 2081.03,262.81,643.34 | 316,0,0 | Gate SPX: [fron09.spx](FRON09.md) |
| 2 | `Asteroid_2` | 654 | Object | -1362.79,223.20,1097.28 | 434,8,267 | Scale/Radius: 10.00 |
| 3 | `Asteroid_2` | 374 | Object | -1728.17,73.91,-466.98 | 432,157,154 | Scale/Radius: 10.00 |
| 4 | `Asteroid_2` | 376 | Object | 178.10,-60.11,1043.38 | 189,238,5 | Scale/Radius: 10.00 |
| 5 | `Asteroid_2` | 378 | Object | 2563.09,223.20,1167.50 | 99,407,267 | Scale/Radius: 10.00 |
| 6 | `Asteroid_2` | 380 | Object | 306.85,-109.38,1165.22 | 158,338,473 | Scale/Radius: 10.00 |
| 7 | `Asteroid_2` | 386 | Object | -419.47,-60.11,1455.85 | 466,20,35 | Scale/Radius: 10.00 |
| 8 | `Asteroid_2` | 390 | Object | 2166.72,517.35,-634.14 | 497,184,301 | Scale/Radius: 10.00 |
| 9 | `Asteroid_2` | 392 | Object | 1818.11,457.24,1376.56 | 490,12,347 | Scale/Radius: 10.00 |
| 10 | `Asteroid_2` | 396 | Object | 1569.11,443.44,-2337.74 | 310,508,129 | Scale/Radius: 10.00 |
| 11 | `Asteroid_2` | 398 | Object | -139.45,-392.69,1120.85 | 490,510,391 | Scale/Radius: 10.00 |
| 12 | `Asteroid_2` | 400 | Object | 2664.71,-183.29,1105.91 | 130,327,51 | Scale/Radius: 10.00 |
| 13 | `Asteroid_2` | 402 | Object | 2090.60,-455.76,-938.61 | 111,261,294 | Scale/Radius: 10.00 |
| 14 | `Asteroid_2` | 404 | Object | -1980.29,-98.54,-303.89 | 261,257,242 | Scale/Radius: 10.00 |
| 15 | `Asteroid_2` | 406 | Object | -1800.66,147.81,-586.86 | 389,230,257 | Scale/Radius: 10.00 |
| 16 | `Asteroid_2` | 408 | Object | 2723.43,-36.95,430.46 | 297,104,60 | Scale/Radius: 10.00 |
| 17 | `Asteroid_2` | 410 | Object | -450.86,136.98,1321.48 | 216,147,77 | Scale/Radius: 10.00 |
| 18 | `Asteroid_2` | 412 | Object | 1042.25,124.66,1128.08 | 175,177,268 | Scale/Radius: 10.00 |
| 19 | `Asteroid_2` | 414 | Object | 1738.48,529.66,-2060.59 | 199,328,141 | Scale/Radius: 10.00 |
| 20 | `Asteroid_2` | 416 | Object | 270.48,173.93,1081.65 | 344,154,217 | Scale/Radius: 10.00 |
| 21 | `Asteroid_2` | 420 | Object | 2215.06,-110.86,-1030.99 | 112,420,4 | Scale/Radius: 10.00 |
| 22 | `Asteroid_2` | 422 | Object | -2031.79,-528.18,1030.14 | 191,451,158 | Scale/Radius: 10.00 |
| 23 | `Asteroid_2` | 424 | Object | 1384.18,431.12,-2372.29 | 351,282,62 | Scale/Radius: 10.00 |
| 24 | `Asteroid_2` | 426 | Object | 1857.68,-283.31,-1479.30 | 77,101,221 | Scale/Radius: 10.00 |
| 25 | `Asteroid_2` | 432 | Object | 1762.04,184.77,-1655.51 | 176,131,425 | Scale/Radius: 10.00 |
| 26 | `Asteroid_2` | 436 | Object | 2892.80,578.94,553.64 | 251,63,230 | Scale/Radius: 10.00 |
| 27 | `Asteroid_2` | 448 | Object | 2171.27,-357.22,-1160.67 | 274,410,509 | Scale/Radius: 10.00 |
| 28 | `Asteroid_2` | 450 | Object | 873.89,297.11,1212.95 | 206,169,449 | Scale/Radius: 10.00 |
| 29 | `Asteroid_2` | 452 | Object | -450.86,75.39,1321.48 | 462,306,445 | Scale/Radius: 10.00 |
| 30 | `Asteroid_2` | 458 | Object | -1616.15,332.58,-333.78 | 81,200,104 | Scale/Radius: 10.00 |
| 31 | `Asteroid_2` | 460 | Object | 1806.22,-49.27,-2245.36 | 249,261,162 | Scale/Radius: 10.00 |
| 32 | `Asteroid_2` | 462 | Object | -737.98,-492.71,-2541.02 | 263,322,42 | Scale/Radius: 10.00 |
| 33 | `Asteroid_2` | 464 | Object | 2951.60,-125.17,1026.48 | 130,125,21 | Scale/Radius: 10.00 |
| 34 | `Asteroid_2` | 468 | Object | -636.36,307.94,-2417.84 | 252,134,330 | Scale/Radius: 10.00 |
| 35 | `Asteroid_2` | 470 | Object | -500.87,-357.22,-2694.99 | 383,83,486 | Scale/Radius: 10.00 |
| 36 | `Asteroid_2` | 472 | Object | -346.57,605.05,1251.25 | 193,319,284 | Scale/Radius: 10.00 |
| 37 | `Asteroid_2` | 476 | Object | 1897.53,-406.49,-1624.71 | 90,230,88 | Scale/Radius: 10.00 |
| 38 | `Asteroid_2` | 478 | Object | 164.96,260.15,1178.57 | 95,292,349 | Scale/Radius: 10.00 |
| 39 | `Asteroid_2` | 480 | Object | -1938.49,-209.40,233.67 | 89,212,231 | Scale/Radius: 10.00 |
| 40 | `Asteroid_2` | 484 | Object | 2866.40,529.66,889.86 | 460,0,409 | Scale/Radius: 10.00 |
| 41 | `Asteroid_2` | 486 | Object | 2866.40,-36.95,797.48 | 77,0,492 | Scale/Radius: 10.00 |
| 42 | `Asteroid_2` | 488 | Object | -1810.92,369.53,-211.51 | 63,344,496 | Scale/Radius: 10.00 |
| 43 | `Asteroid_2` | 490 | Object | 876.33,210.88,1131.92 | 117,12,337 | Scale/Radius: 10.00 |
| 44 | `Asteroid_2` | 500 | Object | -959.31,517.35,-2106.18 | 325,103,441 | Scale/Radius: 10.00 |
| 45 | `Asteroid_2` | 502 | Object | 2469.62,554.30,-315.39 | 440,216,332 | Scale/Radius: 10.00 |
| 46 | `Asteroid_2` | 504 | Object | 2189.84,-97.06,1709.54 | 355,433,257 | Scale/Radius: 10.00 |
| 47 | `Asteroid_2` | 506 | Object | 501.46,505.03,-2886.21 | 359,486,201 | Scale/Radius: 10.00 |
| 48 | `Asteroid_2` | 510 | Object | -1376.30,246.36,-1597.64 | 204,375,26 | Scale/Radius: 10.00 |
| 49 | `Asteroid_2` | 512 | Object | 1873.97,123.18,-2152.97 | 484,23,88 | Scale/Radius: 10.00 |
| 50 | `Asteroid_2` | 514 | Object | -2234.16,-492.71,55.85 | 462,168,154 | Scale/Radius: 10.00 |
| 51 | `Asteroid_2` | 520 | Object | 1076.13,457.24,1312.84 | 300,39,148 | Scale/Radius: 10.00 |
| 52 | `Asteroid_2` | 524 | Object | -1345.88,-320.26,-1013.57 | 444,297,161 | Scale/Radius: 10.00 |
| 53 | `Asteroid_2` | 526 | Object | 2416.57,578.94,45.40 | 140,509,251 | Scale/Radius: 10.00 |
| 54 | `Asteroid_2` | 530 | Object | 1313.25,-10.84,1405.23 | 385,17,274 | Scale/Radius: 10.00 |
| 55 | `Asteroid_2` | 532 | Object | 970.33,-565.14,1019.91 | 374,358,376 | Scale/Radius: 10.00 |
| 56 | `Asteroid_2` | 536 | Object | -1277.83,468.08,-1952.29 | 242,442,505 | Scale/Radius: 10.00 |
| 57 | `Asteroid_2` | 538 | Object | -1193.42,235.52,1189.66 | 159,369,334 | Scale/Radius: 10.00 |
| 58 | `Asteroid_2` | 540 | Object | -1556.61,-357.22,-675.62 | 64,57,186 | Scale/Radius: 10.00 |
| 59 | `Asteroid_2` | 542 | Object | 1719.73,272.47,1559.20 | 496,487,32 | Scale/Radius: 10.00 |
| 60 | `Asteroid_2` | 544 | Object | -1193.42,1.48,1220.46 | 58,459,36 | Scale/Radius: 10.00 |
| 61 | `Asteroid_2` | 546 | Object | -302.42,320.26,-2826.39 | 200,335,335 | Scale/Radius: 10.00 |
| 62 | `Asteroid_2` | 548 | Object | -737.98,270.99,-2448.64 | 323,377,145 | Scale/Radius: 10.00 |
| 63 | `Asteroid_2` | 554 | Object | 1011.82,-47.79,1285.89 | 425,188,134 | Scale/Radius: 10.00 |
| 64 | `Asteroid_2` | 556 | Object | -573.42,-123.18,-2918.77 | 62,319,502 | Scale/Radius: 10.00 |
| 65 | `Asteroid_2` | 558 | Object | 2595.41,86.22,705.10 | 475,317,414 | Scale/Radius: 10.00 |
| 66 | `Asteroid_2` | 560 | Object | -1413.63,431.12,-1167.54 | 280,500,345 | Scale/Radius: 10.00 |
| 67 | `Asteroid_2` | 562 | Object | -1968.61,529.66,704.74 | 79,371,419 | Scale/Radius: 10.00 |
| 68 | `Asteroid_2` | 566 | Object | 477.16,-429.64,1085.49 | 331,6,442 | Scale/Radius: 10.00 |
| 69 | `Asteroid_2` | 568 | Object | -74.40,-505.03,-2855.42 | 439,75,39 | Scale/Radius: 10.00 |
| 70 | `Asteroid_2` | 570 | Object | -1308.55,-578.94,-1566.85 | 158,258,117 | Scale/Radius: 10.00 |
| 71 | `Asteroid_2` | 572 | Object | 2156.84,161.61,1130.21 | 406,189,152 | Scale/Radius: 10.00 |
| 72 | `Asteroid_2` | 576 | Object | 1009.39,63.07,1182.16 | 366,378,371 | Scale/Radius: 10.00 |
| 73 | `Asteroid_2` | 578 | Object | 1636.85,98.54,-2337.74 | 449,293,322 | Scale/Radius: 10.00 |
| 74 | `Asteroid_2` | 582 | Object | 603.08,184.77,-2855.42 | 85,274,268 | Scale/Radius: 10.00 |
| 75 | `Asteroid_2` | 584 | Object | 27.22,123.18,-2855.42 | 162,371,398 | Scale/Radius: 10.00 |
| 76 | `Asteroid_2` | 586 | Object | -1683.89,-332.58,-272.19 | 276,449,245 | Scale/Radius: 10.00 |
| 77 | `Asteroid_2` | 588 | Object | -1855.40,518.83,1246.13 | 286,422,295 | Scale/Radius: 10.00 |
| 78 | `Asteroid_2` | 592 | Object | -1523.78,-541.98,-917.26 | 50,257,232 | Scale/Radius: 10.00 |
| 79 | `Asteroid_2` | 594 | Object | 903.29,172.45,-2639.39 | 174,337,251 | Scale/Radius: 10.00 |
| 80 | `Asteroid_2` | 596 | Object | 555.67,541.98,-2790.26 | 494,190,244 | Scale/Radius: 10.00 |
| 81 | `Asteroid_2` | 598 | Object | 267.52,-246.36,-3068.49 | 406,67,400 | Scale/Radius: 10.00 |
| 82 | `Asteroid_2` | 600 | Object | -839.60,-12.32,-2664.20 | 121,232,463 | Scale/Radius: 10.00 |
| 83 | `Asteroid_2` | 602 | Object | -74.40,123.18,-2855.42 | 224,39,55 | Scale/Radius: 10.00 |
| 84 | `Asteroid_2` | 604 | Object | -2138.04,-270.99,236.70 | 438,266,453 | Scale/Radius: 10.00 |
| 85 | `Asteroid_2` | 606 | Object | -617.56,-429.64,1620.79 | 298,480,143 | Scale/Radius: 10.00 |
| 86 | `Asteroid_2` | 608 | Object | 872.89,100.02,1128.08 | 4,483,435 | Scale/Radius: 10.00 |
| 87 | `Asteroid_2` | 612 | Object | 2229.08,-110.86,-864.08 | 192,312,94 | Scale/Radius: 10.00 |
| 88 | `Asteroid_2` | 620 | Object | -1629.34,246.36,-841.65 | 137,196,85 | Scale/Radius: 10.00 |
| 89 | `Asteroid_2` | 622 | Object | 2382.69,369.53,14.61 | 59,84,459 | Scale/Radius: 10.00 |
| 90 | `Asteroid_2` | 626 | Object | -1464.41,617.37,1559.20 | 274,245,148 | Scale/Radius: 10.00 |
| 91 | `Asteroid_2` | 638 | Object | -413.14,406.49,-2917.01 | 464,199,77 | Scale/Radius: 10.00 |
| 92 | `Asteroid_2` | 642 | Object | 999.95,554.30,-2620.99 | 272,276,352 | Scale/Radius: 10.00 |
| 93 | `Asteroid_2` | 644 | Object | 1143.88,210.88,1158.87 | 489,500,179 | Scale/Radius: 10.00 |
| 94 | `Asteroid_2` | 650 | Object | 165.90,283.31,-3160.87 | 435,320,468 | Scale/Radius: 10.00 |
| 95 | `Asteroid_2` | 658 | Object | 1485.81,-258.67,-2649.44 | 266,328,422 | Scale/Radius: 10.00 |
| 96 | `Asteroid_2` | 660 | Object | -2166.41,344.90,25.06 | 30,26,154 | Scale/Radius: 10.00 |
| 97 | `Asteroid_2` | 662 | Object | 1681.47,-86.22,-1822.80 | 140,433,341 | Scale/Radius: 10.00 |
| 98 | `Asteroid_2` | 664 | Object | 2200.60,-110.86,-634.14 | 206,90,360 | Scale/Radius: 10.00 |
| 99 | `Asteroid_2` | 668 | Object | 2595.41,221.72,859.07 | 32,90,441 | Scale/Radius: 10.00 |
| 100 | `Asteroid_2` | 670 | Object | -1880.67,541.98,404.73 | 90,102,478 | Scale/Radius: 10.00 |
| 101 | `Asteroid_2` | 672 | Object | 2764.78,480.39,828.28 | 217,411,242 | Scale/Radius: 10.00 |
| 102 | `Asteroid_2` | 680 | Object | 1979.03,112.34,1465.76 | 152,325,395 | Scale/Radius: 10.00 |
| 103 | `Asteroid_2` | 682 | Object | 1636.85,-283.31,-2276.15 | 85,421,340 | Scale/Radius: 10.00 |
| 104 | `Asteroid_2` | 686 | Object | -2219.40,-578.94,466.32 | 21,71,182 | Scale/Radius: 10.00 |
| 105 | `Asteroid_2` | 690 | Object | 1831.10,-368.05,1735.01 | 368,353,426 | Scale/Radius: 10.00 |
| 106 | `Asteroid_2` | 698 | Object | 2791.17,-566.62,522.85 | 427,348,20 | Scale/Radius: 10.00 |
| 107 | `Asteroid_2` | 700 | Object | 452.38,566.62,-2725.27 | 7,129,208 | Scale/Radius: 10.00 |
| 108 | `Asteroid_2` | 704 | Object | -466.99,-566.62,-2756.58 | 455,348,361 | Scale/Radius: 10.00 |
| 109 | `Roid_Sm_Brown` | 499 | Object | -719.19,-269.51,1620.79 | 423,404,106 | Scale/Radius: 10.00 |
| 110 | `Roid_Sm_Brown` | 377 | Object | 590.57,346.38,1212.95 | 235,183,105 | Scale/Radius: 10.00 |
| 111 | `Roid_Sm_Brown` | 379 | Object | 2454.66,-246.36,-564.22 | 174,217,225 | Scale/Radius: 10.00 |
| 112 | `Roid_Sm_Brown` | 381 | Object | -2216.43,-10.84,1121.85 | 201,293,423 | Scale/Radius: 10.00 |
| 113 | `Roid_Sm_Brown` | 383 | Object | -1655.73,-529.66,-1056.42 | 510,75,380 | Scale/Radius: 10.00 |
| 114 | `Roid_Sm_Brown` | 385 | Object | -959.31,-36.95,-2260.15 | 367,449,478 | Scale/Radius: 10.00 |
| 115 | `Roid_Sm_Brown` | 387 | Object | 1806.22,517.35,-2276.15 | 240,323,274 | Scale/Radius: 10.00 |
| 116 | `Roid_Sm_Brown` | 389 | Object | 1850.84,529.66,-1730.42 | 29,328,482 | Scale/Radius: 10.00 |
| 117 | `Roid_Sm_Brown` | 391 | Object | -1930.17,469.56,1091.72 | 55,305,289 | Scale/Radius: 10.00 |
| 118 | `Roid_Sm_Brown` | 395 | Object | 2605.12,197.08,-346.18 | 41,312,235 | Scale/Radius: 10.00 |
| 119 | `Roid_Sm_Brown` | 397 | Object | 2900.27,480.39,766.69 | 166,74,431 | Scale/Radius: 10.00 |
| 120 | `Roid_Sm_Brown` | 399 | Object | 2065.53,-344.90,-1438.52 | 415,305,188 | Scale/Radius: 10.00 |
| 121 | `Roid_Sm_Brown` | 401 | Object | -993.19,418.80,-2444.92 | 245,374,191 | Scale/Radius: 10.00 |
| 122 | `Roid_Sm_Brown` | 403 | Object | -840.32,580.42,1255.34 | 35,392,197 | Scale/Radius: 10.00 |
| 123 | `Roid_Sm_Brown` | 405 | Object | 2518.19,258.67,291.76 | 384,98,322 | Scale/Radius: 10.00 |
| 124 | `Roid_Sm_Brown` | 407 | Object | -990.50,-540.50,1652.68 | 489,272,258 | Scale/Radius: 10.00 |
| 125 | `Roid_Sm_Brown` | 413 | Object | 467.58,160.13,-3163.36 | 414,263,238 | Scale/Radius: 10.00 |
| 126 | `Roid_Sm_Brown` | 415 | Object | 1850.84,246.36,-1945.98 | 211,365,301 | Scale/Radius: 10.00 |
| 127 | `Roid_Sm_Brown` | 417 | Object | -1473.85,-554.30,-1412.87 | 249,285,310 | Scale/Radius: 10.00 |
| 128 | `Roid_Sm_Brown` | 419 | Object | 1811.22,529.66,-1075.83 | 83,398,413 | Scale/Radius: 10.00 |
| 129 | `Roid_Sm_Brown` | 421 | Object | 1625.76,-220.24,1225.91 | 382,358,288 | Scale/Radius: 10.00 |
| 130 | `Roid_Sm_Brown` | 423 | Object | -805.73,-73.91,-2263.87 | 128,273,317 | Scale/Radius: 10.00 |
| 131 | `Roid_Sm_Brown` | 425 | Object | 1587.43,-49.27,-2557.06 | 293,5,29 | Scale/Radius: 10.00 |
| 132 | `Roid_Sm_Brown` | 429 | Object | 2021.09,554.30,-1754.88 | 13,270,236 | Scale/Radius: 10.00 |
| 133 | `Roid_Sm_Brown` | 431 | Object | -1821.53,198.56,1369.31 | 194,103,287 | Scale/Radius: 10.00 |
| 134 | `Roid_Sm_Brown` | 433 | Object | 2055.22,-158.65,1191.80 | 32,53,70 | Scale/Radius: 10.00 |
| 135 | `Roid_Sm_Brown` | 435 | Object | -176.02,-12.32,-2886.21 | 225,152,207 | Scale/Radius: 10.00 |
| 136 | `Roid_Sm_Brown` | 437 | Object | 1685.86,444.92,1559.20 | 467,187,416 | Scale/Radius: 10.00 |
| 137 | `Roid_Sm_Brown` | 441 | Object | 9.56,161.61,1263.11 | 156,14,237 | Scale/Radius: 10.00 |
| 138 | `Roid_Sm_Brown` | 443 | Object | 1761.25,-35.47,1195.11 | 432,435,472 | Scale/Radius: 10.00 |
| 139 | `Roid_Sm_Brown` | 445 | Object | 2732.46,334.06,1259.88 | 393,211,288 | Scale/Radius: 10.00 |
| 140 | `Roid_Sm_Brown` | 447 | Object | 1177.75,-441.96,1035.69 | 348,230,200 | Scale/Radius: 10.00 |
| 141 | `Roid_Sm_Brown` | 451 | Object | 2757.30,123.18,553.64 | 84,5,480 | Scale/Radius: 10.00 |
| 142 | `Roid_Sm_Brown` | 453 | Object | -310.30,420.28,1352.83 | 29,276,255 | Scale/Radius: 10.00 |
| 143 | `Roid_Sm_Brown` | 455 | Object | 1519.68,-221.72,-2526.27 | 394,252,266 | Scale/Radius: 10.00 |
| 144 | `Roid_Sm_Brown` | 457 | Object | 1076.13,506.51,1158.87 | 135,373,403 | Scale/Radius: 10.00 |
| 145 | `Roid_Sm_Brown` | 459 | Object | -998.03,234.04,-1495.51 | 176,214,264 | Scale/Radius: 10.00 |
| 146 | `Roid_Sm_Brown` | 461 | Object | 981.16,320.26,-3036.14 | 364,267,157 | Scale/Radius: 10.00 |
| 147 | `Roid_Sm_Brown` | 463 | Object | -1556.61,-147.81,-644.83 | 468,226,430 | Scale/Radius: 10.00 |
| 148 | `Roid_Sm_Brown` | 465 | Object | 2757.30,24.64,276.49 | 367,252,349 | Scale/Radius: 10.00 |
| 149 | `Roid_Sm_Brown` | 467 | Object | -1206.93,-12.32,-1351.28 | 304,261,45 | Scale/Radius: 10.00 |
| 150 | `Roid_Sm_Brown` | 469 | Object | -1024.05,-343.42,1343.64 | 88,143,56 | Scale/Radius: 10.00 |
| 151 | `Roid_Sm_Brown` | 471 | Object | 2619.81,381.85,-46.98 | 286,158,204 | Scale/Radius: 10.00 |
| 152 | `Roid_Sm_Brown` | 473 | Object | -1173.05,394.17,-1536.05 | 110,480,424 | Scale/Radius: 10.00 |
| 153 | `Roid_Sm_Brown` | 475 | Object | 981.16,-517.35,-2974.55 | 218,445,133 | Scale/Radius: 10.00 |
| 154 | `Roid_Sm_Brown` | 477 | Object | 2059.71,160.13,-1140.37 | 132,341,183 | Scale/Radius: 10.00 |
| 155 | `Roid_Sm_Brown` | 479 | Object | 2089.10,506.51,1376.56 | 498,184,465 | Scale/Radius: 10.00 |
| 156 | `Roid_Sm_Brown` | 483 | Object | -1930.17,-294.15,999.34 | 217,352,509 | Scale/Radius: 10.00 |
| 157 | `Roid_Sm_Brown` | 487 | Object | 2395.58,-332.58,-799.43 | 462,427,12 | Scale/Radius: 10.00 |
| 158 | `Roid_Sm_Brown` | 489 | Object | 2056.73,591.25,-907.82 | 10,427,112 | Scale/Radius: 10.00 |
| 159 | `Roid_Sm_Brown` | 491 | Object | -1659.52,-441.96,1609.05 | 418,112,213 | Scale/Radius: 10.00 |
| 160 | `Roid_Sm_Brown` | 493 | Object | 2097.01,24.64,-253.80 | 344,118,173 | Scale/Radius: 10.00 |
| 161 | `Roid_Sm_Brown` | 495 | Object | 1670.73,-566.62,-2460.92 | 89,216,499 | Scale/Radius: 10.00 |
| 162 | `Roid_Sm_Brown` | 497 | Object | 2721.43,480.39,14.61 | 424,258,11 | Scale/Radius: 10.00 |
| 163 | `Roid_Sm_Brown` | 501 | Object | -1196.43,295.63,-2136.98 | 510,317,230 | Scale/Radius: 10.00 |
| 164 | `Roid_Sm_Brown` | 503 | Object | 316.19,-36.95,-2955.96 | 192,176,100 | Scale/Radius: 10.00 |
| 165 | `Roid_Sm_Brown` | 505 | Object | -274.94,383.33,1182.44 | 88,97,89 | Scale/Radius: 10.00 |
| 166 | `Roid_Sm_Brown` | 507 | Object | 1685.86,494.19,1713.17 | 173,136,82 | Scale/Radius: 10.00 |
| 167 | `Roid_Sm_Brown` | 509 | Object | -2287.69,-36.95,739.61 | 51,193,182 | Scale/Radius: 10.00 |
| 168 | `Roid_Sm_Brown` | 511 | Object | -1108.46,-492.71,-1705.93 | 48,381,387 | Scale/Radius: 10.00 |
| 169 | `Roid_Sm_Brown` | 513 | Object | -2055.51,492.71,922.44 | 31,352,426 | Scale/Radius: 10.00 |
| 170 | `Roid_Sm_Brown` | 515 | Object | 2800.20,-565.14,1167.50 | 481,196,234 | Scale/Radius: 10.00 |
| 171 | `Roid_Sm_Brown` | 517 | Object | -2200.29,541.98,-36.53 | 108,300,27 | Scale/Radius: 10.00 |
| 172 | `Roid_Sm_Brown` | 519 | Object | -568.61,234.04,-2571.81 | 358,317,12 | Scale/Radius: 10.00 |
| 173 | `Roid_Sm_Brown` | 521 | Object | 556.70,-72.43,1151.36 | 80,277,365 | Scale/Radius: 10.00 |
| 174 | `Roid_Sm_Brown` | 523 | Object | 30.41,-554.30,-3191.66 | 417,139,166 | Scale/Radius: 10.00 |
| 175 | `Roid_Sm_Brown` | 527 | Object | 1829.78,492.71,-1624.71 | 315,184,336 | Scale/Radius: 10.00 |
| 176 | `Roid_Sm_Brown` | 529 | Object | 704.53,-220.24,1212.95 | 83,339,238 | Scale/Radius: 10.00 |
| 177 | `Roid_Sm_Brown` | 531 | Object | 2022.03,-529.66,-582.99 | 97,241,52 | Scale/Radius: 10.00 |
| 178 | `Roid_Sm_Brown` | 533 | Object | 738.40,629.69,1212.95 | 401,169,268 | Scale/Radius: 10.00 |
| 179 | `Roid_Sm_Brown` | 535 | Object | 1016.66,-394.17,-2765.91 | 23,452,172 | Scale/Radius: 10.00 |
| 180 | `Roid_Sm_Brown` | 537 | Object | -617.56,-257.19,1559.20 | 492,445,141 | Scale/Radius: 10.00 |
| 181 | `Roid_Sm_Brown` | 539 | Object | 679.36,517.35,-2963.09 | 116,20,346 | Scale/Radius: 10.00 |
| 182 | `Roid_Sm_Brown` | 541 | Object | 2201.02,566.62,-1469.31 | 409,444,15 | Scale/Radius: 10.00 |
| 183 | `Roid_Sm_Brown` | 543 | Object | 1023.23,-135.50,-2479.45 | 110,195,206 | Scale/Radius: 10.00 |
| 184 | `Roid_Sm_Brown` | 545 | Object | -518.61,-97.06,1352.27 | 253,130,285 | Scale/Radius: 10.00 |
| 185 | `Roid_Sm_Brown` | 547 | Object | 2190.72,-183.29,1161.00 | 95,61,253 | Scale/Radius: 10.00 |
| 186 | `Roid_Sm_Brown` | 549 | Object | -1980.29,381.85,-211.51 | 50,452,318 | Scale/Radius: 10.00 |
| 187 | `Roid_Sm_Brown` | 551 | Object | 2825.05,-492.71,430.46 | 299,502,49 | Scale/Radius: 10.00 |
| 188 | `Roid_Sm_Brown` | 553 | Object | 1818.11,284.79,1376.56 | 20,510,431 | Scale/Radius: 10.00 |
| 189 | `Roid_Sm_Brown` | 555 | Object | -231.69,-209.40,-3182.12 | 101,57,139 | Scale/Radius: 10.00 |
| 190 | `Roid_Sm_Brown` | 559 | Object | 2461.46,247.84,1321.47 | 509,208,202 | Scale/Radius: 10.00 |
| 191 | `Roid_Sm_Brown` | 561 | Object | 1918.85,-368.05,1617.16 | 158,328,192 | Scale/Radius: 10.00 |
| 192 | `Roid_Sm_Brown` | 563 | Object | -908.06,444.92,1193.75 | 244,472,427 | Scale/Radius: 10.00 |
| 193 | `Roid_Sm_Brown` | 565 | Object | 1350.31,615.89,-2649.44 | 43,263,334 | Scale/Radius: 10.00 |
| 194 | `Roid_Sm_Brown` | 567 | Object | -1694.30,-554.30,-436.19 | 468,212,236 | Scale/Radius: 10.00 |
| 195 | `Roid_Sm_Brown` | 569 | Object | -1404.19,-36.95,-832.27 | 2,327,511 | Scale/Radius: 10.00 |
| 196 | `Roid_Sm_Brown` | 571 | Object | -2083.91,98.54,466.32 | 408,125,198 | Scale/Radius: 10.00 |
| 197 | `Roid_Sm_Brown` | 573 | Object | 842.45,407.97,1285.89 | 151,31,106 | Scale/Radius: 10.00 |
| 198 | `Roid_Sm_Brown` | 575 | Object | 708.60,223.20,1038.80 | 379,236,77 | Scale/Radius: 10.00 |
| 199 | `Roid_Sm_Brown` | 577 | Object | -1227.29,444.92,1312.84 | 279,324,259 | Scale/Radius: 10.00 |
| 200 | `Roid_Sm_Brown` | 579 | Object | -2034.43,-60.11,1284.83 | 184,189,303 | Scale/Radius: 10.00 |
| 201 | `Roid_Sm_Brown` | 583 | Object | -785.91,-468.08,-2857.62 | 384,302,341 | Scale/Radius: 10.00 |
| 202 | `Roid_Sm_Brown` | 585 | Object | -1142.33,-603.57,-1921.49 | 203,506,364 | Scale/Radius: 10.00 |
| 203 | `Roid_Sm_Brown` | 587 | Object | -1914.54,443.44,497.11 | 181,29,150 | Scale/Radius: 10.00 |
| 204 | `Roid_Sm_Brown` | 593 | Object | 1772.35,480.39,-2091.38 | 316,124,377 | Scale/Radius: 10.00 |
| 205 | `Roid_Sm_Brown` | 595 | Object | 298.21,270.99,-3163.36 | 309,507,223 | Scale/Radius: 10.00 |
| 206 | `Roid_Sm_Brown` | 601 | Object | 2764.78,-86.22,766.69 | 274,212,128 | Scale/Radius: 10.00 |
| 207 | `Roid_Sm_Brown` | 603 | Object | -1162.56,-12.32,-2229.36 | 74,357,29 | Scale/Radius: 10.00 |
| 208 | `Roid_Sm_Brown` | 605 | Object | 2096.15,246.36,-1348.93 | 476,498,297 | Scale/Radius: 10.00 |
| 209 | `Roid_Sm_Brown` | 607 | Object | 1618.11,173.93,1620.79 | 71,340,142 | Scale/Radius: 10.00 |
| 210 | `Roid_Sm_Brown` | 609 | Object | -2355.44,-258.67,739.61 | 38,491,172 | Scale/Radius: 10.00 |
| 211 | `Roid_Sm_Brown` | 611 | Object | 178.10,-441.96,1043.38 | 341,418,429 | Scale/Radius: 10.00 |
| 212 | `Roid_Sm_Brown` | 613 | Object | -2287.15,-554.30,373.94 | 510,470,222 | Scale/Radius: 10.00 |
| 213 | `Roid_Sm_Brown` | 615 | Object | 2561.53,615.89,859.07 | 368,247,192 | Scale/Radius: 10.00 |
| 214 | `Roid_Sm_Brown` | 619 | Object | 61.10,-209.40,-2886.21 | 502,228,235 | Scale/Radius: 10.00 |
| 215 | `Roid_Sm_Brown` | 621 | Object | -2149.88,283.31,-210.33 | 511,451,186 | Scale/Radius: 10.00 |
| 216 | `Roid_Sm_Brown` | 625 | Object | -4.42,580.42,1078.48 | 290,71,425 | Scale/Radius: 10.00 |
| 217 | `Roid_Sm_Brown` | 627 | Object | 1636.85,-307.94,-2060.59 | 445,248,29 | Scale/Radius: 10.00 |
| 218 | `Roid_Sm_Brown` | 629 | Object | -1588.08,235.52,1061.55 | 423,37,287 | Scale/Radius: 10.00 |
| 219 | `Roid_Sm_Brown` | 633 | Object | 879.54,-160.13,-3066.93 | 263,435,222 | Scale/Radius: 10.00 |
| 220 | `Roid_Sm_Brown` | 635 | Object | 310.64,-540.50,1200.54 | 439,200,465 | Scale/Radius: 10.00 |
| 221 | `Roid_Sm_Brown` | 637 | Object | 2435.75,283.31,-407.77 | 87,272,161 | Scale/Radius: 10.00 |
| 222 | `Roid_Sm_Brown` | 639 | Object | 1728.16,-443.44,-1655.51 | 300,510,376 | Scale/Radius: 10.00 |
| 223 | `Roid_Sm_Brown` | 641 | Object | -1027.06,-369.53,-2260.15 | 183,364,130 | Scale/Radius: 10.00 |
| 224 | `Roid_Sm_Brown` | 645 | Object | -602.49,492.71,-2602.61 | 163,349,81 | Scale/Radius: 10.00 |
| 225 | `Roid_Sm_Brown` | 647 | Object | 1946.16,455.76,-801.37 | 398,508,342 | Scale/Radius: 10.00 |
| 226 | `Roid_Sm_Brown` | 649 | Object | -1878.67,431.12,34.85 | 164,196,441 | Scale/Radius: 10.00 |
| 227 | `Roid_Sm_Brown` | 651 | Object | 2800.20,13.80,1413.86 | 381,503,477 | Scale/Radius: 10.00 |
| 228 | `Roid_Sm_Brown` | 653 | Object | -704.82,210.88,1255.34 | 153,226,187 | Scale/Radius: 10.00 |
| 229 | `Roid_Sm_Brown` | 655 | Object | 1316.44,36.95,-2526.27 | 388,144,448 | Scale/Radius: 10.00 |
| 230 | `Roid_Sm_Brown` | 659 | Object | 2382.69,-61.59,45.40 | 321,78,38 | Scale/Radius: 10.00 |
| 231 | `Roid_Sm_Brown` | 661 | Object | 1245.50,-392.69,1251.25 | 506,17,198 | Scale/Radius: 10.00 |
| 232 | `Roid_Sm_Brown` | 663 | Object | -1342.42,369.53,-1351.28 | 316,494,368 | Scale/Radius: 10.00 |
| 233 | `Roid_Sm_Brown` | 665 | Object | 1349.15,543.46,1554.72 | 205,48,104 | Scale/Radius: 10.00 |
| 234 | `Roid_Sm_Brown` | 667 | Object | 2689.55,147.81,492.05 | 85,35,509 | Scale/Radius: 10.00 |
| 235 | `Roid_Sm_Brown` | 669 | Object | -959.31,578.94,-2352.54 | 360,119,25 | Scale/Radius: 10.00 |
| 236 | `Roid_Sm_Brown` | 671 | Object | -1532.62,-380.37,1338.32 | 120,28,433 | Scale/Radius: 10.00 |
| 237 | `Roid_Sm_Brown` | 673 | Object | 1584.24,63.07,1374.43 | 50,490,468 | Scale/Radius: 10.00 |
| 238 | `Roid_Sm_Brown` | 675 | Object | -1295.04,605.05,1589.99 | 176,39,388 | Scale/Radius: 10.00 |
| 239 | `Roid_Sm_Brown` | 677 | Object | -1345.88,-234.04,-1075.16 | 231,269,23 | Scale/Radius: 10.00 |
| 240 | `Roid_Sm_Brown` | 679 | Object | 2619.81,-320.26,14.61 | 411,386,356 | Scale/Radius: 10.00 |
| 241 | `Roid_Sm_Brown` | 681 | Object | 938.88,-281.83,1000.47 | 227,509,447 | Scale/Radius: 10.00 |
| 242 | `Roid_Sm_Brown` | 683 | Object | -956.63,-23.16,1683.47 | 94,210,240 | Scale/Radius: 10.00 |
| 243 | `Roid_Sm_Brown` | 687 | Object | -1125.67,-220.24,1436.02 | 41,46,372 | Scale/Radius: 10.00 |
| 244 | `Roid_Sm_Brown` | 689 | Object | 1762.04,234.04,-1686.30 | 225,215,142 | Scale/Radius: 10.00 |
| 245 | `Roid_Sm_Brown` | 693 | Object | 1380.99,223.20,1189.66 | 290,274,337 | Scale/Radius: 10.00 |
| 246 | `Roid_Sm_Brown` | 695 | Object | 1090.97,86.22,-2602.62 | 28,197,305 | Scale/Radius: 10.00 |
| 247 | `Roid_Sm_Brown` | 697 | Object | 443.29,-72.43,1054.69 | 299,297,494 | Scale/Radius: 10.00 |
| 248 | `Roid_Sm_Brown` | 701 | Object | 2200.60,-541.98,-664.93 | 309,149,440 | Scale/Radius: 10.00 |
| 249 | `Roid_Sm_Brown` | 703 | Object | 2630.83,161.61,1547.96 | 378,11,363 | Scale/Radius: 10.00 |
| 250 | `Roid_Sm_Brown` | 705 | Object | -207.20,469.56,1274.82 | 481,316,413 | Scale/Radius: 10.00 |
| 251 | `Roid_Sm_Brown` | 707 | Object | -1878.67,480.39,-303.89 | 488,256,371 | Scale/Radius: 10.00 |
| 252 | `Roid_Sm_Brown` | 709 | Object | 1806.22,541.98,-2399.33 | 208,204,99 | Scale/Radius: 10.00 |
| 253 | `Roid_Sm_Brown` | 1005 | Object | 2415.13,26.12,1619.57 | 0,0,0 | Scale/Radius: 10.00 |
| 254 | `Roid_Sm_Brown` | 1006 | Object | 2194.57,26.12,1474.00 | 0,0,0 | Scale/Radius: 10.00 |
| 255 | `Roid_Sm_Brown` | 1007 | Object | 2328.82,26.12,1193.25 | 0,0,0 | Scale/Radius: 10.00 |
| 256 | `Spcargo_Credits` | 1111 | Interactive | 687.41,-1182.21,-563.25 | 36,172,302 | secondary groups: CONT_065, none |
| 257 | `Baron_Hajod_Slave` | 996 | Interactive | 278.54,-618.36,-722.55 | 444,0,0 | secondary groups: none, IRONHAND_STATION |
| 258 | `Mad_Pirate_Platform` | 1120 | Interactive | -443.75,0.00,-1128.36 | 444,0,0 | None |
