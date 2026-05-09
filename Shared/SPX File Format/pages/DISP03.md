# Tachyon: The Fringe DISP03.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP03.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `DISPUT3.BDF` |
| Region | 6 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 6 |
| Entities | 335 |
| Events | 4 |
| Waypoints | 0 |
| Child Sectors | 6 |
| Scripts | 2 |
| Scenes | 2 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Research_Facility`, `1: Spcargo_Credits`, `2: Arena_Bouy1`, `3: KC2_Asteroid`, `4: Navigational_Bouy`, `5: Hyper_Gate` |
| Scripts | `YOUNG.SCR`, `PLAYER.SCR` |
| Scenes | `D3GC050A.SEN`, `D3DOC01.SEN` |
| Labels | `BFGE_02`, `BFBE_07`, `TNSA`, `BFBE_09`, `adder1`, `BFBF_07`, `ROSS`, `SPIKE`, `atkin`, `cruiser1` |
| Aliases | `fake_2`, `BC10_Waraxe`, `Coward`, `spy_1`, `fake_1`, `tnsa`, `BC10_Claymore4`, `BC10_Claymore3`, `BC10_Claymore2`, `BC10_Claymore1`, `BC10_Warhammer4`, `BC10_Warhammer3`, `BC10_Warhammer2`, `BC10_Warhammer1`, `BC10_Mace3`, `BC10_Mace4`, `BC10_Mace1`, `BC10_Mace2`, `Galileo`, `SPIKE`, `zeus`, `Stocks01` |
| Groups | `CONT_070` |
| Child Sectors | [disp03A.spx](DISP03A.md), [disp03B.spx](DISP03B.md), [disp03C.spx](DISP03C.md), [disp03D.spx](DISP03D.md), [disp03E.spx](DISP03E.md), [disp03F.spx](DISP03F.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 0, value 4018

**Action**

- Gate state/action: param 3, subtype 2, param 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4031

**Action**

- Play dialog: YOUNG.SCR, line/variant 0
- Gate state/action: param 3, subtype 2, param 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 10986; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 183
- Set/add variable: variable group 0, variable 2, subtype 1, value 1000
- Show/update HUD contact: contact/list 0, subtype 9, param 27
- Set/add variable: variable group 18, variable 804, subtype 0, value 1
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 32, op 2, value 10

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 27
- Set/add variable: variable group 20, variable 32, subtype 0, value 0

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | -2156.40,0.00,3201.55 | 228,0,0 | Gate SPX: [disp02.spx](DISP02.md) |
| 1 | `Hyper_Gate` | 3 | Gate | 981.50,0.00,-588.09 | 424,0,0 | Gate SPX: [disp04.spx](DISP04.md) |
| 2 | `Hyper_Gate` | 6591 | Gate | -1053.05,0.00,-688.31 | 0,0,0 | Gate SPX: [disp06.spx](DISP06.md) |
| 3 | `Navigational_Bouy` | 9986 | Interactive | -3766.79,0.00,-3074.16 | 0,0,0 | None |
| 4 | `Navigational_Bouy` | 9991 | Interactive | 627.65,0.00,6233.94 | 0,0,0 | None |
| 5 | `Navigational_Bouy` | 10080 | Interactive | 3295.48,0.00,-3358.20 | 0,0,0 | None |
| 6 | `KC2_Asteroid` | 10341 | Object | -6413.61,519.66,-3276.08 | 79,356,129 | Scale/Radius: 9.00 |
| 7 | `KC2_Asteroid` | 10342 | Object | -6471.35,-565.85,-3495.49 | 279,223,306 | Scale/Radius: 2.00 |
| 8 | `KC2_Asteroid` | 10343 | Object | -6067.18,311.79,-4199.91 | 142,411,235 | Scale/Radius: 5.00 |
| 9 | `KC2_Asteroid` | 10344 | Object | -5882.41,461.92,-3657.16 | 356,501,206 | Scale/Radius: 1.00 |
| 10 | `KC2_Asteroid` | 10345 | Object | -6390.52,542.75,-3911.22 | 311,287,488 | Scale/Radius: 3.00 |
| 11 | `KC2_Asteroid` | 10346 | Object | -5651.45,438.82,-3368.46 | 489,364,71 | Scale/Radius: 1.00 |
| 12 | `KC2_Asteroid` | 10347 | Object | -5709.19,-34.64,-4153.72 | 402,319,48 | Scale/Radius: 2.00 |
| 13 | `KC2_Asteroid` | 10348 | Object | -5859.31,219.41,-3345.37 | 482,383,124 | Scale/Radius: 4.00 |
| 14 | `KC2_Asteroid` | 10349 | Object | -6055.63,-150.12,-3460.85 | 129,334,132 | Scale/Radius: 5.00 |
| 15 | `KC2_Asteroid` | 10350 | Object | -6529.09,-11.55,-3195.25 | 498,205,494 | Scale/Radius: 1.00 |
| 16 | `KC2_Asteroid` | 10351 | Object | -6506.00,-230.96,-4015.15 | 157,103,73 | Scale/Radius: 1.00 |
| 17 | `KC2_Asteroid` | 10352 | Object | -5951.70,-254.05,-4003.60 | 146,332,338 | Scale/Radius: 5.00 |
| 18 | `KC2_Asteroid` | 10353 | Object | -5766.93,-461.92,-3114.41 | 258,177,332 | Scale/Radius: 2.00 |
| 19 | `KC2_Asteroid` | 10354 | Object | -6275.04,-346.44,-3795.74 | 168,441,174 | Scale/Radius: 7.00 |
| 20 | `KC2_Asteroid` | 10355 | Object | -5836.22,427.27,-3403.11 | 263,145,18 | Scale/Radius: 1.00 |
| 21 | `KC2_Asteroid` | 10356 | Object | -5951.70,-46.19,-3772.64 | 222,483,142 | Scale/Radius: 7.00 |
| 22 | `KC2_Asteroid` | 10357 | Object | -5847.77,277.15,-3749.55 | 477,349,494 | Scale/Radius: 3.00 |
| 23 | `KC2_Asteroid` | 10358 | Object | -6609.93,80.84,-3726.45 | 151,17,503 | Scale/Radius: 3.00 |
| 24 | `KC2_Asteroid` | 10359 | Object | -6067.18,-288.70,-3403.11 | 37,13,169 | Scale/Radius: 1.00 |
| 25 | `KC2_Asteroid` | 10360 | Object | -6090.27,-415.72,-4165.27 | 379,351,13 | Scale/Radius: 5.00 |
| 26 | `KC2_Asteroid` | 10362 | Object | -4727.95,577.40,-5149.19 | 64,219,361 | Scale/Radius: 2.00 |
| 27 | `KC2_Asteroid` | 10363 | Object | -4231.39,207.86,-5738.13 | 168,422,114 | Scale/Radius: 3.00 |
| 28 | `KC2_Asteroid` | 10364 | Object | -4496.99,34.64,-5218.48 | 35,235,218 | Scale/Radius: 7.00 |
| 29 | `KC2_Asteroid` | 10365 | Object | -4762.59,577.40,-5264.67 | 409,506,159 | Scale/Radius: 4.00 |
| 30 | `KC2_Asteroid` | 10366 | Object | -3954.24,-415.72,-6084.57 | 307,313,417 | Scale/Radius: 5.00 |
| 31 | `KC2_Asteroid` | 10367 | Object | -4393.06,265.60,-5807.42 | 351,397,430 | Scale/Radius: 1.00 |
| 32 | `KC2_Asteroid` | 10368 | Object | -4081.27,-438.82,-5830.51 | 298,67,163 | Scale/Radius: 1.00 |
| 33 | `KC2_Asteroid` | 10369 | Object | -4323.77,381.08,-5437.89 | 448,75,371 | Scale/Radius: 9.00 |
| 34 | `KC2_Asteroid` | 10370 | Object | -3942.69,23.10,-5807.42 | 259,177,338 | Scale/Radius: 7.00 |
| 35 | `KC2_Asteroid` | 10371 | Object | -4185.20,-207.86,-5414.79 | 359,131,364 | Scale/Radius: 1.00 |
| 36 | `KC2_Asteroid` | 10372 | Object | -4439.25,-46.19,-6038.38 | 212,370,387 | Scale/Radius: 4.00 |
| 37 | `KC2_Asteroid` | 10373 | Object | -3850.31,300.25,-5264.67 | 493,212,461 | Scale/Radius: 4.00 |
| 38 | `KC2_Asteroid` | 10374 | Object | -4462.35,127.03,-6073.02 | 212,295,65 | Scale/Radius: 4.00 |
| 39 | `KC2_Asteroid` | 10375 | Object | -3757.93,-11.55,-5530.27 | 167,231,218 | Scale/Radius: 9.00 |
| 40 | `KC2_Asteroid` | 10376 | Object | -4751.05,-334.89,-5460.98 | 431,481,152 | Scale/Radius: 6.00 |
| 41 | `KC2_Asteroid` | 10377 | Object | -3919.60,-127.03,-5992.19 | 411,497,10 | Scale/Radius: 5.00 |
| 42 | `KC2_Asteroid` | 10378 | Object | -4266.03,-230.96,-6026.83 | 442,57,267 | Scale/Radius: 1.00 |
| 43 | `KC2_Asteroid` | 10379 | Object | -4647.12,427.27,-5980.64 | 289,342,33 | Scale/Radius: 2.00 |
| 44 | `KC2_Asteroid` | 10380 | Object | -4450.80,438.82,-5761.23 | 305,194,505 | Scale/Radius: 4.00 |
| 45 | `KC2_Asteroid` | 10381 | Object | -4058.17,519.66,-5241.57 | 246,208,459 | Scale/Radius: 1.00 |
| 46 | `KC2_Asteroid` | 10402 | Object | -4513.45,1470.47,-3701.71 | 413,340,237 | Scale/Radius: 8.00 |
| 47 | `KC2_Asteroid` | 10403 | Object | -4906.08,2209.53,-3967.31 | 121,23,262 | Scale/Radius: 1.00 |
| 48 | `KC2_Asteroid` | 10404 | Object | -5090.84,2267.27,-4244.46 | 191,186,399 | Scale/Radius: 3.00 |
| 49 | `KC2_Asteroid` | 10405 | Object | -4721.31,2313.46,-4186.72 | 170,334,64 | Scale/Radius: 8.00 |
| 50 | `KC2_Asteroid` | 10406 | Object | -4490.35,2001.67,-3724.81 | 439,221,250 | Scale/Radius: 2.00 |
| 51 | `KC2_Asteroid` | 10407 | Object | -4767.50,1562.85,-3944.22 | 101,19,262 | Scale/Radius: 6.00 |
| 52 | `KC2_Asteroid` | 10408 | Object | -4986.91,1863.10,-4025.05 | 466,22,48 | Scale/Radius: 6.00 |
| 53 | `KC2_Asteroid` | 10409 | Object | -4929.17,1609.04,-4394.59 | 62,246,142 | Scale/Radius: 8.00 |
| 54 | `KC2_Asteroid` | 10410 | Object | -4698.21,2221.08,-3771.00 | 392,365,24 | Scale/Radius: 1.00 |
| 55 | `KC2_Asteroid` | 10411 | Object | -4859.89,2313.46,-3459.21 | 240,59,26 | Scale/Radius: 4.00 |
| 56 | `KC2_Asteroid` | 10412 | Object | -4294.04,1562.85,-4232.92 | 58,439,457 | Scale/Radius: 1.00 |
| 57 | `KC2_Asteroid` | 10413 | Object | -5090.84,2267.27,-3921.12 | 301,339,337 | Scale/Radius: 3.00 |
| 58 | `KC2_Asteroid` | 10414 | Object | -5344.90,2117.15,-3690.16 | 197,106,384 | Scale/Radius: 8.00 |
| 59 | `KC2_Asteroid` | 10415 | Object | -4328.68,1666.78,-4036.60 | 272,184,342 | Scale/Radius: 1.00 |
| 60 | `KC2_Asteroid` | 10416 | Object | -4490.35,2348.11,-3771.00 | 303,236,27 | Scale/Radius: 9.00 |
| 61 | `KC2_Asteroid` | 10417 | Object | -4882.98,1424.28,-3851.83 | 144,278,494 | Scale/Radius: 5.00 |
| 62 | `KC2_Asteroid` | 10418 | Object | -5264.06,2348.11,-4336.85 | 75,395,266 | Scale/Radius: 6.00 |
| 63 | `KC2_Asteroid` | 10419 | Object | -4386.42,1943.93,-3898.03 | 403,414,132 | Scale/Radius: 6.00 |
| 64 | `KC2_Asteroid` | 10420 | Object | -5206.32,2197.99,-4152.08 | 21,22,383 | Scale/Radius: 1.00 |
| 65 | `KC2_Asteroid` | 10421 | Object | -5321.80,2394.30,-3678.62 | 173,218,215 | Scale/Radius: 7.00 |
| 66 | `KC2_Asteroid` | 10423 | Object | 3771.00,-646.73,-3888.72 | 315,106,177 | Scale/Radius: 8.00 |
| 67 | `KC2_Asteroid` | 10424 | Object | 3932.67,-1385.80,-4396.82 | 176,237,44 | Scale/Radius: 1.00 |
| 68 | `KC2_Asteroid` | 10425 | Object | 4279.11,-704.47,-4443.02 | 341,180,333 | Scale/Radius: 6.00 |
| 69 | `KC2_Asteroid` | 10426 | Object | 4279.11,-1408.90,-4581.59 | 166,382,486 | Scale/Radius: 2.00 |
| 70 | `KC2_Asteroid` | 10427 | Object | 3447.66,-1651.40,-4235.15 | 7,119,261 | Scale/Radius: 7.00 |
| 71 | `KC2_Asteroid` | 10428 | Object | 4001.96,-669.83,-3773.24 | 393,380,189 | Scale/Radius: 9.00 |
| 72 | `KC2_Asteroid` | 10429 | Object | 4232.92,-1362.70,-4188.96 | 335,416,304 | Scale/Radius: 9.00 |
| 73 | `KC2_Asteroid` | 10430 | Object | 4325.30,-1535.92,-4165.87 | 347,166,410 | Scale/Radius: 6.00 |
| 74 | `KC2_Asteroid` | 10431 | Object | 3805.64,-1616.76,-3842.52 | 451,499,484 | Scale/Radius: 2.00 |
| 75 | `KC2_Asteroid` | 10432 | Object | 3886.48,-1766.88,-3958.00 | 44,413,150 | Scale/Radius: 5.00 |
| 76 | `KC2_Asteroid` | 10433 | Object | 4325.30,-681.38,-3888.72 | 236,457,246 | Scale/Radius: 8.00 |
| 77 | `KC2_Asteroid` | 10434 | Object | 4198.27,-923.88,-3669.31 | 284,8,17 | Scale/Radius: 6.00 |
| 78 | `KC2_Asteroid` | 10435 | Object | 4221.37,-1074.01,-4489.21 | 154,79,106 | Scale/Radius: 1.00 |
| 79 | `KC2_Asteroid` | 10436 | Object | 3771.00,-785.31,-3750.14 | 112,269,257 | Scale/Radius: 5.00 |
| 80 | `KC2_Asteroid` | 10437 | Object | 3759.45,-1166.39,-4200.51 | 172,98,90 | Scale/Radius: 3.00 |
| 81 | `KC2_Asteroid` | 10438 | Object | 4279.11,-1766.88,-4396.82 | 136,26,497 | Scale/Radius: 7.00 |
| 82 | `KC2_Asteroid` | 10439 | Object | 4256.01,-1097.10,-3923.36 | 463,139,255 | Scale/Radius: 5.00 |
| 83 | `KC2_Asteroid` | 10440 | Object | 3505.40,-762.21,-4246.70 | 250,461,130 | Scale/Radius: 4.00 |
| 84 | `KC2_Asteroid` | 10441 | Object | 4025.05,-1281.87,-4581.59 | 150,166,306 | Scale/Radius: 2.00 |
| 85 | `KC2_Asteroid` | 10442 | Object | 3851.83,-1039.36,-4443.02 | 422,50,139 | Scale/Radius: 5.00 |
| 86 | `KC2_Asteroid` | 10444 | Object | 5801.07,-1037.19,-4804.70 | 83,277,91 | Scale/Radius: 1.00 |
| 87 | `KC2_Asteroid` | 10445 | Object | 5812.62,-275.03,-5359.00 | 167,186,70 | Scale/Radius: 5.00 |
| 88 | `KC2_Asteroid` | 10446 | Object | 5604.75,-263.48,-4677.68 | 231,386,343 | Scale/Radius: 1.00 |
| 89 | `KC2_Asteroid` | 10447 | Object | 5489.28,-1164.22,-5231.98 | 182,456,131 | Scale/Radius: 4.00 |
| 90 | `KC2_Asteroid` | 10448 | Object | 6401.56,-1233.51,-5266.62 | 182,502,449 | Scale/Radius: 1.00 |
| 91 | `KC2_Asteroid` | 10449 | Object | 5443.08,-344.32,-5255.07 | 60,337,219 | Scale/Radius: 6.00 |
| 92 | `KC2_Asteroid` | 10450 | Object | 5466.18,-459.80,-4723.87 | 461,200,139 | Scale/Radius: 2.00 |
| 93 | `KC2_Asteroid` | 10451 | Object | 6297.63,-633.02,-4539.10 | 444,347,228 | Scale/Radius: 4.00 |
| 94 | `KC2_Asteroid` | 10452 | Object | 6332.27,-367.42,-4319.69 | 27,400,143 | Scale/Radius: 1.00 |
| 95 | `KC2_Asteroid` | 10453 | Object | 5373.80,-933.26,-4839.35 | 325,69,6 | Scale/Radius: 9.00 |
| 96 | `KC2_Asteroid` | 10454 | Object | 6251.44,-794.69,-5185.78 | 478,234,336 | Scale/Radius: 2.00 |
| 97 | `KC2_Asteroid` | 10455 | Object | 6459.30,-1118.03,-4954.83 | 424,164,153 | Scale/Radius: 9.00 |
| 98 | `KC2_Asteroid` | 10456 | Object | 5454.63,-598.37,-5416.74 | 275,185,288 | Scale/Radius: 8.00 |
| 99 | `KC2_Asteroid` | 10457 | Object | 6008.93,-1060.29,-5301.26 | 282,226,38 | Scale/Radius: 6.00 |
| 100 | `KC2_Asteroid` | 10458 | Object | 6366.92,-251.94,-4885.54 | 307,429,250 | Scale/Radius: 9.00 |
| 101 | `KC2_Asteroid` | 10459 | Object | 5870.36,-402.06,-4723.87 | 40,454,66 | Scale/Radius: 8.00 |
| 102 | `KC2_Asteroid` | 10460 | Object | 5477.73,-1268.15,-5035.66 | 208,243,505 | Scale/Radius: 3.00 |
| 103 | `KC2_Asteroid` | 10461 | Object | 5939.64,-910.17,-4989.47 | 337,229,511 | Scale/Radius: 6.00 |
| 104 | `KC2_Asteroid` | 10462 | Object | 5396.89,-644.57,-4723.87 | 205,52,493 | Scale/Radius: 5.00 |
| 105 | `KC2_Asteroid` | 10463 | Object | 5477.73,-679.21,-5012.57 | 134,101,256 | Scale/Radius: 9.00 |
| 106 | `KC2_Asteroid` | 10465 | Object | 4513.29,-230.96,-6842.07 | 337,420,478 | Scale/Radius: 5.00 |
| 107 | `KC2_Asteroid` | 10466 | Object | 4905.92,46.19,-7361.73 | 99,472,426 | Scale/Radius: 4.00 |
| 108 | `KC2_Asteroid` | 10467 | Object | 4282.33,496.56,-7234.70 | 218,405,384 | Scale/Radius: 4.00 |
| 109 | `KC2_Asteroid` | 10468 | Object | 4790.44,219.41,-7407.92 | 217,72,391 | Scale/Radius: 2.00 |
| 110 | `KC2_Asteroid` | 10469 | Object | 3889.70,-450.37,-6403.25 | 165,24,29 | Scale/Radius: 1.00 |
| 111 | `KC2_Asteroid` | 10470 | Object | 3947.44,-450.37,-6830.52 | 349,477,51 | Scale/Radius: 2.00 |
| 112 | `KC2_Asteroid` | 10471 | Object | 4397.81,450.37,-6530.28 | 146,467,97 | Scale/Radius: 1.00 |
| 113 | `KC2_Asteroid` | 10472 | Object | 4155.30,542.75,-6726.59 | 427,290,16 | Scale/Radius: 4.00 |
| 114 | `KC2_Asteroid` | 10473 | Object | 4744.25,69.29,-6403.25 | 103,347,7 | Scale/Radius: 4.00 |
| 115 | `KC2_Asteroid` | 10474 | Object | 4028.27,219.41,-6715.04 | 181,202,215 | Scale/Radius: 1.00 |
| 116 | `KC2_Asteroid` | 10475 | Object | 4005.18,427.27,-7384.82 | 91,359,480 | Scale/Radius: 7.00 |
| 117 | `KC2_Asteroid` | 10476 | Object | 3808.86,92.38,-6749.69 | 412,76,109 | Scale/Radius: 7.00 |
| 118 | `KC2_Asteroid` | 10477 | Object | 4501.74,-92.38,-7049.93 | 482,255,428 | Scale/Radius: 9.00 |
| 119 | `KC2_Asteroid` | 10478 | Object | 4813.53,265.60,-7303.99 | 335,135,335 | Scale/Radius: 1.00 |
| 120 | `KC2_Asteroid` | 10479 | Object | 4571.03,150.12,-7269.34 | 78,235,70 | Scale/Radius: 3.00 |
| 121 | `KC2_Asteroid` | 10480 | Object | 3993.63,461.92,-6530.28 | 387,359,30 | Scale/Radius: 5.00 |
| 122 | `KC2_Asteroid` | 10481 | Object | 4247.68,300.25,-7026.84 | 295,418,386 | Scale/Radius: 6.00 |
| 123 | `KC2_Asteroid` | 10482 | Object | 3889.70,519.66,-6749.69 | 357,252,327 | Scale/Radius: 8.00 |
| 124 | `KC2_Asteroid` | 10483 | Object | 4698.05,115.48,-7442.56 | 500,358,470 | Scale/Radius: 6.00 |
| 125 | `KC2_Asteroid` | 10484 | Object | 3901.25,-438.82,-7084.58 | 49,40,381 | Scale/Radius: 7.00 |
| 126 | `KC2_Asteroid` | 10486 | Object | 5266.28,-53.28,1426.10 | 153,93,276 | Scale/Radius: 5.00 |
| 127 | `KC2_Asteroid` | 10487 | Object | 5289.38,39.10,1148.95 | 68,480,93 | Scale/Radius: 3.00 |
| 128 | `KC2_Asteroid` | 10488 | Object | 4307.81,339.35,652.39 | 98,111,350 | Scale/Radius: 4.00 |
| 129 | `KC2_Asteroid` | 10489 | Object | 4792.82,96.84,317.50 | 440,139,357 | Scale/Radius: 3.00 |
| 130 | `KC2_Asteroid` | 10490 | Object | 5173.90,-76.38,675.48 | 298,323,148 | Scale/Radius: 4.00 |
| 131 | `KC2_Asteroid` | 10491 | Object | 4457.93,-238.05,444.53 | 143,265,55 | Scale/Radius: 5.00 |
| 132 | `KC2_Asteroid` | 10492 | Object | 4377.09,616.50,560.00 | 249,159,20 | Scale/Radius: 4.00 |
| 133 | `KC2_Asteroid` | 10493 | Object | 4169.23,570.30,1391.45 | 217,456,63 | Scale/Radius: 4.00 |
| 134 | `KC2_Asteroid` | 10494 | Object | 4457.93,-76.38,1206.69 | 239,426,162 | Scale/Radius: 9.00 |
| 135 | `KC2_Asteroid` | 10495 | Object | 4446.38,39.10,1426.10 | 326,89,349 | Scale/Radius: 3.00 |
| 136 | `KC2_Asteroid` | 10496 | Object | 4885.20,293.15,941.09 | 299,80,95 | Scale/Radius: 4.00 |
| 137 | `KC2_Asteroid` | 10497 | Object | 4284.71,281.61,386.79 | 271,200,472 | Scale/Radius: 2.00 |
| 138 | `KC2_Asteroid` | 10498 | Object | 4527.22,674.23,1287.52 | 302,417,338 | Scale/Radius: 4.00 |
| 139 | `KC2_Asteroid` | 10499 | Object | 5220.09,-307.34,606.20 | 236,478,256 | Scale/Radius: 7.00 |
| 140 | `KC2_Asteroid` | 10500 | Object | 4711.98,789.71,1183.59 | 185,502,176 | Scale/Radius: 2.00 |
| 141 | `KC2_Asteroid` | 10501 | Object | 4365.55,755.07,1172.04 | 246,25,282 | Scale/Radius: 7.00 |
| 142 | `KC2_Asteroid` | 10502 | Object | 5035.33,-203.41,790.96 | 182,70,417 | Scale/Radius: 7.00 |
| 143 | `KC2_Asteroid` | 10503 | Object | 4792.82,-134.12,756.32 | 42,409,441 | Scale/Radius: 5.00 |
| 144 | `KC2_Asteroid` | 10504 | Object | 4711.98,235.41,1218.24 | 286,184,469 | Scale/Radius: 1.00 |
| 145 | `KC2_Asteroid` | 10505 | Object | 4954.49,362.44,663.94 | 338,470,271 | Scale/Radius: 7.00 |
| 146 | `KC2_Asteroid` | 10507 | Object | 7055.18,-163.27,-394.03 | 502,121,179 | Scale/Radius: 5.00 |
| 147 | `KC2_Asteroid` | 10508 | Object | 6466.24,-913.88,-267.00 | 178,9,82 | Scale/Radius: 5.00 |
| 148 | `KC2_Asteroid` | 10509 | Object | 7193.75,-509.71,668.38 | 476,326,411 | Scale/Radius: 1.00 |
| 149 | `KC2_Asteroid` | 10510 | Object | 7020.54,-13.15,218.01 | 59,373,459 | Scale/Radius: 6.00 |
| 150 | `KC2_Asteroid` | 10511 | Object | 6720.29,-960.07,137.17 | 279,156,430 | Scale/Radius: 1.00 |
| 151 | `KC2_Asteroid` | 10512 | Object | 7320.78,-1006.27,-324.74 | 418,227,494 | Scale/Radius: 2.00 |
| 152 | `KC2_Asteroid` | 10513 | Object | 7124.47,-486.61,-451.77 | 100,265,200 | Scale/Radius: 2.00 |
| 153 | `KC2_Asteroid` | 10514 | Object | 7008.99,-625.18,-24.50 | 92,267,491 | Scale/Radius: 2.00 |
| 154 | `KC2_Asteroid` | 10515 | Object | 7228.40,-625.18,-174.62 | 364,251,121 | Scale/Radius: 6.00 |
| 155 | `KC2_Asteroid` | 10516 | Object | 6997.44,-232.56,229.56 | 251,229,323 | Scale/Radius: 5.00 |
| 156 | `KC2_Asteroid` | 10517 | Object | 7286.14,-197.91,483.61 | 29,301,291 | Scale/Radius: 1.00 |
| 157 | `KC2_Asteroid` | 10518 | Object | 6431.59,-440.42,-163.07 | 47,20,59 | Scale/Radius: 5.00 |
| 158 | `KC2_Asteroid` | 10519 | Object | 7101.37,-509.71,-301.65 | 412,462,438 | Scale/Radius: 3.00 |
| 159 | `KC2_Asteroid` | 10520 | Object | 6962.80,-555.90,587.54 | 387,357,313 | Scale/Radius: 5.00 |
| 160 | `KC2_Asteroid` | 10521 | Object | 6916.60,-925.43,-59.14 | 10,362,146 | Scale/Radius: 4.00 |
| 161 | `KC2_Asteroid` | 10522 | Object | 6373.85,-740.66,-163.07 | 341,268,37 | Scale/Radius: 7.00 |
| 162 | `KC2_Asteroid` | 10523 | Object | 7055.18,-1052.46,-370.93 | 319,489,488 | Scale/Radius: 1.00 |
| 163 | `KC2_Asteroid` | 10524 | Object | 7401.62,21.50,218.01 | 113,485,130 | Scale/Radius: 7.00 |
| 164 | `KC2_Asteroid` | 10525 | Object | 7505.55,-221.01,-116.88 | 496,330,227 | Scale/Radius: 3.00 |
| 165 | `KC2_Asteroid` | 10526 | Object | 7112.92,-428.87,148.72 | 499,111,447 | Scale/Radius: 5.00 |
| 166 | `KC2_Asteroid` | 10528 | Object | 6965.94,423.84,2100.19 | 22,123,94 | Scale/Radius: 5.00 |
| 167 | `KC2_Asteroid` | 10529 | Object | 7081.42,389.20,3035.57 | 8,397,174 | Scale/Radius: 1.00 |
| 168 | `KC2_Asteroid` | 10530 | Object | 7231.54,204.43,3093.31 | 158,10,83 | Scale/Radius: 2.00 |
| 169 | `KC2_Asteroid` | 10531 | Object | 6781.17,31.21,2400.43 | 212,201,283 | Scale/Radius: 8.00 |
| 170 | `KC2_Asteroid` | 10532 | Object | 7081.42,816.47,2261.86 | 239,77,459 | Scale/Radius: 6.00 |
| 171 | `KC2_Asteroid` | 10533 | Object | 6388.54,-165.10,2296.50 | 29,24,446 | Scale/Radius: 7.00 |
| 172 | `KC2_Asteroid` | 10534 | Object | 7277.73,493.13,2908.54 | 166,292,179 | Scale/Radius: 9.00 |
| 173 | `KC2_Asteroid` | 10535 | Object | 7058.32,493.13,2666.04 | 484,315,43 | Scale/Radius: 4.00 |
| 174 | `KC2_Asteroid` | 10536 | Object | 6400.09,-26.53,2111.74 | 53,447,350 | Scale/Radius: 6.00 |
| 175 | `KC2_Asteroid` | 10537 | Object | 6215.32,77.41,2977.83 | 464,429,430 | Scale/Radius: 3.00 |
| 176 | `KC2_Asteroid` | 10538 | Object | 6423.19,42.76,2619.84 | 252,108,125 | Scale/Radius: 1.00 |
| 177 | `KC2_Asteroid` | 10539 | Object | 7312.38,747.18,2331.15 | 62,175,212 | Scale/Radius: 7.00 |
| 178 | `KC2_Asteroid` | 10540 | Object | 6989.03,227.53,3012.47 | 190,247,113 | Scale/Radius: 6.00 |
| 179 | `KC2_Asteroid` | 10541 | Object | 7219.99,851.12,3139.50 | 120,330,247 | Scale/Radius: 4.00 |
| 180 | `KC2_Asteroid` | 10542 | Object | 6527.12,285.27,2862.35 | 125,67,86 | Scale/Radius: 5.00 |
| 181 | `KC2_Asteroid` | 10543 | Object | 7104.51,677.90,2157.93 | 224,424,217 | Scale/Radius: 2.00 |
| 182 | `KC2_Asteroid` | 10544 | Object | 6342.35,573.97,2920.09 | 224,92,327 | Scale/Radius: 3.00 |
| 183 | `KC2_Asteroid` | 10545 | Object | 6411.64,-269.03,2481.27 | 133,148,491 | Scale/Radius: 3.00 |
| 184 | `KC2_Asteroid` | 10546 | Object | 7012.13,250.62,2261.86 | 345,91,154 | Scale/Radius: 8.00 |
| 185 | `KC2_Asteroid` | 10547 | Object | 7335.47,19.67,2689.13 | 1,287,155 | Scale/Radius: 7.00 |
| 186 | `KC2_Asteroid` | 10549 | Object | -5222.77,-1796.90,1203.09 | 356,405,39 | Scale/Radius: 6.00 |
| 187 | `KC2_Asteroid` | 10550 | Object | -4726.21,-1866.19,1358.29 | 460,499,117 | Scale/Radius: 9.00 |
| 188 | `KC2_Asteroid` | 10551 | Object | -4495.25,-2235.72,803.99 | 183,383,53 | Scale/Radius: 4.00 |
| 189 | `KC2_Asteroid` | 10552 | Object | -4599.18,-1427.37,881.60 | 98,389,262 | Scale/Radius: 1.00 |
| 190 | `KC2_Asteroid` | 10553 | Object | -4437.51,-2154.88,1092.23 | 451,95,360 | Scale/Radius: 3.00 |
| 191 | `KC2_Asteroid` | 10554 | Object | -4656.92,-1658.32,1103.32 | 451,90,242 | Scale/Radius: 4.00 |
| 192 | `KC2_Asteroid` | 10555 | Object | -4807.05,-1358.08,737.48 | 285,145,158 | Scale/Radius: 1.00 |
| 193 | `KC2_Asteroid` | 10556 | Object | -4853.24,-2339.65,1214.18 | 424,191,385 | Scale/Radius: 7.00 |
| 194 | `KC2_Asteroid` | 10557 | Object | -4472.16,-2050.95,815.08 | 370,335,414 | Scale/Radius: 9.00 |
| 195 | `KC2_Asteroid` | 10558 | Object | -5465.28,-1531.30,826.17 | 435,308,219 | Scale/Radius: 9.00 |
| 196 | `KC2_Asteroid` | 10559 | Object | -4425.96,-2305.01,1247.43 | 14,510,358 | Scale/Radius: 3.00 |
| 197 | `KC2_Asteroid` | 10560 | Object | -4899.43,-1681.42,726.39 | 329,311,96 | Scale/Radius: 5.00 |
| 198 | `KC2_Asteroid` | 10561 | Object | -4795.50,-1923.93,1635.44 | 287,35,256 | Scale/Radius: 4.00 |
| 199 | `KC2_Asteroid` | 10562 | Object | -5315.15,-1450.46,1291.78 | 417,242,142 | Scale/Radius: 2.00 |
| 200 | `KC2_Asteroid` | 10563 | Object | -5419.08,-1750.71,1225.26 | 354,41,340 | Scale/Radius: 4.00 |
| 201 | `KC2_Asteroid` | 10564 | Object | -5245.87,-2432.03,759.65 | 492,366,384 | Scale/Radius: 4.00 |
| 202 | `KC2_Asteroid` | 10565 | Object | -5245.87,-1669.87,1247.43 | 294,60,138 | Scale/Radius: 1.00 |
| 203 | `KC2_Asteroid` | 10566 | Object | -4945.62,-1843.09,781.82 | 483,200,204 | Scale/Radius: 7.00 |
| 204 | `KC2_Asteroid` | 10567 | Object | -5349.80,-1692.97,1336.12 | 214,117,153 | Scale/Radius: 2.00 |
| 205 | `KC2_Asteroid` | 10568 | Object | -5303.61,-2305.01,870.51 | 77,62,256 | Scale/Radius: 8.00 |
| 206 | `KC2_Asteroid` | 10570 | Object | -9002.46,57.74,1314.12 | 201,130,504 | Scale/Radius: 5.00 |
| 207 | `KC2_Asteroid` | 10571 | Object | -9002.46,-277.15,690.54 | 299,121,250 | Scale/Radius: 7.00 |
| 208 | `KC2_Asteroid` | 10572 | Object | -9602.95,369.53,1614.37 | 356,72,1 | Scale/Radius: 5.00 |
| 209 | `KC2_Asteroid` | 10573 | Object | -9395.09,242.51,1498.89 | 437,293,407 | Scale/Radius: 3.00 |
| 210 | `KC2_Asteroid` | 10574 | Object | -9984.03,334.89,1660.56 | 478,197,1 | Scale/Radius: 7.00 |
| 211 | `KC2_Asteroid` | 10575 | Object | -9891.65,265.60,1360.31 | 201,229,369 | Scale/Radius: 9.00 |
| 212 | `KC2_Asteroid` | 10576 | Object | -8910.08,184.77,1267.93 | 336,30,183 | Scale/Radius: 1.00 |
| 213 | `KC2_Asteroid` | 10577 | Object | -9117.94,334.89,1140.90 | 106,155,153 | Scale/Radius: 1.00 |
| 214 | `KC2_Asteroid` | 10578 | Object | -9556.76,-207.86,1371.86 | 104,288,291 | Scale/Radius: 5.00 |
| 215 | `KC2_Asteroid` | 10579 | Object | -9972.49,11.55,967.69 | 317,461,60 | Scale/Radius: 2.00 |
| 216 | `KC2_Asteroid` | 10580 | Object | -8944.72,265.60,1637.46 | 413,344,203 | Scale/Radius: 7.00 |
| 217 | `KC2_Asteroid` | 10581 | Object | -9014.01,346.44,794.47 | 375,408,333 | Scale/Radius: 7.00 |
| 218 | `KC2_Asteroid` | 10582 | Object | -9256.52,-173.22,898.40 | 230,402,29 | Scale/Radius: 3.00 |
| 219 | `KC2_Asteroid` | 10583 | Object | -9475.93,-334.89,806.01 | 236,504,506 | Scale/Radius: 3.00 |
| 220 | `KC2_Asteroid` | 10584 | Object | -9106.39,-392.63,1637.46 | 171,408,206 | Scale/Radius: 5.00 |
| 221 | `KC2_Asteroid` | 10585 | Object | -9406.64,404.18,1279.48 | 486,28,459 | Scale/Radius: 6.00 |
| 222 | `KC2_Asteroid` | 10586 | Object | -9602.95,-265.60,829.11 | 334,276,51 | Scale/Radius: 6.00 |
| 223 | `KC2_Asteroid` | 10587 | Object | -9291.16,69.29,1164.00 | 106,328,377 | Scale/Radius: 3.00 |
| 224 | `KC2_Asteroid` | 10588 | Object | -8967.82,-554.30,1129.36 | 170,78,435 | Scale/Radius: 3.00 |
| 225 | `KC2_Asteroid` | 10589 | Object | -9799.27,-242.51,1602.82 | 504,453,507 | Scale/Radius: 2.00 |
| 226 | `KC2_Asteroid` | 10591 | Object | -7020.40,1677.81,2988.84 | 292,487,92 | Scale/Radius: 1.00 |
| 227 | `KC2_Asteroid` | 10592 | Object | -7551.61,1689.36,2399.90 | 161,109,98 | Scale/Radius: 6.00 |
| 228 | `KC2_Asteroid` | 10593 | Object | -7424.58,1435.31,2896.46 | 439,74,13 | Scale/Radius: 6.00 |
| 229 | `KC2_Asteroid` | 10594 | Object | -6777.90,2035.80,2769.43 | 15,402,270 | Scale/Radius: 6.00 |
| 230 | `KC2_Asteroid` | 10595 | Object | -7205.17,1042.68,2446.09 | 196,297,97 | Scale/Radius: 1.00 |
| 231 | `KC2_Asteroid` | 10596 | Object | -6570.04,1423.76,2226.68 | 114,337,464 | Scale/Radius: 1.00 |
| 232 | `KC2_Asteroid` | 10597 | Object | -7089.69,1100.42,2238.23 | 179,356,429 | Scale/Radius: 6.00 |
| 233 | `KC2_Asteroid` | 10598 | Object | -7436.13,1111.96,3150.51 | 302,284,43 | Scale/Radius: 7.00 |
| 234 | `KC2_Asteroid` | 10599 | Object | -6766.35,1169.70,2399.90 | 206,122,305 | Scale/Radius: 1.00 |
| 235 | `KC2_Asteroid` | 10600 | Object | -7239.82,1643.17,2192.04 | 265,50,460 | Scale/Radius: 6.00 |
| 236 | `KC2_Asteroid` | 10601 | Object | -7274.46,1885.67,2423.00 | 468,181,420 | Scale/Radius: 3.00 |
| 237 | `KC2_Asteroid` | 10602 | Object | -7482.32,1954.96,3000.39 | 68,285,212 | Scale/Radius: 3.00 |
| 238 | `KC2_Asteroid` | 10603 | Object | -6743.25,1435.31,2757.89 | 431,183,134 | Scale/Radius: 5.00 |
| 239 | `KC2_Asteroid` | 10604 | Object | -7574.70,1700.91,2884.91 | 277,442,281 | Scale/Radius: 9.00 |
| 240 | `KC2_Asteroid` | 10605 | Object | -6731.71,1724.00,2168.94 | 113,188,301 | Scale/Radius: 2.00 |
| 241 | `KC2_Asteroid` | 10606 | Object | -6928.02,1204.35,2203.59 | 155,0,262 | Scale/Radius: 9.00 |
| 242 | `KC2_Asteroid` | 10607 | Object | -7447.68,2139.73,3011.94 | 81,324,185 | Scale/Radius: 4.00 |
| 243 | `KC2_Asteroid` | 10608 | Object | -7274.46,1366.02,2330.61 | 201,479,484 | Scale/Radius: 4.00 |
| 244 | `KC2_Asteroid` | 10609 | Object | -6604.68,1077.32,2134.30 | 58,317,16 | Scale/Radius: 5.00 |
| 245 | `KC2_Asteroid` | 10610 | Object | -7343.75,1908.77,3138.97 | 102,41,502 | Scale/Radius: 5.00 |
| 246 | `KC2_Asteroid` | 10612 | Object | -482.36,-438.82,7772.23 | 509,26,158 | Scale/Radius: 3.00 |
| 247 | `KC2_Asteroid` | 10613 | Object | -170.57,34.64,7633.65 | 375,23,168 | Scale/Radius: 3.00 |
| 248 | `KC2_Asteroid` | 10614 | Object | -493.91,-288.70,7864.61 | 49,136,133 | Scale/Radius: 1.00 |
| 249 | `KC2_Asteroid` | 10615 | Object | -205.21,80.84,7853.06 | 69,184,451 | Scale/Radius: 5.00 |
| 250 | `KC2_Asteroid` | 10616 | Object | -205.21,127.03,8384.27 | 122,405,354 | Scale/Radius: 5.00 |
| 251 | `KC2_Asteroid` | 10617 | Object | -343.78,-392.63,7483.53 | 72,336,226 | Scale/Radius: 5.00 |
| 252 | `KC2_Asteroid` | 10618 | Object | 337.54,-69.29,8372.72 | 216,510,205 | Scale/Radius: 4.00 |
| 253 | `KC2_Asteroid` | 10619 | Object | -378.43,23.10,7344.95 | 186,201,475 | Scale/Radius: 1.00 |
| 254 | `KC2_Asteroid` | 10620 | Object | -89.73,-161.67,8453.55 | 9,64,176 | Scale/Radius: 3.00 |
| 255 | `KC2_Asteroid` | 10621 | Object | -667.13,369.53,7599.01 | 115,363,111 | Scale/Radius: 7.00 |
| 256 | `KC2_Asteroid` | 10622 | Object | -563.20,0.00,7402.69 | 215,42,210 | Scale/Radius: 1.00 |
| 257 | `KC2_Asteroid` | 10623 | Object | -332.24,138.57,8003.19 | 363,81,445 | Scale/Radius: 3.00 |
| 258 | `KC2_Asteroid` | 10624 | Object | -343.78,-369.53,7749.13 | 219,132,4 | Scale/Radius: 2.00 |
| 259 | `KC2_Asteroid` | 10625 | Object | 314.45,-150.12,8257.24 | 295,338,168 | Scale/Radius: 6.00 |
| 260 | `KC2_Asteroid` | 10626 | Object | -597.84,357.99,8107.12 | 332,119,508 | Scale/Radius: 1.00 |
| 261 | `KC2_Asteroid` | 10627 | Object | -747.96,-80.84,7483.53 | 169,117,442 | Scale/Radius: 3.00 |
| 262 | `KC2_Asteroid` | 10628 | Object | -736.41,-346.44,8361.17 | 297,435,460 | Scale/Radius: 5.00 |
| 263 | `KC2_Asteroid` | 10629 | Object | -343.78,-127.03,7471.98 | 464,306,474 | Scale/Radius: 4.00 |
| 264 | `KC2_Asteroid` | 10630 | Object | -159.02,196.31,8130.21 | 22,263,213 | Scale/Radius: 3.00 |
| 265 | `KC2_Asteroid` | 10631 | Object | -747.96,-346.44,7437.34 | 456,65,132 | Scale/Radius: 8.00 |
| 266 | `KC2_Asteroid` | 10633 | Object | 1448.60,-712.42,8127.73 | 123,495,171 | Scale/Radius: 3.00 |
| 267 | `KC2_Asteroid` | 10634 | Object | 1344.67,-1324.46,8023.80 | 347,118,402 | Scale/Radius: 3.00 |
| 268 | `KC2_Asteroid` | 10635 | Object | 1668.01,-747.07,8416.43 | 356,384,318 | Scale/Radius: 1.00 |
| 269 | `KC2_Asteroid` | 10636 | Object | 1748.84,-550.75,7792.84 | 400,228,203 | Scale/Radius: 9.00 |
| 270 | `KC2_Asteroid` | 10637 | Object | 1494.79,-1197.44,7896.77 | 6,156,248 | Scale/Radius: 3.00 |
| 271 | `KC2_Asteroid` | 10638 | Object | 1148.35,-481.47,7354.02 | 143,411,165 | Scale/Radius: 7.00 |
| 272 | `KC2_Asteroid` | 10639 | Object | 1852.77,-1382.20,7827.48 | 487,23,309 | Scale/Radius: 1.00 |
| 273 | `KC2_Asteroid` | 10640 | Object | 2176.12,-1093.50,8300.95 | 285,227,273 | Scale/Radius: 9.00 |
| 274 | `KC2_Asteroid` | 10641 | Object | 2072.18,-585.40,8370.24 | 325,100,120 | Scale/Radius: 1.00 |
| 275 | `KC2_Asteroid` | 10642 | Object | 1437.05,-481.47,7919.87 | 193,291,252 | Scale/Radius: 2.00 |
| 276 | `KC2_Asteroid` | 10643 | Object | 1656.46,-354.44,7388.66 | 419,269,6 | Scale/Radius: 6.00 |
| 277 | `KC2_Asteroid` | 10644 | Object | 1656.46,-504.56,8370.24 | 298,346,187 | Scale/Radius: 2.00 |
| 278 | `KC2_Asteroid` | 10645 | Object | 1183.00,-943.38,7850.58 | 441,8,339 | Scale/Radius: 1.00 |
| 279 | `KC2_Asteroid` | 10646 | Object | 1598.72,-1324.46,7839.03 | 247,35,168 | Scale/Radius: 1.00 |
| 280 | `KC2_Asteroid` | 10647 | Object | 1183.00,-874.09,8462.62 | 316,93,454 | Scale/Radius: 8.00 |
| 281 | `KC2_Asteroid` | 10648 | Object | 1910.51,-365.99,7584.98 | 366,151,252 | Scale/Radius: 1.00 |
| 282 | `KC2_Asteroid` | 10649 | Object | 2176.12,-943.38,7423.31 | 464,82,205 | Scale/Radius: 8.00 |
| 283 | `KC2_Asteroid` | 10650 | Object | 1818.13,-851.00,8139.28 | 37,477,163 | Scale/Radius: 1.00 |
| 284 | `KC2_Asteroid` | 10651 | Object | 1737.30,-885.64,8370.24 | 414,450,224 | Scale/Radius: 3.00 |
| 285 | `KC2_Asteroid` | 10652 | Object | 1818.13,-781.71,7885.22 | 373,14,209 | Scale/Radius: 1.00 |
| 286 | `KC2_Asteroid` | 10654 | Object | 892.90,1310.63,9487.85 | 143,26,280 | Scale/Radius: 1.00 |
| 287 | `KC2_Asteroid` | 10655 | Object | 546.46,721.68,10457.87 | 153,74,141 | Scale/Radius: 1.00 |
| 288 | `KC2_Asteroid` | 10656 | Object | 407.89,1345.27,9499.40 | 321,471,38 | Scale/Radius: 2.00 |
| 289 | `KC2_Asteroid` | 10657 | Object | 788.97,1657.07,9845.83 | 362,404,483 | Scale/Radius: 3.00 |
| 290 | `KC2_Asteroid` | 10658 | Object | 465.62,1530.04,10353.94 | 387,15,406 | Scale/Radius: 2.00 |
| 291 | `KC2_Asteroid` | 10659 | Object | 904.45,1472.30,9868.93 | 106,193,202 | Scale/Radius: 7.00 |
| 292 | `KC2_Asteroid` | 10660 | Object | 1077.66,952.64,9961.31 | 92,233,344 | Scale/Radius: 5.00 |
| 293 | `KC2_Asteroid` | 10661 | Object | 962.18,1241.34,10388.58 | 242,496,245 | Scale/Radius: 2.00 |
| 294 | `KC2_Asteroid` | 10662 | Object | 1331.72,1541.59,9499.40 | 330,299,501 | Scale/Radius: 5.00 |
| 295 | `KC2_Asteroid` | 10663 | Object | 1239.33,594.66,9568.68 | 207,241,203 | Scale/Radius: 5.00 |
| 296 | `KC2_Asteroid` | 10664 | Object | 846.71,606.21,10053.70 | 166,421,21 | Scale/Radius: 9.00 |
| 297 | `KC2_Asteroid` | 10665 | Object | 465.62,1206.70,10377.04 | 308,287,213 | Scale/Radius: 1.00 |
| 298 | `KC2_Asteroid` | 10666 | Object | 1170.05,964.19,10423.23 | 52,458,161 | Scale/Radius: 9.00 |
| 299 | `KC2_Asteroid` | 10667 | Object | 627.30,1068.12,9984.41 | 356,505,495 | Scale/Radius: 7.00 |
| 300 | `KC2_Asteroid` | 10668 | Object | 1331.72,1518.49,9938.22 | 330,489,22 | Scale/Radius: 8.00 |
| 301 | `KC2_Asteroid` | 10669 | Object | 1146.95,652.40,9534.04 | 326,78,356 | Scale/Radius: 2.00 |
| 302 | `KC2_Asteroid` | 10670 | Object | 1170.05,548.47,10515.61 | 401,132,492 | Scale/Radius: 9.00 |
| 303 | `KC2_Asteroid` | 10671 | Object | 638.84,825.62,10504.06 | 69,31,124 | Scale/Radius: 3.00 |
| 304 | `KC2_Asteroid` | 10672 | Object | 719.68,1264.44,10538.71 | 509,348,416 | Scale/Radius: 5.00 |
| 305 | `KC2_Asteroid` | 10673 | Object | 1262.43,1287.53,9661.07 | 331,408,510 | Scale/Radius: 1.00 |
| 306 | `Arena_Bouy1` | 10674 | Object | 3126.21,0.00,1654.04 | 0,0,0 | Scale/Radius: 1.00 |
| 307 | `Arena_Bouy1` | 10675 | Object | 3077.21,0.00,1229.07 | 0,0,0 | Scale/Radius: 1.00 |
| 308 | `Arena_Bouy1` | 10676 | Object | 3077.21,0.00,750.98 | 0,0,0 | Scale/Radius: 1.00 |
| 309 | `Arena_Bouy1` | 10677 | Object | 1117.56,0.00,5425.65 | 0,0,0 | Scale/Radius: 1.00 |
| 310 | `Arena_Bouy1` | 10678 | Object | 578.65,0.00,5425.65 | 0,0,0 | Scale/Radius: 1.00 |
| 311 | `Arena_Bouy1` | 10679 | Object | 88.74,0.00,5478.77 | 0,0,0 | Scale/Radius: 1.00 |
| 312 | `Arena_Bouy1` | 10680 | Object | -3046.71,0.00,2185.25 | 0,0,0 | Scale/Radius: 1.00 |
| 313 | `Arena_Bouy1` | 10681 | Object | -3046.71,0.00,1654.04 | 0,0,0 | Scale/Radius: 1.00 |
| 314 | `Arena_Bouy1` | 10682 | Object | -3046.71,0.00,1175.95 | 0,0,0 | Scale/Radius: 1.00 |
| 315 | `Arena_Bouy1` | 10683 | Object | 3077.21,0.00,-2436.30 | 0,0,0 | Scale/Radius: 1.00 |
| 316 | `Arena_Bouy1` | 10684 | Object | 2734.27,0.00,-2755.02 | 0,0,0 | Scale/Radius: 1.00 |
| 317 | `Arena_Bouy1` | 10685 | Object | 2391.33,0.00,-3126.87 | 0,0,0 | Scale/Radius: 1.00 |
| 318 | `Arena_Bouy1` | 10686 | Object | -3389.65,0.00,-2330.05 | 0,0,0 | Scale/Radius: 1.00 |
| 319 | `Arena_Bouy1` | 10687 | Object | -3144.69,0.00,-2701.90 | 0,0,0 | Scale/Radius: 1.00 |
| 320 | `Arena_Bouy1` | 10688 | Object | -2948.73,0.00,-2967.51 | 0,0,0 | Scale/Radius: 1.00 |
| 321 | `Arena_Bouy1` | 10690 | Object | -3438.64,0.00,1388.43 | 0,0,0 | Scale/Radius: 1.00 |
| 322 | `Arena_Bouy1` | 10691 | Object | -3438.64,0.00,1866.53 | 0,0,0 | Scale/Radius: 1.00 |
| 323 | `Arena_Bouy1` | 10693 | Object | 3371.16,0.00,1388.43 | 0,0,0 | Scale/Radius: 1.00 |
| 324 | `Arena_Bouy1` | 10694 | Object | 3371.16,0.00,963.46 | 0,0,0 | Scale/Radius: 1.00 |
| 325 | `Arena_Bouy1` | 10695 | Object | -3585.62,0.00,-2701.90 | 0,0,0 | Scale/Radius: 1.00 |
| 326 | `Arena_Bouy1` | 10696 | Object | -3340.66,0.00,-3020.63 | 0,0,0 | Scale/Radius: 1.00 |
| 327 | `Arena_Bouy1` | 10697 | Object | 2881.25,0.00,-3233.11 | 0,0,0 | Scale/Radius: 1.00 |
| 328 | `Arena_Bouy1` | 10698 | Object | 3175.20,0.00,-2914.39 | 0,0,0 | Scale/Radius: 1.00 |
| 329 | `Arena_Bouy1` | 10699 | Object | 333.70,0.00,5850.62 | 0,0,0 | Scale/Radius: 1.00 |
| 330 | `Arena_Bouy1` | 10700 | Object | 872.60,0.00,5797.50 | 0,0,0 | Scale/Radius: 1.00 |
| 331 | `Navigational_Bouy` | 10701 | Interactive | 3692.55,0.00,1186.57 | 0,0,0 | None |
| 332 | `Navigational_Bouy` | 10702 | Interactive | -3803.14,0.00,1664.66 | 0,0,0 | None |
| 333 | `Spcargo_Credits` | 10986 | Interactive | -84.01,-1200.00,1088.67 | 4,247,247 | secondary groups: CONT_070, none |
| 334 | `GalSpan_Research_Facility` | 8927 | Interactive | -90.78,0.00,1088.67 | 0,0,0 | None |
