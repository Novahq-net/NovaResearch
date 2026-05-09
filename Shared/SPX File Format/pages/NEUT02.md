# Tachyon: The Fringe NEUT02.SPX - Picking the Stone

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT02.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `NEUTRA2.BDF` |
| Region | 1 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 6 |
| Entities | 321 |
| Events | 1 |
| Waypoints | 0 |
| Child Sectors | 2 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Colony_Station`, `1: Spcargo_Food`, `2: Roid_XL_Green`, `3: Roid_Med_Green`, `4: Roid_Med_Green2`, `5: Hyper_Gate` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `G02BFA`, `BFIGH` |
| Aliases | `fred_fighter2`, `fred_fighter1`, `fred_freighter1`, `fred_freighter2` |
| Groups | `CONT_063` |
| Child Sectors | [neut02A.spx](NEUT02A.md), [neut02B.spx](NEUT02B.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 1487; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 198
- Set/add variable: variable group 13, variable 805, subtype 0, value 1

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | -1980.65,0.00,2590.43 | 256,0,0 | Gate SPX: [neut03.spx](NEUT03.md) |
| 1 | `Hyper_Gate` | 2 | Gate | -959.37,0.00,-2118.02 | 0,0,0 | Gate SPX: [neut01.spx](NEUT01.md) |
| 2 | `Roid_Med_Green2` | 46 | Object | 1362.88,-823.14,-808.22 | 325,256,134 | Scale/Radius: 4.00 |
| 3 | `Roid_Med_Green` | 51 | Object | 1335.01,392.86,-2372.07 | 435,383,219 | Scale/Radius: 5.00 |
| 4 | `Roid_Med_Green` | 53 | Object | 3023.56,-561.23,3142.66 | 90,398,121 | Scale/Radius: 3.00 |
| 5 | `Roid_Med_Green` | 55 | Object | 2091.94,-579.94,2528.91 | 220,39,508 | Scale/Radius: 6.00 |
| 6 | `Roid_Med_Green2` | 58 | Object | 3964.29,430.28,2987.55 | 147,199,74 | Scale/Radius: 3.00 |
| 7 | `Roid_Med_Green2` | 59 | Object | 3093.93,-430.28,-3676.16 | 228,63,224 | Scale/Radius: 9.00 |
| 8 | `Roid_Med_Green` | 60 | Object | 680.90,0.00,3191.62 | 68,321,496 | Scale/Radius: 4.00 |
| 9 | `Roid_XL_Green` | 65 | Object | 4106.51,74.83,-1509.35 | 90,253,510 | Scale/Radius: 4.00 |
| 10 | `Roid_Med_Green2` | 68 | Object | 938.91,205.78,1445.71 | 79,10,159 | Scale/Radius: 5.00 |
| 11 | `Roid_XL_Green` | 72 | Object | 4189.45,187.08,-1978.38 | 388,13,393 | Scale/Radius: 4.00 |
| 12 | `Roid_Med_Green2` | 73 | Object | 155.12,448.98,2721.76 | 477,142,499 | Scale/Radius: 7.00 |
| 13 | `Roid_Med_Green2` | 77 | Object | 2641.32,748.30,-1327.41 | 511,315,327 | Scale/Radius: 5.00 |
| 14 | `Roid_Med_Green` | 78 | Object | 3198.29,280.61,-714.51 | 255,469,276 | Scale/Radius: 2.00 |
| 15 | `Roid_Med_Green` | 86 | Object | 616.08,-280.61,1262.82 | 122,42,484 | Scale/Radius: 4.00 |
| 16 | `Roid_Med_Green2` | 87 | Object | 2771.27,-112.25,-2568.89 | 502,331,286 | Scale/Radius: 6.00 |
| 17 | `Roid_Med_Green` | 93 | Object | 4581.74,785.72,-790.83 | 119,424,376 | Scale/Radius: 2.00 |
| 18 | `Roid_Med_Green2` | 96 | Object | 2321.86,-729.60,-2501.06 | 140,72,449 | Scale/Radius: 5.00 |
| 19 | `Roid_Med_Green` | 97 | Object | 2267.30,-224.49,3402.27 | 446,314,44 | Scale/Radius: 7.00 |
| 20 | `Roid_Med_Green` | 100 | Object | 6066.61,-542.52,-1153.71 | 62,498,427 | Scale/Radius: 8.00 |
| 21 | `Roid_Med_Green2` | 102 | Object | 3914.89,-823.14,-2867.08 | 338,5,255 | Scale/Radius: 2.00 |
| 22 | `Roid_Med_Green` | 109 | Object | 4161.80,804.43,-1822.03 | 278,269,42 | Scale/Radius: 6.00 |
| 23 | `Roid_Med_Green` | 110 | Object | 2414.72,505.11,2281.74 | 376,194,291 | Scale/Radius: 8.00 |
| 24 | `Roid_Med_Green` | 112 | Object | 5172.11,-729.60,-112.38 | 127,50,163 | Scale/Radius: 8.00 |
| 25 | `Roid_Med_Green2` | 113 | Object | 2580.61,130.95,1343.67 | 58,40,91 | Scale/Radius: 1.00 |
| 26 | `Roid_Med_Green` | 124 | Object | 2008.43,187.08,-1302.55 | 173,431,259 | Scale/Radius: 2.00 |
| 27 | `Roid_Med_Green2` | 126 | Object | 413.31,561.23,2266.00 | 61,86,493 | Scale/Radius: 7.00 |
| 28 | `Roid_Med_Green` | 130 | Object | 1962.99,-710.89,3831.91 | 18,363,411 | Scale/Radius: 2.00 |
| 29 | `Roid_Med_Green2` | 132 | Object | 2607.75,-897.97,-2683.11 | 109,28,305 | Scale/Radius: 4.00 |
| 30 | `Roid_Med_Green2` | 133 | Object | 2783.39,523.81,340.50 | 383,322,97 | Scale/Radius: 1.00 |
| 31 | `Roid_Med_Green` | 134 | Object | -564.48,0.00,1196.07 | 444,93,46 | Scale/Radius: 5.00 |
| 32 | `Roid_Med_Green2` | 137 | Object | 1916.48,149.66,795.44 | 138,393,345 | Scale/Radius: 9.00 |
| 33 | `Roid_XL_Green` | 138 | Object | 4969.16,-841.84,-399.35 | 423,425,260 | Scale/Radius: 1.00 |
| 34 | `Roid_Med_Green` | 141 | Object | 5937.38,523.81,-2000.95 | 209,23,234 | Scale/Radius: 8.00 |
| 35 | `Roid_Med_Green` | 142 | Object | 4166.73,486.40,-595.92 | 84,352,156 | Scale/Radius: 3.00 |
| 36 | `Roid_Med_Green` | 143 | Object | 2635.23,-748.30,-4129.60 | 131,54,313 | Scale/Radius: 3.00 |
| 37 | `Roid_Med_Green2` | 147 | Object | 6518.51,-729.60,-1413.74 | 325,477,263 | Scale/Radius: 4.00 |
| 38 | `Roid_Med_Green` | 149 | Object | 1667.41,-729.60,482.34 | 125,154,32 | Scale/Radius: 5.00 |
| 39 | `Roid_Med_Green2` | 152 | Object | 3272.34,430.28,1305.51 | 368,320,465 | Scale/Radius: 8.00 |
| 40 | `Roid_Med_Green2` | 153 | Object | 4646.05,748.30,-2732.48 | 439,155,505 | Scale/Radius: 4.00 |
| 41 | `Roid_Med_Green2` | 155 | Object | 1372.29,168.37,573.16 | 333,94,353 | Scale/Radius: 6.00 |
| 42 | `Roid_XL_Green` | 159 | Object | 2927.15,-897.97,-1939.52 | 376,417,22 | Scale/Radius: 1.00 |
| 43 | `Roid_Med_Green2` | 162 | Object | 3097.04,411.57,862.20 | 364,381,125 | Scale/Radius: 3.00 |
| 44 | `Roid_Med_Green2` | 163 | Object | 2737.61,-467.69,2894.67 | 60,37,151 | Scale/Radius: 2.00 |
| 45 | `Roid_Med_Green` | 166 | Object | 3785.77,-860.55,-2854.22 | 281,343,17 | Scale/Radius: 4.00 |
| 46 | `Roid_Med_Green2` | 168 | Object | 2872.74,0.00,-2425.41 | 255,432,313 | Scale/Radius: 2.00 |
| 47 | `Roid_Med_Green2` | 176 | Object | 2295.00,785.72,3675.98 | 227,346,453 | Scale/Radius: 4.00 |
| 48 | `Roid_Med_Green` | 178 | Object | 1151.32,-280.61,3544.11 | 46,189,191 | Scale/Radius: 6.00 |
| 49 | `Roid_Med_Green` | 180 | Object | 4922.93,617.35,-1285.58 | 280,398,229 | Scale/Radius: 4.00 |
| 50 | `Roid_Med_Green2` | 184 | Object | 3426.05,804.43,-2971.99 | 476,140,178 | Scale/Radius: 8.00 |
| 51 | `Roid_Med_Green2` | 185 | Object | -370.60,280.61,2681.95 | 33,510,235 | Scale/Radius: 4.00 |
| 52 | `Roid_XL_Green` | 186 | Object | 4720.21,486.40,147.65 | 231,505,105 | Scale/Radius: 1.00 |
| 53 | `Roid_Med_Green2` | 189 | Object | 2718.29,579.94,-3738.54 | 506,316,194 | Scale/Radius: 9.00 |
| 54 | `Roid_Med_Green2` | 190 | Object | 1483.05,280.61,1237.93 | 194,244,104 | Scale/Radius: 5.00 |
| 55 | `Roid_Med_Green` | 191 | Object | 3121.75,935.38,-2542.36 | 405,401,202 | Scale/Radius: 3.00 |
| 56 | `Roid_Med_Green` | 193 | Object | 3835.06,-523.81,2140.31 | 40,349,44 | Scale/Radius: 9.00 |
| 57 | `Roid_Med_Green` | 196 | Object | 1517.00,-93.54,2584.16 | 413,216,75 | Scale/Radius: 6.00 |
| 58 | `Roid_XL_Green` | 198 | Object | 1851.72,748.30,-703.30 | 41,397,68 | Scale/Radius: 3.00 |
| 59 | `Roid_Med_Green2` | 201 | Object | 708.43,-897.97,2175.17 | 233,411,102 | Scale/Radius: 5.00 |
| 60 | `Roid_Med_Green` | 207 | Object | 3613.75,299.32,2530.97 | 494,15,469 | Scale/Radius: 4.00 |
| 61 | `Roid_Med_Green2` | 212 | Object | 2986.16,-505.11,-662.67 | 327,466,152 | Scale/Radius: 9.00 |
| 62 | `Roid_Med_Green2` | 216 | Object | 3805.31,-74.83,190.31 | 336,140,62 | Scale/Radius: 4.00 |
| 63 | `Roid_Med_Green` | 217 | Object | 5190.52,0.00,-359.96 | 478,333,271 | Scale/Radius: 4.00 |
| 64 | `Roid_XL_Green` | 218 | Object | -186.13,-748.30,2786.46 | 459,305,57 | Scale/Radius: 5.00 |
| 65 | `Roid_Med_Green` | 225 | Object | 2746.67,-767.01,1695.76 | 240,303,266 | Scale/Radius: 5.00 |
| 66 | `Roid_Med_Green2` | 227 | Object | 2248.09,-692.18,-2370.84 | 350,366,417 | Scale/Radius: 5.00 |
| 67 | `Roid_Med_Green2` | 232 | Object | 2451.66,-18.71,2646.68 | 234,429,395 | Scale/Radius: 2.00 |
| 68 | `Roid_Med_Green2` | 234 | Object | 2368.26,-823.14,-324.68 | 4,255,293 | Scale/Radius: 2.00 |
| 69 | `Roid_Med_Green2` | 236 | Object | 2238.74,-374.15,-3322.17 | 503,346,484 | Scale/Radius: 3.00 |
| 70 | `Roid_Med_Green2` | 238 | Object | 3871.66,598.64,-75.04 | 464,271,353 | Scale/Radius: 4.00 |
| 71 | `Roid_Med_Green` | 240 | Object | 2857.49,130.95,2790.58 | 269,32,376 | Scale/Radius: 9.00 |
| 72 | `Roid_Med_Green` | 245 | Object | 3804.24,804.43,-2671.75 | 359,383,85 | Scale/Radius: 3.00 |
| 73 | `Roid_Med_Green2` | 247 | Object | 1944.13,636.06,639.09 | 406,61,58 | Scale/Radius: 8.00 |
| 74 | `Roid_Med_Green2` | 253 | Object | 1307.47,467.69,-1355.63 | 125,373,27 | Scale/Radius: 8.00 |
| 75 | `Roid_Med_Green` | 254 | Object | -730.43,916.67,1704.08 | 395,422,222 | Scale/Radius: 7.00 |
| 76 | `Roid_Med_Green` | 255 | Object | 81.30,93.54,2421.93 | 298,235,39 | Scale/Radius: 9.00 |
| 77 | `Roid_Med_Green` | 259 | Object | 606.68,-804.43,-118.56 | 432,250,172 | Scale/Radius: 6.00 |
| 78 | `Roid_XL_Green` | 260 | Object | -616.53,-224.49,2823.93 | 382,113,309 | Scale/Radius: 1.00 |
| 79 | `Roid_Med_Green` | 262 | Object | 2512.19,-374.15,-1314.56 | 399,87,268 | Scale/Radius: 4.00 |
| 80 | `Roid_Med_Green` | 268 | Object | 2964.75,-336.74,-4093.35 | 3,171,424 | Scale/Radius: 5.00 |
| 81 | `Roid_Med_Green2` | 271 | Object | 1888.60,-561.23,-768.41 | 340,336,347 | Scale/Radius: 3.00 |
| 82 | `Roid_Med_Green2` | 272 | Object | 1621.52,-542.52,2176.41 | 326,449,123 | Scale/Radius: 5.00 |
| 83 | `Roid_Med_Green` | 274 | Object | 1261.52,-56.12,-91.61 | 495,60,30 | Scale/Radius: 9.00 |
| 84 | `Roid_XL_Green` | 275 | Object | 5402.59,860.55,-841.85 | 334,181,363 | Scale/Radius: 3.00 |
| 85 | `Roid_Med_Green2` | 279 | Object | 5070.47,261.91,-1546.01 | 344,223,90 | Scale/Radius: 1.00 |
| 86 | `Roid_Med_Green` | 282 | Object | 4325.99,187.08,-1203.51 | 404,432,421 | Scale/Radius: 4.00 |
| 87 | `Roid_Med_Green` | 285 | Object | 5245.76,897.97,-1102.70 | 235,432,242 | Scale/Radius: 6.00 |
| 88 | `Roid_Med_Green` | 288 | Object | 1067.81,-860.55,-287.35 | 173,281,345 | Scale/Radius: 3.00 |
| 89 | `Roid_Med_Green2` | 293 | Object | 929.51,-804.43,64.32 | 281,42,456 | Scale/Radius: 4.00 |
| 90 | `Roid_Med_Green` | 294 | Object | 5466.95,336.74,-2353.45 | 20,176,420 | Scale/Radius: 3.00 |
| 91 | `Roid_Med_Green2` | 298 | Object | 552.92,-841.84,1483.18 | 261,454,139 | Scale/Radius: 7.00 |
| 92 | `Roid_Med_Green2` | 299 | Object | 2248.66,-74.83,1929.65 | 125,326,48 | Scale/Radius: 5.00 |
| 93 | `Roid_Med_Green` | 301 | Object | 1944.01,748.30,-221.00 | 53,83,280 | Scale/Radius: 3.00 |
| 94 | `Roid_Med_Green` | 304 | Object | 3622.93,-93.54,2192.15 | 359,406,418 | Scale/Radius: 7.00 |
| 95 | `Roid_Med_Green2` | 307 | Object | 5005.93,374.15,-1324.56 | 220,133,170 | Scale/Radius: 7.00 |
| 96 | `Roid_XL_Green` | 309 | Object | 4388.14,168.37,-126.47 | 72,364,294 | Scale/Radius: 2.00 |
| 97 | `Roid_Med_Green` | 312 | Object | 4554.09,280.61,-634.49 | 401,343,390 | Scale/Radius: 8.00 |
| 98 | `Roid_Med_Green` | 314 | Object | -951.73,-673.47,2094.74 | 413,181,447 | Scale/Radius: 3.00 |
| 99 | `Roid_Med_Green2` | 317 | Object | 4021.63,224.49,-1203.93 | 470,301,49 | Scale/Radius: 9.00 |
| 100 | `Roid_Med_Green` | 318 | Object | 5660.83,-505.11,-867.56 | 456,188,296 | Scale/Radius: 2.00 |
| 101 | `Roid_Med_Green2` | 320 | Object | 2183.33,-74.83,-3869.58 | 134,6,50 | Scale/Radius: 3.00 |
| 102 | `Roid_Med_Green` | 321 | Object | 1464.86,579.94,3205.71 | 339,220,86 | Scale/Radius: 5.00 |
| 103 | `Roid_Med_Green` | 324 | Object | -776.49,-224.49,2108.00 | 166,291,297 | Scale/Radius: 9.00 |
| 104 | `Roid_Med_Green2` | 330 | Object | 3108.76,823.14,-1548.88 | 280,116,93 | Scale/Radius: 1.00 |
| 105 | `Roid_Med_Green` | 332 | Object | 3149.34,-748.30,-3128.75 | 336,44,387 | Scale/Radius: 5.00 |
| 106 | `Roid_Med_Green2` | 333 | Object | 5503.89,841.84,-1988.51 | 238,242,365 | Scale/Radius: 8.00 |
| 107 | `Roid_Med_Green2` | 335 | Object | 1842.88,-224.49,2215.80 | 271,158,48 | Scale/Radius: 5.00 |
| 108 | `Roid_Med_Green` | 337 | Object | 127.30,-336.74,1587.96 | 445,186,455 | Scale/Radius: 6.00 |
| 109 | `Roid_Med_Green` | 339 | Object | 855.57,542.52,-1095.61 | 149,389,214 | Scale/Radius: 5.00 |
| 110 | `Roid_Med_Green` | 1370 | Object | 3820.84,1383.87,-1254.96 | 224,380,131 | Scale/Radius: 4.00 |
| 111 | `Roid_Med_Green2` | 1371 | Object | 2910.76,1333.98,569.23 | 353,186,118 | Scale/Radius: 4.00 |
| 112 | `Roid_Med_Green` | 1372 | Object | 578.57,1184.32,1143.72 | 250,207,446 | Scale/Radius: 2.00 |
| 113 | `Roid_Med_Green2` | 1373 | Object | 2888.98,1209.26,3441.59 | 15,200,79 | Scale/Radius: 4.00 |
| 114 | `Roid_Med_Green` | 1374 | Object | 1263.81,1371.40,2020.39 | 241,349,415 | Scale/Radius: 3.00 |
| 115 | `Roid_Med_Green` | 1375 | Object | 2816.77,1290.33,2329.23 | 303,59,459 | Scale/Radius: 2.00 |
| 116 | `Roid_Med_Green` | 1376 | Object | 2398.58,1084.55,-297.85 | 390,305,238 | Scale/Radius: 6.00 |
| 117 | `Roid_Med_Green2` | 1377 | Object | 42.92,1209.26,2182.98 | 334,468,377 | Scale/Radius: 2.00 |
| 118 | `Roid_Med_Green2` | 1378 | Object | 3048.80,1371.40,3779.39 | 446,248,245 | Scale/Radius: 3.00 |
| 119 | `Roid_Med_Green` | 1379 | Object | 633.87,1178.08,2905.87 | 399,250,0 | Scale/Radius: 9.00 |
| 120 | `Roid_Med_Green` | 1380 | Object | 171.32,1377.63,1242.70 | 38,375,391 | Scale/Radius: 4.00 |
| 121 | `Roid_Med_Green2` | 1381 | Object | 1769.20,1502.35,1482.49 | 54,328,352 | Scale/Radius: 6.00 |
| 122 | `Roid_Med_Green2` | 1382 | Object | 2766.81,1203.03,-12.86 | 252,38,250 | Scale/Radius: 5.00 |
| 123 | `Roid_Med_Green2` | 1383 | Object | 3675.63,1539.76,1167.36 | 264,137,240 | Scale/Radius: 3.00 |
| 124 | `Roid_Med_Green` | 1384 | Object | 2350.47,1115.73,1735.39 | 403,495,3 | Scale/Radius: 5.00 |
| 125 | `Roid_Med_Green2` | 1385 | Object | 629.54,1140.67,1855.93 | 278,58,102 | Scale/Radius: 4.00 |
| 126 | `Roid_Med_Green2` | 1386 | Object | 617.66,1034.66,11.99 | 437,229,109 | Scale/Radius: 1.00 |
| 127 | `Roid_Med_Green` | 1387 | Object | -703.34,1290.33,1901.09 | 435,437,249 | Scale/Radius: 8.00 |
| 128 | `Roid_Med_Green2` | 1388 | Object | -417.93,1365.16,1485.83 | 328,239,319 | Scale/Radius: 1.00 |
| 129 | `Roid_Med_Green2` | 1389 | Object | 3252.17,1065.84,-1627.54 | 387,504,316 | Scale/Radius: 9.00 |
| 130 | `Roid_Med_Green` | 1392 | Object | 4350.97,978.54,-1087.50 | 131,91,236 | Scale/Radius: 9.00 |
| 131 | `Roid_Med_Green2` | 1393 | Object | 2902.86,947.36,317.50 | 26,229,20 | Scale/Radius: 6.00 |
| 132 | `Roid_Med_Green2` | 1395 | Object | 2371.84,1383.87,-3527.38 | 147,272,361 | Scale/Radius: 8.00 |
| 133 | `Roid_Med_Green` | 1396 | Object | 3273.24,1009.72,-956.24 | 298,491,197 | Scale/Radius: 8.00 |
| 134 | `Roid_Med_Green2` | 1397 | Object | 4888.03,1383.87,-1721.86 | 105,398,468 | Scale/Radius: 4.00 |
| 135 | `Roid_Med_Green2` | 1398 | Object | 2984.49,1246.68,2918.76 | 1,425,337 | Scale/Radius: 2.00 |
| 136 | `Roid_Med_Green2` | 1400 | Object | 2124.82,1022.19,-700.20 | 169,360,239 | Scale/Radius: 7.00 |
| 137 | `Roid_Med_Green` | 1401 | Object | 1797.28,1003.48,-1627.53 | 91,392,263 | Scale/Radius: 9.00 |
| 138 | `Roid_Med_Green2` | 1402 | Object | 2240.68,991.01,2991.92 | 280,145,450 | Scale/Radius: 4.00 |
| 139 | `Roid_Med_Green` | 1403 | Object | 4780.80,966.06,721.98 | 209,220,198 | Scale/Radius: 1.00 |
| 140 | `Roid_Med_Green` | 1404 | Object | 2286.16,1128.20,874.76 | 364,207,217 | Scale/Radius: 3.00 |
| 141 | `Roid_Med_Green2` | 1405 | Object | 4750.72,978.54,952.20 | 4,278,77 | Scale/Radius: 2.00 |
| 142 | `Roid_Med_Green2` | 1406 | Object | 2198.55,1309.04,1649.33 | 130,445,69 | Scale/Radius: 3.00 |
| 143 | `Roid_Med_Green2` | 1407 | Object | 1983.03,1072.07,-2841.02 | 176,408,317 | Scale/Radius: 1.00 |
| 144 | `Roid_Med_Green` | 1408 | Object | 3314.86,1309.04,-1781.59 | 24,248,85 | Scale/Radius: 6.00 |
| 145 | `Roid_Med_Green` | 1409 | Object | 3205.59,1059.60,1642.87 | 2,282,495 | Scale/Radius: 1.00 |
| 146 | `Roid_Med_Green2` | 1410 | Object | 2575.80,1496.11,1032.81 | 226,96,113 | Scale/Radius: 4.00 |
| 147 | `Roid_Med_Green2` | 1411 | Object | 1970.26,1053.37,-870.17 | 423,122,72 | Scale/Radius: 7.00 |
| 148 | `Roid_Med_Green` | 1412 | Object | -356.25,1327.75,2262.55 | 441,467,17 | Scale/Radius: 7.00 |
| 149 | `Roid_Med_Green` | 1413 | Object | 2103.04,1433.75,2172.17 | 206,126,488 | Scale/Radius: 2.00 |
| 150 | `Roid_Med_Green` | 1416 | Object | 4163.70,959.83,-1111.16 | 169,365,443 | Scale/Radius: 3.00 |
| 151 | `Roid_Med_Green2` | 1417 | Object | 3098.43,947.36,2983.30 | 446,417,62 | Scale/Radius: 1.00 |
| 152 | `Roid_Med_Green2` | 1418 | Object | 676.71,1371.40,704.80 | 99,394,362 | Scale/Radius: 4.00 |
| 153 | `Roid_Med_Green` | 1419 | Object | 1179.60,1408.81,1781.90 | 247,414,98 | Scale/Radius: 9.00 |
| 154 | `Roid_Med_Green2` | 1420 | Object | 1860.48,1421.28,386.35 | 117,280,176 | Scale/Radius: 8.00 |
| 155 | `Roid_Med_Green2` | 1421 | Object | 3930.24,1371.40,-1664.49 | 399,241,165 | Scale/Radius: 4.00 |
| 156 | `Roid_Med_Green` | 1422 | Object | 677.82,1047.13,-448.45 | 166,252,276 | Scale/Radius: 5.00 |
| 157 | `Roid_Med_Green` | 1423 | Object | 2764.51,959.83,3041.40 | 131,237,294 | Scale/Radius: 6.00 |
| 158 | `Roid_Med_Green` | 1424 | Object | 2832.64,1408.81,1729.29 | 431,347,113 | Scale/Radius: 6.00 |
| 159 | `Roid_Med_Green2` | 1425 | Object | 4025.35,1521.06,1612.74 | 344,143,460 | Scale/Radius: 4.00 |
| 160 | `Roid_Med_Green2` | 1426 | Object | 2054.60,1365.16,1067.23 | 311,172,494 | Scale/Radius: 9.00 |
| 161 | `Roid_Med_Green` | 1427 | Object | 3334.99,1533.53,-1282.93 | 311,203,501 | Scale/Radius: 5.00 |
| 162 | `Roid_Med_Green2` | 1428 | Object | 1615.68,1533.53,907.04 | 509,266,426 | Scale/Radius: 2.00 |
| 163 | `Roid_Med_Green2` | 1430 | Object | 2829.60,1153.14,-389.39 | 175,503,287 | Scale/Radius: 2.00 |
| 164 | `Roid_Med_Green` | 1431 | Object | 2866.80,1171.85,3923.55 | 176,300,494 | Scale/Radius: 2.00 |
| 165 | `Roid_Med_Green2` | 1432 | Object | 2152.67,1078.31,1376.08 | 124,141,295 | Scale/Radius: 8.00 |
| 166 | `Roid_Med_Green2` | 1433 | Object | 1945.25,1527.29,1138.17 | 121,291,503 | Scale/Radius: 9.00 |
| 167 | `Roid_Med_Green2` | 1434 | Object | 3839.20,1234.21,435.83 | 110,139,147 | Scale/Radius: 9.00 |
| 168 | `Roid_Med_Green2` | 1436 | Object | 659.79,1371.40,1354.57 | 132,248,490 | Scale/Radius: 7.00 |
| 169 | `Roid_Med_Green2` | 1437 | Object | 3769.62,1084.55,-592.63 | 203,445,355 | Scale/Radius: 5.00 |
| 170 | `Roid_Med_Green` | 1438 | Object | 383.04,1496.11,1976.45 | 408,440,377 | Scale/Radius: 8.00 |
| 171 | `Roid_Med_Green2` | 1439 | Object | 676.54,1153.14,975.94 | 137,39,307 | Scale/Radius: 7.00 |
| 172 | `Roid_Med_Green` | 1440 | Object | 2421.17,1446.23,1610.60 | 208,126,300 | Scale/Radius: 9.00 |
| 173 | `Roid_Med_Green` | 44 | Object | 2211.38,-710.89,-1015.58 | 375,203,223 | Scale/Radius: 1.00 |
| 174 | `Roid_Med_Green` | 52 | Object | 293.08,261.91,-210.21 | 45,88,0 | Scale/Radius: 1.00 |
| 175 | `Roid_Med_Green` | 56 | Object | 735.86,-448.98,298.63 | 324,447,7 | Scale/Radius: 1.00 |
| 176 | `Roid_Med_Green` | 61 | Object | 3373.53,74.83,-701.24 | 504,114,217 | Scale/Radius: 1.00 |
| 177 | `Roid_Med_Green` | 64 | Object | 2820.55,523.81,2425.64 | 486,416,159 | Scale/Radius: 1.00 |
| 178 | `Roid_Med_Green` | 67 | Object | 3379.93,243.20,-2998.12 | 256,478,97 | Scale/Radius: 1.00 |
| 179 | `Roid_Med_Green` | 69 | Object | 4369.67,-205.78,-308.94 | 329,22,403 | Scale/Radius: 1.00 |
| 180 | `Roid_Med_Green` | 70 | Object | 154.72,411.57,-288.58 | 215,131,177 | Scale/Radius: 1.00 |
| 181 | `Roid_Med_Green` | 74 | Object | 2201.92,-448.98,-2827.01 | 379,447,111 | Scale/Radius: 1.00 |
| 182 | `Roid_Med_Green` | 75 | Object | 2346.07,280.61,-2096.69 | 380,210,71 | Scale/Radius: 1.00 |
| 183 | `Roid_Med_Green` | 76 | Object | 2206.85,-130.95,1640.08 | 45,100,404 | Scale/Radius: 1.00 |
| 184 | `Roid_Med_Green` | 79 | Object | 1270.93,598.64,1289.77 | 460,192,436 | Scale/Radius: 1.00 |
| 185 | `Roid_Med_Green` | 81 | Object | 4682.99,-392.86,-2367.54 | 64,454,183 | Scale/Radius: 1.00 |
| 186 | `Roid_Med_Green` | 84 | Object | 1759.37,-841.84,-1615.66 | 503,295,378 | Scale/Radius: 1.00 |
| 187 | `Roid_Med_Green` | 89 | Object | 1120.40,-392.86,2531.50 | 45,273,59 | Scale/Radius: 1.00 |
| 188 | `Roid_Med_Green` | 90 | Object | 782.31,673.47,2905.05 | 476,410,169 | Scale/Radius: 1.00 |
| 189 | `Roid_Med_Green` | 94 | Object | -555.30,-692.18,857.25 | 338,162,440 | Scale/Radius: 1.00 |
| 190 | `Roid_Med_Green` | 95 | Object | 1206.28,374.15,651.13 | 275,376,362 | Scale/Radius: 1.00 |
| 191 | `Roid_Med_Green` | 99 | Object | 2165.71,-879.26,2398.69 | 113,337,270 | Scale/Radius: 1.00 |
| 192 | `Roid_Med_Green` | 103 | Object | 3133.64,673.47,-1353.16 | 333,69,40 | Scale/Radius: 1.00 |
| 193 | `Roid_Med_Green` | 105 | Object | 744.92,56.12,-900.28 | 183,285,462 | Scale/Radius: 1.00 |
| 194 | `Roid_Med_Green` | 106 | Object | 3207.92,-841.84,2387.07 | 470,128,57 | Scale/Radius: 1.00 |
| 195 | `Roid_Med_Green` | 108 | Object | 588.32,-916.67,559.07 | 135,31,379 | Scale/Radius: 1.00 |
| 196 | `Roid_Med_Green` | 111 | Object | 2626.84,18.71,2229.90 | 455,315,123 | Scale/Radius: 1.00 |
| 197 | `Roid_Med_Green` | 115 | Object | 3537.83,-710.89,124.79 | 57,511,116 | Scale/Radius: 1.00 |
| 198 | `Roid_Med_Green` | 116 | Object | 4397.49,280.61,824.86 | 277,162,278 | Scale/Radius: 1.00 |
| 199 | `Roid_Med_Green` | 119 | Object | 3918.00,-280.61,1671.28 | 136,278,389 | Scale/Radius: 1.00 |
| 200 | `Roid_Med_Green` | 123 | Object | 2515.80,-56.12,-585.12 | 205,267,400 | Scale/Radius: 1.00 |
| 201 | `Roid_Med_Green` | 128 | Object | -121.71,-542.52,1704.91 | 38,391,140 | Scale/Radius: 1.00 |
| 202 | `Roid_Med_Green` | 131 | Object | 615.97,-18.71,402.72 | 377,174,505 | Scale/Radius: 1.00 |
| 203 | `Roid_Med_Green` | 135 | Object | 1741.24,617.35,782.17 | 425,363,246 | Scale/Radius: 1.00 |
| 204 | `Roid_Med_Green` | 136 | Object | 302.54,355.44,1601.23 | 218,161,374 | Scale/Radius: 1.00 |
| 205 | `Roid_Med_Green` | 139 | Object | 5411.82,74.83,-750.61 | 229,466,401 | Scale/Radius: 1.00 |
| 206 | `Roid_Med_Green` | 150 | Object | 3887.18,318.03,-3140.78 | 241,193,32 | Scale/Radius: 1.00 |
| 207 | `Roid_Med_Green` | 151 | Object | 920.44,-561.23,1263.24 | 130,179,262 | Scale/Radius: 1.00 |
| 208 | `Roid_Med_Green` | 154 | Object | 330.08,785.72,584.78 | 191,138,338 | Scale/Radius: 1.00 |
| 209 | `Roid_Med_Green` | 156 | Object | 4738.40,729.60,-1820.13 | 332,192,215 | Scale/Radius: 1.00 |
| 210 | `Roid_Med_Green` | 158 | Object | 3573.59,-448.98,-3232.43 | 60,150,168 | Scale/Radius: 1.00 |
| 211 | `Roid_Med_Green` | 160 | Object | 4987.58,-430.28,-646.93 | 368,339,486 | Scale/Radius: 1.00 |
| 212 | `Roid_Med_Green` | 164 | Object | 3761.35,-673.47,2700.58 | 459,401,235 | Scale/Radius: 1.00 |
| 213 | `Roid_Med_Green` | 165 | Object | 2635.23,542.52,-4129.60 | 437,49,399 | Scale/Radius: 1.00 |
| 214 | `Roid_Med_Green` | 167 | Object | -149.41,-411.57,1431.20 | 192,253,394 | Scale/Radius: 1.00 |
| 215 | `Roid_Med_Green` | 169 | Object | 1354.15,187.08,2970.99 | 318,254,499 | Scale/Radius: 1.00 |
| 216 | `Roid_Med_Green` | 172 | Object | 2564.21,841.84,575.90 | 323,240,11 | Scale/Radius: 1.00 |
| 217 | `Roid_Med_Green` | 174 | Object | 2650.44,336.74,-2096.28 | 289,236,135 | Scale/Radius: 1.00 |
| 218 | `Roid_Med_Green` | 179 | Object | 1298.80,-56.12,2853.63 | 93,46,465 | Scale/Radius: 1.00 |
| 219 | `Roid_Med_Green` | 187 | Object | 3029.51,261.91,-2594.61 | 346,263,77 | Scale/Radius: 1.00 |
| 220 | `Roid_Med_Green` | 188 | Object | 4350.92,-430.28,-2641.66 | 510,253,250 | Scale/Radius: 1.00 |
| 221 | `Roid_Med_Green` | 192 | Object | 1323.29,-692.18,2388.42 | 336,179,354 | Scale/Radius: 1.00 |
| 222 | `Roid_Med_Green` | 194 | Object | 2863.39,879.26,-3376.74 | 268,76,16 | Scale/Radius: 1.00 |
| 223 | `Roid_Med_Green` | 199 | Object | 3398.29,448.98,-3675.75 | 269,408,295 | Scale/Radius: 1.00 |
| 224 | `Roid_Med_Green` | 200 | Object | 5033.41,74.83,-2771.05 | 509,180,420 | Scale/Radius: 1.00 |
| 225 | `Roid_Med_Green` | 204 | Object | 3613.70,935.38,2100.92 | 227,92,225 | Scale/Radius: 1.00 |
| 226 | `Roid_Med_Green` | 206 | Object | 2221.24,280.61,3806.20 | 218,246,308 | Scale/Radius: 1.00 |
| 227 | `Roid_Med_Green` | 210 | Object | 5513.07,879.26,-2327.32 | 186,231,500 | Scale/Radius: 1.00 |
| 228 | `Roid_Med_Green` | 211 | Object | 1086.22,374.15,-534.93 | 131,24,220 | Scale/Radius: 1.00 |
| 229 | `Roid_Med_Green` | 213 | Object | 2396.36,-710.89,2959.37 | 464,217,464 | Scale/Radius: 1.00 |
| 230 | `Roid_Med_Green` | 220 | Object | 4498.79,523.81,-321.80 | 36,284,498 | Scale/Radius: 1.00 |
| 231 | `Roid_Med_Green` | 222 | Object | 4729.22,-636.06,-1481.32 | 295,51,77 | Scale/Radius: 1.00 |
| 232 | `Roid_Med_Green` | 226 | Object | 3401.40,804.43,862.61 | 304,433,35 | Scale/Radius: 1.00 |
| 233 | `Roid_Med_Green` | 229 | Object | -610.60,879.26,1169.94 | 194,361,66 | Scale/Radius: 1.00 |
| 234 | `Roid_Med_Green` | 230 | Object | 4028.37,149.66,-674.29 | 288,117,255 | Scale/Radius: 1.00 |
| 235 | `Roid_Med_Green` | 233 | Object | 2488.66,692.18,3441.67 | 6,9,120 | Scale/Radius: 1.00 |
| 236 | `Roid_Med_Green` | 237 | Object | 2663.56,112.25,874.64 | 261,0,88 | Scale/Radius: 1.00 |
| 237 | `Roid_Med_Green` | 239 | Object | 1289.62,-448.98,3192.44 | 251,159,472 | Scale/Radius: 1.00 |
| 238 | `Roid_Med_Green` | 241 | Object | 3518.35,318.03,-2489.69 | 127,340,419 | Scale/Radius: 1.00 |
| 239 | `Roid_Med_Green` | 244 | Object | 53.48,261.91,1288.12 | 16,371,328 | Scale/Radius: 1.00 |
| 240 | `Roid_Med_Green` | 248 | Object | 2810.87,-617.35,-1105.99 | 344,264,256 | Scale/Radius: 1.00 |
| 241 | `Roid_Med_Green` | 249 | Object | 1621.63,-392.86,3036.51 | 333,312,327 | Scale/Radius: 1.00 |
| 242 | `Roid_Med_Green` | 256 | Object | 1759.93,-692.18,2684.84 | 151,401,286 | Scale/Radius: 1.00 |
| 243 | `Roid_Med_Green` | 257 | Object | 5421.12,355.44,-229.33 | 230,177,263 | Scale/Radius: 1.00 |
| 244 | `Roid_Med_Green` | 261 | Object | 1944.01,673.47,-221.00 | 439,46,238 | Scale/Radius: 1.00 |
| 245 | `Roid_Med_Green` | 266 | Object | 6334.15,280.61,-658.14 | 391,484,419 | Scale/Radius: 1.00 |
| 246 | `Roid_Med_Green` | 270 | Object | 4858.40,-149.66,-1064.12 | 195,453,276 | Scale/Radius: 1.00 |
| 247 | `Roid_Med_Green` | 273 | Object | 4489.33,-299.32,-2133.23 | 404,278,1 | Scale/Radius: 1.00 |
| 248 | `Roid_Med_Green` | 280 | Object | 3309.22,-168.37,1240.41 | 54,337,399 | Scale/Radius: 1.00 |
| 249 | `Roid_Med_Green` | 283 | Object | 2432.34,280.61,-3986.53 | 110,261,318 | Scale/Radius: 1.00 |
| 250 | `Roid_Med_Green` | 284 | Object | 2220.61,636.06,-924.35 | 363,473,371 | Scale/Radius: 1.00 |
| 251 | `Roid_Med_Green` | 286 | Object | 855.69,-673.47,-235.51 | 148,74,125 | Scale/Radius: 1.00 |
| 252 | `Roid_Med_Green` | 289 | Object | 4032.74,448.98,-1379.13 | 491,148,143 | Scale/Radius: 1.00 |
| 253 | `Roid_Med_Green` | 290 | Object | 2613.61,-280.61,-1601.12 | 173,404,154 | Scale/Radius: 1.00 |
| 254 | `Roid_Med_Green` | 292 | Object | 4497.03,261.91,152.16 | 168,33,344 | Scale/Radius: 1.00 |
| 255 | `Roid_Med_Green` | 295 | Object | 5319.42,-542.52,-2093.01 | 1,272,500 | Scale/Radius: 1.00 |
| 256 | `Roid_Med_Green` | 296 | Object | 1602.82,-505.11,273.74 | 197,321,92 | Scale/Radius: 1.00 |
| 257 | `Roid_Med_Green` | 297 | Object | 2533.81,-243.20,-3843.04 | 243,455,192 | Scale/Radius: 1.00 |
| 258 | `Roid_Med_Green` | 300 | Object | 2267.24,-56.12,2972.22 | 14,426,263 | Scale/Radius: 1.00 |
| 259 | `Roid_Med_Green` | 306 | Object | 413.36,-74.83,2696.05 | 263,372,131 | Scale/Radius: 1.00 |
| 260 | `Roid_Med_Green` | 308 | Object | -112.58,224.49,936.04 | 473,109,195 | Scale/Radius: 1.00 |
| 261 | `Roid_Med_Green` | 315 | Object | 1280.44,-205.78,3531.25 | 409,463,413 | Scale/Radius: 1.00 |
| 262 | `Roid_Med_Green` | 319 | Object | 689.68,-748.30,-157.54 | 261,189,199 | Scale/Radius: 1.00 |
| 263 | `Roid_Med_Green` | 326 | Object | 5965.08,897.97,-1727.25 | 248,343,267 | Scale/Radius: 1.00 |
| 264 | `Roid_Med_Green` | 327 | Object | 4331.08,-654.77,660.17 | 30,118,421 | Scale/Radius: 1.00 |
| 265 | `Roid_Med_Green` | 329 | Object | 2275.57,-729.60,-3817.33 | 366,203,179 | Scale/Radius: 1.00 |
| 266 | `Roid_Med_Green` | 334 | Object | 4259.02,-841.84,-113.62 | 360,11,337 | Scale/Radius: 1.00 |
| 267 | `Roid_Med_Green` | 336 | Object | 2423.61,-729.60,-207.32 | 386,29,474 | Scale/Radius: 1.00 |
| 268 | `Roid_Med_Green2` | 47 | Object | 1861.01,-130.95,-182.02 | 488,209,304 | Scale/Radius: 1.00 |
| 269 | `Roid_Med_Green2` | 48 | Object | 3530.86,673.47,3430.05 | 388,283,461 | Scale/Radius: 1.00 |
| 270 | `Roid_Med_Green2` | 57 | Object | 3272.23,-710.89,445.42 | 448,489,133 | Scale/Radius: 1.00 |
| 271 | `Roid_Med_Green2` | 62 | Object | 2488.43,0.00,1721.47 | 371,366,93 | Scale/Radius: 1.00 |
| 272 | `Roid_Med_Green2` | 71 | Object | 2327.60,636.06,-2279.16 | 489,445,173 | Scale/Radius: 1.00 |
| 273 | `Roid_Med_Green2` | 80 | Object | 4821.34,-561.23,-2289.16 | 23,414,393 | Scale/Radius: 1.00 |
| 274 | `Roid_Med_Green2` | 83 | Object | -638.19,-448.98,1756.33 | 262,68,71 | Scale/Radius: 1.00 |
| 275 | `Roid_Med_Green2` | 85 | Object | 3897.54,-261.91,242.57 | 244,134,467 | Scale/Radius: 1.00 |
| 276 | `Roid_Med_Green2` | 88 | Object | 3152.40,318.03,979.56 | 97,68,48 | Scale/Radius: 1.00 |
| 277 | `Roid_Med_Green2` | 91 | Object | 5338.17,243.20,239.70 | 294,119,248 | Scale/Radius: 1.00 |
| 278 | `Roid_Med_Green2` | 107 | Object | 2654.78,-56.12,4223.80 | 439,72,241 | Scale/Radius: 1.00 |
| 279 | `Roid_Med_Green2` | 125 | Object | -791.77,-617.35,2810.66 | 346,411,176 | Scale/Radius: 1.00 |
| 280 | `Roid_Med_Green2` | 127 | Object | 865.09,-56.12,1145.87 | 147,197,329 | Scale/Radius: 1.00 |
| 281 | `Roid_Med_Green2` | 129 | Object | 1861.46,243.20,3258.37 | 294,72,378 | Scale/Radius: 1.00 |
| 282 | `Roid_Med_Green2` | 140 | Object | 2327.72,935.38,-1419.06 | 472,465,152 | Scale/Radius: 1.00 |
| 283 | `Roid_Med_Green2` | 144 | Object | 3124.63,37.42,275.80 | 499,58,311 | Scale/Radius: 1.00 |
| 284 | `Roid_Med_Green2` | 157 | Object | 3530.81,860.55,3000.00 | 87,302,21 | Scale/Radius: 1.00 |
| 285 | `Roid_Med_Green2` | 170 | Object | 2392.19,374.15,-2070.56 | 119,343,434 | Scale/Radius: 1.00 |
| 286 | `Roid_Med_Green2` | 171 | Object | 945.16,-710.89,2518.23 | 298,235,391 | Scale/Radius: 1.00 |
| 287 | `Roid_Med_Green2` | 173 | Object | 394.95,205.78,2943.62 | 322,212,65 | Scale/Radius: 1.00 |
| 288 | `Roid_Med_Green2` | 177 | Object | 1842.20,710.89,-2944.79 | 279,422,8 | Scale/Radius: 1.00 |
| 289 | `Roid_Med_Green2` | 181 | Object | 4904.57,-710.89,-607.95 | 140,291,138 | Scale/Radius: 1.00 |
| 290 | `Roid_Med_Green2` | 183 | Object | 3361.58,-523.81,-2320.49 | 295,441,57 | Scale/Radius: 1.00 |
| 291 | `Roid_Med_Green2` | 195 | Object | 1436.70,804.43,-508.39 | 286,508,342 | Scale/Radius: 1.00 |
| 292 | `Roid_Med_Green2` | 202 | Object | -287.88,18.71,492.72 | 178,278,226 | Scale/Radius: 1.00 |
| 293 | `Roid_Med_Green2` | 209 | Object | 2183.45,-37.42,-3009.48 | 297,253,438 | Scale/Radius: 1.00 |
| 294 | `Roid_Med_Green2` | 214 | Object | 2653.70,598.64,-3947.14 | 217,85,236 | Scale/Radius: 1.00 |
| 295 | `Roid_Med_Green2` | 215 | Object | 680.45,-261.91,-248.78 | 441,216,229 | Scale/Radius: 1.00 |
| 296 | `Roid_Med_Green2` | 219 | Object | 35.01,224.49,1105.66 | 140,256,10 | Scale/Radius: 1.00 |
| 297 | `Roid_Med_Green2` | 223 | Object | 926.69,411.57,2335.76 | 408,4,381 | Scale/Radius: 1.00 |
| 298 | `Roid_Med_Green2` | 224 | Object | 4764.51,448.98,217.68 | 40,207,378 | Scale/Radius: 1.00 |
| 299 | `Roid_Med_Green2` | 228 | Object | 4286.50,598.64,-1560.11 | 320,83,366 | Scale/Radius: 1.00 |
| 300 | `Roid_Med_Green2` | 235 | Object | 3103.22,-617.35,-3154.88 | 48,500,134 | Scale/Radius: 1.00 |
| 301 | `Roid_Med_Green2` | 242 | Object | 2626.50,205.78,-350.40 | 280,354,296 | Scale/Radius: 1.00 |
| 302 | `Roid_Med_Green2` | 246 | Object | 3475.28,804.43,1592.49 | 472,336,74 | Scale/Radius: 1.00 |
| 303 | `Roid_Med_Green2` | 250 | Object | 3685.36,561.23,-135.64 | 388,352,99 | Scale/Radius: 1.00 |
| 304 | `Roid_Med_Green2` | 252 | Object | 1544.65,187.08,2427.82 | 410,225,8 | Scale/Radius: 1.00 |
| 305 | `Roid_Med_Green2` | 258 | Object | 2220.67,-598.64,-494.30 | 269,228,189 | Scale/Radius: 1.00 |
| 306 | `Roid_Med_Green2` | 263 | Object | 2055.12,18.71,3024.06 | 343,179,197 | Scale/Radius: 1.00 |
| 307 | `Roid_Med_Green2` | 267 | Object | 3715.00,710.89,954.26 | 231,21,161 | Scale/Radius: 1.00 |
| 308 | `Roid_Med_Green2` | 269 | Object | 4183.49,935.38,490.56 | 415,65,115 | Scale/Radius: 1.00 |
| 309 | `Roid_Med_Green2` | 276 | Object | 3290.70,-411.57,627.89 | 175,503,20 | Scale/Radius: 1.00 |
| 310 | `Roid_Med_Green2` | 278 | Object | 2642.09,93.54,-2986.09 | 478,256,185 | Scale/Radius: 1.00 |
| 311 | `Roid_Med_Green2` | 281 | Object | 5088.77,-785.72,-2653.69 | 80,332,433 | Scale/Radius: 1.00 |
| 312 | `Roid_Med_Green2` | 291 | Object | 1667.24,-505.11,-807.81 | 456,42,199 | Scale/Radius: 1.00 |
| 313 | `Roid_Med_Green2` | 311 | Object | 5181.00,448.98,-2601.44 | 359,155,50 | Scale/Radius: 1.00 |
| 314 | `Roid_Med_Green2` | 316 | Object | 1981.24,579.94,2294.18 | 267,347,305 | Scale/Radius: 1.00 |
| 315 | `Roid_Med_Green2` | 323 | Object | 2964.92,-243.20,-2803.20 | 56,186,368 | Scale/Radius: 1.00 |
| 316 | `Roid_Med_Green2` | 328 | Object | 2450.98,18.71,-2513.91 | 447,190,407 | Scale/Radius: 1.00 |
| 317 | `Roid_Med_Green2` | 331 | Object | 1215.18,-692.18,-1837.93 | 494,55,261 | Scale/Radius: 1.00 |
| 318 | `Roid_Med_Green2` | 338 | Object | 1068.26,392.86,3153.05 | 173,290,20 | Scale/Radius: 1.00 |
| 319 | `Spcargo_Food` | 1487 | Interactive | 2779.25,-251.29,2821.63 | 71,65,273 | secondary groups: CONT_063, none |
| 320 | `Generic_Colony_Station` | 1498 | Interactive | -4150.86,0.00,-749.98 | 363,0,0 | None |
