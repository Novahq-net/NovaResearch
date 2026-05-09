# Tachyon: The Fringe BORA03.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `BORA03.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `BORA3.BDF` |
| Region | 3 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 6 |
| Entities | 421 |
| Events | 1 |
| Waypoints | 0 |
| Child Sectors | 2 |
| Scripts | 0 |
| Scenes | 1 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Space_Station`, `1: Asteroid_2`, `2: Roid_Sm_Brown`, `3: Roid_Sm_Brown2`, `4: Mega_Gate`, `5: Hyper_Gate` |
| Scripts | None |
| Scenes | `B3BC040A.SEN` |
| Labels | `CHAAS`, `ORPHS` |
| Aliases | `frank01`, `frank02`, `frank03`, `frank04` |
| Groups | `VALIANCE` |
| Child Sectors | [bora03A.spx](BORA03A.md), [bora03B.spx](BORA03B.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 0

**Action**

- Gate state/action: param 6, subtype 3, param 0
- Gate state/action: param 7, subtype 3, param 0

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 5 | Gate | -2371.58,0.00,2071.75 | 203,0,0 | Gate SPX: [bora02.spx](BORA02.md) |
| 1 | `Mega_Gate` | 6 | Gate | 2594.92,0.00,3257.06 | 329,0,0 | Gate SPX: [fron01.spx](FRON01.md) |
| 2 | `Mega_Gate` | 7 | Gate | 2590.13,0.00,-2702.51 | 0,0,0 | Gate SPX: [neut03.spx](NEUT03.md) |
| 3 | `Roid_Sm_Brown2` | 287 | Object | -3936.71,739.07,2791.51 | 101,397,458 | Scale/Radius: 5.00 |
| 4 | `Roid_Sm_Brown` | 289 | Object | -4017.55,-531.18,2895.44 | 454,396,236 | Scale/Radius: 6.00 |
| 5 | `Roid_Sm_Brown2` | 296 | Object | -800.66,-754.87,-2551.81 | 391,177,336 | Scale/Radius: 2.00 |
| 6 | `Roid_Sm_Brown` | 298 | Object | -3737.38,461.92,3039.84 | 473,128,109 | Scale/Radius: 2.00 |
| 7 | `Roid_Sm_Brown2` | 305 | Object | -3936.71,577.40,2860.80 | 147,324,101 | Scale/Radius: 6.00 |
| 8 | `Roid_Sm_Brown` | 307 | Object | -425.63,212.08,-1687.86 | 0,453,112 | Scale/Radius: 9.00 |
| 9 | `Roid_Sm_Brown` | 325 | Object | -4743.69,481.16,2419.43 | 81,184,301 | Scale/Radius: 2.00 |
| 10 | `Roid_Sm_Brown2` | 341 | Object | -4865.48,192.47,981.66 | 311,404,44 | Scale/Radius: 4.00 |
| 11 | `Roid_Sm_Brown2` | 350 | Object | -4543.45,-211.71,-476.02 | 251,56,44 | Scale/Radius: 8.00 |
| 12 | `Roid_Sm_Brown` | 352 | Object | -3628.12,-596.62,3494.50 | 445,114,134 | Scale/Radius: 7.00 |
| 13 | `Roid_Sm_Brown2` | 359 | Object | -4866.87,-615.89,1803.54 | 47,433,99 | Scale/Radius: 6.00 |
| 14 | `Roid_Sm_Brown` | 361 | Object | -4020.02,519.66,2727.37 | 441,297,317 | Scale/Radius: 1.00 |
| 15 | `Roid_Sm_Brown` | 366 | Object | 2426.29,-404.18,4079.85 | 347,56,24 | Scale/Radius: 4.00 |
| 16 | `Roid_Sm_Brown` | 373 | Object | -2864.40,76.99,3351.02 | 239,94,445 | Scale/Radius: 6.00 |
| 17 | `Roid_Sm_Brown2` | 378 | Object | 2541.77,904.59,4156.83 | 468,261,243 | Scale/Radius: 3.00 |
| 18 | `Roid_Sm_Brown2` | 385 | Object | 78.27,-442.67,4054.58 | 129,231,13 | Scale/Radius: 6.00 |
| 19 | `Roid_Sm_Brown` | 394 | Object | -2404.53,731.37,3765.88 | 82,297,107 | Scale/Radius: 4.00 |
| 20 | `Roid_Sm_Brown2` | 399 | Object | -2462.27,-577.40,3727.39 | 16,91,133 | Scale/Radius: 9.00 |
| 21 | `Roid_Sm_Brown` | 401 | Object | -2404.53,96.23,4227.80 | 346,441,128 | Scale/Radius: 7.00 |
| 22 | `Asteroid_2` | 641 | Object | -1709.09,-45.73,4312.46 | 468,250,303 | Scale/Radius: 6.00 |
| 23 | `Asteroid_2` | 643 | Object | -804.50,-37.42,4485.68 | 252,226,161 | Scale/Radius: 2.00 |
| 24 | `Asteroid_2` | 645 | Object | -939.23,39.49,4751.29 | 381,404,195 | Scale/Radius: 3.00 |
| 25 | `Asteroid_2` | 647 | Object | -842.99,-60.28,4139.25 | 255,173,195 | Scale/Radius: 3.00 |
| 26 | `Asteroid_2` | 649 | Object | -1478.13,37.42,3977.57 | 387,68,357 | Scale/Radius: 1.00 |
| 27 | `Asteroid_2` | 653 | Object | -2382.72,45.73,4254.72 | 50,11,12 | Scale/Radius: 2.00 |
| 28 | `Asteroid_2` | 655 | Object | -1824.57,33.26,4947.60 | 488,393,2 | Scale/Radius: 3.00 |
| 29 | `Asteroid_2` | 657 | Object | -1170.18,-93.54,4277.82 | 436,500,263 | Scale/Radius: 7.00 |
| 30 | `Asteroid_2` | 659 | Object | -2344.22,-58.20,3815.90 | 171,362,209 | Scale/Radius: 1.00 |
| 31 | `Asteroid_2` | 661 | Object | -2498.19,-16.63,3977.57 | 395,280,338 | Scale/Radius: 3.00 |
| 32 | `Asteroid_2` | 663 | Object | -1247.17,95.62,4889.86 | 448,134,229 | Scale/Radius: 6.00 |
| 33 | `Asteroid_2` | 665 | Object | -3124.10,31.18,3632.65 | 287,25,155 | Scale/Radius: 9.00 |
| 34 | `Asteroid_2` | 667 | Object | -1555.11,-101.85,4912.96 | 330,493,426 | Scale/Radius: 3.00 |
| 35 | `Asteroid_2` | 669 | Object | -2421.21,101.85,4266.27 | 75,225,109 | Scale/Radius: 9.00 |
| 36 | `Asteroid_2` | 671 | Object | -2209.50,-83.14,4832.12 | 151,115,403 | Scale/Radius: 4.00 |
| 37 | `Asteroid_2` | 673 | Object | -2113.26,74.83,4820.57 | 481,507,77 | Scale/Radius: 8.00 |
| 38 | `Asteroid_2` | 675 | Object | -2690.66,72.75,4231.63 | 72,9,317 | Scale/Radius: 5.00 |
| 39 | `Asteroid_2` | 677 | Object | -3797.73,-78.99,3182.28 | 85,58,80 | Scale/Radius: 5.00 |
| 40 | `Asteroid_2` | 679 | Object | -3470.54,-37.42,3540.27 | 123,267,99 | Scale/Radius: 8.00 |
| 41 | `Asteroid_2` | 681 | Object | -3374.30,-87.30,4106.12 | 348,154,342 | Scale/Radius: 4.00 |
| 42 | `Asteroid_2` | 683 | Object | -1073.95,12.47,4289.37 | 116,222,386 | Scale/Radius: 1.00 |
| 43 | `Asteroid_2` | 685 | Object | -2478.95,95.62,4497.23 | 31,197,485 | Scale/Radius: 8.00 |
| 44 | `Asteroid_2` | 687 | Object | -1131.69,-272.50,4472.49 | 354,75,9 | Scale/Radius: 9.00 |
| 45 | `Asteroid_2` | 689 | Object | -1689.84,99.77,4936.05 | 139,410,480 | Scale/Radius: 6.00 |
| 46 | `Asteroid_2` | 691 | Object | -2171.00,-12.47,4127.70 | 476,499,213 | Scale/Radius: 2.00 |
| 47 | `Asteroid_2` | 693 | Object | -2517.44,-87.30,3896.74 | 11,429,120 | Scale/Radius: 5.00 |
| 48 | `Asteroid_2` | 695 | Object | -1362.65,-10.39,3885.19 | 474,47,63 | Scale/Radius: 5.00 |
| 49 | `Asteroid_2` | 699 | Object | -2713.18,81.07,4434.68 | 302,290,325 | Scale/Radius: 7.00 |
| 50 | `Asteroid_2` | 701 | Object | -2344.22,-31.18,4404.85 | 179,21,355 | Scale/Radius: 8.00 |
| 51 | `Asteroid_2` | 703 | Object | -2739.17,47.81,3574.91 | 414,21,437 | Scale/Radius: 2.00 |
| 52 | `Asteroid_2` | 705 | Object | -1324.16,85.22,4855.22 | 246,467,498 | Scale/Radius: 9.00 |
| 53 | `Asteroid_2` | 707 | Object | -1285.66,103.93,4023.77 | 57,164,483 | Scale/Radius: 5.00 |
| 54 | `Asteroid_2` | 709 | Object | -2286.48,449.68,4537.38 | 103,499,446 | Scale/Radius: 7.00 |
| 55 | `Asteroid_2` | 711 | Object | -1574.36,16.63,4150.79 | 243,510,475 | Scale/Radius: 3.00 |
| 56 | `Asteroid_2` | 713 | Object | -2536.69,-37.42,4173.89 | 201,172,239 | Scale/Radius: 4.00 |
| 57 | `Asteroid_2` | 715 | Object | -977.72,-62.36,4289.37 | 253,305,182 | Scale/Radius: 2.00 |
| 58 | `Asteroid_2` | 717 | Object | -2267.24,72.75,3966.03 | 48,71,73 | Scale/Radius: 7.00 |
| 59 | `Asteroid_2` | 719 | Object | -2555.93,103.93,3919.84 | 133,335,12 | Scale/Radius: 1.00 |
| 60 | `Asteroid_2` | 721 | Object | -2478.95,-18.71,4531.87 | 454,455,147 | Scale/Radius: 5.00 |
| 61 | `Asteroid_2` | 723 | Object | -1824.57,0.00,3827.45 | 418,497,415 | Scale/Radius: 1.00 |
| 62 | `Asteroid_2` | 725 | Object | -1208.68,35.34,3954.48 | 122,135,33 | Scale/Radius: 4.00 |
| 63 | `Asteroid_2` | 727 | Object | -2151.76,-4.16,4889.86 | 0,299,32 | Scale/Radius: 1.00 |
| 64 | `Asteroid_2` | 729 | Object | -1728.33,47.81,4335.56 | 53,327,281 | Scale/Radius: 4.00 |
| 65 | `Asteroid_2` | 731 | Object | -1381.90,62.36,3919.84 | 42,73,229 | Scale/Radius: 9.00 |
| 66 | `Asteroid_2` | 735 | Object | -4390.63,127.03,1484.32 | 320,50,233 | Scale/Radius: 3.00 |
| 67 | `Asteroid_2` | 739 | Object | -5175.88,184.77,1214.87 | 432,247,160 | Scale/Radius: 6.00 |
| 68 | `Asteroid_2` | 741 | Object | -4413.72,-123.18,1465.07 | 85,20,157 | Scale/Radius: 9.00 |
| 69 | `Asteroid_2` | 743 | Object | -4494.56,-42.34,2427.40 | 357,511,88 | Scale/Radius: 7.00 |
| 70 | `Asteroid_2` | 745 | Object | -4448.37,-157.82,2254.18 | 94,47,226 | Scale/Radius: 1.00 |
| 71 | `Asteroid_2` | 749 | Object | -5014.21,130.88,1773.02 | 502,120,417 | Scale/Radius: 9.00 |
| 72 | `Asteroid_2` | 755 | Object | -4944.93,-80.84,2311.92 | 445,226,342 | Scale/Radius: 7.00 |
| 73 | `Asteroid_2` | 757 | Object | -4817.90,42.34,2388.90 | 363,226,109 | Scale/Radius: 2.00 |
| 74 | `Asteroid_2` | 759 | Object | -4413.72,-15.40,2985.55 | 285,504,377 | Scale/Radius: 8.00 |
| 75 | `Asteroid_2` | 761 | Object | -5175.88,61.59,1445.83 | 301,13,460 | Scale/Radius: 8.00 |
| 76 | `Asteroid_2` | 763 | Object | -4540.75,119.33,2234.93 | 104,485,95 | Scale/Radius: 9.00 |
| 77 | `Asteroid_2` | 765 | Object | -4540.75,-130.88,1426.58 | 360,110,175 | Scale/Radius: 2.00 |
| 78 | `Asteroid_2` | 767 | Object | -4540.75,80.84,1503.56 | 284,174,400 | Scale/Radius: 5.00 |
| 79 | `Asteroid_2` | 769 | Object | -5233.62,-119.33,1426.58 | 113,93,459 | Scale/Radius: 4.00 |
| 80 | `Asteroid_2` | 771 | Object | -4679.32,88.53,1830.76 | 401,443,495 | Scale/Radius: 1.00 |
| 81 | `Asteroid_2` | 773 | Object | -4875.64,146.27,1561.30 | 281,313,184 | Scale/Radius: 1.00 |
| 82 | `Asteroid_2` | 775 | Object | -4748.61,150.12,1888.50 | 261,25,70 | Scale/Radius: 9.00 |
| 83 | `Asteroid_2` | 779 | Object | -4367.53,73.14,2947.05 | 433,151,17 | Scale/Radius: 2.00 |
| 84 | `Asteroid_2` | 781 | Object | -4737.06,61.59,2408.15 | 275,314,240 | Scale/Radius: 1.00 |
| 85 | `Asteroid_2` | 783 | Object | -4644.68,115.48,1195.62 | 347,371,409 | Scale/Radius: 3.00 |
| 86 | `Asteroid_2` | 785 | Object | -4910.28,0.00,1484.32 | 211,232,28 | Scale/Radius: 7.00 |
| 87 | `Asteroid_2` | 787 | Object | -4517.65,-123.18,2812.33 | 184,230,441 | Scale/Radius: 4.00 |
| 88 | `Asteroid_2` | 791 | Object | -4483.01,65.44,2119.45 | 15,343,107 | Scale/Radius: 7.00 |
| 89 | `Asteroid_2` | 793 | Object | -5037.31,65.44,1503.56 | 180,79,223 | Scale/Radius: 1.00 |
| 90 | `Asteroid_2` | 795 | Object | -5083.50,76.99,2215.69 | 438,311,78 | Scale/Radius: 2.00 |
| 91 | `Asteroid_2` | 797 | Object | -4252.05,84.68,2696.85 | 449,80,400 | Scale/Radius: 6.00 |
| 92 | `Asteroid_2` | 799 | Object | -4540.75,138.57,1830.76 | 326,196,452 | Scale/Radius: 9.00 |
| 93 | `Asteroid_2` | 803 | Object | -5175.88,30.79,1676.78 | 293,45,152 | Scale/Radius: 1.00 |
| 94 | `Asteroid_2` | 805 | Object | -4286.70,65.44,1715.28 | 369,182,166 | Scale/Radius: 4.00 |
| 95 | `Asteroid_2` | 813 | Object | -4344.44,-53.89,2138.70 | 448,283,98 | Scale/Radius: 6.00 |
| 96 | `Asteroid_2` | 815 | Object | -4725.52,61.59,1580.55 | 298,403,424 | Scale/Radius: 8.00 |
| 97 | `Asteroid_2` | 817 | Object | 731.35,-84.68,4228.26 | 241,286,201 | Scale/Radius: 7.00 |
| 98 | `Asteroid_2` | 819 | Object | 1404.92,188.62,4977.20 | 351,278,183 | Scale/Radius: 6.00 |
| 99 | `Asteroid_2` | 821 | Object | 2386.49,-53.89,4700.05 | 350,111,113 | Scale/Radius: 5.00 |
| 100 | `Asteroid_2` | 823 | Object | 577.38,-84.68,3881.82 | 204,324,220 | Scale/Radius: 3.00 |
| 101 | `Asteroid_2` | 827 | Object | 134.71,80.84,3928.01 | 164,434,466 | Scale/Radius: 2.00 |
| 102 | `Asteroid_2` | 829 | Object | 2213.27,-157.82,4596.12 | 363,184,58 | Scale/Radius: 2.00 |
| 103 | `Asteroid_2` | 831 | Object | 250.19,-11.55,4747.91 | 341,77,467 | Scale/Radius: 8.00 |
| 104 | `Asteroid_2` | 833 | Object | 1712.86,69.29,4226.58 | 110,385,40 | Scale/Radius: 7.00 |
| 105 | `Asteroid_2` | 835 | Object | 2040.05,-188.62,4757.79 | 495,245,50 | Scale/Radius: 4.00 |
| 106 | `Asteroid_2` | 837 | Object | 1943.82,-264.27,4240.88 | 431,26,228 | Scale/Radius: 6.00 |
| 107 | `Asteroid_2` | 839 | Object | 2213.27,-88.53,4295.87 | 169,269,173 | Scale/Radius: 2.00 |
| 108 | `Asteroid_2` | 841 | Object | 2059.30,15.40,4607.66 | 440,167,228 | Scale/Radius: 2.00 |
| 109 | `Asteroid_2` | 843 | Object | 635.12,-111.63,4563.15 | 466,314,48 | Scale/Radius: 7.00 |
| 110 | `Asteroid_2` | 845 | Object | 2463.48,53.89,4111.10 | 31,472,431 | Scale/Radius: 1.00 |
| 111 | `Asteroid_2` | 849 | Object | 2078.55,-84.68,4191.94 | 207,410,208 | Scale/Radius: 7.00 |
| 112 | `Asteroid_2` | 851 | Object | -258.12,-50.04,4607.86 | 421,369,366 | Scale/Radius: 7.00 |
| 113 | `Asteroid_2` | 853 | Object | 1366.43,19.25,4757.79 | 384,64,65 | Scale/Radius: 6.00 |
| 114 | `Asteroid_2` | 855 | Object | -277.37,15.40,4550.12 | 390,39,415 | Scale/Radius: 9.00 |
| 115 | `Asteroid_2` | 857 | Object | 2405.74,19.25,4330.51 | 366,435,153 | Scale/Radius: 7.00 |
| 116 | `Asteroid_2` | 859 | Object | 76.97,327.52,4983.82 | 122,456,239 | Scale/Radius: 7.00 |
| 117 | `Asteroid_2` | 861 | Object | -354.35,169.37,4619.41 | 429,399,280 | Scale/Radius: 8.00 |
| 118 | `Asteroid_2` | 863 | Object | 596.62,15.40,4828.75 | 114,286,73 | Scale/Radius: 9.00 |
| 119 | `Asteroid_2` | 865 | Object | 1578.14,-184.77,4088.01 | 314,490,425 | Scale/Radius: 3.00 |
| 120 | `Asteroid_2` | 867 | Object | 365.66,-146.27,4031.94 | 22,476,248 | Scale/Radius: 4.00 |
| 121 | `Asteroid_2` | 869 | Object | 2097.79,-30.79,4492.18 | 64,427,449 | Scale/Radius: 5.00 |
| 122 | `Asteroid_2` | 871 | Object | 1943.82,-150.12,3984.08 | 256,490,78 | Scale/Radius: 1.00 |
| 123 | `Asteroid_2` | 873 | Object | 654.36,23.10,4551.60 | 473,223,400 | Scale/Radius: 2.00 |
| 124 | `Asteroid_2` | 875 | Object | 2367.25,130.88,4573.02 | 300,391,337 | Scale/Radius: 7.00 |
| 125 | `Asteroid_2` | 877 | Object | 384.91,84.68,4771.01 | 228,150,438 | Scale/Radius: 2.00 |
| 126 | `Asteroid_2` | 879 | Object | 2348.00,80.84,4676.95 | 463,413,249 | Scale/Radius: 3.00 |
| 127 | `Asteroid_2` | 881 | Object | 134.71,299.11,4841.40 | 166,36,110 | Scale/Radius: 5.00 |
| 128 | `Asteroid_2` | 883 | Object | 96.21,-100.08,4921.13 | 447,107,510 | Scale/Radius: 9.00 |
| 129 | `Asteroid_2` | 885 | Object | 269.43,69.29,4955.78 | 431,453,422 | Scale/Radius: 3.00 |
| 130 | `Asteroid_2` | 887 | Object | -623.80,-173.22,4861.92 | 118,98,127 | Scale/Radius: 2.00 |
| 131 | `Asteroid_2` | 889 | Object | 211.69,-173.22,4724.82 | 448,466,184 | Scale/Radius: 7.00 |
| 132 | `Asteroid_2` | 891 | Object | 1828.34,150.12,4111.10 | 346,361,143 | Scale/Radius: 3.00 |
| 133 | `Asteroid_2` | 893 | Object | 1674.37,-7.70,4399.80 | 357,367,259 | Scale/Radius: 6.00 |
| 134 | `Asteroid_2` | 895 | Object | 538.88,-26.95,3916.46 | 318,338,100 | Scale/Radius: 1.00 |
| 135 | `Asteroid_2` | 897 | Object | 538.88,23.10,4990.42 | 41,245,135 | Scale/Radius: 3.00 |
| 136 | `Asteroid_2` | 899 | Object | -4756.97,-40.65,945.14 | 53,217,151 | Scale/Radius: 8.00 |
| 137 | `Asteroid_2` | 905 | Object | -5126.50,-57.59,-35.66 | 126,142,329 | Scale/Radius: 2.00 |
| 138 | `Asteroid_2` | 909 | Object | -4780.07,18.63,235.94 | 501,364,133 | Scale/Radius: 6.00 |
| 139 | `Asteroid_2` | 911 | Object | -5011.02,74.52,-126.20 | 323,511,402 | Scale/Radius: 3.00 |
| 140 | `Asteroid_2` | 915 | Object | -4491.37,22.02,-307.27 | 203,339,11 | Scale/Radius: 9.00 |
| 141 | `Asteroid_2` | 917 | Object | -4872.45,33.87,869.69 | 379,457,19 | Scale/Radius: 9.00 |
| 142 | `Asteroid_2` | 923 | Object | -4537.56,47.42,190.68 | 32,496,150 | Scale/Radius: 2.00 |
| 143 | `Asteroid_2` | 927 | Object | -4849.35,-16.94,552.82 | 140,463,510 | Scale/Radius: 9.00 |
| 144 | `Asteroid_2` | 929 | Object | -4884.00,-79.94,-44.46 | 442,183,180 | Scale/Radius: 8.00 |
| 145 | `Asteroid_2` | 931 | Object | -4826.26,-66.05,160.50 | 265,172,168 | Scale/Radius: 2.00 |
| 146 | `Asteroid_2` | 933 | Object | -4687.68,71.14,160.50 | 120,27,177 | Scale/Radius: 3.00 |
| 147 | `Asteroid_2` | 935 | Object | -4502.92,-81.30,417.02 | 334,307,214 | Scale/Radius: 4.00 |
| 148 | `Asteroid_2` | 939 | Object | -5091.86,-3.39,567.91 | 151,219,110 | Scale/Radius: 2.00 |
| 149 | `Asteroid_2` | 941 | Object | -5149.60,-59.28,417.02 | 111,142,213 | Scale/Radius: 4.00 |
| 150 | `Asteroid_2` | 945 | Object | -5184.24,1.69,930.05 | 96,193,383 | Scale/Radius: 1.00 |
| 151 | `Asteroid_2` | 947 | Object | -4641.49,-69.44,160.50 | 372,59,262 | Scale/Radius: 6.00 |
| 152 | `Asteroid_2` | 949 | Object | -4803.16,-76.22,281.21 | 282,502,271 | Scale/Radius: 4.00 |
| 153 | `Asteroid_2` | 953 | Object | -5126.50,-1.69,235.94 | 22,32,290 | Scale/Radius: 1.00 |
| 154 | `Asteroid_2` | 957 | Object | -4618.40,52.50,884.78 | 478,251,325 | Scale/Radius: 8.00 |
| 155 | `Asteroid_2` | 959 | Object | -5045.67,72.83,281.21 | 506,447,337 | Scale/Radius: 5.00 |
| 156 | `Asteroid_2` | 967 | Object | -4526.01,-60.97,220.85 | 82,317,373 | Scale/Radius: 5.00 |
| 157 | `Asteroid_2` | 971 | Object | -3317.78,-11.09,3103.37 | 123,115,117 | Scale/Radius: 1.00 |
| 158 | `Asteroid_2` | 973 | Object | -2826.10,-63.74,3503.21 | 466,15,380 | Scale/Radius: 8.00 |
| 159 | `Asteroid_2` | 975 | Object | -3529.10,-33.26,3700.01 | 96,306,364 | Scale/Radius: 9.00 |
| 160 | `Asteroid_2` | 977 | Object | -565.77,-868.35,-2163.16 | 195,274,41 | Scale/Radius: 10.00 |
| 161 | `Asteroid_2` | 979 | Object | -190.07,-889.13,-2220.90 | 293,155,156 | Scale/Radius: 5.00 |
| 162 | `Asteroid_2` | 981 | Object | -612.73,-904.38,-2028.43 | 22,337,57 | Scale/Radius: 2.00 |
| 163 | `Asteroid_2` | 983 | Object | -166.59,-876.66,-1893.71 | 69,434,69 | Scale/Radius: 4.00 |
| 164 | `Asteroid_2` | 985 | Object | -3180.64,5.54,2921.59 | 94,433,299 | Scale/Radius: 9.00 |
| 165 | `Asteroid_2` | 987 | Object | -577.51,-901.60,-1874.46 | 235,223,381 | Scale/Radius: 1.00 |
| 166 | `Asteroid_2` | 989 | Object | -166.59,-914.08,-2086.17 | 428,349,222 | Scale/Radius: 3.00 |
| 167 | `Asteroid_2` | 991 | Object | -3223.85,455.09,3526.79 | 373,160,78 | Scale/Radius: 5.00 |
| 168 | `Asteroid_2` | 993 | Object | -2.23,-904.38,-2259.39 | 379,441,120 | Scale/Radius: 4.00 |
| 169 | `Asteroid_2` | 995 | Object | -3505.62,-22.17,3276.59 | 437,90,3 | Scale/Radius: 2.00 |
| 170 | `Asteroid_2` | 999 | Object | -225.29,-869.73,-1932.20 | 489,116,44 | Scale/Radius: 6.00 |
| 171 | `Asteroid_2` | 1003 | Object | -3284.43,805.92,3372.82 | 464,468,100 | Scale/Radius: 8.00 |
| 172 | `Asteroid_2` | 1005 | Object | -2837.84,52.66,3637.93 | 220,93,443 | Scale/Radius: 7.00 |
| 173 | `Asteroid_2` | 1007 | Object | -342.70,-882.20,-2471.10 | 2,14,391 | Scale/Radius: 6.00 |
| 174 | `Asteroid_2` | 1009 | Object | -190.07,-858.65,-1797.47 | 324,375,19 | Scale/Radius: 6.00 |
| 175 | `Asteroid_2` | 1011 | Object | -3145.42,55.43,3325.77 | 24,211,257 | Scale/Radius: 8.00 |
| 176 | `Asteroid_2` | 1013 | Object | -13.97,-883.59,-2066.93 | 131,311,384 | Scale/Radius: 6.00 |
| 177 | `Asteroid_2` | 1015 | Object | -3197.32,-581.44,3411.31 | 170,248,7 | Scale/Radius: 6.00 |
| 178 | `Asteroid_2` | 1017 | Object | -84.41,-796.29,-2413.36 | 96,22,164 | Scale/Radius: 8.00 |
| 179 | `Asteroid_2` | 1019 | Object | -3274.56,-51.27,3306.52 | 289,263,118 | Scale/Radius: 1.00 |
| 180 | `Asteroid_2` | 1021 | Object | -107.89,-860.03,-2317.13 | 71,270,368 | Scale/Radius: 3.00 |
| 181 | `Asteroid_2` | 1023 | Object | -178.33,-912.69,-2278.64 | 492,498,386 | Scale/Radius: 1.00 |
| 182 | `Asteroid_2` | 1025 | Object | -659.69,-875.28,-2336.38 | 146,353,244 | Scale/Radius: 3.00 |
| 183 | `Asteroid_2` | 1027 | Object | -3212.11,65.13,3276.59 | 437,6,287 | Scale/Radius: 4.00 |
| 184 | `Asteroid_2` | 1029 | Object | -3259.07,-6.93,3199.60 | 345,366,20 | Scale/Radius: 1.00 |
| 185 | `Asteroid_2` | 1031 | Object | -3517.36,42.96,3834.74 | 167,468,380 | Scale/Radius: 1.00 |
| 186 | `Asteroid_2` | 1035 | Object | -565.77,-860.03,-1797.47 | 408,102,475 | Scale/Radius: 5.00 |
| 187 | `Asteroid_2` | 1037 | Object | -3223.85,69.29,3026.38 | 290,229,465 | Scale/Radius: 2.00 |
| 188 | `Asteroid_2` | 1039 | Object | -3274.56,41.57,3094.81 | 336,438,194 | Scale/Radius: 3.00 |
| 189 | `Asteroid_2` | 1041 | Object | -683.17,-836.47,-2066.93 | 203,116,118 | Scale/Radius: 8.00 |
| 190 | `Asteroid_2` | 1043 | Object | -3353.00,-66.52,3180.35 | 59,24,277 | Scale/Radius: 4.00 |
| 191 | `Asteroid_2` | 1051 | Object | -3306.04,63.74,3969.46 | 64,303,237 | Scale/Radius: 1.00 |
| 192 | `Asteroid_2` | 1053 | Object | -3529.10,37.42,3141.86 | 4,185,472 | Scale/Radius: 8.00 |
| 193 | `Asteroid_2` | 1055 | Object | -3470.40,55.43,3430.56 | 74,269,0 | Scale/Radius: 2.00 |
| 194 | `Asteroid_2` | 1057 | Object | -3353.00,20.79,3161.11 | 151,162,408 | Scale/Radius: 8.00 |
| 195 | `Asteroid_2` | 1059 | Object | -3235.59,69.29,3873.23 | 114,381,219 | Scale/Radius: 2.00 |
| 196 | `Asteroid_2` | 1061 | Object | -2849.58,59.59,3291.49 | 348,118,145 | Scale/Radius: 3.00 |
| 197 | `Asteroid_2` | 786 | Object | -4355.98,100.08,2754.59 | 489,263,432 | Scale/Radius: 10.00 |
| 198 | `Asteroid_2` | 642 | Object | -1901.55,20.79,4185.44 | 109,490,226 | Scale/Radius: 10.00 |
| 199 | `Asteroid_2` | 644 | Object | -958.47,208.60,4317.42 | 342,224,480 | Scale/Radius: 10.00 |
| 200 | `Asteroid_2` | 646 | Object | -1439.64,87.30,4243.18 | 259,205,237 | Scale/Radius: 10.00 |
| 201 | `Asteroid_2` | 648 | Object | -1227.92,12.47,4797.48 | 499,250,496 | Scale/Radius: 10.00 |
| 202 | `Asteroid_2` | 650 | Object | -1940.05,-54.04,4000.67 | 270,441,509 | Scale/Radius: 10.00 |
| 203 | `Asteroid_2` | 652 | Object | -2719.92,-35.34,3574.91 | 31,354,419 | Scale/Radius: 10.00 |
| 204 | `Asteroid_2` | 654 | Object | -1786.07,-6.24,4277.82 | 308,210,304 | Scale/Radius: 10.00 |
| 205 | `Asteroid_2` | 656 | Object | -1304.91,103.93,4566.52 | 326,241,86 | Scale/Radius: 10.00 |
| 206 | `Asteroid_2` | 658 | Object | -3624.51,-24.94,3332.41 | 107,418,492 | Scale/Radius: 10.00 |
| 207 | `Asteroid_2` | 660 | Object | -1112.44,33.26,4762.83 | 112,116,173 | Scale/Radius: 10.00 |
| 208 | `Asteroid_2` | 662 | Object | -842.99,290.35,4148.59 | 252,35,14 | Scale/Radius: 10.00 |
| 209 | `Asteroid_2` | 664 | Object | -1920.80,68.59,3931.38 | 414,154,358 | Scale/Radius: 10.00 |
| 210 | `Asteroid_2` | 666 | Object | -2652.17,101.85,4035.31 | 95,393,286 | Scale/Radius: 10.00 |
| 211 | `Asteroid_2` | 668 | Object | -1112.44,60.28,4543.42 | 167,391,312 | Scale/Radius: 10.00 |
| 212 | `Asteroid_2` | 670 | Object | -2671.41,81.07,4023.77 | 43,90,170 | Scale/Radius: 10.00 |
| 213 | `Asteroid_2` | 672 | Object | -2674.68,-81.07,4411.59 | 120,324,450 | Scale/Radius: 10.00 |
| 214 | `Asteroid_2` | 674 | Object | -1478.13,97.70,3942.93 | 240,455,395 | Scale/Radius: 10.00 |
| 215 | `Asteroid_2` | 676 | Object | -1381.90,-93.54,4936.05 | 304,247,329 | Scale/Radius: 10.00 |
| 216 | `Asteroid_2` | 678 | Object | -1420.39,33.26,4393.30 | 163,98,438 | Scale/Radius: 10.00 |
| 217 | `Asteroid_2` | 682 | Object | -1901.55,-43.65,4243.18 | 175,43,343 | Scale/Radius: 10.00 |
| 218 | `Asteroid_2` | 684 | Object | -900.73,-8.31,4566.52 | 203,396,111 | Scale/Radius: 10.00 |
| 219 | `Asteroid_2` | 686 | Object | -1824.57,-292.31,4832.12 | 454,331,488 | Scale/Radius: 10.00 |
| 220 | `Asteroid_2` | 688 | Object | -1497.38,93.54,4162.34 | 33,337,480 | Scale/Radius: 10.00 |
| 221 | `Asteroid_2` | 690 | Object | -1978.54,-87.30,4427.94 | 330,240,437 | Scale/Radius: 10.00 |
| 222 | `Asteroid_2` | 692 | Object | -1208.68,-72.75,3954.48 | 162,38,184 | Scale/Radius: 10.00 |
| 223 | `Asteroid_2` | 694 | Object | -2594.43,51.97,4658.90 | 257,314,511 | Scale/Radius: 10.00 |
| 224 | `Asteroid_2` | 696 | Object | -2478.95,78.99,4196.99 | 141,217,282 | Scale/Radius: 10.00 |
| 225 | `Asteroid_2` | 698 | Object | -2017.03,47.81,4162.34 | 367,334,116 | Scale/Radius: 10.00 |
| 226 | `Asteroid_2` | 700 | Object | -1247.17,-27.02,4012.22 | 363,51,57 | Scale/Radius: 10.00 |
| 227 | `Asteroid_2` | 702 | Object | -919.98,2.08,4728.19 | 264,465,465 | Scale/Radius: 10.00 |
| 228 | `Asteroid_2` | 704 | Object | -1458.88,12.47,3989.12 | 299,489,387 | Scale/Radius: 10.00 |
| 229 | `Asteroid_2` | 706 | Object | -1208.68,83.14,4266.27 | 504,455,208 | Scale/Radius: 10.00 |
| 230 | `Asteroid_2` | 708 | Object | -2171.00,97.70,3908.29 | 471,483,197 | Scale/Radius: 10.00 |
| 231 | `Asteroid_2` | 710 | Object | -2247.99,-97.70,3815.90 | 262,474,17 | Scale/Radius: 10.00 |
| 232 | `Asteroid_2` | 712 | Object | -2613.67,-49.89,4705.09 | 280,18,223 | Scale/Radius: 10.00 |
| 233 | `Asteroid_2` | 714 | Object | -958.47,81.07,4832.12 | 457,220,164 | Scale/Radius: 10.00 |
| 234 | `Asteroid_2` | 716 | Object | -1112.44,-12.47,3977.57 | 359,261,417 | Scale/Radius: 10.00 |
| 235 | `Asteroid_2` | 718 | Object | -2613.67,-101.85,3989.12 | 172,438,385 | Scale/Radius: 10.00 |
| 236 | `Asteroid_2` | 720 | Object | -2498.19,43.65,4820.57 | 69,67,506 | Scale/Radius: 10.00 |
| 237 | `Asteroid_2` | 724 | Object | -2132.51,-87.30,4797.48 | 263,209,62 | Scale/Radius: 10.00 |
| 238 | `Asteroid_2` | 726 | Object | -2113.26,45.73,3896.74 | 391,376,411 | Scale/Radius: 10.00 |
| 239 | `Asteroid_2` | 728 | Object | -2632.92,89.38,4162.34 | 47,282,388 | Scale/Radius: 10.00 |
| 240 | `Asteroid_2` | 730 | Object | -862.24,-6.24,4150.79 | 389,117,310 | Scale/Radius: 10.00 |
| 241 | `Asteroid_2` | 732 | Object | -1420.39,35.34,4312.46 | 162,465,72 | Scale/Radius: 10.00 |
| 242 | `Asteroid_2` | 738 | Object | -4864.09,46.19,2427.40 | 439,146,478 | Scale/Radius: 10.00 |
| 243 | `Asteroid_2` | 740 | Object | -4563.85,-161.67,2600.62 | 207,193,496 | Scale/Radius: 10.00 |
| 244 | `Asteroid_2` | 742 | Object | -4321.34,69.29,2485.14 | 503,302,126 | Scale/Radius: 10.00 |
| 245 | `Asteroid_2` | 744 | Object | -4367.53,-3.85,2003.97 | 396,38,209 | Scale/Radius: 10.00 |
| 246 | `Asteroid_2` | 748 | Object | -4448.37,38.49,1869.25 | 181,344,213 | Scale/Radius: 10.00 |
| 247 | `Asteroid_2` | 750 | Object | -5198.98,-119.33,1773.02 | 292,406,243 | Scale/Radius: 10.00 |
| 248 | `Asteroid_2` | 752 | Object | -4968.02,73.14,1676.78 | 239,469,92 | Scale/Radius: 10.00 |
| 249 | `Asteroid_2` | 754 | Object | -5233.62,180.92,1734.52 | 108,137,268 | Scale/Radius: 10.00 |
| 250 | `Asteroid_2` | 756 | Object | -4413.72,61.59,1984.73 | 422,250,150 | Scale/Radius: 10.00 |
| 251 | `Asteroid_2` | 758 | Object | -4529.20,103.93,1638.29 | 485,459,368 | Scale/Radius: 10.00 |
| 252 | `Asteroid_2` | 760 | Object | -4794.80,7.70,1773.02 | 431,252,253 | Scale/Radius: 10.00 |
| 253 | `Asteroid_2` | 762 | Object | -4529.20,-115.48,2177.19 | 371,296,85 | Scale/Radius: 10.00 |
| 254 | `Asteroid_2` | 764 | Object | -5268.27,138.57,1830.76 | 307,81,376 | Scale/Radius: 10.00 |
| 255 | `Asteroid_2` | 766 | Object | -5222.08,103.93,1368.84 | 351,509,494 | Scale/Radius: 10.00 |
| 256 | `Asteroid_2` | 770 | Object | -5175.88,-3.85,2023.22 | 242,144,284 | Scale/Radius: 10.00 |
| 257 | `Asteroid_2` | 772 | Object | -4887.19,-46.19,1291.85 | 269,168,61 | Scale/Radius: 10.00 |
| 258 | `Asteroid_2` | 774 | Object | -4298.24,188.62,2080.96 | 38,343,330 | Scale/Radius: 10.00 |
| 259 | `Asteroid_2` | 776 | Object | -4713.97,-57.74,1522.81 | 305,104,355 | Scale/Radius: 10.00 |
| 260 | `Asteroid_2` | 778 | Object | -4332.89,142.42,1580.55 | 52,359,204 | Scale/Radius: 10.00 |
| 261 | `Asteroid_2` | 780 | Object | -4563.85,42.34,2003.97 | 384,501,292 | Scale/Radius: 10.00 |
| 262 | `Asteroid_2` | 782 | Object | -5083.50,-38.49,1426.58 | 80,509,1 | Scale/Radius: 10.00 |
| 263 | `Asteroid_2` | 788 | Object | -4575.39,150.12,2331.17 | 326,142,24 | Scale/Radius: 10.00 |
| 264 | `Asteroid_2` | 790 | Object | -4263.60,30.79,1984.73 | 156,348,410 | Scale/Radius: 10.00 |
| 265 | `Asteroid_2` | 792 | Object | -4275.15,92.38,1484.32 | 239,446,154 | Scale/Radius: 10.00 |
| 266 | `Asteroid_2` | 794 | Object | -4852.54,-7.70,1811.51 | 82,239,407 | Scale/Radius: 10.00 |
| 267 | `Asteroid_2` | 796 | Object | -4644.68,111.63,1368.84 | 430,303,434 | Scale/Radius: 10.00 |
| 268 | `Asteroid_2` | 798 | Object | -4737.06,-76.99,2119.45 | 26,426,418 | Scale/Radius: 10.00 |
| 269 | `Asteroid_2` | 800 | Object | -4436.82,38.49,1580.55 | 119,135,379 | Scale/Radius: 10.00 |
| 270 | `Asteroid_2` | 804 | Object | -4760.16,150.12,1445.83 | 27,41,357 | Scale/Radius: 10.00 |
| 271 | `Asteroid_2` | 810 | Object | -4991.12,-146.27,1330.35 | 317,1,337 | Scale/Radius: 10.00 |
| 272 | `Asteroid_2` | 812 | Object | -4263.60,-88.53,1792.26 | 311,461,445 | Scale/Radius: 10.00 |
| 273 | `Asteroid_2` | 814 | Object | -4483.01,88.53,1715.28 | 141,65,285 | Scale/Radius: 10.00 |
| 274 | `Asteroid_2` | 818 | Object | 2386.49,-23.10,4157.29 | 484,244,352 | Scale/Radius: 10.00 |
| 275 | `Asteroid_2` | 820 | Object | 230.94,19.25,4182.07 | 178,481,56 | Scale/Radius: 10.00 |
| 276 | `Asteroid_2` | 822 | Object | 96.21,-142.42,4158.97 | 254,181,334 | Scale/Radius: 10.00 |
| 277 | `Asteroid_2` | 824 | Object | 2059.30,-53.89,4526.83 | 236,261,501 | Scale/Radius: 10.00 |
| 278 | `Asteroid_2` | 826 | Object | 1481.91,38.49,4907.91 | 309,504,407 | Scale/Radius: 10.00 |
| 279 | `Asteroid_2` | 828 | Object | 712.10,-103.93,3870.27 | 316,133,399 | Scale/Radius: 10.00 |
| 280 | `Asteroid_2` | 830 | Object | -315.86,-96.23,4607.86 | 291,367,96 | Scale/Radius: 10.00 |
| 281 | `Asteroid_2` | 832 | Object | 134.71,-157.82,3904.92 | 190,499,85 | Scale/Radius: 10.00 |
| 282 | `Asteroid_2` | 834 | Object | 173.20,19.25,4470.76 | 349,441,25 | Scale/Radius: 10.00 |
| 283 | `Asteroid_2` | 842 | Object | 615.87,-188.62,4378.38 | 478,17,313 | Scale/Radius: 10.00 |
| 284 | `Asteroid_2` | 844 | Object | 2444.23,196.55,3963.18 | 411,466,489 | Scale/Radius: 10.00 |
| 285 | `Asteroid_2` | 846 | Object | -354.35,-26.95,4665.60 | 421,32,58 | Scale/Radius: 10.00 |
| 286 | `Asteroid_2` | 848 | Object | 2232.52,30.79,4549.92 | 43,72,489 | Scale/Radius: 10.00 |
| 287 | `Asteroid_2` | 850 | Object | 404.16,142.42,4898.04 | 296,380,425 | Scale/Radius: 10.00 |
| 288 | `Asteroid_2` | 852 | Object | -643.05,-15.40,4861.92 | 207,138,507 | Scale/Radius: 10.00 |
| 289 | `Asteroid_2` | 854 | Object | 192.45,-165.52,4447.67 | 411,411,252 | Scale/Radius: 10.00 |
| 290 | `Asteroid_2` | 856 | Object | 615.87,-119.33,4182.07 | 55,453,6 | Scale/Radius: 10.00 |
| 291 | `Asteroid_2` | 860 | Object | 1539.65,-23.10,4203.49 | 244,478,171 | Scale/Radius: 10.00 |
| 292 | `Asteroid_2` | 862 | Object | 2290.26,173.22,4561.47 | 447,276,376 | Scale/Radius: 10.00 |
| 293 | `Asteroid_2` | 864 | Object | 1905.33,-150.12,4053.36 | 39,142,48 | Scale/Radius: 10.00 |
| 294 | `Asteroid_2` | 866 | Object | 261.54,169.37,4111.30 | 157,23,363 | Scale/Radius: 10.00 |
| 295 | `Asteroid_2` | 868 | Object | 2020.81,-7.70,4803.98 | 205,185,39 | Scale/Radius: 10.00 |
| 296 | `Asteroid_2` | 870 | Object | 1693.62,241.86,4506.48 | 51,161,183 | Scale/Radius: 10.00 |
| 297 | `Asteroid_2` | 872 | Object | 230.94,-7.70,4898.04 | 365,49,141 | Scale/Radius: 10.00 |
| 298 | `Asteroid_2` | 874 | Object | 307.93,84.68,4251.35 | 391,386,396 | Scale/Radius: 10.00 |
| 299 | `Asteroid_2` | 878 | Object | 731.35,30.79,4031.94 | 176,293,480 | Scale/Radius: 10.00 |
| 300 | `Asteroid_2` | 880 | Object | 1828.34,-84.68,4538.38 | 130,157,467 | Scale/Radius: 10.00 |
| 301 | `Asteroid_2` | 882 | Object | 615.87,-157.82,4909.58 | 106,50,321 | Scale/Radius: 10.00 |
| 302 | `Asteroid_2` | 884 | Object | 2463.48,100.08,4261.23 | 242,142,41 | Scale/Radius: 10.00 |
| 303 | `Asteroid_2` | 886 | Object | 173.20,100.08,4736.37 | 462,324,197 | Scale/Radius: 10.00 |
| 304 | `Asteroid_2` | 888 | Object | 1712.86,-142.42,4515.28 | 393,301,313 | Scale/Radius: 10.00 |
| 305 | `Asteroid_2` | 890 | Object | 404.16,100.08,5001.97 | 4,235,61 | Scale/Radius: 10.00 |
| 306 | `Asteroid_2` | 892 | Object | 461.90,-61.59,4274.45 | 133,232,258 | Scale/Radius: 10.00 |
| 307 | `Asteroid_2` | 894 | Object | 2271.01,130.88,4607.66 | 343,66,474 | Scale/Radius: 10.00 |
| 308 | `Asteroid_2` | 896 | Object | 1866.84,-184.77,3926.34 | 246,271,29 | Scale/Radius: 10.00 |
| 309 | `Asteroid_2` | 902 | Object | -4687.68,6.77,-50.75 | 483,102,439 | Scale/Radius: 10.00 |
| 310 | `Asteroid_2` | 904 | Object | -4491.37,-13.55,-427.98 | 7,508,352 | Scale/Radius: 10.00 |
| 311 | `Asteroid_2` | 910 | Object | -4641.49,-3.39,-5.48 | 122,103,267 | Scale/Radius: 10.00 |
| 312 | `Asteroid_2` | 914 | Object | -5034.12,28.79,930.05 | 148,428,36 | Scale/Radius: 10.00 |
| 313 | `Asteroid_2` | 916 | Object | -4514.46,44.04,507.55 | 390,269,102 | Scale/Radius: 10.00 |
| 314 | `Asteroid_2` | 922 | Object | -5068.76,-79.60,-201.65 | 304,196,0 | Scale/Radius: 10.00 |
| 315 | `Asteroid_2` | 924 | Object | -4629.94,59.28,281.21 | 194,425,315 | Scale/Radius: 10.00 |
| 316 | `Asteroid_2` | 926 | Object | -4549.11,-25.41,-246.91 | 250,502,26 | Scale/Radius: 10.00 |
| 317 | `Asteroid_2` | 928 | Object | -5080.31,45.73,658.44 | 215,72,349 | Scale/Radius: 10.00 |
| 318 | `Asteroid_2` | 930 | Object | -4849.35,-57.59,869.69 | 490,35,507 | Scale/Radius: 10.00 |
| 319 | `Asteroid_2` | 932 | Object | -4964.83,1.69,39.78 | 206,178,80 | Scale/Radius: 10.00 |
| 320 | `Asteroid_2` | 934 | Object | -4780.07,-66.05,235.94 | 56,21,308 | Scale/Radius: 10.00 |
| 321 | `Asteroid_2` | 936 | Object | -4699.23,22.02,-216.73 | 27,398,26 | Scale/Radius: 10.00 |
| 322 | `Asteroid_2` | 938 | Object | -5288.17,20.32,854.60 | 165,505,317 | Scale/Radius: 10.00 |
| 323 | `Asteroid_2` | 940 | Object | -4872.45,81.30,-20.57 | 383,397,265 | Scale/Radius: 10.00 |
| 324 | `Asteroid_2` | 942 | Object | -4549.11,74.52,205.77 | 229,30,64 | Scale/Radius: 10.00 |
| 325 | `Asteroid_2` | 944 | Object | -4884.00,44.04,-141.29 | 284,417,117 | Scale/Radius: 10.00 |
| 326 | `Asteroid_2` | 948 | Object | -5195.79,37.26,341.57 | 41,20,5 | Scale/Radius: 10.00 |
| 327 | `Asteroid_2` | 950 | Object | -4687.68,-50.81,477.37 | 160,402,415 | Scale/Radius: 10.00 |
| 328 | `Asteroid_2` | 952 | Object | -4791.61,60.97,-5.48 | 308,455,463 | Scale/Radius: 10.00 |
| 329 | `Asteroid_2` | 958 | Object | -4749.57,-377.96,-126.20 | 107,338,215 | Scale/Radius: 10.00 |
| 330 | `Asteroid_2` | 960 | Object | -4618.40,-66.05,809.34 | 281,384,292 | Scale/Radius: 10.00 |
| 331 | `Asteroid_2` | 968 | Object | -5057.22,-64.36,-322.36 | 401,368,507 | Scale/Radius: 10.00 |
| 332 | `Asteroid_2` | 974 | Object | -3235.59,5.54,3796.24 | 229,188,371 | Scale/Radius: 10.00 |
| 333 | `Asteroid_2` | 976 | Object | -366.18,-842.02,-2336.38 | 240,378,382 | Scale/Radius: 10.00 |
| 334 | `Asteroid_2` | 978 | Object | -401.40,-796.29,-1701.24 | 348,448,199 | Scale/Radius: 10.00 |
| 335 | `Asteroid_2` | 980 | Object | -131.37,-828.16,-1758.98 | 326,462,24 | Scale/Radius: 10.00 |
| 336 | `Asteroid_2` | 982 | Object | -3458.66,67.90,3719.26 | 201,262,83 | Scale/Radius: 10.00 |
| 337 | `Asteroid_2` | 984 | Object | -3576.06,16.63,3180.35 | 395,437,30 | Scale/Radius: 10.00 |
| 338 | `Asteroid_2` | 988 | Object | -25.71,-790.74,-2355.62 | 360,447,488 | Scale/Radius: 10.00 |
| 339 | `Asteroid_2` | 990 | Object | -3193.56,-198.72,3007.14 | 61,241,317 | Scale/Radius: 10.00 |
| 340 | `Asteroid_2` | 992 | Object | -248.78,-801.83,-1855.21 | 27,154,76 | Scale/Radius: 10.00 |
| 341 | `Asteroid_2` | 994 | Object | -3239.34,-16.63,3402.75 | 163,21,107 | Scale/Radius: 10.00 |
| 342 | `Asteroid_2` | 996 | Object | -907.07,29.10,-2605.83 | 332,473,495 | Scale/Radius: 10.00 |
| 343 | `Asteroid_2` | 1002 | Object | -2908.29,33.26,3349.23 | 433,143,411 | Scale/Radius: 10.00 |
| 344 | `Asteroid_2` | 1004 | Object | -3317.78,-40.19,3719.26 | 355,491,122 | Scale/Radius: 10.00 |
| 345 | `Asteroid_2` | 1006 | Object | -3286.30,-58.20,2921.59 | 385,302,116 | Scale/Radius: 10.00 |
| 346 | `Asteroid_2` | 1014 | Object | -3470.40,22.17,3507.54 | 418,479,503 | Scale/Radius: 10.00 |
| 347 | `Asteroid_2` | 1016 | Object | -3235.59,69.29,3757.75 | 78,168,314 | Scale/Radius: 10.00 |
| 348 | `Asteroid_2` | 1018 | Object | -3341.26,2.77,3873.23 | 381,79,474 | Scale/Radius: 10.00 |
| 349 | `Asteroid_2` | 1020 | Object | -2873.06,-58.20,3349.23 | 352,299,40 | Scale/Radius: 10.00 |
| 350 | `Asteroid_2` | 1024 | Object | -730.13,-864.19,-1932.20 | 64,53,224 | Scale/Radius: 10.00 |
| 351 | `Asteroid_2` | 1026 | Object | -530.54,-800.45,-2374.87 | 8,81,406 | Scale/Radius: 10.00 |
| 352 | `Asteroid_2` | 1028 | Object | -3063.24,-16.63,3171.80 | 75,310,233 | Scale/Radius: 10.00 |
| 353 | `Asteroid_2` | 1032 | Object | -683.17,-880.82,-2413.36 | 135,503,448 | Scale/Radius: 10.00 |
| 354 | `Asteroid_2` | 1034 | Object | -3438.93,52.66,3094.81 | 142,42,351 | Scale/Radius: 10.00 |
| 355 | `Asteroid_2` | 1036 | Object | -49.19,-915.46,-2432.61 | 505,347,15 | Scale/Radius: 10.00 |
| 356 | `Asteroid_2` | 1038 | Object | -3333.26,-66.52,3306.52 | 268,15,463 | Scale/Radius: 10.00 |
| 357 | `Asteroid_2` | 1040 | Object | -3200.37,37.42,3873.23 | 279,222,238 | Scale/Radius: 10.00 |
| 358 | `Asteroid_2` | 1042 | Object | -3474.15,-67.90,3094.81 | 405,491,420 | Scale/Radius: 10.00 |
| 359 | `Asteroid_2` | 1044 | Object | -3309.78,-59.59,3672.20 | 93,164,419 | Scale/Radius: 10.00 |
| 360 | `Asteroid_2` | 1048 | Object | -354.44,-797.67,-1912.95 | 449,103,111 | Scale/Radius: 10.00 |
| 361 | `Asteroid_2` | 1052 | Object | -3121.94,-11.09,3479.74 | 173,439,336 | Scale/Radius: 10.00 |
| 362 | `Asteroid_2` | 1054 | Object | -3458.66,9.70,3334.33 | 384,7,240 | Scale/Radius: 10.00 |
| 363 | `Asteroid_2` | 1056 | Object | -765.35,-790.74,-2143.91 | 186,423,351 | Scale/Radius: 10.00 |
| 364 | `Asteroid_2` | 1058 | Object | -119.63,-781.04,-2124.67 | 300,328,472 | Scale/Radius: 10.00 |
| 365 | `Asteroid_2` | 1060 | Object | -3204.12,-16.63,3710.70 | 486,193,413 | Scale/Radius: 10.00 |
| 366 | `Asteroid_2` | 1062 | Object | -3294.30,31.87,3738.50 | 273,368,62 | Scale/Radius: 10.00 |
| 367 | `Roid_Sm_Brown2` | 329 | Object | -4297.17,-134.73,2788.96 | 429,315,404 | Scale/Radius: 10.00 |
| 368 | `Roid_Sm_Brown2` | 257 | Object | -3267.66,-230.96,2677.15 | 243,482,116 | Scale/Radius: 10.00 |
| 369 | `Roid_Sm_Brown2` | 311 | Object | -3801.98,-623.59,2583.65 | 236,376,249 | Scale/Radius: 10.00 |
| 370 | `Roid_Sm_Brown2` | 320 | Object | -3990.60,-69.29,2756.87 | 366,417,41 | Scale/Radius: 10.00 |
| 371 | `Roid_Sm_Brown2` | 338 | Object | -4788.49,962.33,920.07 | 72,452,8 | Scale/Radius: 10.00 |
| 372 | `Roid_Sm_Brown2` | 347 | Object | -5113.15,-96.23,139.86 | 442,93,263 | Scale/Radius: 10.00 |
| 373 | `Roid_Sm_Brown2` | 376 | Object | 1791.16,-346.44,4618.75 | 129,140,490 | Scale/Radius: 10.00 |
| 374 | `Roid_Sm_Brown2` | 383 | Object | -2513.03,500.41,3566.83 | 104,245,416 | Scale/Radius: 10.00 |
| 375 | `Roid_Sm_Brown2` | 390 | Object | -94.94,-134.73,4939.92 | 24,469,23 | Scale/Radius: 10.00 |
| 376 | `Roid_Sm_Brown` | 403 | Object | 1906.64,-519.63,3771.90 | 197,125,325 | Scale/Radius: 10.00 |
| 377 | `Roid_Sm_Brown` | 256 | Object | -452.57,188.98,-1757.15 | 16,403,480 | Scale/Radius: 10.00 |
| 378 | `Roid_Sm_Brown` | 310 | Object | -425.63,-781.04,-1826.43 | 257,391,254 | Scale/Radius: 10.00 |
| 379 | `Roid_Sm_Brown` | 328 | Object | -3789.07,461.92,2481.02 | 444,181,8 | Scale/Radius: 10.00 |
| 380 | `Roid_Sm_Brown` | 337 | Object | -4588.33,-596.62,981.66 | 136,504,157 | Scale/Radius: 10.00 |
| 381 | `Roid_Sm_Brown` | 346 | Object | -4912.98,192.47,-352.85 | 304,70,185 | Scale/Radius: 10.00 |
| 382 | `Roid_Sm_Brown` | 355 | Object | -5251.72,827.60,570.99 | 44,91,137 | Scale/Radius: 10.00 |
| 383 | `Roid_Sm_Brown` | 368 | Object | 309.23,866.09,4324.03 | 393,336,45 | Scale/Radius: 10.00 |
| 384 | `Roid_Sm_Brown` | 382 | Object | -1365.21,384.93,3785.13 | 323,351,266 | Scale/Radius: 10.00 |
| 385 | `Roid_Sm_Brown` | 389 | Object | -2866.44,615.89,4189.30 | 191,496,220 | Scale/Radius: 10.00 |
| 386 | `Roid_Sm_Brown` | 396 | Object | 1617.94,-346.44,4291.56 | 487,159,474 | Scale/Radius: 10.00 |
| 387 | `Roid_Sm_Brown` | 370 | Object | 2714.99,846.85,3887.38 | 121,83,503 | Scale/Radius: 7.56 |
| 388 | `Roid_Sm_Brown` | 268 | Object | -3240.71,461.92,3335.38 | 487,203,453 | Scale/Radius: 7.56 |
| 389 | `Roid_Sm_Brown` | 277 | Object | -3537.11,-623.59,3681.82 | 24,261,306 | Scale/Radius: 7.56 |
| 390 | `Roid_Sm_Brown` | 331 | Object | -5005.37,134.73,-44.90 | 145,335,331 | Scale/Radius: 7.56 |
| 391 | `Roid_Sm_Brown` | 377 | Object | -3068.92,-134.73,3139.96 | 230,488,508 | Scale/Radius: 7.56 |
| 392 | `Roid_Sm_Brown2` | 342 | Object | -4266.30,-115.48,201.45 | 264,403,285 | Scale/Radius: 8.36 |
| 393 | `Roid_Sm_Brown2` | 288 | Object | -533.41,235.17,-1757.15 | 508,472,474 | Scale/Radius: 8.36 |
| 394 | `Roid_Sm_Brown2` | 297 | Object | -3496.09,-161.67,3514.53 | 28,105,242 | Scale/Radius: 8.36 |
| 395 | `Roid_Sm_Brown2` | 333 | Object | -4882.19,-19.25,78.27 | 378,42,100 | Scale/Radius: 8.36 |
| 396 | `Roid_Sm_Brown2` | 351 | Object | -4603.73,211.71,735.30 | 144,473,279 | Scale/Radius: 8.36 |
| 397 | `Roid_Sm_Brown2` | 360 | Object | -5312.08,-404.18,1290.38 | 206,423,210 | Scale/Radius: 8.36 |
| 398 | `Roid_Sm_Brown2` | 365 | Object | -94.94,-294.31,3897.84 | 71,451,419 | Scale/Radius: 8.36 |
| 399 | `Roid_Sm_Brown2` | 379 | Object | -2864.40,923.83,3351.02 | 48,239,143 | Scale/Radius: 8.36 |
| 400 | `Roid_Sm_Brown2` | 386 | Object | -1365.21,384.93,4227.80 | 79,479,305 | Scale/Radius: 8.36 |
| 401 | `Roid_Sm_Brown2` | 400 | Object | -2979.87,-57.74,3370.27 | 36,176,453 | Scale/Radius: 8.36 |
| 402 | `Roid_Sm_Brown` | 303 | Object | -746.77,119.69,-2544.95 | 48,18,163 | Scale/Radius: 10.00 |
| 403 | `Roid_Sm_Brown` | 258 | Object | -3240.71,-554.30,3404.67 | 412,33,105 | Scale/Radius: 10.00 |
| 404 | `Roid_Sm_Brown` | 330 | Object | -5050.24,442.67,1104.84 | 442,259,154 | Scale/Radius: 10.00 |
| 405 | `Roid_Sm_Brown` | 339 | Object | -4466.47,808.35,-414.44 | 295,430,41 | Scale/Radius: 10.00 |
| 406 | `Roid_Sm_Brown` | 348 | Object | -4418.96,673.63,673.71 | 214,171,444 | Scale/Radius: 10.00 |
| 407 | `Roid_Sm_Brown` | 1296 | Object | 649.50,0.00,3756.76 | 0,0,0 | Scale/Radius: 9.99 |
| 408 | `Roid_Sm_Brown` | 254 | Object | -3748.09,785.26,2549.01 | 232,498,346 | Scale/Radius: 9.99 |
| 409 | `Roid_Sm_Brown` | 263 | Object | -3494.87,-554.27,3143.77 | 194,380,144 | Scale/Radius: 9.99 |
| 410 | `Roid_Sm_Brown` | 272 | Object | -3602.65,-485.01,3178.42 | 382,193,347 | Scale/Radius: 9.99 |
| 411 | `Roid_Sm_Brown` | 281 | Object | -3442.20,392.63,3757.04 | 507,488,321 | Scale/Radius: 9.99 |
| 412 | `Roid_Sm_Brown` | 317 | Object | -2822.15,577.40,3286.93 | 356,42,383 | Scale/Radius: 9.99 |
| 413 | `Roid_Sm_Brown` | 326 | Object | -3551.14,500.41,3124.96 | 315,408,357 | Scale/Radius: 9.99 |
| 414 | `Roid_Sm_Brown` | 353 | Object | -5174.74,750.61,570.99 | 139,374,76 | Scale/Radius: 9.99 |
| 415 | `Roid_Sm_Brown` | 374 | Object | 224.35,-500.38,4157.04 | 121,370,430 | Scale/Radius: 9.99 |
| 416 | `Roid_Sm_Brown` | 381 | Object | -1827.13,365.68,3708.14 | 261,135,351 | Scale/Radius: 9.99 |
| 417 | `Roid_Sm_Brown` | 388 | Object | -3205.91,-57.74,4124.98 | 223,298,368 | Scale/Radius: 9.99 |
| 418 | `Roid_Sm_Brown` | 395 | Object | 2310.81,-230.96,4349.30 | 19,211,238 | Scale/Radius: 9.99 |
| 419 | `Roid_Sm_Brown` | 402 | Object | 136.01,307.94,3900.61 | 27,237,360 | Scale/Radius: 9.99 |
| 420 | `Bora_Space_Station` | 1075 | Interactive | -1580.85,0.00,-363.57 | 78,0,0 | secondary groups: none, VALIANCE |
