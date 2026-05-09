# Tachyon: The Fringe DISP01.SPX - The Grand Plan; Saving Spike; Fleet Battle

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP01.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `DISPUT1.BDF` |
| Region | 6 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 7 |
| Entities | 273 |
| Events | 6 |
| Waypoints | 0 |
| Child Sectors | 5 |
| Scripts | 2 |
| Scenes | 3 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Disputed_Bora_Base_Mine`, `1: DisputB_StarBase`, `2: Roid_Sm_Brown2`, `3: Roid_Sm_Brown`, `4: Navigational_Bouy`, `5: Mega_Gate`, `6: Hyper_Gate` |
| Scripts | `ANNAH.SCR`, `PLAYER.SCR` |
| Scenes | `D01BC10.SEN`, `D1DOC01.SEN`, `RIP2BOR.SEN` |
| Labels | `TNSA`, `SPIKE`, `capb` |
| Aliases | `BC10_Claymore4`, `BC10_Claymore1`, `BC10_Claymore3`, `BC10_Claymore2`, `BC10_Waraxe`, `tnsa`, `BC10_Mace4`, `BC10_Mace2`, `BC10_Mace1`, `BC10_Mace3`, `BC10_Warhammer3`, `BC10_Warhammer2`, `BC10_Warhammer4`, `BC10_Warhammer1`, `SPIKE`, `Stocks01` |
| Groups | `LIBERTY_STARBASE` |
| Child Sectors | [disp01A.spx](DISP01A.md), [disp01B.spx](DISP01B.md), [disp01C.spx](DISP01C.md), [disp01D.spx](DISP01D.md), [disp01E.spx](DISP01E.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 2011

**Action**

- Broadcast HUD contact action: contact/list 0, subtype 0, param 9
- Set runtime trigger variable: variable group 20, variable 1, subtype 0, value 0
- Gate state/action: param 9, subtype 3, param 0
- Mission objective/state: param 393218, subtype 0, param 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 5
- Variable comparison: subject variable group 0, variable 4, op 1, value 2011

**Action**

- Play dialog: ANNAH.SCR, line/variant 0
- Set runtime trigger variable: variable group 20, variable 1, subtype 1, value 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 2010

**Action**

- Mission objective/state: param 393218, subtype 0, param 0

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4018

**Action**

- Mission objective/state: param 393217, subtype 0, param 0
- Gate state/action: param 9, subtype 3, param 0
- Play dialog: PLAYER.SCR, line/variant 97

### Event 4

**Trigger**

- Variable comparison: subject variable group 18, variable 407, op 0, value 2

**Action**

- Set/add variable: variable group 22, variable 18, subtype 0, value 1

### Event 5

**Trigger**

- Variable comparison: subject variable group 18, variable 409, op 0, value 2

**Action**

- Set/add variable: variable group 22, variable 17, subtype 0, value 1

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 8 | Gate | 2.12,312.17,-3431.17 | 434,507,0 | Gate SPX: [disp02.spx](DISP02.md) |
| 1 | `Mega_Gate` | 9 | Gate | -869.39,1442.93,-2328.16 | 477,470,0 | Gate SPX: [bora08.spx](BORA08.md) |
| 2 | `none` | 490 | Marker | 53.54,186.54,-2543.19 | 0,0,0 | None |
| 3 | `Navigational_Bouy` | 501 | Interactive | 80.44,630.43,-2853.46 | 0,0,0 | secondary groups: none, LIBERTY_STARBASE |
| 4 | `Roid_Sm_Brown` | 469 | Object | 4742.79,-1923.84,3141.80 | 63,386,407 | Scale/Radius: 1.00 |
| 5 | `Roid_Sm_Brown` | 205 | Object | 3836.57,-2296.40,2125.02 | 324,434,458 | Scale/Radius: 1.00 |
| 6 | `Roid_Sm_Brown` | 207 | Object | 3767.00,-2287.43,2163.89 | 445,172,478 | Scale/Radius: 1.00 |
| 7 | `Roid_Sm_Brown` | 209 | Object | 3848.16,-2307.20,2170.65 | 6,26,232 | Scale/Radius: 1.00 |
| 8 | `Roid_Sm_Brown` | 211 | Object | 3834.73,-2339.06,2125.31 | 69,405,162 | Scale/Radius: 1.00 |
| 9 | `Roid_Sm_Brown` | 213 | Object | 3770.66,-2303.36,2059.40 | 317,266,229 | Scale/Radius: 1.00 |
| 10 | `Roid_Sm_Brown` | 216 | Object | 3893.32,-2318.92,2126.71 | 256,455,405 | Scale/Radius: 1.00 |
| 11 | `Roid_Sm_Brown` | 218 | Object | 3842.06,-2306.47,2060.24 | 135,71,400 | Scale/Radius: 1.00 |
| 12 | `Roid_Sm_Brown` | 220 | Object | 3746.86,-2286.70,2087.28 | 279,306,37 | Scale/Radius: 1.00 |
| 13 | `Roid_Sm_Brown` | 222 | Object | 3862.20,-2253.38,2156.57 | 77,70,248 | Scale/Radius: 1.00 |
| 14 | `Roid_Sm_Brown` | 224 | Object | 3836.26,-2264.36,2243.88 | 490,444,340 | Scale/Radius: 1.00 |
| 15 | `Roid_Sm_Brown` | 226 | Object | 3792.02,-2259.79,2062.22 | 377,219,394 | Scale/Radius: 1.00 |
| 16 | `Roid_Sm_Brown` | 228 | Object | 3862.20,-2378.60,2257.97 | 91,505,304 | Scale/Radius: 1.00 |
| 17 | `Roid_Sm_Brown` | 230 | Object | 3873.18,-2294.02,2224.17 | 170,11,356 | Scale/Radius: 1.00 |
| 18 | `Roid_Sm_Brown` | 232 | Object | 3761.50,-2308.30,2269.80 | 372,227,154 | Scale/Radius: 1.00 |
| 19 | `Roid_Sm_Brown` | 234 | Object | 3686.14,-2255.39,2186.43 | 358,54,48 | Scale/Radius: 1.00 |
| 20 | `Roid_Sm_Brown` | 236 | Object | 3741.67,-2236.17,2172.62 | 51,420,219 | Scale/Radius: 1.00 |
| 21 | `Roid_Sm_Brown` | 238 | Object | 3818.87,-2386.29,2122.21 | 69,102,7 | Scale/Radius: 1.00 |
| 22 | `Roid_Sm_Brown` | 240 | Object | 3687.05,-2292.56,2101.93 | 117,276,497 | Scale/Radius: 1.00 |
| 23 | `Roid_Sm_Brown` | 242 | Object | 3691.93,-2206.14,2264.16 | 211,297,200 | Scale/Radius: 1.00 |
| 24 | `Roid_Sm_Brown` | 244 | Object | 3610.46,-2335.76,2161.64 | 453,206,493 | Scale/Radius: 1.00 |
| 25 | `Roid_Sm_Brown` | 246 | Object | 3615.96,-2301.16,2047.57 | 137,331,424 | Scale/Radius: 1.00 |
| 26 | `Roid_Sm_Brown` | 248 | Object | 3782.86,-2172.82,2373.45 | 163,291,294 | Scale/Radius: 1.00 |
| 27 | `Roid_Sm_Brown` | 250 | Object | 3746.25,-2169.16,1936.88 | 112,288,189 | Scale/Radius: 1.00 |
| 28 | `Roid_Sm_Brown` | 252 | Object | 4081.89,-2445.61,2114.32 | 403,351,397 | Scale/Radius: 1.00 |
| 29 | `Roid_Sm_Brown` | 254 | Object | 3923.83,-2409.54,2072.36 | 25,365,320 | Scale/Radius: 1.00 |
| 30 | `Roid_Sm_Brown` | 256 | Object | 3920.48,-2429.68,2140.52 | 141,489,38 | Scale/Radius: 1.00 |
| 31 | `Roid_Sm_Brown` | 258 | Object | 3878.67,-2430.23,2185.30 | 38,403,262 | Scale/Radius: 1.00 |
| 32 | `Roid_Sm_Brown` | 260 | Object | 3812.77,-2232.51,1823.65 | 47,24,230 | Scale/Radius: 1.00 |
| 33 | `Roid_Sm_Brown` | 262 | Object | 3728.55,-2340.16,2425.27 | 293,394,96 | Scale/Radius: 1.00 |
| 34 | `Roid_Sm_Brown` | 264 | Object | 4002.86,-2152.87,2263.04 | 265,128,294 | Scale/Radius: 1.00 |
| 35 | `Roid_Sm_Brown` | 266 | Object | 3578.43,-2488.45,2094.61 | 120,330,236 | Scale/Radius: 1.00 |
| 36 | `Roid_Sm_Brown` | 268 | Object | 3423.42,-2338.69,2206.14 | 172,241,87 | Scale/Radius: 1.00 |
| 37 | `Roid_Sm_Brown` | 270 | Object | 4030.01,-2161.84,2079.96 | 44,332,254 | Scale/Radius: 1.00 |
| 38 | `Roid_Sm_Brown` | 272 | Object | 3777.98,-2295.12,1772.39 | 400,248,9 | Scale/Radius: 1.00 |
| 39 | `Roid_Sm_Brown` | 274 | Object | 4127.66,-2052.91,2372.04 | 130,207,222 | Scale/Radius: 1.00 |
| 40 | `Roid_Sm_Brown` | 276 | Object | 3756.93,-2258.87,2017.15 | 406,407,83 | Scale/Radius: 1.00 |
| 41 | `Roid_Sm_Brown` | 278 | Object | 4138.64,-2335.03,1914.91 | 245,443,12 | Scale/Radius: 1.00 |
| 42 | `Roid_Sm_Brown` | 280 | Object | 3977.53,-2352.61,2090.66 | 145,342,342 | Scale/Radius: 1.00 |
| 43 | `Roid_Sm_Brown` | 282 | Object | 4148.41,-2355.72,2289.23 | 23,442,221 | Scale/Radius: 1.00 |
| 44 | `Roid_Sm_Brown` | 284 | Object | 4106.91,-2414.85,2035.46 | 308,205,153 | Scale/Radius: 1.00 |
| 45 | `Roid_Sm_Brown` | 286 | Object | 3712.07,-2052.36,2151.50 | 138,83,234 | Scale/Radius: 1.00 |
| 46 | `Roid_Sm_Brown` | 288 | Object | 3788.97,-2058.95,2328.94 | 475,263,60 | Scale/Radius: 1.00 |
| 47 | `Roid_Sm_Brown` | 290 | Object | 3584.53,-2299.33,2243.60 | 383,234,367 | Scale/Radius: 1.00 |
| 48 | `Roid_Sm_Brown` | 292 | Object | 4141.08,-2462.82,1767.32 | 22,416,342 | Scale/Radius: 1.00 |
| 49 | `Roid_Sm_Brown` | 294 | Object | 4182.58,-2079.46,1849.57 | 143,221,489 | Scale/Radius: 1.00 |
| 50 | `Roid_Sm_Brown` | 296 | Object | 3676.07,-2108.75,2170.65 | 89,98,322 | Scale/Radius: 1.00 |
| 51 | `Roid_Sm_Brown` | 298 | Object | 3399.93,-2164.40,2326.41 | 511,46,81 | Scale/Radius: 1.00 |
| 52 | `Roid_Sm_Brown` | 300 | Object | 3258.96,-2256.67,2409.22 | 224,404,386 | Scale/Radius: 1.00 |
| 53 | `Roid_Sm_Brown` | 302 | Object | 4071.51,-2177.95,2472.03 | 66,318,0 | Scale/Radius: 1.00 |
| 54 | `Roid_Sm_Brown` | 304 | Object | 3796.29,-2032.95,2211.78 | 420,286,272 | Scale/Radius: 1.00 |
| 55 | `Roid_Sm_Brown` | 306 | Object | 4097.14,-2172.28,1761.97 | 162,324,134 | Scale/Radius: 1.00 |
| 56 | `Roid_Sm_Brown` | 308 | Object | 3472.55,-2319.65,2364.43 | 99,403,160 | Scale/Radius: 1.00 |
| 57 | `Roid_Sm_Brown` | 310 | Object | 4277.78,-2368.72,2198.82 | 240,411,478 | Scale/Radius: 1.00 |
| 58 | `Roid_Sm_Brown` | 312 | Object | 3743.20,-2074.33,1928.43 | 393,214,490 | Scale/Radius: 1.00 |
| 59 | `Roid_Sm_Brown` | 314 | Object | 4258.86,-2165.50,1849.57 | 428,34,160 | Scale/Radius: 1.00 |
| 60 | `Roid_Sm_Brown` | 316 | Object | 3356.29,-2436.09,2577.93 | 187,80,426 | Scale/Radius: 1.00 |
| 61 | `Roid_Sm_Brown` | 318 | Object | 3348.36,-2359.93,2768.33 | 411,63,175 | Scale/Radius: 1.00 |
| 62 | `Roid_Sm_Brown` | 320 | Object | 4022.39,-2411.56,1865.06 | 501,141,316 | Scale/Radius: 1.00 |
| 63 | `Roid_Sm_Brown` | 322 | Object | 4303.41,-2348.94,1768.45 | 448,34,374 | Scale/Radius: 1.00 |
| 64 | `Roid_Sm_Brown` | 324 | Object | 4012.93,-2348.94,2588.63 | 363,120,1 | Scale/Radius: 1.00 |
| 65 | `Roid_Sm_Brown` | 326 | Object | 3489.02,-2021.42,2114.89 | 252,342,314 | Scale/Radius: 1.00 |
| 66 | `Roid_Sm_Brown` | 328 | Object | 3212.27,-2412.66,2511.46 | 92,68,408 | Scale/Radius: 1.00 |
| 67 | `Roid_Sm_Brown` | 330 | Object | 4145.97,-2066.64,1387.65 | 452,168,22 | Scale/Radius: 1.00 |
| 68 | `Roid_Sm_Brown` | 332 | Object | 3750.21,-2365.24,1546.22 | 270,480,88 | Scale/Radius: 1.00 |
| 69 | `Roid_Sm_Brown` | 334 | Object | 4412.04,-2021.60,1797.74 | 139,5,263 | Scale/Radius: 1.00 |
| 70 | `Roid_Sm_Brown` | 336 | Object | 4148.41,-2584.01,2104.18 | 25,11,274 | Scale/Radius: 1.00 |
| 71 | `Roid_Sm_Brown` | 338 | Object | 3172.00,-1958.44,2224.17 | 472,49,8 | Scale/Radius: 1.00 |
| 72 | `Roid_Sm_Brown` | 340 | Object | 3183.59,-2022.70,1997.15 | 336,494,465 | Scale/Radius: 1.00 |
| 73 | `Roid_Sm_Brown` | 342 | Object | 3079.85,-2190.77,2380.21 | 84,95,403 | Scale/Radius: 1.00 |
| 74 | `Roid_Sm_Brown` | 344 | Object | 3581.48,-1892.72,2279.09 | 36,46,249 | Scale/Radius: 1.00 |
| 75 | `Roid_Sm_Brown` | 346 | Object | 3080.46,-1848.05,2313.73 | 130,286,401 | Scale/Radius: 1.00 |
| 76 | `Roid_Sm_Brown` | 348 | Object | 4837.99,-2586.21,2334.01 | 152,197,375 | Scale/Radius: 1.00 |
| 77 | `Roid_Sm_Brown` | 350 | Object | 4629.29,-2641.50,1537.21 | 305,15,400 | Scale/Radius: 1.00 |
| 78 | `Roid_Sm_Brown` | 352 | Object | 3630.91,-2761.96,2826.91 | 261,137,373 | Scale/Radius: 1.00 |
| 79 | `Roid_Sm_Brown` | 354 | Object | 3816.43,-2688.37,1592.98 | 307,480,457 | Scale/Radius: 1.00 |
| 80 | `Roid_Sm_Brown` | 356 | Object | 4023.91,-2690.93,2345.28 | 25,169,431 | Scale/Radius: 1.00 |
| 81 | `Roid_Sm_Brown` | 358 | Object | 3954.04,-2175.20,1819.43 | 198,62,228 | Scale/Radius: 1.00 |
| 82 | `Roid_Sm_Brown` | 360 | Object | 4290.60,-2679.58,2107.56 | 461,359,340 | Scale/Radius: 1.00 |
| 83 | `Roid_Sm_Brown` | 362 | Object | 4315.01,-2373.66,1295.55 | 297,388,233 | Scale/Radius: 1.00 |
| 84 | `Roid_Sm_Brown` | 364 | Object | 4836.77,-2697.52,1350.47 | 411,62,57 | Scale/Radius: 1.00 |
| 85 | `Roid_Sm_Brown` | 366 | Object | 2834.07,-1882.65,4287.54 | 226,509,490 | Scale/Radius: 1.00 |
| 86 | `Roid_Sm_Brown` | 368 | Object | 3802.39,-1940.68,2196.00 | 175,29,158 | Scale/Radius: 1.00 |
| 87 | `Roid_Sm_Brown` | 370 | Object | 3658.68,-2793.27,2290.08 | 192,365,433 | Scale/Radius: 1.00 |
| 88 | `Roid_Sm_Brown` | 372 | Object | 3435.63,-2750.98,2117.70 | 91,0,349 | Scale/Radius: 1.00 |
| 89 | `Roid_Sm_Brown` | 374 | Object | 4100.50,-1836.33,3221.51 | 122,259,403 | Scale/Radius: 1.00 |
| 90 | `Roid_Sm_Brown` | 376 | Object | 3846.94,-2348.58,1849.57 | 233,44,100 | Scale/Radius: 1.00 |
| 91 | `Roid_Sm_Brown` | 378 | Object | 4376.64,-2480.21,2303.60 | 94,264,407 | Scale/Radius: 1.00 |
| 92 | `Roid_Sm_Brown` | 380 | Object | 3689.11,-2588.41,1251.21 | 265,453,478 | Scale/Radius: 1.00 |
| 93 | `Roid_Sm_Brown` | 382 | Object | 2902.27,-1594.49,3859.67 | 175,398,299 | Scale/Radius: 1.00 |
| 94 | `Roid_Sm_Brown` | 384 | Object | 3931.77,-2164.40,1538.05 | 172,329,91 | Scale/Radius: 1.00 |
| 95 | `Roid_Sm_Brown` | 386 | Object | 2926.98,-2776.06,1867.87 | 121,393,442 | Scale/Radius: 1.00 |
| 96 | `Roid_Sm_Brown` | 388 | Object | 4055.65,-2466.85,2446.68 | 341,362,313 | Scale/Radius: 1.00 |
| 97 | `Roid_Sm_Brown` | 390 | Object | 4912.14,-2021.05,2050.95 | 162,1,24 | Scale/Radius: 1.00 |
| 98 | `Roid_Sm_Brown` | 392 | Object | 4152.68,-2313.43,2147.56 | 125,124,444 | Scale/Radius: 1.00 |
| 99 | `Roid_Sm_Brown` | 394 | Object | 2558.77,-1951.30,4165.22 | 329,3,44 | Scale/Radius: 1.00 |
| 100 | `Roid_Sm_Brown` | 396 | Object | 4327.21,-2927.10,2602.71 | 248,101,123 | Scale/Radius: 1.00 |
| 101 | `Roid_Sm_Brown` | 398 | Object | 2644.74,-2279.38,1644.52 | 17,289,235 | Scale/Radius: 1.00 |
| 102 | `Roid_Sm_Brown` | 400 | Object | 3997.67,-1771.16,3079.28 | 138,357,68 | Scale/Radius: 1.00 |
| 103 | `Roid_Sm_Brown` | 402 | Object | 4293.65,-2190.77,2284.44 | 250,383,26 | Scale/Radius: 1.00 |
| 104 | `Roid_Sm_Brown` | 404 | Object | 4094.09,-2366.89,1618.61 | 130,54,175 | Scale/Radius: 1.00 |
| 105 | `Roid_Sm_Brown` | 406 | Object | 2915.69,-1854.64,1786.47 | 262,300,244 | Scale/Radius: 1.00 |
| 106 | `Roid_Sm_Brown` | 408 | Object | 3748.69,-1571.24,2131.22 | 62,416,507 | Scale/Radius: 1.00 |
| 107 | `Roid_Sm_Brown` | 410 | Object | 3862.81,-2539.34,2687.77 | 371,182,164 | Scale/Radius: 1.00 |
| 108 | `Roid_Sm_Brown` | 412 | Object | 4244.83,-2902.57,2306.98 | 131,267,357 | Scale/Radius: 1.00 |
| 109 | `Roid_Sm_Brown` | 414 | Object | 2584.18,-2112.41,3608.37 | 412,21,261 | Scale/Radius: 1.00 |
| 110 | `Roid_Sm_Brown` | 416 | Object | 4892.31,-3038.41,2315.99 | 148,419,165 | Scale/Radius: 1.00 |
| 111 | `Roid_Sm_Brown` | 418 | Object | 4505.47,-2072.13,477.37 | 3,13,307 | Scale/Radius: 1.00 |
| 112 | `Roid_Sm_Brown` | 420 | Object | 3606.50,-2397.28,2567.23 | 23,411,107 | Scale/Radius: 1.00 |
| 113 | `Roid_Sm_Brown` | 422 | Object | 4368.78,-2318.92,466.10 | 132,110,359 | Scale/Radius: 1.00 |
| 114 | `Roid_Sm_Brown` | 424 | Object | 3541.81,-2830.07,1700.29 | 462,490,51 | Scale/Radius: 1.00 |
| 115 | `Roid_Sm_Brown` | 426 | Object | 4602.44,-2605.98,1198.38 | 229,27,211 | Scale/Radius: 1.00 |
| 116 | `Roid_Sm_Brown` | 428 | Object | 2722.09,-2182.34,3640.48 | 54,206,173 | Scale/Radius: 1.00 |
| 117 | `Roid_Sm_Brown` | 431 | Object | 4205.16,-2589.87,3097.30 | 162,61,376 | Scale/Radius: 1.00 |
| 118 | `Roid_Sm_Brown` | 433 | Object | 2910.35,-1588.81,4434.00 | 316,506,506 | Scale/Radius: 1.00 |
| 119 | `Roid_Sm_Brown` | 435 | Object | 5030.23,-1686.57,2016.31 | 286,80,167 | Scale/Radius: 1.00 |
| 120 | `Roid_Sm_Brown` | 437 | Object | 4387.63,-1579.29,2336.27 | 421,402,376 | Scale/Radius: 1.00 |
| 121 | `Roid_Sm_Brown` | 439 | Object | 2716.75,-2011.72,1116.13 | 0,333,351 | Scale/Radius: 1.00 |
| 122 | `Roid_Sm_Brown` | 442 | Object | 3111.58,-1678.52,1511.58 | 228,449,257 | Scale/Radius: 1.00 |
| 123 | `Roid_Sm_Brown` | 444 | Object | 4226.52,-2815.42,1752.68 | 388,18,373 | Scale/Radius: 1.00 |
| 124 | `Roid_Sm_Brown` | 446 | Object | 3851.21,-1634.95,3126.60 | 16,359,178 | Scale/Radius: 1.00 |
| 125 | `Roid_Sm_Brown` | 448 | Object | 3993.40,-2791.26,2751.99 | 216,348,113 | Scale/Radius: 1.00 |
| 126 | `Roid_Sm_Brown` | 450 | Object | 2628.26,-2432.43,2230.93 | 273,40,500 | Scale/Radius: 1.00 |
| 127 | `Roid_Sm_Brown` | 452 | Object | 4951.50,-2808.10,2570.61 | 122,59,16 | Scale/Radius: 1.00 |
| 128 | `Roid_Sm_Brown` | 454 | Object | 3332.49,-1833.77,2887.19 | 158,29,95 | Scale/Radius: 1.00 |
| 129 | `Roid_Sm_Brown` | 456 | Object | 3929.93,-3051.96,3144.06 | 245,137,149 | Scale/Radius: 1.00 |
| 130 | `Roid_Sm_Brown` | 459 | Object | 2840.02,-1904.43,2203.33 | 237,91,121 | Scale/Radius: 1.00 |
| 131 | `Roid_Sm_Brown` | 461 | Object | 4847.76,-2374.21,1069.38 | 198,250,307 | Scale/Radius: 1.00 |
| 132 | `Roid_Sm_Brown` | 463 | Object | 2809.50,-1771.16,2019.69 | 288,219,40 | Scale/Radius: 1.00 |
| 133 | `Roid_Sm_Brown` | 465 | Object | 2630.70,-2376.41,2659.61 | 460,419,185 | Scale/Radius: 1.00 |
| 134 | `Roid_Sm_Brown` | 467 | Object | 2778.99,-2551.79,2437.66 | 422,359,394 | Scale/Radius: 1.00 |
| 135 | `Roid_Sm_Brown2` | 369 | Object | 2636.88,-2547.03,4360.13 | 39,93,131 | Scale/Radius: 1.00 |
| 136 | `Roid_Sm_Brown2` | 203 | Object | 3805.14,-2300.25,2118.27 | 351,122,383 | Scale/Radius: 1.00 |
| 137 | `Roid_Sm_Brown2` | 204 | Object | 3824.06,-2308.30,2148.12 | 151,282,363 | Scale/Radius: 1.00 |
| 138 | `Roid_Sm_Brown2` | 206 | Object | 3844.50,-2328.44,2145.30 | 139,227,498 | Scale/Radius: 1.00 |
| 139 | `Roid_Sm_Brown2` | 208 | Object | 3849.38,-2286.33,2096.86 | 324,94,468 | Scale/Radius: 1.00 |
| 140 | `Roid_Sm_Brown2` | 210 | Object | 3745.94,-2300.61,2115.17 | 425,45,385 | Scale/Radius: 1.00 |
| 141 | `Roid_Sm_Brown2` | 212 | Object | 3802.70,-2335.76,2071.23 | 31,479,19 | Scale/Radius: 1.00 |
| 142 | `Roid_Sm_Brown2` | 214 | Object | 3765.17,-2329.17,2129.53 | 458,205,78 | Scale/Radius: 1.00 |
| 143 | `Roid_Sm_Brown2` | 215 | Object | 3912.85,-2346.01,2124.46 | 337,466,261 | Scale/Radius: 1.00 |
| 144 | `Roid_Sm_Brown2` | 217 | Object | 3844.50,-2294.02,2152.63 | 213,485,491 | Scale/Radius: 1.00 |
| 145 | `Roid_Sm_Brown2` | 219 | Object | 3732.21,-2261.80,2078.27 | 253,154,64 | Scale/Radius: 1.00 |
| 146 | `Roid_Sm_Brown2` | 221 | Object | 3741.67,-2376.04,2103.06 | 510,327,55 | Scale/Radius: 1.00 |
| 147 | `Roid_Sm_Brown2` | 223 | Object | 3735.57,-2351.32,2173.47 | 188,32,330 | Scale/Radius: 1.00 |
| 148 | `Roid_Sm_Brown2` | 225 | Object | 3941.53,-2235.99,2079.12 | 483,51,79 | Scale/Radius: 1.00 |
| 149 | `Roid_Sm_Brown2` | 227 | Object | 3935.43,-2247.89,2132.91 | 474,387,484 | Scale/Radius: 1.00 |
| 150 | `Roid_Sm_Brown2` | 229 | Object | 3788.97,-2207.24,2122.77 | 93,159,60 | Scale/Radius: 1.00 |
| 151 | `Roid_Sm_Brown2` | 231 | Object | 3948.24,-2210.54,2033.21 | 233,347,31 | Scale/Radius: 1.00 |
| 152 | `Roid_Sm_Brown2` | 233 | Object | 3837.79,-2391.24,2046.44 | 87,238,347 | Scale/Radius: 1.00 |
| 153 | `Roid_Sm_Brown2` | 235 | Object | 3897.59,-2302.81,2048.41 | 117,252,336 | Scale/Radius: 1.00 |
| 154 | `Roid_Sm_Brown2` | 237 | Object | 3857.01,-2252.83,2050.39 | 360,211,185 | Scale/Radius: 1.00 |
| 155 | `Roid_Sm_Brown2` | 239 | Object | 3813.99,-2327.71,2304.72 | 488,310,277 | Scale/Radius: 1.00 |
| 156 | `Roid_Sm_Brown2` | 241 | Object | 3916.51,-2428.77,1975.75 | 353,101,135 | Scale/Radius: 1.00 |
| 157 | `Roid_Sm_Brown2` | 243 | Object | 3665.39,-2259.97,1946.17 | 455,236,190 | Scale/Radius: 1.00 |
| 158 | `Roid_Sm_Brown2` | 245 | Object | 3714.82,-2279.74,2303.60 | 86,230,398 | Scale/Radius: 1.00 |
| 159 | `Roid_Sm_Brown2` | 247 | Object | 3923.53,-2217.13,2151.50 | 70,437,94 | Scale/Radius: 1.00 |
| 160 | `Roid_Sm_Brown2` | 249 | Object | 3547.91,-2249.72,2088.97 | 472,0,124 | Scale/Radius: 1.00 |
| 161 | `Roid_Sm_Brown2` | 251 | Object | 3636.40,-2463.92,2359.36 | 177,280,463 | Scale/Radius: 1.00 |
| 162 | `Roid_Sm_Brown2` | 253 | Object | 3719.09,-2367.25,1942.23 | 300,165,128 | Scale/Radius: 1.00 |
| 163 | `Roid_Sm_Brown2` | 255 | Object | 3789.58,-2300.80,1954.62 | 469,234,43 | Scale/Radius: 1.00 |
| 164 | `Roid_Sm_Brown2` | 257 | Object | 3591.55,-2391.42,2001.10 | 10,377,379 | Scale/Radius: 1.00 |
| 165 | `Roid_Sm_Brown2` | 259 | Object | 3951.90,-2373.11,2222.48 | 144,31,129 | Scale/Radius: 1.00 |
| 166 | `Roid_Sm_Brown2` | 261 | Object | 3724.89,-2223.72,1837.17 | 263,114,477 | Scale/Radius: 1.00 |
| 167 | `Roid_Sm_Brown2` | 263 | Object | 3641.89,-2136.21,2424.14 | 178,356,465 | Scale/Radius: 1.00 |
| 168 | `Roid_Sm_Brown2` | 265 | Object | 3653.79,-2357.55,1948.15 | 313,88,383 | Scale/Radius: 1.00 |
| 169 | `Roid_Sm_Brown2` | 267 | Object | 3602.23,-2262.35,2350.91 | 294,410,203 | Scale/Radius: 1.00 |
| 170 | `Roid_Sm_Brown2` | 269 | Object | 4000.11,-2243.86,2391.47 | 100,237,196 | Scale/Radius: 1.00 |
| 171 | `Roid_Sm_Brown2` | 271 | Object | 3854.87,-2149.02,2261.35 | 253,449,138 | Scale/Radius: 1.00 |
| 172 | `Roid_Sm_Brown2` | 273 | Object | 3564.70,-2258.87,1881.96 | 119,390,262 | Scale/Radius: 1.00 |
| 173 | `Roid_Sm_Brown2` | 275 | Object | 3766.08,-2415.40,2274.87 | 305,345,463 | Scale/Radius: 1.00 |
| 174 | `Roid_Sm_Brown2` | 277 | Object | 3425.86,-2065.54,1847.31 | 344,107,275 | Scale/Radius: 1.00 |
| 175 | `Roid_Sm_Brown2` | 279 | Object | 3752.96,-2531.29,1761.69 | 0,460,14 | Scale/Radius: 1.00 |
| 176 | `Roid_Sm_Brown2` | 281 | Object | 3691.93,-2187.65,2088.13 | 110,451,358 | Scale/Radius: 1.00 |
| 177 | `Roid_Sm_Brown2` | 283 | Object | 3847.55,-2225.00,2217.41 | 254,497,39 | Scale/Radius: 1.00 |
| 178 | `Roid_Sm_Brown2` | 285 | Object | 3349.58,-2365.42,2374.57 | 80,459,256 | Scale/Radius: 1.00 |
| 179 | `Roid_Sm_Brown2` | 287 | Object | 3706.58,-2131.45,1669.87 | 491,203,46 | Scale/Radius: 1.00 |
| 180 | `Roid_Sm_Brown2` | 289 | Object | 4071.51,-2306.29,2013.49 | 166,511,242 | Scale/Radius: 1.00 |
| 181 | `Roid_Sm_Brown2` | 291 | Object | 3381.62,-2441.95,2222.20 | 254,33,137 | Scale/Radius: 1.00 |
| 182 | `Roid_Sm_Brown2` | 293 | Object | 4292.43,-2299.15,1945.33 | 98,433,264 | Scale/Radius: 1.00 |
| 183 | `Roid_Sm_Brown2` | 295 | Object | 3706.58,-2288.16,1742.54 | 397,173,243 | Scale/Radius: 1.00 |
| 184 | `Roid_Sm_Brown2` | 297 | Object | 3874.10,-2495.04,2018.84 | 377,82,476 | Scale/Radius: 1.00 |
| 185 | `Roid_Sm_Brown2` | 299 | Object | 3842.06,-2506.57,2379.64 | 305,213,91 | Scale/Radius: 1.00 |
| 186 | `Roid_Sm_Brown2` | 301 | Object | 3561.34,-2262.53,1802.81 | 264,152,366 | Scale/Radius: 1.00 |
| 187 | `Roid_Sm_Brown2` | 303 | Object | 4037.95,-2121.56,1957.72 | 456,402,260 | Scale/Radius: 1.00 |
| 188 | `Roid_Sm_Brown2` | 305 | Object | 3381.31,-2496.50,1787.88 | 204,104,440 | Scale/Radius: 1.00 |
| 189 | `Roid_Sm_Brown2` | 307 | Object | 3851.52,-2576.51,1923.92 | 295,441,321 | Scale/Radius: 1.00 |
| 190 | `Roid_Sm_Brown2` | 309 | Object | 3948.24,-2043.57,2401.61 | 32,409,322 | Scale/Radius: 1.00 |
| 191 | `Roid_Sm_Brown2` | 311 | Object | 3911.63,-2210.54,1914.91 | 41,472,209 | Scale/Radius: 1.00 |
| 192 | `Roid_Sm_Brown2` | 313 | Object | 3335.85,-2160.92,2419.92 | 507,269,45 | Scale/Radius: 1.00 |
| 193 | `Roid_Sm_Brown2` | 315 | Object | 3785.91,-1945.81,1955.19 | 390,64,4 | Scale/Radius: 1.00 |
| 194 | `Roid_Sm_Brown2` | 317 | Object | 3292.83,-2588.41,2658.48 | 505,226,346 | Scale/Radius: 1.00 |
| 195 | `Roid_Sm_Brown2` | 319 | Object | 4121.25,-2233.61,2336.55 | 476,138,444 | Scale/Radius: 1.00 |
| 196 | `Roid_Sm_Brown2` | 321 | Object | 3865.86,-2782.29,2328.94 | 91,290,434 | Scale/Radius: 1.00 |
| 197 | `Roid_Sm_Brown2` | 323 | Object | 4012.93,-2461.72,2036.58 | 259,454,457 | Scale/Radius: 1.00 |
| 198 | `Roid_Sm_Brown2` | 325 | Object | 3320.90,-2292.19,2327.25 | 501,241,411 | Scale/Radius: 1.00 |
| 199 | `Roid_Sm_Brown2` | 327 | Object | 3179.32,-2557.65,1722.82 | 375,14,272 | Scale/Radius: 1.00 |
| 200 | `Roid_Sm_Brown2` | 329 | Object | 3889.66,-2335.76,2367.81 | 298,95,499 | Scale/Radius: 1.00 |
| 201 | `Roid_Sm_Brown2` | 331 | Object | 3504.28,-2217.68,2838.46 | 464,83,198 | Scale/Radius: 1.00 |
| 202 | `Roid_Sm_Brown2` | 333 | Object | 4327.21,-2019.04,2410.62 | 504,420,169 | Scale/Radius: 1.00 |
| 203 | `Roid_Sm_Brown2` | 335 | Object | 3865.25,-2496.14,1887.87 | 65,316,317 | Scale/Radius: 1.00 |
| 204 | `Roid_Sm_Brown2` | 337 | Object | 3494.21,-2284.68,2010.39 | 360,379,13 | Scale/Radius: 1.00 |
| 205 | `Roid_Sm_Brown2` | 339 | Object | 3182.07,-2248.44,2289.23 | 325,293,285 | Scale/Radius: 1.00 |
| 206 | `Roid_Sm_Brown2` | 341 | Object | 4096.53,-2165.87,1575.80 | 505,256,130 | Scale/Radius: 1.00 |
| 207 | `Roid_Sm_Brown2` | 343 | Object | 3100.90,-2315.62,2564.97 | 504,5,365 | Scale/Radius: 1.00 |
| 208 | `Roid_Sm_Brown2` | 345 | Object | 3079.54,-2712.90,2279.09 | 118,417,477 | Scale/Radius: 1.00 |
| 209 | `Roid_Sm_Brown2` | 347 | Object | 2992.58,-2790.52,1715.50 | 28,225,139 | Scale/Radius: 1.00 |
| 210 | `Roid_Sm_Brown2` | 349 | Object | 3421.29,-2445.06,1787.32 | 364,141,162 | Scale/Radius: 1.00 |
| 211 | `Roid_Sm_Brown2` | 351 | Object | 3568.05,-1706.71,2714.81 | 129,267,493 | Scale/Radius: 1.00 |
| 212 | `Roid_Sm_Brown2` | 353 | Object | 3584.53,-2629.78,2323.87 | 261,16,333 | Scale/Radius: 1.00 |
| 213 | `Roid_Sm_Brown2` | 355 | Object | 3602.23,-2374.21,1724.79 | 382,182,416 | Scale/Radius: 1.00 |
| 214 | `Roid_Sm_Brown2` | 357 | Object | 3242.79,-2075.79,1928.43 | 229,114,52 | Scale/Radius: 1.00 |
| 215 | `Roid_Sm_Brown2` | 359 | Object | 4679.63,-2400.39,2131.22 | 264,266,478 | Scale/Radius: 1.00 |
| 216 | `Roid_Sm_Brown2` | 361 | Object | 3226.92,-2541.18,1953.78 | 22,43,20 | Scale/Radius: 1.00 |
| 217 | `Roid_Sm_Brown2` | 363 | Object | 4446.21,-2011.53,2530.89 | 15,167,79 | Scale/Radius: 1.00 |
| 218 | `Roid_Sm_Brown2` | 365 | Object | 4648.82,-2810.30,1796.61 | 89,320,48 | Scale/Radius: 1.00 |
| 219 | `Roid_Sm_Brown2` | 367 | Object | 4489.23,-2220.42,1700.29 | 361,399,132 | Scale/Radius: 1.00 |
| 220 | `Roid_Sm_Brown2` | 371 | Object | 2851.92,-2294.20,3994.02 | 305,499,204 | Scale/Radius: 1.00 |
| 221 | `Roid_Sm_Brown2` | 373 | Object | 2717.97,-2575.23,1766.19 | 308,8,182 | Scale/Radius: 1.00 |
| 222 | `Roid_Sm_Brown2` | 375 | Object | 2959.63,-2204.13,3996.28 | 288,231,96 | Scale/Radius: 1.00 |
| 223 | `Roid_Sm_Brown2` | 377 | Object | 4518.22,-2357.73,1300.34 | 104,408,462 | Scale/Radius: 1.00 |
| 224 | `Roid_Sm_Brown2` | 379 | Object | 2980.08,-1938.67,4068.10 | 352,383,147 | Scale/Radius: 1.00 |
| 225 | `Roid_Sm_Brown2` | 381 | Object | 3324.56,-2074.33,3112.51 | 201,128,479 | Scale/Radius: 1.00 |
| 226 | `Roid_Sm_Brown2` | 383 | Object | 4625.02,-2069.94,2295.43 | 284,508,18 | Scale/Radius: 1.00 |
| 227 | `Roid_Sm_Brown2` | 385 | Object | 4080.06,-2797.11,2891.69 | 493,405,442 | Scale/Radius: 1.00 |
| 228 | `Roid_Sm_Brown2` | 387 | Object | 3615.04,-2484.05,1836.89 | 482,383,121 | Scale/Radius: 1.00 |
| 229 | `Roid_Sm_Brown2` | 389 | Object | 4072.73,-1841.46,1768.45 | 365,143,293 | Scale/Radius: 1.00 |
| 230 | `Roid_Sm_Brown2` | 391 | Object | 4459.94,-2271.50,1039.52 | 301,116,349 | Scale/Radius: 1.00 |
| 231 | `Roid_Sm_Brown2` | 393 | Object | 2808.28,-2853.69,1898.57 | 91,256,29 | Scale/Radius: 1.00 |
| 232 | `Roid_Sm_Brown2` | 395 | Object | 3601.54,-2939.37,1318.80 | 149,106,43 | Scale/Radius: 1.00 |
| 233 | `Roid_Sm_Brown2` | 397 | Object | 4085.55,-1956.79,1669.87 | 493,235,347 | Scale/Radius: 1.00 |
| 234 | `Roid_Sm_Brown2` | 399 | Object | 3875.93,-2374.21,2771.99 | 88,307,75 | Scale/Radius: 1.00 |
| 235 | `Roid_Sm_Brown2` | 401 | Object | 3080.46,-2241.48,1621.71 | 416,373,340 | Scale/Radius: 1.00 |
| 236 | `Roid_Sm_Brown2` | 403 | Object | 3584.83,-2669.15,2461.60 | 391,251,121 | Scale/Radius: 1.00 |
| 237 | `Roid_Sm_Brown2` | 405 | Object | 3296.49,-1665.89,2831.14 | 93,469,449 | Scale/Radius: 1.00 |
| 238 | `Roid_Sm_Brown2` | 407 | Object | 2768.17,-2262.72,3467.54 | 257,337,105 | Scale/Radius: 1.00 |
| 239 | `Roid_Sm_Brown2` | 409 | Object | 3862.20,-2138.04,2976.19 | 137,55,74 | Scale/Radius: 1.00 |
| 240 | `Roid_Sm_Brown2` | 411 | Object | 2277.67,-2471.97,1128.63 | 105,510,109 | Scale/Radius: 1.00 |
| 241 | `Roid_Sm_Brown2` | 413 | Object | 3334.32,-2837.94,2242.48 | 270,431,164 | Scale/Radius: 1.00 |
| 242 | `Roid_Sm_Brown2` | 415 | Object | 3124.40,-2376.96,1697.75 | 256,63,243 | Scale/Radius: 1.00 |
| 243 | `Roid_Sm_Brown2` | 417 | Object | 2702.10,-2789.06,1570.16 | 42,242,173 | Scale/Radius: 1.00 |
| 244 | `Roid_Sm_Brown2` | 419 | Object | 3894.23,-2318.37,1508.76 | 147,307,324 | Scale/Radius: 1.00 |
| 245 | `Roid_Sm_Brown2` | 421 | Object | 2834.22,-2239.10,1690.15 | 228,407,56 | Scale/Radius: 1.00 |
| 246 | `Roid_Sm_Brown2` | 423 | Object | 4848.37,-1667.35,2381.90 | 489,198,254 | Scale/Radius: 1.00 |
| 247 | `Roid_Sm_Brown2` | 425 | Object | 4510.59,-1836.33,2438.79 | 294,242,425 | Scale/Radius: 1.00 |
| 248 | `Roid_Sm_Brown2` | 427 | Object | 4213.70,-2217.68,2628.91 | 462,85,252 | Scale/Radius: 1.00 |
| 249 | `Roid_Sm_Brown2` | 429 | Object | 2646.73,-1554.94,3477.40 | 187,358,498 | Scale/Radius: 1.00 |
| 250 | `Roid_Sm_Brown2` | 430 | Object | 5000.32,-2231.78,2541.03 | 255,226,431 | Scale/Radius: 1.00 |
| 251 | `Roid_Sm_Brown2` | 432 | Object | 4360.16,-2610.93,2326.41 | 236,424,315 | Scale/Radius: 1.00 |
| 252 | `Roid_Sm_Brown2` | 434 | Object | 3261.70,-3023.95,2102.77 | 460,316,409 | Scale/Radius: 1.00 |
| 253 | `Roid_Sm_Brown2` | 436 | Object | 2863.21,-2623.38,3901.64 | 266,4,76 | Scale/Radius: 1.00 |
| 254 | `Roid_Sm_Brown2` | 438 | Object | 3656.23,-3033.28,2219.94 | 100,134,182 | Scale/Radius: 1.00 |
| 255 | `Roid_Sm_Brown2` | 440 | Object | 4240.86,-1852.26,1377.79 | 405,370,113 | Scale/Radius: 1.00 |
| 256 | `Roid_Sm_Brown2` | 441 | Object | 4814.19,-3041.16,2100.52 | 101,151,236 | Scale/Radius: 1.00 |
| 257 | `Roid_Sm_Brown2` | 443 | Object | 4832.50,-2729.56,1068.25 | 90,329,309 | Scale/Radius: 1.00 |
| 258 | `Roid_Sm_Brown2` | 445 | Object | 3437.15,-2820.00,3245.17 | 47,368,469 | Scale/Radius: 1.00 |
| 259 | `Roid_Sm_Brown2` | 447 | Object | 4798.94,-2176.49,2649.47 | 254,81,135 | Scale/Radius: 1.00 |
| 260 | `Roid_Sm_Brown2` | 449 | Object | 4494.73,-2688.37,1340.33 | 206,87,124 | Scale/Radius: 1.00 |
| 261 | `Roid_Sm_Brown2` | 451 | Object | 4942.04,-2346.38,1393.85 | 305,149,460 | Scale/Radius: 1.00 |
| 262 | `Roid_Sm_Brown2` | 453 | Object | 2742.08,-2546.48,3871.78 | 428,399,268 | Scale/Radius: 1.00 |
| 263 | `Roid_Sm_Brown2` | 455 | Object | 4491.98,-1739.85,1022.62 | 283,201,352 | Scale/Radius: 1.00 |
| 264 | `Roid_Sm_Brown2` | 457 | Object | 3244.31,-2600.31,3257.85 | 4,305,32 | Scale/Radius: 1.00 |
| 265 | `Roid_Sm_Brown2` | 458 | Object | 3932.68,-2744.57,1916.60 | 419,259,9 | Scale/Radius: 1.00 |
| 266 | `Roid_Sm_Brown2` | 460 | Object | 4328.13,-2846.00,1077.55 | 113,319,214 | Scale/Radius: 1.00 |
| 267 | `Roid_Sm_Brown2` | 462 | Object | 4136.20,-1967.05,2942.96 | 428,490,503 | Scale/Radius: 1.00 |
| 268 | `Roid_Sm_Brown2` | 464 | Object | 2801.88,-2400.21,1794.08 | 444,16,98 | Scale/Radius: 1.00 |
| 269 | `Roid_Sm_Brown2` | 466 | Object | 2704.23,-2994.84,1332.73 | 211,81,174 | Scale/Radius: 1.00 |
| 270 | `Roid_Sm_Brown2` | 468 | Object | 3565.61,-1901.51,2015.46 | 417,26,168 | Scale/Radius: 1.00 |
| 271 | `DisputB_StarBase` | 10 | Interactive | 26.61,0.00,-22.11 | 0,0,0 | None |
| 272 | `Disputed_Bora_Base_Mine` | 487 | Interactive | 280.77,-2535.46,779.99 | 0,0,0 | None |
