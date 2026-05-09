# Tachyon: The Fringe EARTH06.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH06.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `EARTH06.BDF` |
| Region | 0 |
| Sector ID | 5 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 5 |
| Entities | 314 |
| Events | 1 |
| Waypoints | 0 |
| Child Sectors | 2 |
| Scripts | 1 |
| Scenes | 1 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Roid_Med_Green2`, `1: Roid_Med_Green`, `2: Roid_XL_Green`, `3: Spcargo_Goods`, `4: Hyper_Gate` |
| Scripts | `PLAYER.SCR` |
| Scenes | `earth06a.sen` |
| Labels | `STPF`, `ARI2`, `bfne_08`, `bfne_01`, `PIRA`, `PIRB`, `MINE`, `FRTB` |
| Aliases | None |
| Groups | `CONT_059` |
| Child Sectors | [earth06A.spx](EARTH06A.md), [earth06B.spx](EARTH06B.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 2849; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 59
- Set/add variable: variable group 12, variable 302, subtype 0, value 1

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 2 | Gate | -829.44,148.00,1302.00 | 55,0,0 | Gate SPX: [Earth03.spx](EARTH03.md) |
| 1 | `Spcargo_Goods` | 2849 | Interactive | -1539.69,1191.14,1890.08 | 284,185,505 | secondary groups: CONT_059, none |
| 2 | `Roid_XL_Green` | 2598 | Object | -1630.11,3040.49,3979.40 | 5,340,258 | Scale/Radius: 1.00 |
| 3 | `Roid_XL_Green` | 1801 | Object | 815.05,178.65,-1450.06 | 353,176,499 | Scale/Radius: 1.00 |
| 4 | `Roid_XL_Green` | 1802 | Object | -516.53,476.39,2533.49 | 455,426,52 | Scale/Radius: 1.00 |
| 5 | `Roid_XL_Green` | 1803 | Object | 1989.76,1726.91,565.51 | 476,153,509 | Scale/Radius: 1.00 |
| 6 | `Roid_XL_Green` | 1816 | Object | -1076.77,-2024.66,735.47 | 88,476,396 | Scale/Radius: 1.00 |
| 7 | `Roid_XL_Green` | 1822 | Object | -863.85,2084.21,-435.08 | 486,369,306 | Scale/Radius: 1.00 |
| 8 | `Roid_XL_Green` | 1839 | Object | 1951.28,-2560.60,3845.95 | 94,64,344 | Scale/Radius: 1.00 |
| 9 | `Roid_XL_Green` | 1840 | Object | 1412.34,-1846.01,-703.49 | 22,424,26 | Scale/Radius: 1.00 |
| 10 | `Roid_XL_Green` | 1850 | Object | 1846.89,-1965.11,320.38 | 221,397,57 | Scale/Radius: 1.00 |
| 11 | `Roid_XL_Green` | 1855 | Object | -1533.02,2917.89,2149.78 | 358,112,475 | Scale/Radius: 1.00 |
| 12 | `Roid_XL_Green` | 1864 | Object | -2641.23,2917.89,1858.21 | 181,97,356 | Scale/Radius: 1.00 |
| 13 | `Roid_XL_Green` | 1868 | Object | -395.77,-167.16,1645.19 | 245,85,64 | Scale/Radius: 1.00 |
| 14 | `Roid_XL_Green` | 1897 | Object | -2551.93,-535.94,1733.18 | 104,142,324 | Scale/Radius: 1.00 |
| 15 | `Roid_XL_Green` | 1900 | Object | 1340.96,-1250.52,-1939.01 | 104,165,326 | Scale/Radius: 1.00 |
| 16 | `Roid_XL_Green` | 1901 | Object | -929.68,1599.66,3755.33 | 263,422,88 | Scale/Radius: 1.00 |
| 17 | `Roid_XL_Green` | 1916 | Object | 1965.29,-1488.72,3213.48 | 330,124,508 | Scale/Radius: 1.00 |
| 18 | `Roid_XL_Green` | 1921 | Object | 630.50,833.68,-1488.45 | 97,48,263 | Scale/Radius: 1.00 |
| 19 | `Roid_XL_Green` | 1924 | Object | -1390.15,-1726.91,2394.91 | 237,476,362 | Scale/Radius: 1.00 |
| 20 | `Roid_XL_Green` | 1937 | Object | -1317.29,-2322.40,1306.89 | 372,82,380 | Scale/Radius: 1.00 |
| 21 | `Roid_XL_Green` | 1941 | Object | -2234.09,-476.39,3107.27 | 153,429,24 | Scale/Radius: 1.00 |
| 22 | `Roid_XL_Green` | 1943 | Object | -363.26,2191.69,1536.24 | 250,330,180 | Scale/Radius: 1.00 |
| 23 | `Roid_XL_Green` | 1946 | Object | -1469.10,1548.27,3125.15 | 115,115,341 | Scale/Radius: 1.00 |
| 24 | `Roid_XL_Green` | 1950 | Object | 2464.15,-655.04,-1681.39 | 181,148,502 | Scale/Radius: 1.00 |
| 25 | `Roid_XL_Green` | 1967 | Object | 473.53,-2560.60,2549.78 | 73,344,97 | Scale/Radius: 1.00 |
| 26 | `Roid_XL_Green` | 1971 | Object | -355.74,2679.69,1418.08 | 266,20,180 | Scale/Radius: 1.00 |
| 27 | `Roid_XL_Green` | 1979 | Object | 3224.18,-1548.27,-1212.12 | 20,352,139 | Scale/Radius: 1.00 |
| 28 | `Roid_XL_Green` | 1990 | Object | -127.58,-1071.88,-1119.61 | 323,4,272 | Scale/Radius: 1.00 |
| 29 | `Roid_XL_Green` | 2009 | Object | 2795.57,1190.97,-1947.53 | 35,289,185 | Scale/Radius: 1.00 |
| 30 | `Roid_XL_Green` | 2016 | Object | 1582.97,1607.82,145.79 | 50,140,117 | Scale/Radius: 1.00 |
| 31 | `Roid_XL_Green` | 2018 | Object | -136.45,893.23,2672.68 | 444,187,189 | Scale/Radius: 1.00 |
| 32 | `Roid_XL_Green` | 2027 | Object | 2666.52,297.74,-777.64 | 375,156,377 | Scale/Radius: 1.00 |
| 33 | `Roid_XL_Green` | 2034 | Object | -2477.03,476.39,3306.39 | 126,28,255 | Scale/Radius: 1.00 |
| 34 | `Roid_XL_Green` | 2051 | Object | -843.96,-2917.89,2249.96 | 134,58,268 | Scale/Radius: 1.00 |
| 35 | `Roid_XL_Green` | 2064 | Object | 566.90,774.13,628.50 | 83,506,184 | Scale/Radius: 1.00 |
| 36 | `Roid_XL_Green` | 2079 | Object | -2473.73,1667.36,2727.01 | 387,371,487 | Scale/Radius: 1.00 |
| 37 | `Roid_XL_Green` | 2081 | Object | -466.98,0.00,245.86 | 509,452,475 | Scale/Radius: 1.00 |
| 38 | `Roid_XL_Green` | 2082 | Object | 594.66,833.68,1232.65 | 127,135,15 | Scale/Radius: 1.00 |
| 39 | `Roid_XL_Green` | 2109 | Object | -894.05,-1190.97,2689.61 | 182,43,300 | Scale/Radius: 1.00 |
| 40 | `Roid_XL_Green` | 2118 | Object | -2673.59,-1786.46,3419.12 | 271,491,418 | Scale/Radius: 1.00 |
| 41 | `Roid_XL_Green` | 2121 | Object | 741.52,297.74,928.12 | 436,192,243 | Scale/Radius: 1.00 |
| 42 | `Roid_XL_Green` | 2127 | Object | 973.70,2739.24,1048.22 | 109,169,455 | Scale/Radius: 1.00 |
| 43 | `Roid_XL_Green` | 2134 | Object | -2122.33,-1905.56,3805.60 | 151,81,234 | Scale/Radius: 1.00 |
| 44 | `Roid_XL_Green` | 2143 | Object | 1299.28,-2739.24,-1732.27 | 187,469,477 | Scale/Radius: 1.00 |
| 45 | `Roid_XL_Green` | 2173 | Object | -424.93,-5320.85,4511.37 | 447,509,60 | Scale/Radius: 1.00 |
| 46 | `Roid_XL_Green` | 2194 | Object | 1193.61,4343.55,2702.63 | 365,32,369 | Scale/Radius: 1.00 |
| 47 | `Roid_XL_Green` | 2202 | Object | -2327.85,-66.25,3650.52 | 0,72,416 | Scale/Radius: 1.00 |
| 48 | `Roid_XL_Green` | 2236 | Object | 1390.88,2606.13,4432.40 | 21,65,74 | Scale/Radius: 1.00 |
| 49 | `Roid_XL_Green` | 2239 | Object | 1312.68,-2823.31,1703.37 | 447,88,372 | Scale/Radius: 1.00 |
| 50 | `Roid_XL_Green` | 2250 | Object | 119.70,4343.55,896.59 | 482,39,384 | Scale/Radius: 1.00 |
| 51 | `Roid_XL_Green` | 2263 | Object | 1390.88,3692.02,4432.40 | 14,393,182 | Scale/Radius: 1.00 |
| 52 | `Roid_XL_Green` | 2265 | Object | -842.34,217.18,1193.75 | 228,54,371 | Scale/Radius: 1.00 |
| 53 | `Roid_XL_Green` | 2269 | Object | 1273.53,3692.02,5344.10 | 31,189,235 | Scale/Radius: 1.00 |
| 54 | `Roid_XL_Green` | 2280 | Object | 65.68,4234.97,4941.22 | 224,380,254 | Scale/Radius: 1.00 |
| 55 | `Roid_XL_Green` | 2307 | Object | 305.09,-4777.91,5908.52 | 298,5,269 | Scale/Radius: 1.00 |
| 56 | `Roid_XL_Green` | 2309 | Object | 3516.59,-3692.02,1401.46 | 369,240,477 | Scale/Radius: 1.00 |
| 57 | `Roid_XL_Green` | 2311 | Object | 1389.86,977.30,2482.84 | 286,371,306 | Scale/Radius: 1.00 |
| 58 | `Roid_XL_Green` | 2319 | Object | 1867.68,-977.30,2467.89 | 226,324,376 | Scale/Radius: 1.00 |
| 59 | `Roid_XL_Green` | 2323 | Object | 1210.14,-4560.73,3009.24 | 262,464,327 | Scale/Radius: 1.00 |
| 60 | `Roid_XL_Green` | 2343 | Object | 430.60,-760.12,873.52 | 85,419,134 | Scale/Radius: 1.00 |
| 61 | `Roid_XL_Green` | 2367 | Object | 3379.01,-108.59,1165.41 | 385,500,355 | Scale/Radius: 1.00 |
| 62 | `Roid_XL_Green` | 2368 | Object | 2937.96,-1628.83,2634.72 | 304,344,144 | Scale/Radius: 1.00 |
| 63 | `Roid_XL_Green` | 2375 | Object | -381.91,-3366.25,2941.83 | 128,343,322 | Scale/Radius: 1.00 |
| 64 | `Roid_XL_Green` | 2376 | Object | 2009.98,-217.18,5494.66 | 51,355,329 | Scale/Radius: 1.00 |
| 65 | `Roid_XL_Green` | 2388 | Object | 2828.03,3800.61,5228.71 | 166,504,485 | Scale/Radius: 1.00 |
| 66 | `Roid_XL_Green` | 2389 | Object | 2289.52,-4126.38,1800.38 | 164,157,56 | Scale/Radius: 1.00 |
| 67 | `Roid_XL_Green` | 2419 | Object | 3552.33,-1303.07,906.27 | 303,324,311 | Scale/Radius: 1.00 |
| 68 | `Roid_XL_Green` | 2439 | Object | 289.43,-2714.72,2533.55 | 79,388,95 | Scale/Radius: 1.00 |
| 69 | `Roid_XL_Green` | 2453 | Object | -2196.70,4886.50,3786.34 | 315,123,316 | Scale/Radius: 1.00 |
| 70 | `Roid_XL_Green` | 2465 | Object | 2889.14,1954.60,526.18 | 224,239,191 | Scale/Radius: 1.00 |
| 71 | `Roid_XL_Green` | 2468 | Object | 978.85,651.53,1687.10 | 65,329,152 | Scale/Radius: 1.00 |
| 72 | `Roid_XL_Green` | 2475 | Object | 3214.13,-1846.01,5056.40 | 175,147,22 | Scale/Radius: 1.00 |
| 73 | `Roid_XL_Green` | 2478 | Object | 2275.02,3692.02,5392.90 | 438,92,134 | Scale/Radius: 1.00 |
| 74 | `Roid_XL_Green` | 2490 | Object | 1642.09,-1411.66,2915.61 | 278,218,408 | Scale/Radius: 1.00 |
| 75 | `Roid_XL_Green` | 2511 | Object | -2444.22,-1260.73,3541.36 | 111,406,470 | Scale/Radius: 1.00 |
| 76 | `Roid_XL_Green` | 2524 | Object | -2345.68,58.11,3837.94 | 153,96,224 | Scale/Radius: 1.00 |
| 77 | `Roid_XL_Green` | 2531 | Object | -9.14,-5212.27,1753.66 | 312,402,464 | Scale/Radius: 1.00 |
| 78 | `Roid_XL_Green` | 2534 | Object | 3678.11,-5320.85,3626.43 | 4,53,502 | Scale/Radius: 1.00 |
| 79 | `Roid_XL_Green` | 2536 | Object | 1463.38,4886.50,5391.57 | 280,231,292 | Scale/Radius: 1.00 |
| 80 | `Roid_XL_Green` | 2546 | Object | -2490.65,6666.25,3785.37 | 408,107,78 | Scale/Radius: 1.00 |
| 81 | `Roid_XL_Green` | 2570 | Object | 1397.99,-4777.91,2128.01 | 466,511,343 | Scale/Radius: 1.00 |
| 82 | `Roid_XL_Green` | 2585 | Object | 1343.19,2823.31,3842.44 | 494,116,348 | Scale/Radius: 1.00 |
| 83 | `Roid_XL_Green` | 2608 | Object | 737.05,977.30,5814.89 | 165,312,149 | Scale/Radius: 1.00 |
| 84 | `Roid_XL_Green` | 2610 | Object | 1594.22,4126.38,4034.89 | 348,280,475 | Scale/Radius: 1.00 |
| 85 | `Roid_XL_Green` | 2617 | Object | 1579.71,-760.12,2530.31 | 49,348,196 | Scale/Radius: 1.00 |
| 86 | `Roid_XL_Green` | 2622 | Object | -238.82,108.59,4697.02 | 125,354,435 | Scale/Radius: 1.00 |
| 87 | `Roid_XL_Green` | 2629 | Object | 3683.51,-2714.72,1409.60 | 446,119,455 | Scale/Radius: 1.00 |
| 88 | `Roid_XL_Green` | 2631 | Object | 2160.37,-4886.50,5196.18 | 67,329,426 | Scale/Radius: 1.00 |
| 89 | `Roid_XL_Green` | 2634 | Object | 2419.73,3474.84,2663.39 | 111,348,71 | Scale/Radius: 1.00 |
| 90 | `Roid_XL_Green` | 2648 | Object | -2270.45,3366.25,3761.96 | 77,283,3 | Scale/Radius: 1.00 |
| 91 | `Roid_XL_Green` | 2656 | Object | 2030.65,-4126.38,4519.23 | 375,24,351 | Scale/Radius: 1.00 |
| 92 | `Roid_XL_Green` | 2662 | Object | -1000.41,5429.44,4403.17 | 442,227,504 | Scale/Radius: 1.00 |
| 93 | `Roid_XL_Green` | 2726 | Object | 1803.31,0.00,-489.20 | 0,0,0 | Scale/Radius: 1.00 |
| 94 | `Roid_Med_Green` | 2530 | Object | -2356.44,3692.02,4402.72 | 372,129,401 | Scale/Radius: 1.00 |
| 95 | `Roid_Med_Green` | 1797 | Object | -2474.26,59.55,2242.58 | 369,142,132 | Scale/Radius: 1.00 |
| 96 | `Roid_Med_Green` | 1808 | Object | -2082.80,-2322.40,3119.50 | 254,207,114 | Scale/Radius: 1.00 |
| 97 | `Roid_Med_Green` | 1825 | Object | -1227.41,-2917.89,2117.62 | 260,139,192 | Scale/Radius: 1.00 |
| 98 | `Roid_Med_Green` | 1845 | Object | -1612.39,119.10,2013.59 | 140,510,23 | Scale/Radius: 1.00 |
| 99 | `Roid_Med_Green` | 1849 | Object | -130.12,-1429.17,3062.82 | 104,16,99 | Scale/Radius: 1.00 |
| 100 | `Roid_Med_Green` | 1853 | Object | -2493.20,-2664.66,2367.06 | 98,409,156 | Scale/Radius: 1.00 |
| 101 | `Roid_Med_Green` | 1877 | Object | -2593.26,-2739.24,2769.26 | 209,77,223 | Scale/Radius: 1.00 |
| 102 | `Roid_Med_Green` | 1878 | Object | -286.32,0.00,-1391.98 | 157,122,444 | Scale/Radius: 1.00 |
| 103 | `Roid_Med_Green` | 1889 | Object | 414.20,-1190.97,-1581.33 | 174,52,124 | Scale/Radius: 1.00 |
| 104 | `Roid_Med_Green` | 1896 | Object | 1612.12,1310.07,802.83 | 265,5,62 | Scale/Radius: 1.00 |
| 105 | `Roid_Med_Green` | 1910 | Object | -2380.32,893.23,3919.47 | 321,178,254 | Scale/Radius: 1.00 |
| 106 | `Roid_Med_Green` | 1911 | Object | 2325.17,-2798.79,-250.29 | 116,278,417 | Scale/Radius: 1.00 |
| 107 | `Roid_Med_Green` | 1914 | Object | -357.81,2798.79,-401.60 | 288,132,485 | Scale/Radius: 1.00 |
| 108 | `Roid_Med_Green` | 1929 | Object | 2521.71,238.20,-1860.90 | 236,263,388 | Scale/Radius: 1.00 |
| 109 | `Roid_Med_Green` | 1945 | Object | 2329.17,-714.58,-799.96 | 299,7,39 | Scale/Radius: 1.00 |
| 110 | `Roid_Med_Green` | 1959 | Object | -2240.03,2679.69,2818.81 | 421,414,26 | Scale/Radius: 1.00 |
| 111 | `Roid_Med_Green` | 1968 | Object | 253.41,-1071.88,-465.91 | 475,456,411 | Scale/Radius: 1.00 |
| 112 | `Roid_Med_Green` | 2005 | Object | -1889.37,-2679.69,2406.91 | 308,328,362 | Scale/Radius: 1.00 |
| 113 | `Roid_Med_Green` | 2013 | Object | -2625.01,2262.85,2714.78 | 171,233,42 | Scale/Radius: 1.00 |
| 114 | `Roid_Med_Green` | 2025 | Object | 2505.83,2620.14,-1888.13 | 252,187,470 | Scale/Radius: 1.00 |
| 115 | `Roid_Med_Green` | 2026 | Object | -834.02,-416.84,1988.74 | 355,363,22 | Scale/Radius: 1.00 |
| 116 | `Roid_Med_Green` | 2032 | Object | -650.46,-2858.34,224.95 | 507,243,212 | Scale/Radius: 1.00 |
| 117 | `Roid_Med_Green` | 2035 | Object | 1773.46,-1965.11,472.64 | 68,105,409 | Scale/Radius: 1.00 |
| 118 | `Roid_Med_Green` | 2042 | Object | 1555.21,2679.69,-458.35 | 140,296,262 | Scale/Radius: 1.00 |
| 119 | `Roid_Med_Green` | 2054 | Object | -155.31,595.49,1483.71 | 334,446,313 | Scale/Radius: 1.00 |
| 120 | `Roid_Med_Green` | 2056 | Object | -2563.03,2322.40,2852.04 | 19,264,268 | Scale/Radius: 1.00 |
| 121 | `Roid_Med_Green` | 2071 | Object | 1359.83,1786.46,-744.21 | 152,101,301 | Scale/Radius: 1.00 |
| 122 | `Roid_Med_Green` | 2086 | Object | 1035.35,-1071.88,-1906.85 | 221,299,311 | Scale/Radius: 1.00 |
| 123 | `Roid_Med_Green` | 2091 | Object | -2338.63,2322.40,2647.04 | 69,475,53 | Scale/Radius: 1.00 |
| 124 | `Roid_Med_Green` | 2093 | Object | -1629.79,1369.62,2014.66 | 339,182,145 | Scale/Radius: 1.00 |
| 125 | `Roid_Med_Green` | 2099 | Object | 2817.38,-655.04,-1631.84 | 198,453,192 | Scale/Radius: 1.00 |
| 126 | `Roid_Med_Green` | 2108 | Object | -40.32,833.68,143.15 | 505,482,510 | Scale/Radius: 1.00 |
| 127 | `Roid_Med_Green` | 2117 | Object | -34.38,-2798.79,431.60 | 202,346,347 | Scale/Radius: 1.00 |
| 128 | `Roid_Med_Green` | 2125 | Object | -910.01,1846.01,3795.98 | 239,148,85 | Scale/Radius: 1.00 |
| 129 | `Roid_Med_Green` | 2133 | Object | 2393.97,357.29,300.28 | 375,92,404 | Scale/Radius: 1.00 |
| 130 | `Roid_Med_Green` | 2148 | Object | -1549.34,1182.36,1884.55 | 346,386,136 | Scale/Radius: 1.00 |
| 131 | `Roid_Med_Green` | 2154 | Object | 2093.03,3800.61,4904.53 | 98,175,195 | Scale/Radius: 1.00 |
| 132 | `Roid_Med_Green` | 2156 | Object | 104.11,-2823.31,3337.61 | 365,398,323 | Scale/Radius: 1.00 |
| 133 | `Roid_Med_Green` | 2159 | Object | 1327.95,-4669.32,1979.70 | 427,396,475 | Scale/Radius: 1.00 |
| 134 | `Roid_Med_Green` | 2163 | Object | -146.72,2280.37,1517.61 | 61,485,399 | Scale/Radius: 1.00 |
| 135 | `Roid_Med_Green` | 2165 | Object | -278.27,2280.37,4351.07 | 100,335,66 | Scale/Radius: 1.00 |
| 136 | `Roid_Med_Green` | 2169 | Object | 386.69,2063.19,5492.02 | 418,317,433 | Scale/Radius: 1.00 |
| 137 | `Roid_Med_Green` | 2172 | Object | 608.14,868.71,3532.44 | 224,218,80 | Scale/Radius: 1.00 |
| 138 | `Roid_Med_Green` | 2192 | Object | 3218.97,2280.37,3785.52 | 289,72,309 | Scale/Radius: 1.00 |
| 139 | `Roid_Med_Green` | 2196 | Object | 3356.08,-2171.78,1126.06 | 509,44,11 | Scale/Radius: 1.00 |
| 140 | `Roid_Med_Green` | 2198 | Object | -285.30,-3784.08,2880.32 | 175,173,509 | Scale/Radius: 1.00 |
| 141 | `Roid_Med_Green` | 2199 | Object | 1642.09,-2063.19,2915.61 | 231,43,38 | Scale/Radius: 1.00 |
| 142 | `Roid_Med_Green` | 2201 | Object | 127.04,-108.59,3376.95 | 126,314,383 | Scale/Radius: 1.00 |
| 143 | `Roid_Med_Green` | 2209 | Object | 2131.76,2280.37,2725.81 | 123,302,248 | Scale/Radius: 1.00 |
| 144 | `Roid_Med_Green` | 2215 | Object | 1610.02,977.30,3115.43 | 224,262,73 | Scale/Radius: 1.00 |
| 145 | `Roid_Med_Green` | 2231 | Object | 3340.45,4669.32,1851.02 | 410,260,198 | Scale/Radius: 1.00 |
| 146 | `Roid_Med_Green` | 2249 | Object | 1364.94,-4777.91,1514.79 | 396,78,320 | Scale/Radius: 1.00 |
| 147 | `Roid_Med_Green` | 2256 | Object | 1461.11,-2497.54,4376.81 | 70,31,269 | Scale/Radius: 1.00 |
| 148 | `Roid_Med_Green` | 2268 | Object | -985.38,-4560.73,3972.59 | 325,238,306 | Scale/Radius: 1.00 |
| 149 | `Roid_Med_Green` | 2272 | Object | -316.83,-5483.09,1658.71 | 97,197,497 | Scale/Radius: 1.00 |
| 150 | `Roid_Med_Green` | 2275 | Object | 3003.32,-2497.54,530.74 | 95,462,252 | Scale/Radius: 1.00 |
| 151 | `Roid_Med_Green` | 2277 | Object | -1030.77,-1954.60,3576.49 | 140,356,245 | Scale/Radius: 1.00 |
| 152 | `Roid_Med_Green` | 2288 | Object | 3033.38,651.53,3633.24 | 138,17,106 | Scale/Radius: 1.00 |
| 153 | `Roid_Med_Green` | 2292 | Object | 203.25,2171.78,5177.27 | 112,25,443 | Scale/Radius: 1.00 |
| 154 | `Roid_Med_Green` | 2295 | Object | -663.98,3149.08,1186.60 | 453,212,3 | Scale/Radius: 1.00 |
| 155 | `Roid_Med_Green` | 2297 | Object | 2963.58,-977.30,1565.65 | 283,429,170 | Scale/Radius: 1.00 |
| 156 | `Roid_Med_Green` | 2298 | Object | 1954.00,1520.24,4842.09 | 476,376,196 | Scale/Radius: 1.00 |
| 157 | `Roid_Med_Green` | 2303 | Object | 4060.50,-434.36,2612.96 | 437,253,220 | Scale/Radius: 1.00 |
| 158 | `Roid_Med_Green` | 2314 | Object | 1141.90,3800.61,2125.33 | 300,496,230 | Scale/Radius: 1.00 |
| 159 | `Roid_Med_Green` | 2322 | Object | -1154.99,1954.60,5072.87 | 42,492,46 | Scale/Radius: 1.00 |
| 160 | `Roid_Med_Green` | 2327 | Object | 2996.63,434.36,2178.87 | 384,50,54 | Scale/Radius: 1.00 |
| 161 | `Roid_Med_Green` | 2332 | Object | -1872.22,108.59,4120.50 | 294,324,215 | Scale/Radius: 1.00 |
| 162 | `Roid_Med_Green` | 2335 | Object | 3186.47,-2497.54,2226.34 | 497,274,213 | Scale/Radius: 1.00 |
| 163 | `Roid_Med_Green` | 2342 | Object | 3248.74,-2931.90,1693.65 | 68,366,47 | Scale/Radius: 1.00 |
| 164 | `Roid_Med_Green` | 2346 | Object | -143.39,3040.49,5695.54 | 457,153,285 | Scale/Radius: 1.00 |
| 165 | `Roid_Med_Green` | 2353 | Object | -2533.51,203.46,3706.68 | 261,157,231 | Scale/Radius: 1.00 |
| 166 | `Roid_Med_Green` | 2361 | Object | 2168.46,-5103.68,1870.94 | 397,169,302 | Scale/Radius: 1.00 |
| 167 | `Roid_Med_Green` | 2379 | Object | 69.39,-4452.14,5782.36 | 33,475,45 | Scale/Radius: 1.00 |
| 168 | `Roid_Med_Green` | 2404 | Object | -215.51,-3366.25,1399.58 | 262,258,473 | Scale/Radius: 1.00 |
| 169 | `Roid_Med_Green` | 2406 | Object | 357.05,4995.09,1733.26 | 479,304,19 | Scale/Radius: 1.00 |
| 170 | `Roid_Med_Green` | 2408 | Object | -127.88,3040.49,4052.59 | 189,418,180 | Scale/Radius: 1.00 |
| 171 | `Roid_Med_Green` | 2416 | Object | -185.97,4017.79,1957.43 | 408,76,213 | Scale/Radius: 1.00 |
| 172 | `Roid_Med_Green` | 2421 | Object | -723.04,1303.07,4979.24 | 85,93,23 | Scale/Radius: 1.00 |
| 173 | `Roid_Med_Green` | 2425 | Object | 4298.90,3800.61,1630.71 | 261,150,304 | Scale/Radius: 1.00 |
| 174 | `Roid_Med_Green` | 2435 | Object | -37.10,-542.94,1462.34 | 171,460,26 | Scale/Radius: 1.00 |
| 175 | `Roid_Med_Green` | 2442 | Object | 3455.22,977.30,2965.73 | 42,143,69 | Scale/Radius: 1.00 |
| 176 | `Roid_Med_Green` | 2448 | Object | 2379.55,4995.09,5015.73 | 293,493,313 | Scale/Radius: 1.00 |
| 177 | `Roid_Med_Green` | 2454 | Object | 2637.56,4017.79,4142.37 | 384,449,39 | Scale/Radius: 1.00 |
| 178 | `Roid_Med_Green` | 2488 | Object | -921.04,-5026.50,2475.56 | 463,363,383 | Scale/Radius: 1.00 |
| 179 | `Roid_Med_Green` | 2498 | Object | -645.55,-325.77,2203.55 | 8,185,160 | Scale/Radius: 1.00 |
| 180 | `Roid_Med_Green` | 2506 | Object | -125.18,-2931.90,2944.18 | 127,294,205 | Scale/Radius: 1.00 |
| 181 | `Roid_Med_Green` | 2527 | Object | 701.00,542.94,2323.40 | 66,476,41 | Scale/Radius: 1.00 |
| 182 | `Roid_Med_Green` | 2545 | Object | 2280.61,-5212.27,2152.24 | 467,174,460 | Scale/Radius: 1.00 |
| 183 | `Roid_Med_Green` | 2552 | Object | -60.03,325.77,1423.00 | 115,56,359 | Scale/Radius: 1.00 |
| 184 | `Roid_Med_Green` | 2556 | Object | -595.58,868.71,4641.42 | 95,462,478 | Scale/Radius: 1.00 |
| 185 | `Roid_Med_Green` | 2575 | Object | 3866.94,3800.61,1724.34 | 242,38,11 | Scale/Radius: 1.00 |
| 186 | `Roid_Med_Green` | 2580 | Object | 537.08,-5212.27,5193.54 | 469,292,66 | Scale/Radius: 1.00 |
| 187 | `Roid_Med_Green` | 2583 | Object | 514.54,-2823.31,1817.41 | 347,489,106 | Scale/Radius: 1.00 |
| 188 | `Roid_Med_Green` | 2590 | Object | -377.76,4264.84,2882.71 | 290,228,426 | Scale/Radius: 1.00 |
| 189 | `Roid_Med_Green` | 2597 | Object | 2456.43,-1411.66,1808.52 | 286,501,453 | Scale/Radius: 1.00 |
| 190 | `Roid_Med_Green` | 2607 | Object | -2559.44,7209.20,3667.34 | 142,405,110 | Scale/Radius: 1.00 |
| 191 | `Roid_Med_Green` | 2611 | Object | -1371.48,1737.42,4144.90 | 11,147,276 | Scale/Radius: 1.00 |
| 192 | `Roid_Med_Green` | 2627 | Object | 3415.65,-2823.31,1701.78 | 108,365,82 | Scale/Radius: 1.00 |
| 193 | `Roid_Med_Green` | 2636 | Object | 2860.06,-2714.72,3892.37 | 199,92,126 | Scale/Radius: 1.00 |
| 194 | `Roid_Med_Green` | 2647 | Object | 216.07,1520.24,4642.74 | 306,148,358 | Scale/Radius: 1.00 |
| 195 | `Roid_Med_Green` | 2651 | Object | -210.42,-1520.24,1721.47 | 201,322,142 | Scale/Radius: 1.00 |
| 196 | `Roid_Med_Green` | 2659 | Object | 1292.75,4995.09,4542.29 | 486,90,472 | Scale/Radius: 1.00 |
| 197 | `Roid_Med_Green` | 2661 | Object | -565.86,4995.09,1076.70 | 186,127,165 | Scale/Radius: 1.00 |
| 198 | `Roid_Med_Green2` | 2466 | Object | -1122.96,-1954.60,3736.53 | 147,106,93 | Scale/Radius: 1.00 |
| 199 | `Roid_Med_Green2` | 1831 | Object | -1211.54,-2381.95,2144.86 | 401,491,210 | Scale/Radius: 1.00 |
| 200 | `Roid_Med_Green2` | 1859 | Object | 1594.85,119.10,722.70 | 262,176,244 | Scale/Radius: 1.00 |
| 201 | `Roid_Med_Green2` | 1879 | Object | -989.39,357.29,3659.79 | 280,227,59 | Scale/Radius: 1.00 |
| 202 | `Roid_Med_Green2` | 1893 | Object | -929.90,59.55,430.94 | 435,81,285 | Scale/Radius: 1.00 |
| 203 | `Roid_Med_Green2` | 1894 | Object | 1561.15,-1369.62,-169.90 | 314,96,186 | Scale/Radius: 1.00 |
| 204 | `Roid_Med_Green2` | 1918 | Object | -2264.27,-2084.21,3585.75 | 203,97,106 | Scale/Radius: 1.00 |
| 205 | `Roid_Med_Green2` | 1922 | Object | -181.12,-238.19,1717.69 | 423,301,82 | Scale/Radius: 1.00 |
| 206 | `Roid_Med_Green2` | 1938 | Object | 2005.74,833.68,-1633.16 | 10,487,34 | Scale/Radius: 1.00 |
| 207 | `Roid_Med_Green2` | 1958 | Object | 1434.16,1846.01,-387.80 | 292,48,117 | Scale/Radius: 1.00 |
| 208 | `Roid_Med_Green2` | 1960 | Object | 1780.74,-2501.05,3175.08 | 386,64,183 | Scale/Radius: 1.00 |
| 209 | `Roid_Med_Green2` | 1966 | Object | 1932.21,-2322.40,745.02 | 153,294,215 | Scale/Radius: 1.00 |
| 210 | `Roid_Med_Green2` | 1976 | Object | -2380.32,-2501.05,3919.47 | 33,478,141 | Scale/Radius: 1.00 |
| 211 | `Roid_Med_Green2` | 1998 | Object | -145.99,-2858.34,3035.59 | 233,167,371 | Scale/Radius: 1.00 |
| 212 | `Roid_Med_Green2` | 2017 | Object | -1427.84,2203.30,2051.99 | 142,436,403 | Scale/Radius: 1.00 |
| 213 | `Roid_Med_Green2` | 2038 | Object | 2847.08,-297.74,-189.57 | 2,391,255 | Scale/Radius: 1.00 |
| 214 | `Roid_Med_Green2` | 2055 | Object | 421.99,-2441.50,1771.16 | 296,311,450 | Scale/Radius: 1.00 |
| 215 | `Roid_Med_Green2` | 2073 | Object | -768.60,-1846.01,-271.65 | 82,334,414 | Scale/Radius: 1.00 |
| 216 | `Roid_Med_Green2` | 2094 | Object | -2191.77,-2739.24,3408.19 | 398,238,314 | Scale/Radius: 1.00 |
| 217 | `Roid_Med_Green2` | 2106 | Object | 1688.15,-1131.43,48.00 | 476,374,263 | Scale/Radius: 1.00 |
| 218 | `Roid_Med_Green2` | 2128 | Object | -1319.42,-1429.17,3415.76 | 316,20,158 | Scale/Radius: 1.00 |
| 219 | `Roid_Med_Green2` | 2130 | Object | 2440.29,-1965.11,-609.30 | 30,343,343 | Scale/Radius: 1.00 |
| 220 | `Roid_Med_Green2` | 2136 | Object | 2092.29,-1607.82,3431.38 | 439,444,434 | Scale/Radius: 1.00 |
| 221 | `Roid_Med_Green2` | 2139 | Object | -1993.06,1310.07,4452.23 | 44,73,329 | Scale/Radius: 1.00 |
| 222 | `Roid_Med_Green2` | 2157 | Object | -164.05,2171.78,2825.95 | 414,80,473 | Scale/Radius: 1.00 |
| 223 | `Roid_Med_Green2` | 2180 | Object | 1482.60,5103.68,4589.77 | 489,287,151 | Scale/Radius: 1.00 |
| 224 | `Roid_Med_Green2` | 2193 | Object | 1516.51,3474.84,3583.31 | 211,68,308 | Scale/Radius: 1.00 |
| 225 | `Roid_Med_Green2` | 2258 | Object | -127.72,990.64,2425.95 | 441,89,29 | Scale/Radius: 1.00 |
| 226 | `Roid_Med_Green2` | 2328 | Object | 1206.89,-3692.02,2050.26 | 98,325,225 | Scale/Radius: 1.00 |
| 227 | `Roid_Med_Green2` | 2340 | Object | 1775.96,2497.54,2310.52 | 189,6,335 | Scale/Radius: 1.00 |
| 228 | `Roid_Med_Green2` | 2366 | Object | 3092.44,-4017.79,4088.08 | 311,191,10 | Scale/Radius: 1.00 |
| 229 | `Roid_Med_Green2` | 2396 | Object | 2174.87,760.12,1603.67 | 213,167,303 | Scale/Radius: 1.00 |
| 230 | `Roid_Med_Green2` | 2414 | Object | 2575.80,1846.01,4795.94 | 75,52,406 | Scale/Radius: 1.00 |
| 231 | `Roid_Med_Green2` | 2437 | Object | 3363.50,-2063.19,2808.36 | 72,102,173 | Scale/Radius: 1.00 |
| 232 | `Roid_Med_Green2` | 2458 | Object | -738.86,-2171.78,4143.84 | 180,335,270 | Scale/Radius: 1.00 |
| 233 | `Roid_Med_Green2` | 2512 | Object | 3218.97,2823.31,3785.52 | 162,182,97 | Scale/Radius: 1.00 |
| 234 | `Roid_Med_Green2` | 2525 | Object | 655.14,-4995.09,2244.72 | 20,332,223 | Scale/Radius: 1.00 |
| 235 | `Roid_Med_Green2` | 2586 | Object | 3003.03,-2171.78,1911.60 | 389,172,498 | Scale/Radius: 1.00 |
| 236 | `Roid_Med_Green2` | 2589 | Object | -974.65,2284.36,3814.00 | 250,128,321 | Scale/Radius: 1.00 |
| 237 | `Roid_Med_Green2` | 2592 | Object | 3497.37,-2280.37,2203.27 | 33,265,67 | Scale/Radius: 1.00 |
| 238 | `Roid_Med_Green2` | 2595 | Object | 2826.00,3040.49,1329.59 | 382,243,434 | Scale/Radius: 1.00 |
| 239 | `Roid_Med_Green2` | 2618 | Object | 595.76,2714.72,4737.69 | 107,207,32 | Scale/Radius: 1.00 |
| 240 | `Roid_Med_Green2` | 2639 | Object | -1136.32,2061.90,3922.85 | 185,116,386 | Scale/Radius: 1.00 |
| 241 | `Roid_Med_Green2` | 2667 | Object | 2712.76,3800.61,3993.13 | 139,389,206 | Scale/Radius: 1.00 |
| 242 | `Roid_Med_Green2` | 2671 | Object | 1037.83,-325.77,5217.94 | 238,122,131 | Scale/Radius: 1.00 |
| 243 | `Roid_XL_Green` | 2191 | Object | 1626.58,2606.13,4558.56 | 52,260,25 | Scale/Radius: 1.00 |
| 244 | `Roid_XL_Green` | 1800 | Object | 414.10,2739.24,644.58 | 261,374,43 | Scale/Radius: 1.00 |
| 245 | `Roid_XL_Green` | 1815 | Object | -1348.47,-416.84,2188.17 | 240,503,261 | Scale/Radius: 1.00 |
| 246 | `Roid_XL_Green` | 1817 | Object | -858.31,2977.44,2194.41 | 360,178,86 | Scale/Radius: 1.00 |
| 247 | `Roid_XL_Green` | 1835 | Object | 436.01,-1429.17,-1265.64 | 290,262,303 | Scale/Radius: 1.00 |
| 248 | `Roid_XL_Green` | 1843 | Object | -2122.69,2739.24,2211.13 | 503,94,386 | Scale/Radius: 1.00 |
| 249 | `Roid_XL_Green` | 1857 | Object | -1798.99,-1548.27,3362.98 | 165,11,158 | Scale/Radius: 1.00 |
| 250 | `Roid_XL_Green` | 1867 | Object | -1888.32,-595.49,2896.68 | 412,88,216 | Scale/Radius: 1.00 |
| 251 | `Roid_XL_Green` | 1915 | Object | -296.26,2798.79,-1130.77 | 405,286,396 | Scale/Radius: 1.00 |
| 252 | `Roid_XL_Green` | 1923 | Object | -923.33,2620.14,2113.77 | 205,424,11 | Scale/Radius: 1.00 |
| 253 | `Roid_XL_Green` | 2030 | Object | -2547.16,119.10,2879.28 | 145,469,71 | Scale/Radius: 1.00 |
| 254 | `Roid_XL_Green` | 2033 | Object | 2654.64,2143.75,-1354.54 | 205,152,57 | Scale/Radius: 1.00 |
| 255 | `Roid_XL_Green` | 2036 | Object | -345.93,-1190.97,175.31 | 492,43,427 | Scale/Radius: 1.00 |
| 256 | `Roid_XL_Green` | 2057 | Object | -2031.19,-833.68,2651.54 | 297,105,427 | Scale/Radius: 1.00 |
| 257 | `Roid_XL_Green` | 2062 | Object | 1120.56,833.68,743.69 | 140,0,5 | Scale/Radius: 1.00 |
| 258 | `Roid_XL_Green` | 2100 | Object | 842.81,-2381.95,-845.92 | 166,471,39 | Scale/Radius: 1.00 |
| 259 | `Roid_XL_Green` | 2105 | Object | -431.22,-238.19,2958.13 | 325,0,323 | Scale/Radius: 1.00 |
| 260 | `Roid_XL_Green` | 2107 | Object | 1628.00,-2858.34,830.07 | 63,147,81 | Scale/Radius: 1.00 |
| 261 | `Roid_XL_Green` | 2145 | Object | 1653.80,-1071.88,596.09 | 88,298,448 | Scale/Radius: 1.00 |
| 262 | `Roid_XL_Green` | 2182 | Object | 2108.11,5320.85,5384.76 | 236,222,327 | Scale/Radius: 1.00 |
| 263 | `Roid_XL_Green` | 2205 | Object | 445.36,-5212.27,5036.17 | 72,171,343 | Scale/Radius: 1.00 |
| 264 | `Roid_XL_Green` | 2245 | Object | -54.48,-2606.13,2700.77 | 106,415,86 | Scale/Radius: 1.00 |
| 265 | `Roid_XL_Green` | 2255 | Object | 2729.28,108.59,4299.74 | 438,304,382 | Scale/Radius: 1.00 |
| 266 | `Roid_XL_Green` | 2318 | Object | 1490.45,3583.43,4148.88 | 346,212,449 | Scale/Radius: 1.00 |
| 267 | `Roid_XL_Green` | 2391 | Object | -79.32,1628.83,3022.86 | 448,41,89 | Scale/Radius: 1.00 |
| 268 | `Roid_XL_Green` | 2407 | Object | 792.71,4452.14,2480.77 | 167,488,246 | Scale/Radius: 1.00 |
| 269 | `Roid_XL_Green` | 2415 | Object | -1872.22,4452.14,4120.50 | 342,238,404 | Scale/Radius: 1.00 |
| 270 | `Roid_XL_Green` | 2434 | Object | -948.63,-3040.49,5426.95 | 439,184,428 | Scale/Radius: 1.00 |
| 271 | `Roid_XL_Green` | 2446 | Object | -241.87,-1085.89,3429.21 | 153,195,396 | Scale/Radius: 1.00 |
| 272 | `Roid_XL_Green` | 2480 | Object | -591.84,2931.90,4503.24 | 442,422,139 | Scale/Radius: 1.00 |
| 273 | `Roid_XL_Green` | 2521 | Object | 1506.23,2931.90,2591.99 | 414,474,376 | Scale/Radius: 1.00 |
| 274 | `Roid_XL_Green` | 2539 | Object | 163.80,3692.02,4831.32 | 197,504,156 | Scale/Radius: 1.00 |
| 275 | `Roid_XL_Green` | 2540 | Object | 290.33,2388.96,1745.87 | 142,505,480 | Scale/Radius: 1.00 |
| 276 | `Roid_XL_Green` | 2553 | Object | -1159.25,-2933.19,3883.51 | 293,449,461 | Scale/Radius: 1.00 |
| 277 | `Roid_XL_Green` | 2572 | Object | 2676.12,108.59,2527.23 | 364,195,121 | Scale/Radius: 1.00 |
| 278 | `Roid_XL_Green` | 2582 | Object | 1886.66,-3149.08,4550.44 | 105,491,72 | Scale/Radius: 1.00 |
| 279 | `Roid_XL_Green` | 2591 | Object | 3362.96,-3366.25,3754.31 | 165,122,288 | Scale/Radius: 1.00 |
| 280 | `Roid_XL_Green` | 2596 | Object | -949.04,1198.47,3724.25 | 437,41,224 | Scale/Radius: 1.00 |
| 281 | `Roid_XL_Green` | 2605 | Object | 278.45,2714.72,5028.03 | 182,378,339 | Scale/Radius: 1.00 |
| 282 | `Roid_XL_Green` | 2635 | Object | -888.20,108.59,1115.06 | 347,236,138 | Scale/Radius: 1.00 |
| 283 | `Roid_XL_Green` | 2665 | Object | 817.72,-1194.48,3041.10 | 504,297,51 | Scale/Radius: 1.00 |
| 284 | `Roid_XL_Green` | 2678 | Object | 2788.58,0.00,4882.76 | 164,469,413 | Scale/Radius: 1.00 |
| 285 | `Roid_XL_Green` | 2683 | Object | -339.76,272.12,1619.37 | 71,304,328 | Scale/Radius: 1.00 |
| 286 | `Roid_XL_Green` | 2197 | Object | -693.70,-2497.54,4751.31 | 19,70,92 | Scale/Radius: 1.00 |
| 287 | `Roid_XL_Green` | 1806 | Object | -214.94,2084.21,-156.46 | 230,12,184 | Scale/Radius: 1.00 |
| 288 | `Roid_XL_Green` | 1824 | Object | -1565.34,2917.89,1159.54 | 458,354,229 | Scale/Radius: 1.00 |
| 289 | `Roid_XL_Green` | 1834 | Object | 947.99,2441.50,-943.71 | 323,280,279 | Scale/Radius: 1.00 |
| 290 | `Roid_XL_Green` | 1872 | Object | -1793.52,2917.89,489.76 | 62,399,162 | Scale/Radius: 1.00 |
| 291 | `Roid_XL_Green` | 1892 | Object | 68.85,-2679.69,-504.31 | 250,445,23 | Scale/Radius: 1.00 |
| 292 | `Roid_XL_Green` | 1902 | Object | -2240.03,-416.84,2818.81 | 280,287,258 | Scale/Radius: 1.00 |
| 293 | `Roid_XL_Green` | 1913 | Object | 1241.62,-1607.82,673.14 | 310,497,173 | Scale/Radius: 1.00 |
| 294 | `Roid_XL_Green` | 1996 | Object | 654.26,595.49,-334.64 | 248,130,88 | Scale/Radius: 1.00 |
| 295 | `Roid_XL_Green` | 2053 | Object | -358.78,-2679.69,1003.68 | 69,261,136 | Scale/Radius: 1.00 |
| 296 | `Roid_XL_Green` | 2063 | Object | -2098.68,-59.55,3092.26 | 171,446,454 | Scale/Radius: 1.00 |
| 297 | `Roid_XL_Green` | 2066 | Object | 2950.32,1786.46,-1125.49 | 245,392,25 | Scale/Radius: 1.00 |
| 298 | `Roid_XL_Green` | 2080 | Object | -791.03,2858.34,1225.75 | 383,220,210 | Scale/Radius: 1.00 |
| 299 | `Roid_XL_Green` | 2087 | Object | -2547.47,-1250.52,2158.99 | 291,215,10 | Scale/Radius: 1.00 |
| 300 | `Roid_XL_Green` | 2089 | Object | -2343.64,2679.69,3449.56 | 443,111,479 | Scale/Radius: 1.00 |
| 301 | `Roid_XL_Green` | 2111 | Object | -1890.82,2798.79,1714.13 | 288,269,209 | Scale/Radius: 1.00 |
| 302 | `Roid_XL_Green` | 2122 | Object | -224.75,2084.21,1086.31 | 84,250,321 | Scale/Radius: 1.00 |
| 303 | `Roid_XL_Green` | 2129 | Object | -2783.51,476.39,3581.52 | 436,505,292 | Scale/Radius: 1.00 |
| 304 | `Roid_XL_Green` | 2137 | Object | 687.96,-476.39,557.95 | 405,263,181 | Scale/Radius: 1.00 |
| 305 | `Roid_XL_Green` | 2142 | Object | 1436.20,-1012.33,-1775.59 | 180,483,108 | Scale/Radius: 1.00 |
| 306 | `Roid_XL_Green` | 2238 | Object | -565.86,3800.61,1076.70 | 231,289,447 | Scale/Radius: 1.00 |
| 307 | `Roid_XL_Green` | 2313 | Object | 2774.49,3149.08,329.47 | 51,167,85 | Scale/Radius: 1.00 |
| 308 | `Roid_XL_Green` | 2484 | Object | 619.39,5320.85,2739.91 | 6,152,455 | Scale/Radius: 1.00 |
| 309 | `Roid_XL_Green` | 2496 | Object | 357.05,5212.27,1733.26 | 164,318,320 | Scale/Radius: 1.00 |
| 310 | `Roid_XL_Green` | 2510 | Object | 2522.52,-325.77,3034.96 | 490,110,244 | Scale/Radius: 1.00 |
| 311 | `Roid_XL_Green` | 2625 | Object | 497.63,325.77,4847.58 | 345,216,487 | Scale/Radius: 1.00 |
| 312 | `Roid_XL_Green` | 2660 | Object | 988.58,1303.07,3624.37 | 61,351,437 | Scale/Radius: 1.00 |
| 313 | `Roid_XL_Green` | 2684 | Object | -1266.95,-4777.91,3767.74 | 360,227,20 | Scale/Radius: 1.00 |
