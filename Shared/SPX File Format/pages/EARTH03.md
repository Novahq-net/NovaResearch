# Tachyon: The Fringe EARTH03.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH03.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `EARTH03.BDF` |
| Region | 0 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 7 |
| Entities | 350 |
| Events | 3 |
| Waypoints | 1 |
| Child Sectors | 7 |
| Scripts | 0 |
| Scenes | 1 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Roid_Med_Green2`, `1: Roid_Med_Green`, `2: Roid_XL_Green`, `3: Navigational_Bouy`, `4: AGT_Mako`, `5: Earth_StarBase`, `6: Hyper_Gate` |
| Scripts | None |
| Scenes | `SOL_INT1.SEN` |
| Labels | `SHUT`, `bfnf_03`, `PLAYER`, `ORION03`, `ORION02`, `ORION01`, `PEGASUS01`, `PEGASUS02`, `PEGASUS03`, `MAKO01`, `MAKO03`, `PIRANHA01`, `PIRANHA02`, `PIRANHA03`, `PIRANHA04`, `DART01`, `DART02`, `DART03`, `DART04`, `FRGT`, `CPSH`, `SAMA`, `FREIGHT01` |
| Aliases | `fred2`, `fred1`, `fred3` |
| Groups | `FG_AGT1`, `FG_AGT2` |
| Child Sectors | [earth03A.spx](EARTH03A.md), [earth03B.spx](EARTH03B.md), [earth03C.spx](EARTH03C.md), [earth03D.spx](EARTH03D.md), [earth03E.spx](EARTH03E.md), [earth03F.spx](EARTH03F.md), [earth03G.spx](EARTH03G.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4044

**Action**

- Mission objective/state: param 7, subtype 0, param 0
- Gate state/action: param 301, subtype 2, param 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4043

**Action**

- Mission objective/state: param 9, subtype 0, param 0

### Event 2

**Trigger**

- Variable comparison: subject variable group 0, variable 4, op 1, value 4043
- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 8, param 0

## Waypoints

### Waypoint 0

- Tag: `4`
- Members: `AGT_Mako (object 5, id 358, starts at point 0)`, `AGT_Mako (object 6, id 357, starts at point 0)`, `AGT_Mako (object 7, id 360, starts at point 4)`, `AGT_Mako (object 8, id 359, starts at point 4)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1070.50, 0.00, -828.29) | None |
| 1 | (-398.72, 0.00, -640.19) | None |
| 2 | (-2313.41, 0.00, -156.07) | None |
| 3 | (-1930.26, 0.00, 1194.22) | None |
| 4 | (233.11, 0.00, 930.56) | None |
| 5 | (440.70, -392.00, -170.42) | None |
| 6 | (4.90, -8.00, -717.31) | None |
| 7 | (-478.36, 400.00, -136.66) | None |
| 8 | (-28.70, 0.00, 711.61) | None |
| 9 | (1088.15, 0.00, 230.30) | on arrival redirect to Waypoint 0 (tag 4), point 0 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | -925.53,344.00,5685.95 | 242,0,0 | Gate SPX: [Earth06.spx](EARTH06.md) |
| 1 | `Hyper_Gate` | 301 | Gate | 1634.37,442.00,5466.81 | 256,0,0 | Gate SPX: [earth02.spx](EARTH02.md) |
| 2 | `Earth_StarBase` | 60 | Interactive | 1.00,0.00,-6.00 | 509,0,0 | None |
| 3 | `none` | 906 | Marker | 74.46,0.00,532.55 | 0,0,0 | None |
| 4 | `Hyper_Gate` | 913 | Gate | -1967.16,344.00,4715.92 | 223,0,0 | Gate SPX: [earth10.spx](EARTH10.md) |
| 5 | `AGT_Mako` | 358 | Interactive | 1173.91,0.00,-591.31 | 0,0,0 | label: bfnf_03; group/role: FG_AGT1 / 2; waypoint: Waypoint 0 (tag 4, 10 point(s)), starting point 0, arrival event value 262144 |
| 6 | `AGT_Mako` | 357 | Interactive | 1235.11,0.00,-628.64 | 0,0,0 | group/role: FG_AGT1 / 1; waypoint: Waypoint 0 (tag 4, 10 point(s)), starting point 0, arrival event value 262144 |
| 7 | `AGT_Mako` | 360 | Interactive | 150.15,0.00,1001.83 | 0,0,0 | label: bfnf_03; group/role: FG_AGT2 / 2; waypoint: Waypoint 0 (tag 4, 10 point(s)), starting point 4, arrival event value 262148 |
| 8 | `AGT_Mako` | 359 | Interactive | 141.24,0.00,890.85 | 0,0,0 | group/role: FG_AGT2 / 1; waypoint: Waypoint 0 (tag 4, 10 point(s)), starting point 4, arrival event value 262148 |
| 9 | `Navigational_Bouy` | 920 | Interactive | -5.56,-56.64,270.92 | 0,0,0 | None |
| 10 | `Roid_XL_Green` | 716 | Object | -3444.75,-817.52,4145.05 | 230,51,350 | Scale/Radius: 1.00 |
| 11 | `Roid_XL_Green` | 428 | Object | 2750.06,-468.83,4986.08 | 60,160,180 | Scale/Radius: 1.00 |
| 12 | `Roid_XL_Green` | 432 | Object | 3204.13,-843.61,1433.35 | 496,363,5 | Scale/Radius: 1.00 |
| 13 | `Roid_XL_Green` | 437 | Object | 2800.48,599.72,2778.99 | 72,392,462 | Scale/Radius: 1.00 |
| 14 | `Roid_XL_Green` | 451 | Object | 2572.56,-614.77,5092.75 | 285,4,404 | Scale/Radius: 1.00 |
| 15 | `Roid_XL_Green` | 458 | Object | 2718.36,-528.81,5192.68 | 348,453,415 | Scale/Radius: 1.00 |
| 16 | `Roid_XL_Green` | 462 | Object | 2562.44,539.75,3989.58 | 469,276,75 | Scale/Radius: 1.00 |
| 17 | `Roid_XL_Green` | 465 | Object | 2681.94,-359.83,2701.03 | 192,131,362 | Scale/Radius: 1.00 |
| 18 | `Roid_XL_Green` | 474 | Object | 2161.24,-464.84,4629.24 | 93,133,459 | Scale/Radius: 1.00 |
| 19 | `Roid_XL_Green` | 481 | Object | 2231.83,0.00,2825.42 | 488,334,275 | Scale/Radius: 1.00 |
| 20 | `Roid_XL_Green` | 512 | Object | 1922.19,-490.09,5706.73 | 136,37,85 | Scale/Radius: 1.00 |
| 21 | `Roid_XL_Green` | 526 | Object | -2017.87,656.54,5696.13 | 458,177,229 | Scale/Radius: 1.00 |
| 22 | `Roid_XL_Green` | 558 | Object | -1449.01,-490.09,5202.04 | 303,211,490 | Scale/Radius: 1.00 |
| 23 | `Roid_XL_Green` | 574 | Object | 1716.13,88.38,5616.93 | 478,26,5 | Scale/Radius: 1.00 |
| 24 | `Roid_XL_Green` | 584 | Object | -3060.86,265.14,4107.11 | 22,457,160 | Scale/Radius: 1.00 |
| 25 | `Roid_XL_Green` | 591 | Object | 2076.66,-883.80,5210.71 | 269,80,175 | Scale/Radius: 1.00 |
| 26 | `Roid_XL_Green` | 597 | Object | -2815.35,464.00,3308.08 | 420,55,470 | Scale/Radius: 1.00 |
| 27 | `Roid_XL_Green` | 599 | Object | -3402.35,842.05,3817.11 | 36,174,192 | Scale/Radius: 1.00 |
| 28 | `Roid_XL_Green` | 601 | Object | -679.46,176.76,6129.26 | 0,57,389 | Scale/Radius: 1.00 |
| 29 | `Roid_XL_Green` | 604 | Object | -2543.05,-88.38,4765.53 | 235,134,270 | Scale/Radius: 1.00 |
| 30 | `Roid_XL_Green` | 606 | Object | -3841.96,198.86,2565.64 | 153,431,47 | Scale/Radius: 1.00 |
| 31 | `Roid_XL_Green` | 609 | Object | -988.58,-751.23,6161.62 | 375,138,383 | Scale/Radius: 1.00 |
| 32 | `Roid_XL_Green` | 613 | Object | -3008.41,842.05,4391.83 | 229,479,145 | Scale/Radius: 1.00 |
| 33 | `Roid_XL_Green` | 625 | Object | -3233.76,-574.47,3133.67 | 324,325,387 | Scale/Radius: 1.00 |
| 34 | `Roid_XL_Green` | 630 | Object | -287.73,-618.66,5759.12 | 385,309,234 | Scale/Radius: 1.00 |
| 35 | `Roid_XL_Green` | 632 | Object | 1370.38,773.33,5641.14 | 50,278,331 | Scale/Radius: 1.00 |
| 36 | `Roid_XL_Green` | 634 | Object | -2959.31,-618.66,3244.47 | 215,468,154 | Scale/Radius: 1.00 |
| 37 | `Roid_XL_Green` | 635 | Object | -2836.55,353.52,3467.66 | 500,261,400 | Scale/Radius: 1.00 |
| 38 | `Roid_XL_Green` | 639 | Object | 1448.50,-905.90,5839.78 | 76,495,20 | Scale/Radius: 1.00 |
| 39 | `Roid_XL_Green` | 647 | Object | -1032.11,-707.04,5997.58 | 238,168,224 | Scale/Radius: 1.00 |
| 40 | `Roid_XL_Green` | 660 | Object | -3036.24,441.90,2728.57 | 375,170,397 | Scale/Radius: 1.00 |
| 41 | `Roid_XL_Green` | 665 | Object | 2051.27,-543.75,5452.61 | 264,430,295 | Scale/Radius: 1.00 |
| 42 | `Roid_XL_Green` | 680 | Object | -1531.99,-521.65,4827.41 | 36,409,25 | Scale/Radius: 1.00 |
| 43 | `Roid_XL_Green` | 683 | Object | 2039.41,-220.95,5173.24 | 243,440,243 | Scale/Radius: 1.00 |
| 44 | `Roid_XL_Green` | 693 | Object | -393.75,750.61,5934.32 | 449,461,15 | Scale/Radius: 1.00 |
| 45 | `Roid_XL_Green` | 694 | Object | -3348.71,-243.05,3179.42 | 469,322,211 | Scale/Radius: 1.00 |
| 46 | `Roid_XL_Green` | 703 | Object | -3465.96,-419.81,3681.93 | 94,406,190 | Scale/Radius: 1.00 |
| 47 | `Roid_XL_Green` | 720 | Object | -214.08,-220.95,5893.03 | 386,157,501 | Scale/Radius: 1.00 |
| 48 | `Roid_XL_Green` | 726 | Object | -3625.47,-176.76,2902.66 | 10,200,146 | Scale/Radius: 1.00 |
| 49 | `Roid_XL_Green` | 730 | Object | 1785.32,-552.38,5686.12 | 198,212,350 | Scale/Radius: 1.00 |
| 50 | `Roid_XL_Green` | 734 | Object | -2500.65,0.00,4446.36 | 491,149,368 | Scale/Radius: 1.00 |
| 51 | `Roid_XL_Green` | 744 | Object | -3602.03,-220.95,2464.09 | 495,459,262 | Scale/Radius: 1.00 |
| 52 | `Roid_XL_Green` | 747 | Object | -3088.76,-795.42,4480.96 | 187,320,434 | Scale/Radius: 1.00 |
| 53 | `Roid_XL_Green` | 750 | Object | -2423.64,864.15,4153.02 | 214,123,476 | Scale/Radius: 1.00 |
| 54 | `Roid_XL_Green` | 754 | Object | -2596.62,287.24,4611.53 | 254,174,160 | Scale/Radius: 1.00 |
| 55 | `Roid_XL_Green` | 763 | Object | -2208.26,-477.46,5296.12 | 365,237,316 | Scale/Radius: 1.00 |
| 56 | `Roid_Med_Green` | 767 | Object | -2502.88,-375.62,4725.35 | 259,231,441 | Scale/Radius: 1.00 |
| 57 | `Roid_Med_Green` | 392 | Object | 2168.43,59.97,3238.62 | 389,149,336 | Scale/Radius: 1.00 |
| 58 | `Roid_Med_Green` | 394 | Object | 3138.06,-479.78,1999.28 | 254,74,301 | Scale/Radius: 1.00 |
| 59 | `Roid_Med_Green` | 395 | Object | -1815.98,389.82,5481.23 | 394,190,169 | Scale/Radius: 1.00 |
| 60 | `Roid_Med_Green` | 396 | Object | 2911.53,719.67,4343.24 | 259,200,321 | Scale/Radius: 1.00 |
| 61 | `Roid_Med_Green` | 400 | Object | 3643.82,747.36,2814.86 | 171,261,250 | Scale/Radius: 1.00 |
| 62 | `Roid_Med_Green` | 401 | Object | 3550.18,542.99,2772.07 | 346,309,384 | Scale/Radius: 1.00 |
| 63 | `Roid_Med_Green` | 403 | Object | 3031.61,782.88,2775.62 | 464,319,81 | Scale/Radius: 1.00 |
| 64 | `Roid_Med_Green` | 405 | Object | 3650.12,209.90,2115.51 | 408,420,489 | Scale/Radius: 1.00 |
| 65 | `Roid_Med_Green` | 407 | Object | 3247.87,-614.77,4840.79 | 354,166,68 | Scale/Radius: 1.00 |
| 66 | `Roid_Med_Green` | 409 | Object | 2504.39,989.54,4806.05 | 446,493,333 | Scale/Radius: 1.00 |
| 67 | `Roid_Med_Green` | 411 | Object | 2878.35,752.89,3050.62 | 186,224,351 | Scale/Radius: 1.00 |
| 68 | `Roid_Med_Green` | 414 | Object | 2328.98,119.94,5021.51 | 124,421,358 | Scale/Radius: 1.00 |
| 69 | `Roid_Med_Green` | 416 | Object | 3015.20,749.65,3778.13 | 109,380,114 | Scale/Radius: 1.00 |
| 70 | `Roid_Med_Green` | 420 | Object | 2447.04,-438.85,1969.88 | 332,109,73 | Scale/Radius: 1.00 |
| 71 | `Roid_Med_Green` | 422 | Object | 2758.62,-588.78,3950.96 | 271,12,379 | Scale/Radius: 1.00 |
| 72 | `Roid_Med_Green` | 427 | Object | 3194.00,987.25,2808.49 | 50,351,510 | Scale/Radius: 1.00 |
| 73 | `Roid_Med_Green` | 429 | Object | 2462.09,632.95,3214.33 | 377,494,29 | Scale/Radius: 1.00 |
| 74 | `Roid_Med_Green` | 434 | Object | 3680.36,299.86,2562.73 | 330,46,279 | Scale/Radius: 1.00 |
| 75 | `Roid_Med_Green` | 436 | Object | 2112.43,807.33,3130.97 | 205,162,264 | Scale/Radius: 1.00 |
| 76 | `Roid_Med_Green` | 439 | Object | 3072.15,722.91,2998.88 | 177,455,147 | Scale/Radius: 1.00 |
| 77 | `Roid_Med_Green` | 441 | Object | 2393.42,-419.81,2522.69 | 299,256,298 | Scale/Radius: 1.00 |
| 78 | `Roid_Med_Green` | 442 | Object | 1969.36,927.28,2159.19 | 268,224,160 | Scale/Radius: 1.00 |
| 79 | `Roid_Med_Green` | 444 | Object | 3034.23,987.25,3203.26 | 130,100,475 | Scale/Radius: 1.00 |
| 80 | `Roid_Med_Green` | 450 | Object | 2379.73,89.96,3742.89 | 249,401,382 | Scale/Radius: 1.00 |
| 81 | `Roid_Med_Green` | 453 | Object | 2738.25,-29.99,2669.14 | 156,18,257 | Scale/Radius: 1.00 |
| 82 | `Roid_Med_Green` | 455 | Object | 3639.71,-29.99,1178.19 | 466,327,253 | Scale/Radius: 1.00 |
| 83 | `Roid_Med_Green` | 456 | Object | 3315.49,-558.79,2646.82 | 159,466,302 | Scale/Radius: 1.00 |
| 84 | `Roid_Med_Green` | 461 | Object | 2574.40,-479.78,3298.86 | 189,221,362 | Scale/Radius: 1.00 |
| 85 | `Roid_Med_Green` | 467 | Object | 2526.61,-588.78,4329.08 | 235,141,220 | Scale/Radius: 1.00 |
| 86 | `Roid_Med_Green` | 469 | Object | 3231.99,-179.92,1902.53 | 291,366,198 | Scale/Radius: 1.00 |
| 87 | `Roid_Med_Green` | 472 | Object | 3918.51,717.38,2905.94 | 15,445,329 | Scale/Radius: 1.00 |
| 88 | `Roid_Med_Green` | 477 | Object | 3257.01,662.93,3491.50 | 47,306,151 | Scale/Radius: 1.00 |
| 89 | `Roid_Med_Green` | 484 | Object | -559.84,164.13,5613.37 | 167,409,239 | Scale/Radius: 1.00 |
| 90 | `Roid_Med_Green` | 487 | Object | 3592.66,-492.40,3582.51 | 403,507,83 | Scale/Radius: 1.00 |
| 91 | `Roid_Med_Green` | 488 | Object | 800.39,-574.47,5657.93 | 335,356,176 | Scale/Radius: 1.00 |
| 92 | `Roid_Med_Green` | 490 | Object | 438.40,451.37,5483.33 | 462,320,122 | Scale/Radius: 1.00 |
| 93 | `Roid_Med_Green` | 491 | Object | -1606.97,328.27,5405.99 | 28,419,45 | Scale/Radius: 1.00 |
| 94 | `Roid_Med_Green` | 492 | Object | 481.01,594.99,5372.85 | 75,281,440 | Scale/Radius: 1.00 |
| 95 | `Roid_Med_Green` | 493 | Object | 736.68,800.15,5527.52 | 196,101,492 | Scale/Radius: 1.00 |
| 96 | `Roid_Med_Green` | 494 | Object | 821.90,-449.05,5043.38 | 440,342,263 | Scale/Radius: 1.00 |
| 97 | `Roid_Med_Green` | 495 | Object | 517.86,615.50,4608.38 | 383,305,325 | Scale/Radius: 1.00 |
| 98 | `Roid_Med_Green` | 497 | Object | 1929.47,-759.12,5506.93 | 290,100,421 | Scale/Radius: 1.00 |
| 99 | `Roid_Med_Green` | 498 | Object | 3547.66,-636.02,3296.08 | 51,449,325 | Scale/Radius: 1.00 |
| 100 | `Roid_Med_Green` | 499 | Object | -1308.69,-471.89,5273.42 | 403,336,179 | Scale/Radius: 1.00 |
| 101 | `Roid_Med_Green` | 500 | Object | -1436.52,-841.19,5405.99 | 360,293,365 | Scale/Radius: 1.00 |
| 102 | `Roid_Med_Green` | 501 | Object | -602.45,-820.67,5072.04 | 94,73,454 | Scale/Radius: 1.00 |
| 103 | `Roid_Med_Green` | 502 | Object | 3632.89,-512.92,3218.75 | 340,25,61 | Scale/Radius: 1.00 |
| 104 | `Roid_Med_Green` | 503 | Object | -347.86,246.20,5279.01 | 288,276,352 | Scale/Radius: 1.00 |
| 105 | `Roid_Med_Green` | 506 | Object | -669.51,872.13,5980.46 | 79,352,487 | Scale/Radius: 1.00 |
| 106 | `Roid_Med_Green` | 507 | Object | -1138.24,-471.89,5903.13 | 402,157,474 | Scale/Radius: 1.00 |
| 107 | `Roid_Med_Green` | 508 | Object | 709.40,82.07,4562.04 | 244,322,496 | Scale/Radius: 1.00 |
| 108 | `Roid_Med_Green` | 509 | Object | -559.84,718.09,5149.38 | 11,457,273 | Scale/Radius: 1.00 |
| 109 | `Roid_Med_Green` | 510 | Object | 481.01,533.44,5626.94 | 304,239,70 | Scale/Radius: 1.00 |
| 110 | `Roid_Med_Green` | 514 | Object | -626.90,677.05,5295.52 | 434,297,386 | Scale/Radius: 1.00 |
| 111 | `Roid_Med_Green` | 515 | Object | -1890.03,697.57,5718.23 | 125,186,238 | Scale/Radius: 1.00 |
| 112 | `Roid_Med_Green` | 518 | Object | 666.79,791.55,4730.03 | 413,251,270 | Scale/Radius: 1.00 |
| 113 | `Roid_Med_Green` | 519 | Object | -626.90,759.12,5174.00 | 140,420,449 | Scale/Radius: 1.00 |
| 114 | `Roid_Med_Green` | 520 | Object | -158.17,-861.71,5306.57 | 438,464,25 | Scale/Radius: 1.00 |
| 115 | `Roid_Med_Green` | 521 | Object | 3677.89,-82.07,3560.41 | 477,468,57 | Scale/Radius: 1.00 |
| 116 | `Roid_Med_Green` | 522 | Object | -1363.79,-369.30,5189.04 | 438,10,319 | Scale/Radius: 1.00 |
| 117 | `Roid_Med_Green` | 523 | Object | -115.56,-738.60,5461.23 | 42,113,371 | Scale/Radius: 1.00 |
| 118 | `Roid_Med_Green` | 524 | Object | -1692.19,-882.22,5869.99 | 361,126,478 | Scale/Radius: 1.00 |
| 119 | `Roid_Med_Green` | 525 | Object | -1278.57,-451.37,5288.46 | 509,90,306 | Scale/Radius: 1.00 |
| 120 | `Roid_Med_Green` | 527 | Object | -72.95,-328.27,5637.99 | 375,341,118 | Scale/Radius: 1.00 |
| 121 | `Roid_Med_Green` | 529 | Object | 1922.45,-677.05,5314.86 | 256,288,66 | Scale/Radius: 1.00 |
| 122 | `Roid_Med_Green` | 530 | Object | 523.62,-510.60,5606.80 | 79,416,51 | Scale/Radius: 1.00 |
| 123 | `Roid_Med_Green` | 532 | Object | -390.47,143.62,5146.44 | 248,324,111 | Scale/Radius: 1.00 |
| 124 | `Roid_Med_Green` | 533 | Object | 353.17,790.06,5770.56 | 116,340,174 | Scale/Radius: 1.00 |
| 125 | `Roid_Med_Green` | 534 | Object | 560.47,-410.34,4729.91 | 95,252,445 | Scale/Radius: 1.00 |
| 126 | `Roid_Med_Green` | 535 | Object | -1692.19,20.52,5019.33 | 477,332,124 | Scale/Radius: 1.00 |
| 127 | `Roid_Med_Green` | 536 | Object | 2234.61,-615.50,5166.96 | 480,105,41 | Scale/Radius: 1.00 |
| 128 | `Roid_Med_Green` | 537 | Object | -432.01,-510.60,5416.47 | 127,262,248 | Scale/Radius: 1.00 |
| 129 | `Roid_Med_Green` | 538 | Object | -517.23,184.65,5304.04 | 217,2,39 | Scale/Radius: 1.00 |
| 130 | `Roid_Med_Green` | 540 | Object | -669.51,369.30,5273.42 | 55,61,261 | Scale/Radius: 1.00 |
| 131 | `Roid_Med_Green` | 541 | Object | -1890.03,533.44,5784.51 | 496,403,441 | Scale/Radius: 1.00 |
| 132 | `Roid_Med_Green` | 543 | Object | -30.33,20.52,5615.90 | 331,52,138 | Scale/Radius: 1.00 |
| 133 | `Roid_Med_Green` | 544 | Object | -1795.03,205.17,5352.04 | 182,317,17 | Scale/Radius: 1.00 |
| 134 | `Roid_Med_Green` | 545 | Object | -626.90,266.72,5439.14 | 37,357,503 | Scale/Radius: 1.00 |
| 135 | `Roid_Med_Green` | 546 | Object | -1734.81,-656.54,5030.38 | 37,368,318 | Scale/Radius: 1.00 |
| 136 | `Roid_Med_Green` | 547 | Object | -30.33,-510.60,5816.71 | 438,386,194 | Scale/Radius: 1.00 |
| 137 | `Roid_Med_Green` | 550 | Object | 2121.13,-594.99,5012.06 | 105,139,107 | Scale/Radius: 1.00 |
| 138 | `Roid_Med_Green` | 552 | Object | 715.16,831.10,5691.08 | 60,167,472 | Scale/Radius: 1.00 |
| 139 | `Roid_Med_Green` | 553 | Object | -669.51,369.30,5317.61 | 377,122,228 | Scale/Radius: 1.00 |
| 140 | `Roid_Med_Green` | 554 | Object | 544.96,-201.03,5268.17 | 287,59,388 | Scale/Radius: 1.00 |
| 141 | `Roid_Med_Green` | 555 | Object | 651.45,800.15,5085.62 | 454,491,139 | Scale/Radius: 1.00 |
| 142 | `Roid_Med_Green` | 556 | Object | -412.65,-82.07,5577.30 | 163,414,52 | Scale/Radius: 1.00 |
| 143 | `Roid_Med_Green` | 557 | Object | -1734.81,451.37,6119.65 | 434,111,30 | Scale/Radius: 1.00 |
| 144 | `Roid_Med_Green` | 559 | Object | -645.06,677.05,5701.75 | 446,436,101 | Scale/Radius: 1.00 |
| 145 | `Roid_Med_Green` | 561 | Object | 608.84,831.10,5715.32 | 271,117,383 | Scale/Radius: 1.00 |
| 146 | `Roid_Med_Green` | 562 | Object | 3547.66,730.00,3221.02 | 20,328,358 | Scale/Radius: 1.00 |
| 147 | `Roid_Med_Green` | 564 | Object | 779.29,61.55,5284.47 | 10,222,94 | Scale/Radius: 1.00 |
| 148 | `Roid_Med_Green` | 568 | Object | -3072.02,-132.57,4256.65 | 96,227,347 | Scale/Radius: 1.00 |
| 149 | `Roid_Med_Green` | 570 | Object | -1295.07,-198.86,6106.36 | 502,318,232 | Scale/Radius: 1.00 |
| 150 | `Roid_Med_Green` | 572 | Object | -2881.19,-198.86,4065.82 | 377,321,292 | Scale/Radius: 1.00 |
| 151 | `Roid_Med_Green` | 573 | Object | -1562.12,905.90,4822.44 | 118,28,239 | Scale/Radius: 1.00 |
| 152 | `Roid_Med_Green` | 577 | Object | -3455.84,886.24,2862.64 | 302,359,303 | Scale/Radius: 1.00 |
| 153 | `Roid_Med_Green` | 580 | Object | -2942.50,309.33,2842.40 | 190,389,163 | Scale/Radius: 1.00 |
| 154 | `Roid_Med_Green` | 581 | Object | 876.01,-543.75,5824.66 | 313,485,503 | Scale/Radius: 1.00 |
| 155 | `Roid_Med_Green` | 583 | Object | 1663.90,-905.90,4361.04 | 78,500,84 | Scale/Radius: 1.00 |
| 156 | `Roid_Med_Green` | 586 | Object | 1481.51,-486.09,5926.25 | 462,113,341 | Scale/Radius: 1.00 |
| 157 | `Roid_Med_Green` | 590 | Object | -2226.12,110.48,4379.40 | 137,445,247 | Scale/Radius: 1.00 |
| 158 | `Roid_Med_Green` | 592 | Object | -3214.86,-353.52,3430.84 | 440,395,441 | Scale/Radius: 1.00 |
| 159 | `Roid_Med_Green` | 595 | Object | -1239.27,838.99,5981.38 | 511,448,487 | Scale/Radius: 1.00 |
| 160 | `Roid_Med_Green` | 598 | Object | -2892.35,66.29,4215.36 | 286,45,306 | Scale/Radius: 1.00 |
| 161 | `Roid_Med_Green` | 600 | Object | -1334.13,707.04,6007.04 | 255,396,162 | Scale/Radius: 1.00 |
| 162 | `Roid_Med_Green` | 602 | Object | -1999.58,-375.62,4083.67 | 309,162,324 | Scale/Radius: 1.00 |
| 163 | `Roid_Med_Green` | 603 | Object | -734.14,-455.37,6149.85 | 142,33,293 | Scale/Radius: 1.00 |
| 164 | `Roid_Med_Green` | 605 | Object | -265.38,-464.00,6345.04 | 254,136,16 | Scale/Radius: 1.00 |
| 165 | `Roid_Med_Green` | 611 | Object | -4199.07,684.95,2369.23 | 171,173,365 | Scale/Radius: 1.00 |
| 166 | `Roid_Med_Green` | 615 | Object | 2265.41,927.99,5419.62 | 87,49,307 | Scale/Radius: 1.00 |
| 167 | `Roid_Med_Green` | 616 | Object | 536.16,-565.84,5883.49 | 456,149,402 | Scale/Radius: 1.00 |
| 168 | `Roid_Med_Green` | 617 | Object | -2113.41,66.29,5235.35 | 240,61,195 | Scale/Radius: 1.00 |
| 169 | `Roid_Med_Green` | 619 | Object | -3676.80,198.86,2469.67 | 499,324,319 | Scale/Radius: 1.00 |
| 170 | `Roid_Med_Green` | 620 | Object | -3331.97,486.09,2955.11 | 420,380,468 | Scale/Radius: 1.00 |
| 171 | `Roid_Med_Green` | 621 | Object | -1843.34,552.38,5103.67 | 359,43,139 | Scale/Radius: 1.00 |
| 172 | `Roid_Med_Green` | 623 | Object | -3828.57,687.39,2128.34 | 237,55,64 | Scale/Radius: 1.00 |
| 173 | `Roid_Med_Green` | 628 | Object | -2953.73,886.24,3783.63 | 164,311,220 | Scale/Radius: 1.00 |
| 174 | `Roid_Med_Green` | 631 | Object | 530.72,44.19,5987.38 | 406,147,405 | Scale/Radius: 1.00 |
| 175 | `Roid_Med_Green` | 637 | Object | 1615.69,530.28,5717.36 | 469,308,488 | Scale/Radius: 1.00 |
| 176 | `Roid_Med_Green` | 638 | Object | -2539.70,-499.56,5004.85 | 12,274,437 | Scale/Radius: 1.00 |
| 177 | `Roid_Med_Green` | 643 | Object | -2053.41,-477.46,5477.75 | 412,279,42 | Scale/Radius: 1.00 |
| 178 | `Roid_Med_Green` | 651 | Object | -2605.55,-243.05,4482.07 | 157,371,216 | Scale/Radius: 1.00 |
| 179 | `Roid_Med_Green` | 653 | Object | 1697.16,751.23,5767.63 | 361,117,233 | Scale/Radius: 1.00 |
| 180 | `Roid_Med_Green` | 658 | Object | 1540.01,176.76,5609.89 | 184,146,65 | Scale/Radius: 1.00 |
| 181 | `Roid_Med_Green` | 667 | Object | -1617.92,353.52,4947.43 | 511,352,312 | Scale/Radius: 1.00 |
| 182 | `Roid_Med_Green` | 671 | Object | -3300.72,665.29,2776.71 | 211,335,383 | Scale/Radius: 1.00 |
| 183 | `Roid_Med_Green` | 673 | Object | -2612.24,132.57,4073.63 | 126,79,471 | Scale/Radius: 1.00 |
| 184 | `Roid_Med_Green` | 674 | Object | 1803.39,66.29,4359.92 | 457,249,408 | Scale/Radius: 1.00 |
| 185 | `Roid_Med_Green` | 676 | Object | -3529.49,842.05,2728.73 | 90,371,405 | Scale/Radius: 1.00 |
| 186 | `Roid_Med_Green` | 682 | Object | 1571.51,839.61,5568.54 | 488,317,90 | Scale/Radius: 1.00 |
| 187 | `Roid_Med_Green` | 686 | Object | -1992.88,822.45,5114.83 | 151,394,333 | Scale/Radius: 1.00 |
| 188 | `Roid_Med_Green` | 687 | Object | -2824.28,0.00,3801.33 | 164,460,354 | Scale/Radius: 1.00 |
| 189 | `Roid_Med_Green` | 689 | Object | -2223.89,-22.09,4100.41 | 115,223,194 | Scale/Radius: 1.00 |
| 190 | `Roid_Med_Green` | 691 | Object | 1349.18,-508.19,5800.72 | 448,373,31 | Scale/Radius: 1.00 |
| 191 | `Roid_Med_Green` | 695 | Object | 1675.06,198.86,4211.50 | 408,249,505 | Scale/Radius: 1.00 |
| 192 | `Roid_Med_Green` | 696 | Object | -2791.91,22.10,3492.21 | 327,480,245 | Scale/Radius: 1.00 |
| 193 | `Roid_Med_Green` | 698 | Object | 565.31,-375.62,6021.98 | 20,177,352 | Scale/Radius: 1.00 |
| 194 | `Roid_Med_Green` | 700 | Object | -2522.97,861.71,4745.44 | 277,328,11 | Scale/Radius: 1.00 |
| 195 | `Roid_Med_Green` | 701 | Object | -1354.21,265.14,6027.13 | 54,427,447 | Scale/Radius: 1.00 |
| 196 | `Roid_Med_Green` | 702 | Object | -4183.45,-684.95,2284.42 | 289,213,360 | Scale/Radius: 1.00 |
| 197 | `Roid_Med_Green` | 704 | Object | 1665.91,-817.52,5667.15 | 80,179,452 | Scale/Radius: 1.00 |
| 198 | `Roid_Med_Green` | 706 | Object | -3974.76,-751.23,2352.49 | 81,118,60 | Scale/Radius: 1.00 |
| 199 | `Roid_Med_Green` | 707 | Object | -2903.51,-640.76,3742.19 | 114,233,383 | Scale/Radius: 1.00 |
| 200 | `Roid_Med_Green` | 708 | Object | -2295.31,486.09,4932.92 | 451,102,64 | Scale/Radius: 1.00 |
| 201 | `Roid_Med_Green` | 710 | Object | -2976.05,-817.52,4091.48 | 77,295,127 | Scale/Radius: 1.00 |
| 202 | `Roid_Med_Green` | 712 | Object | -3541.84,-596.57,3827.00 | 421,271,481 | Scale/Radius: 1.00 |
| 203 | `Roid_Med_Green` | 713 | Object | -3127.75,-729.14,2958.46 | 95,405,235 | Scale/Radius: 1.00 |
| 204 | `Roid_Med_Green` | 715 | Object | 801.24,662.85,5795.14 | 491,411,229 | Scale/Radius: 1.00 |
| 205 | `Roid_Med_Green` | 717 | Object | -2997.18,640.76,2827.89 | 223,437,449 | Scale/Radius: 1.00 |
| 206 | `Roid_Med_Green` | 719 | Object | -3479.35,0.00,3487.75 | 335,177,483 | Scale/Radius: 1.00 |
| 207 | `Roid_Med_Green` | 722 | Object | -2801.96,-433.27,4782.77 | 427,511,129 | Scale/Radius: 1.00 |
| 208 | `Roid_Med_Green` | 728 | Object | -1923.69,-419.81,5184.02 | 114,43,316 | Scale/Radius: 1.00 |
| 209 | `Roid_Med_Green` | 735 | Object | -3434.71,265.14,4135.01 | 321,79,279 | Scale/Radius: 1.00 |
| 210 | `Roid_Med_Green` | 737 | Object | -4231.44,-596.57,2055.64 | 118,482,48 | Scale/Radius: 1.00 |
| 211 | `Roid_Med_Green` | 742 | Object | -2478.33,711.98,4769.99 | 227,458,345 | Scale/Radius: 1.00 |
| 212 | `Roid_Med_Green` | 746 | Object | -3451.38,-618.66,2936.14 | 457,498,3 | Scale/Radius: 1.00 |
| 213 | `Roid_Med_Green` | 755 | Object | -3242.76,-521.65,3839.78 | 96,41,494 | Scale/Radius: 1.00 |
| 214 | `Roid_Med_Green` | 761 | Object | -2123.45,441.90,5245.39 | 207,463,5 | Scale/Radius: 1.00 |
| 215 | `Roid_Med_Green` | 764 | Object | -714.06,773.33,6094.67 | 205,267,407 | Scale/Radius: 1.00 |
| 216 | `Roid_Med_Green` | 766 | Object | -4057.34,-265.14,2089.12 | 445,42,226 | Scale/Radius: 1.00 |
| 217 | `Roid_Med_Green` | 769 | Object | -2712.68,375.62,4796.78 | 421,172,434 | Scale/Radius: 1.00 |
| 218 | `Roid_Med_Green2` | 705 | Object | -3086.53,-397.71,3579.26 | 407,430,404 | Scale/Radius: 1.00 |
| 219 | `Roid_Med_Green2` | 391 | Object | 2509.74,419.81,5209.32 | 298,142,501 | Scale/Radius: 1.00 |
| 220 | `Roid_Med_Green2` | 393 | Object | 2217.25,89.96,4693.01 | 465,229,128 | Scale/Radius: 1.00 |
| 221 | `Roid_Med_Green2` | 398 | Object | 3436.78,-779.64,2526.58 | 89,159,53 | Scale/Radius: 1.00 |
| 222 | `Roid_Med_Green2` | 399 | Object | 3194.29,-659.69,2686.50 | 3,285,115 | Scale/Radius: 1.00 |
| 223 | `Roid_Med_Green2` | 402 | Object | 2487.64,-479.78,2295.18 | 106,307,31 | Scale/Radius: 1.00 |
| 224 | `Roid_Med_Green2` | 404 | Object | 1995.28,-209.90,3706.71 | 59,26,14 | Scale/Radius: 1.00 |
| 225 | `Roid_Med_Green2` | 406 | Object | 2702.78,-588.78,2158.76 | 387,111,495 | Scale/Radius: 1.00 |
| 226 | `Roid_Med_Green2` | 408 | Object | 2928.07,389.82,3624.34 | 273,168,131 | Scale/Radius: 1.00 |
| 227 | `Roid_Med_Green2` | 410 | Object | 3056.28,179.92,2248.76 | 452,9,335 | Scale/Radius: 1.00 |
| 228 | `Roid_Med_Green2` | 412 | Object | 2032.33,897.29,3894.61 | 266,204,247 | Scale/Radius: 1.00 |
| 229 | `Roid_Med_Green2` | 415 | Object | 2630.41,359.83,3397.73 | 325,468,104 | Scale/Radius: 1.00 |
| 230 | `Roid_Med_Green2` | 418 | Object | 2193.98,-659.69,2301.92 | 100,239,443 | Scale/Radius: 1.00 |
| 231 | `Roid_Med_Green2` | 419 | Object | 3041.03,-434.85,2996.59 | 389,307,157 | Scale/Radius: 1.00 |
| 232 | `Roid_Med_Green2` | 421 | Object | 2831.67,239.89,2114.81 | 85,277,225 | Scale/Radius: 1.00 |
| 233 | `Roid_Med_Green2` | 423 | Object | 2229.40,719.67,4845.74 | 161,251,504 | Scale/Radius: 1.00 |
| 234 | `Roid_Med_Green2` | 424 | Object | 2855.03,660.64,3505.35 | 45,118,452 | Scale/Radius: 1.00 |
| 235 | `Roid_Med_Green2` | 425 | Object | 2242.44,-479.78,4606.19 | 484,85,15 | Scale/Radius: 1.00 |
| 236 | `Roid_Med_Green2` | 426 | Object | 2936.71,660.64,4230.09 | 146,403,179 | Scale/Radius: 1.00 |
| 237 | `Roid_Med_Green2` | 430 | Object | -1561.36,-239.89,5585.18 | 437,481,188 | Scale/Radius: 1.00 |
| 238 | `Roid_Med_Green2` | 431 | Object | 2688.53,779.64,1862.14 | 29,426,466 | Scale/Radius: 1.00 |
| 239 | `Roid_Med_Green2` | 433 | Object | 2532.00,209.90,2698.91 | 7,325,186 | Scale/Radius: 1.00 |
| 240 | `Roid_Med_Green2` | 435 | Object | 2807.36,419.81,1809.34 | 381,469,45 | Scale/Radius: 1.00 |
| 241 | `Roid_Med_Green2` | 438 | Object | 3092.58,957.26,4391.51 | 85,367,10 | Scale/Radius: 1.00 |
| 242 | `Roid_Med_Green2` | 440 | Object | 2338.21,419.81,2750.65 | 235,238,45 | Scale/Radius: 1.00 |
| 243 | `Roid_Med_Green2` | 443 | Object | -1947.24,-119.94,5967.91 | 489,449,199 | Scale/Radius: 1.00 |
| 244 | `Roid_Med_Green2` | 445 | Object | 3150.63,-119.94,3583.82 | 208,195,161 | Scale/Radius: 1.00 |
| 245 | `Roid_Med_Green2` | 448 | Object | 3593.23,-329.85,2408.93 | 59,49,402 | Scale/Radius: 1.00 |
| 246 | `Roid_Med_Green2` | 452 | Object | 2902.66,29.99,3373.63 | 205,292,360 | Scale/Radius: 1.00 |
| 247 | `Roid_Med_Green2` | 457 | Object | 3583.62,777.35,3385.41 | 253,196,312 | Scale/Radius: 1.00 |
| 248 | `Roid_Med_Green2` | 459 | Object | 3209.64,632.95,2979.03 | 108,18,91 | Scale/Radius: 1.00 |
| 249 | `Roid_Med_Green2` | 460 | Object | 3608.86,-558.79,2770.85 | 168,497,198 | Scale/Radius: 1.00 |
| 250 | `Roid_Med_Green2` | 463 | Object | 2893.90,299.86,2224.66 | 316,211,249 | Scale/Radius: 1.00 |
| 251 | `Roid_Med_Green2` | 464 | Object | 2374.58,837.32,4174.29 | 248,199,471 | Scale/Radius: 1.00 |
| 252 | `Roid_Med_Green2` | 466 | Object | 3169.47,359.83,1923.44 | 340,121,22 | Scale/Radius: 1.00 |
| 253 | `Roid_Med_Green2` | 468 | Object | 3762.06,-269.87,3032.36 | 198,339,108 | Scale/Radius: 1.00 |
| 254 | `Roid_Med_Green2` | 471 | Object | -1561.36,789.31,5585.18 | 147,250,117 | Scale/Radius: 1.00 |
| 255 | `Roid_Med_Green2` | 476 | Object | 2854.93,927.28,4497.12 | 132,356,413 | Scale/Radius: 1.00 |
| 256 | `Roid_Med_Green2` | 478 | Object | 2567.30,779.64,3680.16 | 61,87,160 | Scale/Radius: 1.00 |
| 257 | `Roid_Med_Green2` | 480 | Object | 2469.48,-359.83,2719.82 | 179,207,189 | Scale/Radius: 1.00 |
| 258 | `Roid_Med_Green2` | 482 | Object | 3632.03,747.36,1812.25 | 139,203,181 | Scale/Radius: 1.00 |
| 259 | `Roid_Med_Green2` | 486 | Object | 709.40,266.72,4849.28 | 376,484,471 | Scale/Radius: 1.00 |
| 260 | `Roid_Med_Green2` | 489 | Object | -72.95,-510.60,5330.62 | 510,322,267 | Scale/Radius: 1.00 |
| 261 | `Roid_Med_Green2` | 505 | Object | -1308.69,765.64,5593.80 | 55,56,452 | Scale/Radius: 1.00 |
| 262 | `Roid_Med_Green2` | 516 | Object | -347.86,738.60,5124.35 | 179,391,361 | Scale/Radius: 1.00 |
| 263 | `Roid_Med_Green2` | 528 | Object | 353.17,-779.64,5317.61 | 265,474,433 | Scale/Radius: 1.00 |
| 264 | `Roid_Med_Green2` | 539 | Object | -30.33,328.27,6002.56 | 167,27,95 | Scale/Radius: 1.00 |
| 265 | `Roid_Med_Green2` | 548 | Object | -474.62,677.05,5613.37 | 173,175,273 | Scale/Radius: 1.00 |
| 266 | `Roid_Med_Green2` | 549 | Object | -669.51,123.10,5936.27 | 426,85,230 | Scale/Radius: 1.00 |
| 267 | `Roid_Med_Green2` | 578 | Object | -3104.31,110.48,2519.89 | 136,326,438 | Scale/Radius: 1.00 |
| 268 | `Roid_Med_Green2` | 582 | Object | -3725.90,775.77,2371.62 | 475,38,238 | Scale/Radius: 1.00 |
| 269 | `Roid_Med_Green2` | 587 | Object | -2835.44,751.23,4573.58 | 284,44,299 | Scale/Radius: 1.00 |
| 270 | `Roid_Med_Green2` | 588 | Object | 1714.74,0.00,6038.97 | 443,259,304 | Scale/Radius: 1.00 |
| 271 | `Roid_Med_Green2` | 593 | Object | -3931.24,-154.67,2516.54 | 466,126,197 | Scale/Radius: 1.00 |
| 272 | `Roid_Med_Green2` | 596 | Object | -2204.23,-309.33,5114.99 | 55,213,403 | Scale/Radius: 1.00 |
| 273 | `Roid_Med_Green2` | 610 | Object | -2317.48,-795.42,5180.74 | 435,160,207 | Scale/Radius: 1.00 |
| 274 | `Roid_Med_Green2` | 612 | Object | 2543.66,-508.19,5491.35 | 172,497,226 | Scale/Radius: 1.00 |
| 275 | `Roid_Med_Green2` | 614 | Object | -2939.22,-565.84,3882.19 | 491,65,448 | Scale/Radius: 1.00 |
| 276 | `Roid_Med_Green2` | 618 | Object | -3808.48,596.57,2739.73 | 272,74,432 | Scale/Radius: 1.00 |
| 277 | `Roid_Med_Green2` | 624 | Object | -2604.43,842.05,3711.09 | 57,121,289 | Scale/Radius: 1.00 |
| 278 | `Roid_Med_Green2` | 627 | Object | -883.68,-508.19,6125.91 | 426,182,223 | Scale/Radius: 1.00 |
| 279 | `Roid_Med_Green2` | 629 | Object | 1605.38,66.29,6009.95 | 56,480,454 | Scale/Radius: 1.00 |
| 280 | `Roid_Med_Green2` | 633 | Object | 1553.40,530.28,5804.07 | 464,447,230 | Scale/Radius: 1.00 |
| 281 | `Roid_Med_Green2` | 641 | Object | 2395.98,-166.31,5306.61 | 97,346,86 | Scale/Radius: 1.00 |
| 282 | `Roid_Med_Green2` | 644 | Object | -3252.74,287.24,3014.26 | 206,209,22 | Scale/Radius: 1.00 |
| 283 | `Roid_Med_Green2` | 646 | Object | -3822.99,-773.33,2685.05 | 159,215,77 | Scale/Radius: 1.00 |
| 284 | `Roid_Med_Green2` | 654 | Object | -4097.52,220.95,2752.01 | 464,270,357 | Scale/Radius: 1.00 |
| 285 | `Roid_Med_Green2` | 656 | Object | -1439.03,773.33,6042.75 | 394,386,490 | Scale/Radius: 1.00 |
| 286 | `Roid_Med_Green2` | 659 | Object | 2380.80,-353.52,5426.42 | 289,451,395 | Scale/Radius: 1.00 |
| 287 | `Roid_Med_Green2` | 662 | Object | -4122.07,-22.09,2084.66 | 390,341,252 | Scale/Radius: 1.00 |
| 288 | `Roid_Med_Green2` | 663 | Object | 680.26,618.66,5976.22 | 221,336,301 | Scale/Radius: 1.00 |
| 289 | `Roid_Med_Green2` | 668 | Object | -2749.51,753.67,4409.69 | 307,255,290 | Scale/Radius: 1.00 |
| 290 | `Roid_Med_Green2` | 672 | Object | -3001.64,574.47,2763.17 | 296,48,504 | Scale/Radius: 1.00 |
| 291 | `Roid_Med_Green2` | 675 | Object | -3489.32,-486.09,2697.32 | 216,274,132 | Scale/Radius: 1.00 |
| 292 | `Roid_Med_Green2` | 677 | Object | -2382.79,552.38,5016.78 | 250,22,22 | Scale/Radius: 1.00 |
| 293 | `Roid_Med_Green2` | 679 | Object | -3158.99,-905.90,2505.38 | 222,455,12 | Scale/Radius: 1.00 |
| 294 | `Roid_Med_Green2` | 685 | Object | -2362.27,287.24,4584.74 | 29,276,120 | Scale/Radius: 1.00 |
| 295 | `Roid_Med_Green2` | 688 | Object | -3067.56,773.33,3698.67 | 357,102,116 | Scale/Radius: 1.00 |
| 296 | `Roid_Med_Green2` | 690 | Object | -785.48,-375.62,6304.47 | 220,49,345 | Scale/Radius: 1.00 |
| 297 | `Roid_Med_Green2` | 692 | Object | -2394.63,0.00,4271.16 | 66,329,290 | Scale/Radius: 1.00 |
| 298 | `Roid_Med_Green2` | 697 | Object | 1481.11,751.23,5658.93 | 256,166,86 | Scale/Radius: 1.00 |
| 299 | `Roid_Med_Green2` | 711 | Object | 1680.42,971.56,5721.83 | 206,194,87 | Scale/Radius: 1.00 |
| 300 | `Roid_Med_Green2` | 718 | Object | -2508.46,-331.43,3554.71 | 119,154,139 | Scale/Radius: 1.00 |
| 301 | `Roid_Med_Green2` | 723 | Object | -2481.67,-773.33,3943.06 | 170,258,506 | Scale/Radius: 1.00 |
| 302 | `Roid_Med_Green2` | 724 | Object | -1292.84,0.00,5827.37 | 38,460,285 | Scale/Radius: 1.00 |
| 303 | `Roid_Med_Green2` | 729 | Object | -2368.28,88.38,5071.46 | 176,25,359 | Scale/Radius: 1.00 |
| 304 | `Roid_Med_Green2` | 736 | Object | -3531.80,-729.14,3816.96 | 353,308,78 | Scale/Radius: 1.00 |
| 305 | `Roid_Med_Green2` | 738 | Object | -3097.62,-455.37,2963.43 | 379,434,283 | Scale/Radius: 1.00 |
| 306 | `Roid_Med_Green2` | 743 | Object | -729.62,0.00,5840.62 | 446,454,206 | Scale/Radius: 1.00 |
| 307 | `Roid_Med_Green2` | 749 | Object | -3183.62,-441.90,3261.21 | 75,288,145 | Scale/Radius: 1.00 |
| 308 | `Roid_Med_Green2` | 751 | Object | -2307.44,0.00,5170.70 | 328,39,284 | Scale/Radius: 1.00 |
| 309 | `Roid_Med_Green2` | 753 | Object | -3461.49,-773.33,3746.65 | 444,317,472 | Scale/Radius: 1.00 |
| 310 | `Roid_Med_Green2` | 756 | Object | -3035.19,-66.28,3389.54 | 445,12,164 | Scale/Radius: 1.00 |
| 311 | `Roid_Med_Green2` | 760 | Object | -269.88,486.09,6018.02 | 169,170,152 | Scale/Radius: 1.00 |
| 312 | `Roid_Med_Green2` | 762 | Object | -3942.37,0.00,2928.37 | 171,318,335 | Scale/Radius: 1.00 |
| 313 | `Roid_Med_Green2` | 765 | Object | -1402.20,44.19,5798.36 | 184,173,56 | Scale/Radius: 1.00 |
| 314 | `Roid_Med_Green2` | 768 | Object | -3535.07,864.15,2803.49 | 491,467,437 | Scale/Radius: 1.00 |
| 315 | `Roid_XL_Green` | 585 | Object | -3718.09,486.09,2649.34 | 139,79,172 | Scale/Radius: 1.00 |
| 316 | `Roid_XL_Green` | 447 | Object | 3707.58,-179.92,1560.56 | 451,75,511 | Scale/Radius: 1.00 |
| 317 | `Roid_XL_Green` | 449 | Object | 2237.09,-494.82,4238.01 | 88,415,474 | Scale/Radius: 1.00 |
| 318 | `Roid_XL_Green` | 470 | Object | 3762.43,717.38,2173.71 | 397,362,4 | Scale/Radius: 1.00 |
| 319 | `Roid_XL_Green` | 475 | Object | 1848.92,-659.69,4567.92 | 247,203,489 | Scale/Radius: 1.00 |
| 320 | `Roid_XL_Green` | 496 | Object | -1479.14,-677.05,5472.28 | 19,493,57 | Scale/Radius: 1.00 |
| 321 | `Roid_XL_Green` | 517 | Object | -327.43,102.58,5433.68 | 345,498,141 | Scale/Radius: 1.00 |
| 322 | `Roid_XL_Green` | 531 | Object | 1437.43,841.19,5980.05 | 365,343,454 | Scale/Radius: 1.00 |
| 323 | `Roid_XL_Green` | 551 | Object | -284.81,-553.95,5488.92 | 436,85,247 | Scale/Radius: 1.00 |
| 324 | `Roid_XL_Green` | 560 | Object | -1308.69,-533.44,5737.42 | 115,480,434 | Scale/Radius: 1.00 |
| 325 | `Roid_XL_Green` | 607 | Object | 1803.39,309.33,4359.92 | 38,296,303 | Scale/Radius: 1.00 |
| 326 | `Roid_XL_Green` | 699 | Object | 1678.19,-353.52,5648.23 | 145,6,16 | Scale/Radius: 1.00 |
| 327 | `Roid_XL_Green` | 732 | Object | -314.51,667.17,5993.47 | 259,30,232 | Scale/Radius: 1.00 |
| 328 | `Roid_Med_Green` | 513 | Object | -967.79,266.72,5947.32 | 313,250,97 | Scale/Radius: 1.00 |
| 329 | `Roid_Med_Green` | 397 | Object | 3445.83,-689.68,3544.79 | 105,229,456 | Scale/Radius: 1.00 |
| 330 | `Roid_Med_Green` | 413 | Object | 2429.42,-869.60,4804.99 | 396,281,196 | Scale/Radius: 1.00 |
| 331 | `Roid_Med_Green` | 417 | Object | 2374.09,-869.60,3470.38 | 187,162,63 | Scale/Radius: 1.00 |
| 332 | `Roid_Med_Green` | 446 | Object | 2810.03,-468.83,1691.70 | 262,24,357 | Scale/Radius: 1.00 |
| 333 | `Roid_Med_Green` | 454 | Object | 2387.49,690.63,2354.62 | 75,471,464 | Scale/Radius: 1.00 |
| 334 | `Roid_Med_Green` | 473 | Object | 3328.17,-419.81,3074.54 | 186,49,45 | Scale/Radius: 1.00 |
| 335 | `Roid_Med_Green` | 479 | Object | 3897.27,-494.82,2368.20 | 396,471,278 | Scale/Radius: 1.00 |
| 336 | `Roid_Med_Green` | 485 | Object | -1990.48,-471.89,5317.61 | 349,285,343 | Scale/Radius: 1.00 |
| 337 | `Roid_Med_Green` | 504 | Object | 2248.97,205.17,5244.06 | 330,183,36 | Scale/Radius: 1.00 |
| 338 | `Roid_Med_Green` | 511 | Object | 1922.19,-389.82,5693.72 | 106,461,430 | Scale/Radius: 1.00 |
| 339 | `Roid_Med_Green` | 542 | Object | 2149.39,820.67,5387.91 | 124,455,70 | Scale/Radius: 1.00 |
| 340 | `Roid_Med_Green` | 563 | Object | 566.23,307.75,5052.47 | 174,102,226 | Scale/Radius: 1.00 |
| 341 | `Roid_Med_Green` | 569 | Object | -4120.96,530.28,2567.87 | 398,343,444 | Scale/Radius: 1.00 |
| 342 | `Roid_Med_Green` | 594 | Object | -2694.05,-530.28,4993.25 | 137,375,179 | Scale/Radius: 1.00 |
| 343 | `Roid_Med_Green` | 666 | Object | -4069.62,-552.38,2378.16 | 280,497,349 | Scale/Radius: 1.00 |
| 344 | `Roid_Med_Green` | 670 | Object | -3248.34,665.29,3870.68 | 146,472,191 | Scale/Radius: 1.00 |
| 345 | `Roid_Med_Green` | 678 | Object | -2992.79,-375.62,3070.38 | 331,2,157 | Scale/Radius: 1.00 |
| 346 | `Roid_Med_Green` | 709 | Object | -2242.71,-508.19,5175.16 | 261,322,276 | Scale/Radius: 1.00 |
| 347 | `Roid_Med_Green` | 721 | Object | -408.26,132.57,5879.64 | 358,472,431 | Scale/Radius: 1.00 |
| 348 | `Roid_Med_Green` | 731 | Object | -1173.43,265.14,5846.34 | 247,355,214 | Scale/Radius: 1.00 |
| 349 | `Roid_Med_Green` | 739 | Object | -2759.55,154.67,3805.80 | 319,204,420 | Scale/Radius: 1.00 |
