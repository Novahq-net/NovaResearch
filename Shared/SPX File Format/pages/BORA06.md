# Tachyon: The Fringe BORA06.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `BORA06.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `BORA6.BDF` |
| Region | 3 |
| Sector ID | 5 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 10 |
| Entities | 325 |
| Events | 4 |
| Waypoints | 0 |
| Child Sectors | 1 |
| Scripts | 0 |
| Scenes | 1 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Mad_Pirate_Platform`, `1: Retribution_Shipyard`, `2: Spcargo_Parts`, `3: Satellite`, `4: Pirate_Mine_HvyLaser`, `5: Roid_XL_Green`, `6: Roid_Med_Green`, `7: Asteroid_1`, `8: Roid_Med_Green2`, `9: Hyper_Gate` |
| Scripts | None |
| Scenes | `B6BC011B.SEN` |
| Labels | None |
| Aliases | None |
| Groups | `FG_ANVIL`, `CONT_060`, `RETRIBUTION` |
| Child Sectors | [bora06A.spx](BORA06A.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Group/spawn-list action: spawn list/group 15, subtype 4, param 1

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 1800 (extra 1, 927; flags 2)
- Variable comparison: subject variable group 0, variable 4, op 1, value 2001

**Action**

- Set/add variable: variable group 21, variable 21, subtype 0, value 1
- Group/spawn-list action: spawn list/group 15, subtype 4, param 9

### Event 2

**Trigger**

- Group/spawn-list event: subject 15, op 0, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 0, value 1

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 930; flags 2)

**Action**

- Set/add variable: variable group 15, variable 806, subtype 0, value 1

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 5 | Gate | -1774.24,-451.00,-1942.76 | 448,0,0 | Gate SPX: [bora07.spx](BORA07.md) |
| 1 | `Roid_Med_Green2` | 528 | Object | -3478.68,555.57,-2640.20 | 484,4,321 | Scale/Radius: 4.00 |
| 2 | `Asteroid_1` | 529 | Object | -2296.63,843.97,-6836.95 | 168,121,0 | Scale/Radius: 7.00 |
| 3 | `Roid_Med_Green2` | 530 | Object | -6137.75,843.97,-5525.26 | 386,106,92 | Scale/Radius: 2.00 |
| 4 | `Roid_Med_Green2` | 531 | Object | -6022.38,1420.79,-5525.26 | 36,331,448 | Scale/Radius: 1.00 |
| 5 | `Roid_Med_Green2` | 532 | Object | -2707.22,-367.34,-3865.31 | 218,247,442 | Scale/Radius: 2.00 |
| 6 | `Asteroid_1` | 533 | Object | -6310.98,1247.75,-4339.95 | 387,1,251 | Scale/Radius: 1.00 |
| 7 | `Roid_Med_Green2` | 534 | Object | -4996.11,94.11,-3887.41 | 321,331,173 | Scale/Radius: 4.00 |
| 8 | `Roid_Med_Green2` | 535 | Object | -5748.57,-1715.03,-2929.38 | 394,268,330 | Scale/Radius: 6.00 |
| 9 | `Roid_Med_Green` | 536 | Object | -5053.79,497.88,-4392.52 | 429,212,193 | Scale/Radius: 4.00 |
| 10 | `Asteroid_1` | 537 | Object | -3052.10,1190.07,-6142.84 | 387,348,65 | Scale/Radius: 8.00 |
| 11 | `Roid_Med_Green` | 538 | Object | -2701.75,253.61,-3863.86 | 29,86,422 | Scale/Radius: 4.00 |
| 12 | `Roid_XL_Green` | 539 | Object | -6479.45,-2581.13,-4820.51 | 137,154,152 | Scale/Radius: 2.00 |
| 13 | `Asteroid_1` | 540 | Object | -5816.73,-698.63,-4930.89 | 137,14,317 | Scale/Radius: 3.00 |
| 14 | `Asteroid_1` | 541 | Object | -5169.15,-828.80,-3831.29 | 500,433,89 | Scale/Radius: 6.00 |
| 15 | `Roid_Med_Green2` | 542 | Object | -2432.49,2228.34,-5433.77 | 437,433,174 | Scale/Radius: 4.00 |
| 16 | `Roid_Med_Green` | 543 | Object | -4663.92,-194.30,-3099.38 | 493,44,370 | Scale/Radius: 3.00 |
| 17 | `Roid_Med_Green` | 544 | Object | -1955.02,1420.79,-6495.66 | 167,84,479 | Scale/Radius: 5.00 |
| 18 | `Asteroid_1` | 545 | Object | -3366.33,209.47,-2835.80 | 120,480,226 | Scale/Radius: 1.00 |
| 19 | `Roid_Med_Green` | 546 | Object | -5733.97,36.43,-5693.62 | 493,327,461 | Scale/Radius: 8.00 |
| 20 | `Roid_Med_Green` | 547 | Object | -2596.36,-528.17,-4456.81 | 387,68,32 | Scale/Radius: 6.00 |
| 21 | `Roid_Med_Green2` | 548 | Object | -4840.23,-4405.07,-7096.92 | 66,499,330 | Scale/Radius: 9.00 |
| 22 | `Roid_Med_Green2` | 549 | Object | -5676.29,-3309.12,-6367.10 | 63,391,444 | Scale/Radius: 4.00 |
| 23 | `Roid_Med_Green2` | 550 | Object | -4133.80,324.84,-4087.43 | 490,337,47 | Scale/Radius: 1.00 |
| 24 | `Roid_Med_Green2` | 551 | Object | -3952.90,-730.30,-6785.22 | 154,399,195 | Scale/Radius: 4.00 |
| 25 | `Roid_Med_Green2` | 552 | Object | -5665.72,-1574.84,-6152.32 | 409,358,474 | Scale/Radius: 2.00 |
| 26 | `Roid_Med_Green2` | 553 | Object | -4275.80,3381.97,-6934.28 | 76,277,423 | Scale/Radius: 9.00 |
| 27 | `Roid_Med_Green2` | 554 | Object | -3991.95,-771.12,-3891.38 | 217,285,94 | Scale/Radius: 9.00 |
| 28 | `Roid_Med_Green` | 555 | Object | -3802.45,-540.39,-3604.45 | 186,261,161 | Scale/Radius: 2.00 |
| 29 | `Roid_XL_Green` | 556 | Object | -2800.66,-4174.34,-4832.57 | 146,99,298 | Scale/Radius: 1.00 |
| 30 | `Roid_Med_Green` | 557 | Object | -1839.66,-771.12,-6383.41 | 46,372,318 | Scale/Radius: 5.00 |
| 31 | `Roid_Med_Green` | 558 | Object | -4897.92,2516.75,-7265.29 | 201,113,411 | Scale/Radius: 1.00 |
| 32 | `Roid_Med_Green2` | 559 | Object | -5086.76,-1605.57,-3570.92 | 331,407,9 | Scale/Radius: 2.00 |
| 33 | `Roid_Med_Green` | 560 | Object | -4799.88,-4174.34,-4480.56 | 215,64,94 | Scale/Radius: 9.00 |
| 34 | `Roid_Med_Green2` | 561 | Object | -5610.51,3497.34,-5416.65 | 85,426,35 | Scale/Radius: 5.00 |
| 35 | `Asteroid_1` | 562 | Object | -3035.74,-4232.03,-3235.86 | 48,130,56 | Scale/Radius: 7.00 |
| 36 | `Roid_Med_Green` | 563 | Object | -2244.55,3913.33,-5607.78 | 212,392,239 | Scale/Radius: 9.00 |
| 37 | `Roid_Med_Green2` | 564 | Object | -4492.64,-655.75,-4204.50 | 140,151,33 | Scale/Radius: 9.00 |
| 38 | `Roid_XL_Green` | 565 | Object | -3563.06,-1595.53,-2779.68 | 438,423,375 | Scale/Radius: 3.00 |
| 39 | `Roid_XL_Green` | 566 | Object | -4993.50,267.16,-2920.87 | 419,204,214 | Scale/Radius: 1.00 |
| 40 | `Roid_Med_Green` | 567 | Object | -5226.83,-1347.93,-2989.45 | 449,475,72 | Scale/Radius: 9.00 |
| 41 | `Asteroid_1` | 568 | Object | -4680.40,670.93,-3346.99 | 0,20,482 | Scale/Radius: 4.00 |
| 42 | `Roid_Med_Green` | 569 | Object | -5434.67,-3078.39,-5586.76 | 508,76,463 | Scale/Radius: 3.00 |
| 43 | `Roid_Med_Green2` | 570 | Object | -6137.93,151.79,-3890.97 | 115,224,251 | Scale/Radius: 2.00 |
| 44 | `Roid_Med_Green` | 571 | Object | -5164.95,-1422.39,-4361.18 | 176,474,313 | Scale/Radius: 4.00 |
| 45 | `Roid_Med_Green` | 572 | Object | -1955.02,2632.11,-6215.05 | 131,7,139 | Scale/Radius: 8.00 |
| 46 | `Asteroid_1` | 573 | Object | -3471.26,440.20,-4147.61 | 413,511,60 | Scale/Radius: 5.00 |
| 47 | `Roid_Med_Green2` | 574 | Object | -4409.15,1363.11,-3921.30 | 363,483,137 | Scale/Radius: 4.00 |
| 48 | `Roid_XL_Green` | 575 | Object | -3103.66,-3078.39,-7346.22 | 62,270,342 | Scale/Radius: 3.00 |
| 49 | `Roid_Med_Green` | 576 | Object | -3219.78,1882.25,-3408.40 | 197,213,45 | Scale/Radius: 5.00 |
| 50 | `Roid_Med_Green2` | 577 | Object | -2547.99,1536.16,-7518.19 | 218,435,342 | Scale/Radius: 5.00 |
| 51 | `Roid_Med_Green` | 578 | Object | -1840.78,2228.34,-7096.92 | 282,445,128 | Scale/Radius: 6.00 |
| 52 | `Roid_Med_Green2` | 579 | Object | -5604.82,670.93,-5929.96 | 288,364,241 | Scale/Radius: 7.00 |
| 53 | `Roid_Med_Green2` | 580 | Object | -3631.11,4259.42,-7187.54 | 202,69,381 | Scale/Radius: 7.00 |
| 54 | `Asteroid_1` | 581 | Object | -2508.31,-969.48,-6443.90 | 472,397,154 | Scale/Radius: 6.00 |
| 55 | `Roid_Med_Green2` | 582 | Object | -5608.82,4420.25,-4377.24 | 434,182,86 | Scale/Radius: 7.00 |
| 56 | `Roid_XL_Green` | 583 | Object | -2516.62,-3482.16,-4854.98 | 345,505,79 | Scale/Radius: 1.00 |
| 57 | `Asteroid_1` | 584 | Object | -4102.26,1002.53,-6916.08 | 193,308,227 | Scale/Radius: 1.00 |
| 58 | `Roid_Med_Green2` | 585 | Object | -1955.02,728.61,-5878.31 | 285,392,272 | Scale/Radius: 1.00 |
| 59 | `Asteroid_1` | 586 | Object | -6127.96,670.93,-3367.03 | 350,301,287 | Scale/Radius: 6.00 |
| 60 | `Roid_Med_Green` | 587 | Object | -4264.63,3035.88,-3865.31 | 469,488,84 | Scale/Radius: 3.00 |
| 61 | `Roid_XL_Green` | 588 | Object | -5295.59,-1768.48,-3223.19 | 198,47,26 | Scale/Radius: 2.00 |
| 62 | `Roid_Med_Green` | 589 | Object | -3505.17,3093.57,-6910.42 | 297,64,215 | Scale/Radius: 5.00 |
| 63 | `Roid_Med_Green2` | 590 | Object | -5257.73,-3323.61,-6498.42 | 49,329,179 | Scale/Radius: 1.00 |
| 64 | `Roid_Med_Green` | 591 | Object | -4534.65,-3943.62,-3831.29 | 333,455,68 | Scale/Radius: 8.00 |
| 65 | `Asteroid_1` | 592 | Object | -2417.60,-4693.48,-5974.47 | 75,362,357 | Scale/Radius: 7.00 |
| 66 | `Roid_Med_Green` | 593 | Object | -6104.96,-965.16,-4208.87 | 344,217,471 | Scale/Radius: 4.00 |
| 67 | `Roid_Med_Green2` | 594 | Object | -2475.28,-4058.98,-6198.96 | 110,57,501 | Scale/Radius: 3.00 |
| 68 | `Asteroid_1` | 595 | Object | -3577.89,267.16,-6602.09 | 423,73,59 | Scale/Radius: 9.00 |
| 69 | `Roid_Med_Green2` | 596 | Object | -4909.34,3439.66,-4924.06 | 42,8,496 | Scale/Radius: 7.00 |
| 70 | `Roid_Med_Green2` | 597 | Object | -4042.12,-1653.21,-3806.81 | 394,268,73 | Scale/Radius: 7.00 |
| 71 | `Roid_Med_Green` | 598 | Object | -1856.54,-911.80,-6836.95 | 220,37,35 | Scale/Radius: 1.00 |
| 72 | `Roid_Med_Green` | 599 | Object | -4967.02,4650.97,-4643.44 | 433,219,177 | Scale/Radius: 8.00 |
| 73 | `Asteroid_1` | 600 | Object | -5685.06,-1762.39,-4573.48 | 212,227,503 | Scale/Radius: 2.00 |
| 74 | `Roid_Med_Green2` | 601 | Object | -4842.83,-6174.57,-4177.51 | 438,178,120 | Scale/Radius: 4.00 |
| 75 | `Roid_Med_Green` | 602 | Object | -1968.16,-3885.93,-6057.14 | 349,382,201 | Scale/Radius: 7.00 |
| 76 | `Asteroid_1` | 603 | Object | -5191.84,1478.47,-4321.94 | 127,92,471 | Scale/Radius: 1.00 |
| 77 | `Roid_Med_Green2` | 604 | Object | -4871.27,-1001.84,-3731.92 | 267,391,57 | Scale/Radius: 5.00 |
| 78 | `Roid_Med_Green2` | 605 | Object | -2008.22,1363.11,-7117.56 | 96,412,97 | Scale/Radius: 6.00 |
| 79 | `Asteroid_1` | 606 | Object | -6580.82,2805.16,-4992.12 | 29,347,353 | Scale/Radius: 7.00 |
| 80 | `Asteroid_1` | 607 | Object | -5137.61,-4232.03,-6310.73 | 106,12,165 | Scale/Radius: 3.00 |
| 81 | `Roid_Med_Green` | 608 | Object | -4527.61,-531.93,-7066.20 | 12,400,64 | Scale/Radius: 3.00 |
| 82 | `Roid_XL_Green` | 609 | Object | -2816.24,2574.43,-5789.86 | 476,146,397 | Scale/Radius: 3.00 |
| 83 | `Roid_Med_Green` | 610 | Object | -5724.18,-4232.03,-4264.99 | 20,461,47 | Scale/Radius: 5.00 |
| 84 | `Asteroid_1` | 611 | Object | -3874.69,-1307.12,-4109.26 | 214,223,435 | Scale/Radius: 9.00 |
| 85 | `Asteroid_1` | 612 | Object | -2847.12,-1174.89,-6560.88 | 482,506,358 | Scale/Radius: 3.00 |
| 86 | `Roid_Med_Green` | 613 | Object | -5367.34,-6215.09,-4305.56 | 241,104,10 | Scale/Radius: 3.00 |
| 87 | `Roid_Med_Green` | 614 | Object | -3620.28,1363.11,-4165.38 | 198,375,284 | Scale/Radius: 7.00 |
| 88 | `Asteroid_1` | 615 | Object | -2821.37,-5154.93,-6255.08 | 455,429,256 | Scale/Radius: 4.00 |
| 89 | `Roid_Med_Green` | 616 | Object | -3943.15,-5212.62,-3060.29 | 71,233,337 | Scale/Radius: 1.00 |
| 90 | `Roid_XL_Green` | 617 | Object | -3226.36,-4693.48,-4370.42 | 262,484,254 | Scale/Radius: 1.00 |
| 91 | `Roid_Med_Green` | 618 | Object | -3130.33,-5270.30,-6661.94 | 72,242,200 | Scale/Radius: 7.00 |
| 92 | `Roid_Med_Green` | 619 | Object | -2747.35,1766.88,-5398.16 | 279,190,345 | Scale/Radius: 6.00 |
| 93 | `Roid_Med_Green2` | 620 | Object | -4487.45,-1800.93,-2971.45 | 408,305,413 | Scale/Radius: 1.00 |
| 94 | `Asteroid_1` | 621 | Object | -2976.95,-1720.63,-3775.46 | 27,237,111 | Scale/Radius: 2.00 |
| 95 | `Roid_Med_Green` | 622 | Object | -5903.74,2978.20,-5180.43 | 448,3,102 | Scale/Radius: 1.00 |
| 96 | `Roid_Med_Green` | 623 | Object | -4241.38,613.25,-3058.08 | 208,486,183 | Scale/Radius: 3.00 |
| 97 | `Roid_Med_Green` | 624 | Object | -4444.94,-425.03,-3586.01 | 190,231,458 | Scale/Radius: 7.00 |
| 98 | `Roid_Med_Green2` | 626 | Object | -3122.67,-1059.53,-3649.53 | 390,460,257 | Scale/Radius: 2.00 |
| 99 | `Roid_XL_Green` | 627 | Object | -3654.74,151.79,-2891.92 | 26,278,300 | Scale/Radius: 1.00 |
| 100 | `Roid_Med_Green` | 628 | Object | -3528.94,-4116.66,-3810.87 | 252,166,356 | Scale/Radius: 3.00 |
| 101 | `Roid_Med_Green` | 629 | Object | -6041.69,-1948.98,-4550.19 | 510,99,265 | Scale/Radius: 7.00 |
| 102 | `Asteroid_1` | 630 | Object | -6659.46,129.91,-5292.60 | 165,102,228 | Scale/Radius: 9.00 |
| 103 | `Roid_Med_Green` | 631 | Object | -5892.50,-561.39,-5894.51 | 483,14,17 | Scale/Radius: 8.00 |
| 104 | `Roid_Med_Green` | 632 | Object | -2571.96,-1223.75,-5300.99 | 469,499,474 | Scale/Radius: 2.00 |
| 105 | `Roid_Med_Green` | 633 | Object | -5145.56,-78.93,-4065.27 | 354,478,113 | Scale/Radius: 2.00 |
| 106 | `Roid_Med_Green` | 634 | Object | -3746.04,1190.07,-7177.95 | 136,263,43 | Scale/Radius: 3.00 |
| 107 | `Roid_Med_Green` | 635 | Object | -4071.75,2574.43,-4312.00 | 465,44,461 | Scale/Radius: 8.00 |
| 108 | `Roid_XL_Green` | 636 | Object | -2417.60,-598.07,-5637.73 | 229,499,383 | Scale/Radius: 1.00 |
| 109 | `Roid_Med_Green` | 637 | Object | -2993.80,-2905.34,-6720.93 | 292,195,510 | Scale/Radius: 8.00 |
| 110 | `Roid_Med_Green` | 638 | Object | -3469.81,-1826.25,-2751.32 | 219,462,40 | Scale/Radius: 8.00 |
| 111 | `Roid_Med_Green` | 639 | Object | -4969.32,1247.75,-6760.42 | 206,272,411 | Scale/Radius: 4.00 |
| 112 | `Roid_XL_Green` | 640 | Object | -3999.74,-1982.43,-7285.21 | 21,386,85 | Scale/Radius: 3.00 |
| 113 | `Roid_Med_Green2` | 641 | Object | -2420.40,94.11,-6153.15 | 502,426,45 | Scale/Radius: 8.00 |
| 114 | `Asteroid_1` | 642 | Object | -4372.08,-1512.53,-3083.69 | 151,150,403 | Scale/Radius: 6.00 |
| 115 | `Roid_Med_Green2` | 643 | Object | -4131.29,-1751.71,-2513.67 | 271,320,283 | Scale/Radius: 4.00 |
| 116 | `Roid_Med_Green` | 644 | Object | -5608.82,728.61,-3198.66 | 195,353,196 | Scale/Radius: 4.00 |
| 117 | `Asteroid_1` | 645 | Object | -3413.58,1190.07,-3810.87 | 189,190,291 | Scale/Radius: 2.00 |
| 118 | `Roid_Med_Green2` | 646 | Object | -5572.19,-3309.12,-5574.35 | 281,299,26 | Scale/Radius: 9.00 |
| 119 | `Roid_Med_Green` | 647 | Object | -5382.68,-1001.84,-5118.74 | 158,402,85 | Scale/Radius: 4.00 |
| 120 | `Roid_Med_Green` | 648 | Object | -3911.96,-3828.25,-3368.59 | 335,204,126 | Scale/Radius: 5.00 |
| 121 | `Roid_Med_Green` | 649 | Object | -5140.66,3612.70,-6701.32 | 171,20,476 | Scale/Radius: 3.00 |
| 122 | `Roid_Med_Green2` | 650 | Object | -4952.80,-4751.16,-2702.64 | 225,430,505 | Scale/Radius: 2.00 |
| 123 | `Asteroid_1` | 651 | Object | -4645.31,-771.12,-2596.36 | 345,111,269 | Scale/Radius: 3.00 |
| 124 | `Roid_Med_Green2` | 652 | Object | -6397.64,1017.02,-4234.66 | 313,361,162 | Scale/Radius: 7.00 |
| 125 | `Roid_XL_Green` | 654 | Object | -4183.85,1997.61,-3325.95 | 186,121,155 | Scale/Radius: 2.00 |
| 126 | `Roid_Med_Green` | 655 | Object | -3911.96,209.47,-3705.32 | 149,333,428 | Scale/Radius: 3.00 |
| 127 | `Roid_Med_Green2` | 656 | Object | -2260.89,-1359.43,-5944.89 | 17,155,273 | Scale/Radius: 8.00 |
| 128 | `Asteroid_1` | 657 | Object | -2724.99,-824.34,-5448.78 | 113,53,327 | Scale/Radius: 4.00 |
| 129 | `Roid_Med_Green2` | 658 | Object | -3292.91,382.52,-6365.96 | 50,287,392 | Scale/Radius: 9.00 |
| 130 | `Roid_Med_Green2` | 659 | Object | -3135.53,1190.07,-7122.11 | 18,324,451 | Scale/Radius: 7.00 |
| 131 | `Roid_Med_Green` | 660 | Object | -4485.26,-1924.75,-2764.71 | 485,314,510 | Scale/Radius: 7.00 |
| 132 | `Roid_Med_Green2` | 662 | Object | -6238.46,-367.34,-5369.57 | 135,292,433 | Scale/Radius: 5.00 |
| 133 | `Roid_Med_Green` | 663 | Object | -5497.77,324.84,-4771.79 | 403,188,362 | Scale/Radius: 4.00 |
| 134 | `Roid_Med_Green` | 664 | Object | -3054.90,-6020.16,-5760.29 | 458,277,409 | Scale/Radius: 9.00 |
| 135 | `Roid_XL_Green` | 665 | Object | -5070.96,-5097.25,-7321.41 | 471,286,410 | Scale/Radius: 2.00 |
| 136 | `Asteroid_1` | 666 | Object | -4104.19,959.34,-4467.33 | 376,100,448 | Scale/Radius: 6.00 |
| 137 | `Roid_Med_Green2` | 667 | Object | -5163.39,-251.98,-4674.15 | 385,135,204 | Scale/Radius: 3.00 |
| 138 | `Roid_Med_Green2` | 668 | Object | -2916.02,-540.39,-4888.70 | 308,227,506 | Scale/Radius: 8.00 |
| 139 | `Roid_Med_Green` | 669 | Object | -6164.85,683.15,-4802.30 | 387,273,206 | Scale/Radius: 5.00 |
| 140 | `Roid_Med_Green` | 670 | Object | -5425.02,1341.23,-4530.05 | 307,469,489 | Scale/Radius: 9.00 |
| 141 | `Asteroid_1` | 671 | Object | -2647.04,1766.88,-7244.28 | 90,158,101 | Scale/Radius: 3.00 |
| 142 | `Roid_Med_Green` | 672 | Object | -5781.87,786.29,-4152.75 | 399,67,440 | Scale/Radius: 1.00 |
| 143 | `Asteroid_1` | 673 | Object | -5465.41,843.97,-3039.11 | 309,310,338 | Scale/Radius: 8.00 |
| 144 | `Roid_Med_Green2` | 674 | Object | -3827.84,-672.62,-6880.75 | 203,246,293 | Scale/Radius: 3.00 |
| 145 | `Roid_Med_Green` | 675 | Object | -5430.77,-502.98,-6406.82 | 443,89,222 | Scale/Radius: 2.00 |
| 146 | `Roid_Med_Green2` | 676 | Object | -2239.08,-3416.71,-5138.15 | 165,322,4 | Scale/Radius: 3.00 |
| 147 | `Roid_Med_Green` | 677 | Object | -4920.60,-1194.43,-6928.55 | 343,158,300 | Scale/Radius: 3.00 |
| 148 | `Asteroid_1` | 678 | Object | -4057.42,-3885.93,-7397.46 | 218,21,377 | Scale/Radius: 5.00 |
| 149 | `Roid_Med_Green` | 679 | Object | -3197.11,-1570.90,-3210.05 | 324,31,265 | Scale/Radius: 5.00 |
| 150 | `Roid_XL_Green` | 680 | Object | -5546.13,-1310.52,-6350.69 | 433,130,151 | Scale/Radius: 1.00 |
| 151 | `Asteroid_1` | 681 | Object | -2569.36,-1950.07,-4206.94 | 128,325,230 | Scale/Radius: 9.00 |
| 152 | `Roid_Med_Green2` | 682 | Object | -5724.18,1766.88,-3254.78 | 298,491,151 | Scale/Radius: 9.00 |
| 153 | `Roid_Med_Green` | 683 | Object | -5507.25,2228.34,-5077.66 | 426,59,167 | Scale/Radius: 5.00 |
| 154 | `Roid_Med_Green2` | 684 | Object | -5613.14,-5616.39,-4771.79 | 238,288,488 | Scale/Radius: 6.00 |
| 155 | `Roid_Med_Green2` | 685 | Object | -4157.44,3728.02,-2917.36 | 373,165,152 | Scale/Radius: 6.00 |
| 156 | `Roid_Med_Green` | 686 | Object | -5252.97,-1578.66,-6142.36 | 411,179,91 | Scale/Radius: 2.00 |
| 157 | `Roid_Med_Green2` | 687 | Object | -5795.45,-1559.34,-6264.56 | 19,121,229 | Scale/Radius: 5.00 |
| 158 | `Roid_XL_Green` | 688 | Object | -2321.59,-724.93,-6395.73 | 68,294,483 | Scale/Radius: 5.00 |
| 159 | `Asteroid_1` | 689 | Object | -3769.01,22.88,-7509.71 | 296,52,50 | Scale/Radius: 2.00 |
| 160 | `Roid_Med_Green` | 690 | Object | -4806.28,-1224.12,-3484.82 | 425,399,441 | Scale/Radius: 2.00 |
| 161 | `Asteroid_1` | 691 | Object | -4561.57,-4289.71,-6791.15 | 221,128,280 | Scale/Radius: 3.00 |
| 162 | `Roid_XL_Green` | 692 | Object | -3446.13,-251.98,-3200.30 | 89,294,441 | Scale/Radius: 2.00 |
| 163 | `Roid_Med_Green` | 693 | Object | -4472.10,324.84,-3394.82 | 126,235,106 | Scale/Radius: 4.00 |
| 164 | `Roid_Med_Green2` | 694 | Object | -6016.91,728.61,-4827.91 | 76,82,131 | Scale/Radius: 2.00 |
| 165 | `Roid_Med_Green2` | 695 | Object | -5619.95,-828.80,-5082.40 | 177,136,399 | Scale/Radius: 5.00 |
| 166 | `Roid_XL_Green` | 696 | Object | -5578.59,28.02,-3734.84 | 192,323,77 | Scale/Radius: 6.00 |
| 167 | `Roid_Med_Green` | 697 | Object | -5329.32,-482.71,-4518.07 | 433,357,264 | Scale/Radius: 3.00 |
| 168 | `Roid_Med_Green2` | 698 | Object | -3426.48,2516.75,-2902.38 | 71,317,201 | Scale/Radius: 2.00 |
| 169 | `Roid_Med_Green` | 699 | Object | -2820.09,-425.03,-7132.04 | 43,79,209 | Scale/Radius: 3.00 |
| 170 | `Roid_Med_Green2` | 700 | Object | -5154.44,-5154.93,-3458.67 | 90,206,274 | Scale/Radius: 6.00 |
| 171 | `Roid_Med_Green` | 701 | Object | -2853.74,-1301.15,-5332.36 | 395,83,177 | Scale/Radius: 4.00 |
| 172 | `Roid_Med_Green` | 702 | Object | -5666.50,-1578.66,-3984.38 | 226,141,210 | Scale/Radius: 9.00 |
| 173 | `Asteroid_1` | 703 | Object | -5877.52,-1736.71,-4402.39 | 188,63,242 | Scale/Radius: 1.00 |
| 174 | `Roid_Med_Green2` | 704 | Object | -5217.25,-5385.66,-2664.99 | 76,172,383 | Scale/Radius: 4.00 |
| 175 | `Roid_XL_Green` | 705 | Object | -6310.79,3324.29,-6198.73 | 317,207,278 | Scale/Radius: 1.00 |
| 176 | `Roid_Med_Green` | 706 | Object | -5265.00,-1647.03,-5062.61 | 179,12,97 | Scale/Radius: 5.00 |
| 177 | `Roid_XL_Green` | 707 | Object | -6253.11,-194.30,-5132.40 | 334,136,472 | Scale/Radius: 2.00 |
| 178 | `Roid_XL_Green` | 708 | Object | -2248.87,-782.62,-6647.94 | 196,411,281 | Scale/Radius: 1.00 |
| 179 | `Roid_Med_Green` | 709 | Object | -5247.94,-367.34,-4998.80 | 252,495,267 | Scale/Radius: 2.00 |
| 180 | `Roid_Med_Green` | 710 | Object | -2759.43,3137.70,-3695.49 | 91,161,144 | Scale/Radius: 3.00 |
| 181 | `Roid_Med_Green` | 711 | Object | -4180.46,-1793.75,-4212.44 | 178,287,62 | Scale/Radius: 4.00 |
| 182 | `Roid_Med_Green` | 712 | Object | -3227.95,1478.47,-6377.64 | 464,147,395 | Scale/Radius: 3.00 |
| 183 | `Roid_Med_Green2` | 713 | Object | -4989.70,-2117.34,-4531.20 | 321,325,364 | Scale/Radius: 1.00 |
| 184 | `Roid_Med_Green` | 714 | Object | -2721.42,-309.66,-5996.90 | 327,445,124 | Scale/Radius: 1.00 |
| 185 | `Roid_XL_Green` | 715 | Object | -5030.20,959.34,-3111.18 | 469,199,366 | Scale/Radius: 1.00 |
| 186 | `Asteroid_1` | 716 | Object | -5293.62,-1625.39,-6772.02 | 142,339,126 | Scale/Radius: 1.00 |
| 187 | `Roid_Med_Green2` | 717 | Object | -6028.16,-194.30,-5061.72 | 387,278,60 | Scale/Radius: 4.00 |
| 188 | `Roid_Med_Green` | 718 | Object | -2417.60,1074.70,-4683.64 | 156,430,62 | Scale/Radius: 2.00 |
| 189 | `Roid_Med_Green2` | 719 | Object | -5324.73,1536.16,-4827.91 | 505,89,454 | Scale/Radius: 4.00 |
| 190 | `Roid_Med_Green` | 720 | Object | -5025.29,1017.02,-6645.19 | 393,210,329 | Scale/Radius: 3.00 |
| 191 | `Asteroid_1` | 721 | Object | -6689.81,209.47,-4797.69 | 200,43,353 | Scale/Radius: 7.00 |
| 192 | `Roid_XL_Green` | 722 | Object | -2663.74,-4001.30,-6053.03 | 381,159,508 | Scale/Radius: 4.00 |
| 193 | `Roid_XL_Green` | 723 | Object | -3565.51,2112.97,-4549.43 | 461,47,47 | Scale/Radius: 2.00 |
| 194 | `Asteroid_1` | 724 | Object | -5685.81,-1782.66,-4549.04 | 60,271,366 | Scale/Radius: 2.00 |
| 195 | `Roid_Med_Green` | 725 | Object | -3503.81,-828.80,-3144.18 | 175,416,213 | Scale/Radius: 2.00 |
| 196 | `Roid_Med_Green2` | 726 | Object | -5438.32,-1578.66,-3546.57 | 216,293,226 | Scale/Radius: 6.00 |
| 197 | `Asteroid_1` | 727 | Object | -5085.13,1536.16,-6538.68 | 51,34,6 | Scale/Radius: 1.00 |
| 198 | `Roid_XL_Green` | 728 | Object | -3203.86,-3705.12,-6829.92 | 169,207,185 | Scale/Radius: 1.00 |
| 199 | `Asteroid_1` | 729 | Object | -4239.83,-2059.66,-3969.97 | 233,299,86 | Scale/Radius: 8.00 |
| 200 | `Roid_Med_Green2` | 730 | Object | -4345.87,1939.93,-4414.53 | 166,255,317 | Scale/Radius: 5.00 |
| 201 | `Asteroid_1` | 731 | Object | -4647.88,-1700.30,-3819.47 | 438,33,77 | Scale/Radius: 8.00 |
| 202 | `Roid_Med_Green2` | 732 | Object | -3099.35,-1130.75,-3954.57 | 83,309,191 | Scale/Radius: 4.00 |
| 203 | `Roid_Med_Green` | 733 | Object | -4197.43,48.65,-3581.75 | 438,37,364 | Scale/Radius: 4.00 |
| 204 | `Roid_Med_Green2` | 734 | Object | -4220.34,-1578.66,-2579.11 | 486,493,212 | Scale/Radius: 2.00 |
| 205 | `Roid_XL_Green` | 735 | Object | -3786.86,2343.70,-4338.21 | 329,57,316 | Scale/Radius: 3.00 |
| 206 | `Asteroid_1` | 736 | Object | -2129.19,3266.61,-6872.43 | 134,108,65 | Scale/Radius: 1.00 |
| 207 | `Roid_Med_Green` | 737 | Object | -2083.53,-655.75,-6001.02 | 24,367,360 | Scale/Radius: 9.00 |
| 208 | `Roid_Med_Green` | 738 | Object | -5386.00,-3712.89,-5811.48 | 23,14,331 | Scale/Radius: 1.00 |
| 209 | `Roid_Med_Green` | 739 | Object | -4707.76,-1490.21,-4281.26 | 27,126,365 | Scale/Radius: 1.00 |
| 210 | `Roid_Med_Green2` | 740 | Object | -2146.23,-655.75,-5495.63 | 270,167,314 | Scale/Radius: 5.00 |
| 211 | `Roid_Med_Green` | 741 | Object | -4842.83,747.25,-4233.63 | 40,24,49 | Scale/Radius: 1.00 |
| 212 | `Roid_Med_Green` | 742 | Object | -5931.91,-1311.25,-3254.78 | 185,341,149 | Scale/Radius: 2.00 |
| 213 | `Roid_Med_Green2` | 743 | Object | -4505.45,1882.25,-2971.45 | 352,413,360 | Scale/Radius: 3.00 |
| 214 | `Roid_Med_Green` | 744 | Object | -4418.46,-647.30,-7209.17 | 179,66,372 | Scale/Radius: 9.00 |
| 215 | `Asteroid_1` | 745 | Object | -2558.71,-713.43,-6841.49 | 41,83,412 | Scale/Radius: 1.00 |
| 216 | `Roid_Med_Green` | 746 | Object | -5774.61,-4418.61,-6615.34 | 264,378,33 | Scale/Radius: 1.00 |
| 217 | `Roid_Med_Green2` | 747 | Object | -5768.66,-446.03,-5637.50 | 252,249,271 | Scale/Radius: 5.00 |
| 218 | `Roid_Med_Green2` | 748 | Object | -4669.91,-1108.75,-4169.99 | 23,502,109 | Scale/Radius: 6.00 |
| 219 | `Roid_Med_Green2` | 749 | Object | -2880.27,-3965.50,-3887.70 | 278,356,382 | Scale/Radius: 8.00 |
| 220 | `Roid_Med_Green` | 750 | Object | -4378.78,1247.75,-7321.41 | 343,219,249 | Scale/Radius: 6.00 |
| 221 | `Asteroid_1` | 751 | Object | -3621.39,-1232.57,-3348.10 | 266,320,451 | Scale/Radius: 1.00 |
| 222 | `Asteroid_1` | 752 | Object | -3687.09,1420.79,-3492.20 | 44,301,6 | Scale/Radius: 2.00 |
| 223 | `Asteroid_1` | 753 | Object | -5082.38,-309.66,-3969.97 | 152,266,10 | Scale/Radius: 1.00 |
| 224 | `Roid_Med_Green` | 754 | Object | -5331.09,1827.79,-4118.50 | 76,102,292 | Scale/Radius: 9.00 |
| 225 | `Roid_Med_Green2` | 755 | Object | -4862.74,-1281.80,-3943.54 | 271,142,421 | Scale/Radius: 2.00 |
| 226 | `Roid_Med_Green` | 756 | Object | -4618.40,-1512.53,-3671.78 | 459,231,103 | Scale/Radius: 5.00 |
| 227 | `Roid_Med_Green2` | 757 | Object | -2936.11,856.19,-6971.60 | 376,338,413 | Scale/Radius: 5.00 |
| 228 | `Roid_Med_Green` | 758 | Object | -4438.07,-1290.25,-2603.95 | 266,447,346 | Scale/Radius: 1.00 |
| 229 | `Asteroid_1` | 759 | Object | -4010.81,901.66,-3550.45 | 15,390,300 | Scale/Radius: 5.00 |
| 230 | `Roid_Med_Green2` | 760 | Object | -5964.70,-2213.16,-5581.38 | 357,396,193 | Scale/Radius: 1.00 |
| 231 | `Roid_Med_Green` | 761 | Object | -3869.32,-1867.07,-2721.95 | 133,23,180 | Scale/Radius: 1.00 |
| 232 | `Roid_XL_Green` | 762 | Object | -4804.54,1420.79,-3144.41 | 197,265,272 | Scale/Radius: 1.00 |
| 233 | `Roid_Med_Green` | 763 | Object | -2927.14,-1001.84,-3467.23 | 165,480,97 | Scale/Radius: 9.00 |
| 234 | `Roid_Med_Green` | 764 | Object | -2403.60,-939.71,-5020.38 | 183,77,156 | Scale/Radius: 2.00 |
| 235 | `Asteroid_1` | 765 | Object | -6304.62,3555.02,-3807.31 | 375,333,183 | Scale/Radius: 2.00 |
| 236 | `Roid_Med_Green` | 766 | Object | -5376.31,1305.43,-7009.64 | 402,208,83 | Scale/Radius: 6.00 |
| 237 | `Roid_Med_Green2` | 767 | Object | -4521.91,-3078.39,-6566.89 | 377,281,175 | Scale/Radius: 2.00 |
| 238 | `Roid_Med_Green` | 768 | Object | -2675.66,-1055.07,-5229.79 | 343,219,155 | Scale/Radius: 2.00 |
| 239 | `Roid_Med_Green2` | 769 | Object | -4637.27,-3885.93,-7240.37 | 203,472,113 | Scale/Radius: 6.00 |
| 240 | `Roid_Med_Green` | 770 | Object | -2616.40,-5789.44,-6785.37 | 78,268,397 | Scale/Radius: 1.00 |
| 241 | `Asteroid_1` | 771 | Object | -2916.02,786.29,-5000.94 | 224,370,86 | Scale/Radius: 4.00 |
| 242 | `Roid_Med_Green` | 772 | Object | -3527.64,-1826.25,-3579.48 | 110,52,371 | Scale/Radius: 8.00 |
| 243 | `Roid_Med_Green2` | 773 | Object | -6426.16,1593.84,-5581.38 | 323,217,396 | Scale/Radius: 5.00 |
| 244 | `Roid_Med_Green2` | 774 | Object | -2764.91,2459.07,-4538.78 | 379,174,378 | Scale/Radius: 6.00 |
| 245 | `Roid_Med_Green` | 775 | Object | -5376.99,2632.11,-5642.88 | 222,453,496 | Scale/Radius: 4.00 |
| 246 | `Roid_XL_Green` | 776 | Object | -2880.27,-1232.57,-4426.54 | 370,347,304 | Scale/Radius: 2.00 |
| 247 | `Roid_Med_Green2` | 777 | Object | -6195.43,-2386.21,-5749.75 | 285,24,75 | Scale/Radius: 6.00 |
| 248 | `Asteroid_1` | 778 | Object | -2520.25,-540.39,-4296.41 | 282,391,16 | Scale/Radius: 2.00 |
| 249 | `Roid_Med_Green` | 779 | Object | -2735.83,1247.75,-5052.57 | 399,268,173 | Scale/Radius: 4.00 |
| 250 | `Asteroid_1` | 780 | Object | -4479.24,151.79,-6656.21 | 287,441,468 | Scale/Radius: 2.00 |
| 251 | `Asteroid_1` | 781 | Object | -2351.57,959.34,-5744.47 | 459,315,85 | Scale/Radius: 9.00 |
| 252 | `Roid_Med_Green` | 782 | Object | -3221.06,670.93,-4140.05 | 306,220,449 | Scale/Radius: 8.00 |
| 253 | `Roid_Med_Green2` | 783 | Object | -5793.85,-4693.48,-5181.88 | 134,65,381 | Scale/Radius: 3.00 |
| 254 | `Roid_Med_Green` | 784 | Object | -2882.85,36.43,-3219.83 | 212,506,476 | Scale/Radius: 4.00 |
| 255 | `Roid_Med_Green2` | 785 | Object | -3706.27,-470.49,-3883.13 | 447,83,96 | Scale/Radius: 6.00 |
| 256 | `Asteroid_1` | 786 | Object | -6029.02,-619.07,-6086.66 | 262,282,335 | Scale/Radius: 9.00 |
| 257 | `Roid_Med_Green` | 787 | Object | -3098.49,2286.02,-4576.73 | 401,27,501 | Scale/Radius: 6.00 |
| 258 | `Roid_Med_Green` | 788 | Object | -3792.22,1997.61,-3200.30 | 39,508,491 | Scale/Radius: 3.00 |
| 259 | `Roid_Med_Green` | 789 | Object | -6224.59,-309.66,-4234.66 | 22,392,129 | Scale/Radius: 1.00 |
| 260 | `Roid_Med_Green` | 790 | Object | -6513.00,1017.02,-4290.78 | 265,316,371 | Scale/Radius: 3.00 |
| 261 | `Roid_XL_Green` | 791 | Object | -5030.20,1651.52,-3616.28 | 53,423,235 | Scale/Radius: 2.00 |
| 262 | `Roid_Med_Green2` | 792 | Object | -5791.66,2978.20,-5469.13 | 502,279,178 | Scale/Radius: 4.00 |
| 263 | `Roid_Med_Green` | 793 | Object | -2302.24,-136.62,-6872.43 | 359,96,252 | Scale/Radius: 3.00 |
| 264 | `Asteroid_1` | 794 | Object | -2302.24,2574.43,-7321.41 | 351,149,380 | Scale/Radius: 8.00 |
| 265 | `Roid_Med_Green` | 795 | Object | -3428.54,-2097.80,-3527.78 | 337,230,213 | Scale/Radius: 7.00 |
| 266 | `Roid_Med_Green` | 796 | Object | -6134.67,2459.07,-5232.13 | 320,64,284 | Scale/Radius: 5.00 |
| 267 | `Roid_Med_Green` | 797 | Object | -4188.97,1939.93,-2625.91 | 120,51,399 | Scale/Radius: 5.00 |
| 268 | `Roid_Med_Green2` | 798 | Object | -4010.81,324.84,-3213.71 | 62,116,405 | Scale/Radius: 2.00 |
| 269 | `Asteroid_1` | 799 | Object | -5791.66,2055.29,-6030.36 | 473,506,170 | Scale/Radius: 6.00 |
| 270 | `Roid_Med_Green` | 800 | Object | -5551.14,2286.02,-4096.62 | 449,368,137 | Scale/Radius: 2.00 |
| 271 | `Roid_Med_Green` | 801 | Object | -5957.08,-21.25,-4822.18 | 483,113,98 | Scale/Radius: 2.00 |
| 272 | `Roid_Med_Green` | 802 | Object | -3005.87,-1059.53,-4292.84 | 261,307,408 | Scale/Radius: 1.00 |
| 273 | `Asteroid_1` | 803 | Object | -5145.56,267.16,-4065.27 | 314,480,364 | Scale/Radius: 4.00 |
| 274 | `Roid_Med_Green` | 804 | Object | -2978.74,-1001.84,-3433.35 | 337,426,294 | Scale/Radius: 1.00 |
| 275 | `Roid_Med_Green2` | 805 | Object | -3397.51,3670.38,-7084.92 | 246,45,164 | Scale/Radius: 2.00 |
| 276 | `Roid_Med_Green` | 806 | Object | -5954.91,-1001.84,-4096.62 | 86,111,128 | Scale/Radius: 2.00 |
| 277 | `Roid_Med_Green2` | 807 | Object | -1955.02,-4693.48,-6495.66 | 274,218,276 | Scale/Radius: 9.00 |
| 278 | `Asteroid_1` | 808 | Object | -5431.78,2228.34,-5986.08 | 471,10,269 | Scale/Radius: 5.00 |
| 279 | `Roid_Med_Green2` | 809 | Object | -5424.96,3151.25,-3447.69 | 387,114,315 | Scale/Radius: 2.00 |
| 280 | `Asteroid_1` | 810 | Object | -4799.47,-1636.34,-3616.28 | 388,390,116 | Scale/Radius: 5.00 |
| 281 | `Roid_Med_Green` | 811 | Object | -6282.28,-5270.30,-5076.50 | 41,257,421 | Scale/Radius: 2.00 |
| 282 | `Roid_Med_Green2` | 812 | Object | -2596.36,324.84,-4655.13 | 298,298,397 | Scale/Radius: 4.00 |
| 283 | `Roid_Med_Green` | 813 | Object | -3035.26,-598.07,-4165.93 | 214,335,343 | Scale/Radius: 2.00 |
| 284 | `Asteroid_1` | 814 | Object | -2417.60,1247.75,-4066.29 | 366,283,198 | Scale/Radius: 8.00 |
| 285 | `Roid_Med_Green` | 815 | Object | -2071.51,1478.47,-6928.55 | 339,210,219 | Scale/Radius: 3.00 |
| 286 | `Roid_Med_Green` | 816 | Object | -3609.10,-309.66,-3679.61 | 198,269,147 | Scale/Radius: 4.00 |
| 287 | `Roid_Med_Green2` | 817 | Object | -6486.67,2862.84,-3751.42 | 68,390,75 | Scale/Radius: 2.00 |
| 288 | `Roid_Med_Green` | 818 | Object | -5420.98,3439.66,-4942.68 | 31,67,156 | Scale/Radius: 6.00 |
| 289 | `Roid_Med_Green` | 819 | Object | -4312.22,-828.80,-3269.81 | 323,53,425 | Scale/Radius: 5.00 |
| 290 | `Roid_Med_Green2` | 820 | Object | -4972.51,2459.07,-3279.55 | 156,311,60 | Scale/Radius: 4.00 |
| 291 | `Asteroid_1` | 821 | Object | -6391.32,-1121.03,-5076.50 | 328,212,361 | Scale/Radius: 9.00 |
| 292 | `Roid_Med_Green2` | 822 | Object | -3215.55,2805.16,-3579.48 | 172,299,66 | Scale/Radius: 2.00 |
| 293 | `Roid_Med_Green2` | 823 | Object | -4616.75,1593.84,-3542.23 | 49,196,316 | Scale/Radius: 9.00 |
| 294 | `Asteroid_1` | 824 | Object | -6358.62,-4542.31,-4594.57 | 288,94,397 | Scale/Radius: 9.00 |
| 295 | `Roid_Med_Green` | 825 | Object | -5526.35,2747.47,-6715.90 | 398,448,484 | Scale/Radius: 4.00 |
| 296 | `Roid_Med_Green` | 826 | Object | -6455.32,-309.66,-4346.90 | 168,479,403 | Scale/Radius: 1.00 |
| 297 | `Roid_XL_Green` | 827 | Object | -5316.31,3958.79,-5324.12 | 105,154,344 | Scale/Radius: 3.00 |
| 298 | `Asteroid_1` | 828 | Object | -2318.12,-1244.07,-5438.06 | 499,345,447 | Scale/Radius: 1.00 |
| 299 | `Roid_Med_Green2` | 829 | Object | -5987.08,3901.11,-3023.01 | 113,411,81 | Scale/Radius: 1.00 |
| 300 | `Roid_Med_Green` | 830 | Object | -3958.25,-1751.71,-2682.03 | 26,176,161 | Scale/Radius: 6.00 |
| 301 | `Roid_Med_Green2` | 831 | Object | -4663.83,-1982.43,-2783.33 | 130,480,488 | Scale/Radius: 1.00 |
| 302 | `Roid_Med_Green` | 832 | Object | -2707.22,-540.39,-4538.78 | 354,162,348 | Scale/Radius: 1.00 |
| 303 | `Asteroid_1` | 833 | Object | -3205.95,36.43,-2999.59 | 498,50,143 | Scale/Radius: 8.00 |
| 304 | `Roid_Med_Green` | 834 | Object | -4900.51,-6462.98,-4121.39 | 357,53,511 | Scale/Radius: 6.00 |
| 305 | `Roid_XL_Green` | 835 | Object | -3266.90,-1809.39,-3917.16 | 88,334,168 | Scale/Radius: 2.00 |
| 306 | `Roid_Med_Green` | 836 | Object | -3525.66,-4635.80,-7224.53 | 348,495,379 | Scale/Radius: 9.00 |
| 307 | `Roid_Med_Green2` | 837 | Object | -3391.01,-194.30,-4693.41 | 284,85,243 | Scale/Radius: 3.00 |
| 308 | `Roid_Med_Green2` | 838 | Object | -3054.90,-4001.30,-6040.91 | 74,256,365 | Scale/Radius: 8.00 |
| 309 | `Roid_XL_Green` | 839 | Object | -6368.47,-3136.07,-6030.36 | 411,84,180 | Scale/Radius: 2.00 |
| 310 | `Roid_Med_Green2` | 840 | Object | -6012.59,-771.12,-3647.64 | 148,182,56 | Scale/Radius: 2.00 |
| 311 | `Roid_Med_Green2` | 842 | Object | -6536.05,-1578.66,-5467.68 | 244,306,224 | Scale/Radius: 1.00 |
| 312 | `Asteroid_1` | 843 | Object | -2359.92,1074.70,-7096.92 | 103,53,120 | Scale/Radius: 4.00 |
| 313 | `Pirate_Mine_HvyLaser` | 850 | Interactive | -4428.01,-743.56,-5001.57 | 0,0,0 | group/role: FG_ANVIL / 0 |
| 314 | `Pirate_Mine_HvyLaser` | 859 | Interactive | -3334.59,-159.01,-5302.39 | 0,0,0 | group/role: FG_ANVIL / 0 |
| 315 | `Pirate_Mine_HvyLaser` | 864 | Interactive | -3895.10,-652.41,-4728.58 | 0,0,0 | group/role: FG_ANVIL / 0 |
| 316 | `Pirate_Mine_HvyLaser` | 867 | Interactive | -4996.33,-644.41,-6117.38 | 0,0,0 | group/role: FG_ANVIL / 0 |
| 317 | `Pirate_Mine_HvyLaser` | 868 | Interactive | -4173.48,-146.63,-6593.56 | 0,0,0 | group/role: FG_ANVIL / 0 |
| 318 | `Pirate_Mine_HvyLaser` | 875 | Interactive | -3395.74,-809.13,-5910.92 | 0,0,0 | group/role: FG_ANVIL / 0 |
| 319 | `Pirate_Mine_HvyLaser` | 877 | Interactive | -5125.26,-139.13,-5425.93 | 0,0,0 | group/role: FG_ANVIL / 0 |
| 320 | `Pirate_Mine_HvyLaser` | 922 | Interactive | -4219.84,104.00,-6000.83 | 0,0,0 | group/role: FG_ANVIL / 0 |
| 321 | `Satellite` | 927 | Interactive | -4135.46,-377.00,-5786.17 | 0,0,0 | None |
| 322 | `Spcargo_Parts` | 930 | Interactive | -4649.58,-557.42,-6269.63 | 0,0,0 | secondary groups: CONT_060, none |
| 323 | `Retribution_Shipyard` | 917 | Interactive | -4203.44,-60.00,-5651.82 | 435,0,0 | secondary groups: none, RETRIBUTION |
| 324 | `Mad_Pirate_Platform` | 926 | Interactive | -3348.56,-58.50,-6268.93 | 435,0,0 | None |
