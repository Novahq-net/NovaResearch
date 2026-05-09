# Tachyon: The Fringe FRON05.SPX - Risky Venture; Hunting the Hunter

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON05.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `FRONTI5.BDF` |
| Region | 4 |
| Sector ID | 4 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 8 |
| Entities | 215 |
| Events | 2 |
| Waypoints | 0 |
| Child Sectors | 3 |
| Scripts | 1 |
| Scenes | 2 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Frontier_Station_Pltform`, `1: Mad_Pirate_Platform`, `2: Bora_Frontier_Station`, `3: Spcargo_Mining`, `4: Roid_Sm_Brown2`, `5: Roid_Sm_Brown`, `6: Asteroid_2`, `7: Hyper_Gate` |
| Scripts | `PLAYER.SCR` |
| Scenes | `F5LAN01.SEN`, `F5GC040A.SEN` |
| Labels | `BFGF_05`, `Ripstar`, `BFGE_05`, `Cephius` |
| Aliases | `Kimodo 4`, `Python 2`, `Python 1`, `Python 4`, `Kimodo 3`, `Kimodo 1`, `Kimodo 2`, `Python 3`, `Jerome13`, `Cephius` |
| Groups | `CONT_027`, `BLANK` |
| Child Sectors | [fron05A.spx](FRON05A.md), [fron05B.spx](FRON05B.md), [fron05C.spx](FRON05C.md) |

## Events

### Event 0

**Trigger**

- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Object spawn/action: Spcargo_Mining (object 211, id 1001), subtype 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 1001; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 145
- Set/add variable: variable group 16, variable 808, subtype 0, value 1

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | -3485.14,789.72,-1917.93 | 71,496,0 | Gate SPX: [fron04.spx](FRON04.md) |
| 1 | `Asteroid_2` | 79 | Object | -4527.28,1251.09,2328.52 | 268,210,503 | Scale/Radius: 3.00 |
| 2 | `Asteroid_2` | 82 | Object | -4331.19,1338.39,410.02 | 113,228,425 | Scale/Radius: 3.00 |
| 3 | `Asteroid_2` | 83 | Object | -10.24,421.72,-1611.12 | 440,346,259 | Scale/Radius: 1.00 |
| 4 | `Asteroid_2` | 84 | Object | 1429.29,-36.62,-1636.23 | 315,90,503 | Scale/Radius: 6.00 |
| 5 | `Asteroid_2` | 87 | Object | -4112.93,1065.57,1624.46 | 24,465,24 | Scale/Radius: 4.00 |
| 6 | `Asteroid_2` | 89 | Object | -5173.03,159.81,1505.98 | 422,181,236 | Scale/Radius: 9.00 |
| 7 | `Asteroid_2` | 94 | Object | 662.55,792.75,-520.31 | 461,315,43 | Scale/Radius: 4.00 |
| 8 | `Asteroid_2` | 101 | Object | -4175.29,-58.44,321.16 | 318,71,478 | Scale/Radius: 6.00 |
| 9 | `Asteroid_2` | 108 | Object | -4487.09,563.58,587.74 | 510,231,32 | Scale/Radius: 1.00 |
| 10 | `Asteroid_2` | 113 | Object | -3997.23,454.46,2210.04 | 35,498,267 | Scale/Radius: 3.00 |
| 11 | `Asteroid_2` | 114 | Object | 129.25,1611.21,-1307.63 | 154,491,402 | Scale/Radius: 7.00 |
| 12 | `Asteroid_2` | 117 | Object | -4580.63,749.10,1565.22 | 447,43,245 | Scale/Radius: 8.00 |
| 13 | `Asteroid_2` | 119 | Object | -3826.27,159.81,225.26 | 120,317,238 | Scale/Radius: 1.00 |
| 14 | `Asteroid_2` | 124 | Object | -2455.00,-3.88,3267.95 | 15,422,102 | Scale/Radius: 8.00 |
| 15 | `Asteroid_2` | 131 | Object | -1650.70,487.19,-1431.20 | 491,303,171 | Scale/Radius: 5.00 |
| 16 | `Asteroid_2` | 135 | Object | 1099.07,650.89,-1201.58 | 484,376,319 | Scale/Radius: 7.00 |
| 17 | `Asteroid_2` | 143 | Object | 1504.40,727.28,-283.34 | 252,489,505 | Scale/Radius: 3.00 |
| 18 | `Asteroid_2` | 147 | Object | -10.24,727.28,-1463.02 | 248,275,454 | Scale/Radius: 3.00 |
| 19 | `Asteroid_2` | 150 | Object | -4175.29,585.41,765.47 | 509,508,362 | Scale/Radius: 6.00 |
| 20 | `Asteroid_2` | 151 | Object | -4153.13,159.81,2121.18 | 234,260,420 | Scale/Radius: 8.00 |
| 21 | `Asteroid_2` | 153 | Object | -4549.45,192.55,-300.87 | 97,442,61 | Scale/Radius: 8.00 |
| 22 | `Asteroid_2` | 155 | Object | 2137.00,312.59,-1080.78 | 168,13,303 | Scale/Radius: 5.00 |
| 23 | `Asteroid_2` | 157 | Object | 381.94,607.23,-875.75 | 141,278,237 | Scale/Radius: 1.00 |
| 24 | `Asteroid_2` | 159 | Object | -4013.84,727.28,1222.29 | 474,402,26 | Scale/Radius: 2.00 |
| 25 | `Asteroid_2` | 160 | Object | -4371.39,934.62,2180.42 | 284,254,107 | Scale/Radius: 7.00 |
| 26 | `Asteroid_2` | 166 | Object | 2084.06,454.46,-1517.75 | 225,385,297 | Scale/Radius: 3.00 |
| 27 | `Asteroid_2` | 172 | Object | -3030.67,1185.61,3039.41 | 33,84,184 | Scale/Radius: 4.00 |
| 28 | `Asteroid_2` | 179 | Object | 176.84,629.06,-1522.26 | 492,380,162 | Scale/Radius: 2.00 |
| 29 | `Asteroid_2` | 183 | Object | 1473.22,869.14,-698.03 | 325,93,314 | Scale/Radius: 9.00 |
| 30 | `Asteroid_2` | 184 | Object | 1205.76,-58.26,-268.14 | 470,19,91 | Scale/Radius: 4.00 |
| 31 | `Asteroid_2` | 189 | Object | -3888.63,639.97,-367.14 | 325,268,231 | Scale/Radius: 8.00 |
| 32 | `Asteroid_2` | 191 | Object | -4870.26,1054.66,2121.18 | 92,156,386 | Scale/Radius: 8.00 |
| 33 | `Asteroid_2` | 202 | Object | 2034.45,28.86,-905.37 | 303,168,47 | Scale/Radius: 9.00 |
| 34 | `Asteroid_2` | 204 | Object | -4767.70,1185.61,-212.01 | 186,61,432 | Scale/Radius: 8.00 |
| 35 | `Asteroid_2` | 206 | Object | 2693.41,629.06,-562.06 | 29,32,161 | Scale/Radius: 5.00 |
| 36 | `Asteroid_2` | 209 | Object | 2034.45,225.29,-609.17 | 269,305,177 | Scale/Radius: 6.00 |
| 37 | `Asteroid_2` | 211 | Object | 1442.04,1196.52,-816.51 | 103,15,455 | Scale/Radius: 5.00 |
| 38 | `Asteroid_2` | 215 | Object | 1442.04,694.54,-757.27 | 99,486,2 | Scale/Radius: 9.00 |
| 39 | `Asteroid_2` | 216 | Object | -3514.48,399.89,-11.70 | 359,317,304 | Scale/Radius: 4.00 |
| 40 | `Asteroid_2` | 221 | Object | -4268.83,1109.22,972.81 | 456,227,413 | Scale/Radius: 6.00 |
| 41 | `Asteroid_2` | 222 | Object | -5119.69,880.05,2328.52 | 388,477,267 | Scale/Radius: 3.00 |
| 42 | `Asteroid_2` | 223 | Object | -681.42,705.45,-1189.15 | 305,390,348 | Scale/Radius: 2.00 |
| 43 | `Asteroid_2` | 225 | Object | -4237.65,814.58,1417.11 | 249,406,451 | Scale/Radius: 1.00 |
| 44 | `Asteroid_2` | 231 | Object | -3841.34,1371.13,2713.59 | 363,246,490 | Scale/Radius: 3.00 |
| 45 | `Asteroid_2` | 235 | Object | -5017.14,978.27,-448.97 | 379,131,86 | Scale/Radius: 1.00 |
| 46 | `Asteroid_2` | 239 | Object | 2542.33,1076.48,-932.67 | 223,240,312 | Scale/Radius: 7.00 |
| 47 | `Asteroid_2` | 241 | Object | -3841.34,509.02,3305.99 | 185,453,60 | Scale/Radius: 5.00 |
| 48 | `Asteroid_2` | 243 | Object | 1597.94,323.50,-312.97 | 142,87,473 | Scale/Radius: 5.00 |
| 49 | `Asteroid_2` | 249 | Object | -3654.26,770.93,2713.59 | 69,186,105 | Scale/Radius: 2.00 |
| 50 | `Asteroid_2` | 250 | Object | -4206.47,770.93,-715.55 | 353,511,496 | Scale/Radius: 5.00 |
| 51 | `Asteroid_2` | 252 | Object | -3608.01,519.93,106.78 | 230,446,360 | Scale/Radius: 1.00 |
| 52 | `Asteroid_2` | 254 | Object | 830.36,-222.14,-415.67 | 436,216,351 | Scale/Radius: 8.00 |
| 53 | `Asteroid_2` | 256 | Object | -1744.24,519.93,-1016.52 | 93,255,430 | Scale/Radius: 8.00 |
| 54 | `Asteroid_2` | 257 | Object | -4300.01,716.36,380.40 | 502,220,506 | Scale/Radius: 9.00 |
| 55 | `Asteroid_2` | 261 | Object | -3857.45,72.51,-159.80 | 326,366,471 | Scale/Radius: 6.00 |
| 56 | `Asteroid_2` | 263 | Object | -3841.34,148.90,2121.18 | 488,507,206 | Scale/Radius: 5.00 |
| 57 | `Asteroid_2` | 267 | Object | -415.57,236.20,-1759.22 | 37,146,362 | Scale/Radius: 8.00 |
| 58 | `Asteroid_2` | 268 | Object | 239.20,694.54,-1492.64 | 78,498,139 | Scale/Radius: 9.00 |
| 59 | `Asteroid_2` | 269 | Object | -3795.09,225.29,47.54 | 378,272,133 | Scale/Radius: 2.00 |
| 60 | `Asteroid_2` | 277 | Object | -5328.93,334.42,1831.80 | 263,14,414 | Scale/Radius: 9.00 |
| 61 | `Asteroid_2` | 285 | Object | -3810.16,781.84,2713.59 | 477,462,385 | Scale/Radius: 2.00 |
| 62 | `Asteroid_2` | 291 | Object | 1741.09,1305.65,-2495.22 | 483,471,482 | Scale/Radius: 9.00 |
| 63 | `Asteroid_2` | 307 | Object | 381.94,890.97,-934.99 | 56,421,47 | Scale/Radius: 4.00 |
| 64 | `Asteroid_2` | 308 | Object | -3716.62,923.71,2506.24 | 163,311,265 | Scale/Radius: 7.00 |
| 65 | `Asteroid_2` | 311 | Object | -3452.12,1032.83,-307.90 | 162,408,89 | Scale/Radius: 9.00 |
| 66 | `Asteroid_2` | 319 | Object | 1597.94,487.19,-846.13 | 291,453,425 | Scale/Radius: 6.00 |
| 67 | `Asteroid_2` | 327 | Object | 52.12,1174.70,-1492.64 | 307,362,300 | Scale/Radius: 3.00 |
| 68 | `Asteroid_2` | 328 | Object | 2693.41,421.72,-621.30 | 159,429,375 | Scale/Radius: 9.00 |
| 69 | `Asteroid_2` | 340 | Object | -4620.82,-113.01,2387.76 | 437,440,39 | Scale/Radius: 6.00 |
| 70 | `Asteroid_2` | 345 | Object | 372.93,1360.22,-1046.01 | 18,221,135 | Scale/Radius: 6.00 |
| 71 | `Asteroid_2` | 347 | Object | 622.36,727.28,-957.15 | 9,191,494 | Scale/Radius: 2.00 |
| 72 | `Asteroid_2` | 348 | Object | -2781.24,498.11,3928.02 | 100,443,438 | Scale/Radius: 8.00 |
| 73 | `Asteroid_2` | 353 | Object | 1473.22,1109.22,-698.03 | 447,483,53 | Scale/Radius: 6.00 |
| 74 | `Asteroid_2` | 355 | Object | -4901.44,1163.79,2358.14 | 215,157,188 | Scale/Radius: 5.00 |
| 75 | `Asteroid_2` | 357 | Object | -868.49,203.46,-1455.73 | 450,327,418 | Scale/Radius: 3.00 |
| 76 | `Asteroid_2` | 361 | Object | -4580.63,978.27,1742.94 | 354,270,153 | Scale/Radius: 6.00 |
| 77 | `Asteroid_2` | 369 | Object | -259.67,1491.17,-929.85 | 60,104,17 | Scale/Radius: 2.00 |
| 78 | `Asteroid_2` | 372 | Object | -743.78,1174.70,-1396.49 | 173,175,186 | Scale/Radius: 9.00 |
| 79 | `Asteroid_2` | 376 | Object | 1585.19,498.11,-1962.05 | 30,11,462 | Scale/Radius: 1.00 |
| 80 | `Asteroid_2` | 378 | Object | -2656.52,858.23,3157.89 | 315,238,350 | Scale/Radius: 7.00 |
| 81 | `Asteroid_2` | 381 | Object | -4340.21,378.07,2950.55 | 316,214,154 | Scale/Radius: 9.00 |
| 82 | `Asteroid_2` | 383 | Object | -1336.18,596.32,-1396.49 | 45,40,415 | Scale/Radius: 6.00 |
| 83 | `Asteroid_2` | 385 | Object | -4767.70,683.62,1861.42 | 279,48,133 | Scale/Radius: 3.00 |
| 84 | `Asteroid_2` | 752 | Object | -4763.35,192.55,162.74 | 97,442,61 | Scale/Radius: 8.00 |
| 85 | `Asteroid_2` | 753 | Object | -4556.93,1185.61,244.13 | 186,61,432 | Scale/Radius: 8.00 |
| 86 | `Asteroid_2` | 755 | Object | -5119.91,770.93,-264.57 | 353,511,496 | Scale/Radius: 5.00 |
| 87 | `Asteroid_2` | 760 | Object | -4369.27,192.55,101.69 | 97,442,61 | Scale/Radius: 8.00 |
| 88 | `Asteroid_2` | 761 | Object | -4162.84,1185.61,183.09 | 186,61,432 | Scale/Radius: 8.00 |
| 89 | `Asteroid_2` | 763 | Object | -4725.82,770.93,-325.61 | 353,511,496 | Scale/Radius: 5.00 |
| 90 | `Asteroid_2` | 768 | Object | -2248.69,192.55,-1831.37 | 97,442,61 | Scale/Radius: 8.00 |
| 91 | `Asteroid_2` | 769 | Object | -2042.27,1185.61,-1749.98 | 186,61,432 | Scale/Radius: 8.00 |
| 92 | `Asteroid_2` | 776 | Object | -1610.65,192.55,-1770.32 | 97,442,61 | Scale/Radius: 8.00 |
| 93 | `Asteroid_2` | 777 | Object | -1404.22,1185.61,-1688.93 | 186,61,432 | Scale/Radius: 8.00 |
| 94 | `Asteroid_2` | 779 | Object | -1967.20,770.93,-2197.63 | 353,511,496 | Scale/Radius: 5.00 |
| 95 | `Roid_Sm_Brown` | 229 | Object | -2531.80,-47.53,3572.58 | 71,25,263 | Scale/Radius: 10.00 |
| 96 | `Roid_Sm_Brown` | 107 | Object | -3452.12,487.19,-367.14 | 68,205,274 | Scale/Radius: 10.00 |
| 97 | `Roid_Sm_Brown` | 161 | Object | -5328.93,356.24,943.19 | 342,397,397 | Scale/Radius: 10.00 |
| 98 | `Roid_Sm_Brown` | 176 | Object | -4175.29,192.55,1476.36 | 488,144,387 | Scale/Radius: 10.00 |
| 99 | `Roid_Sm_Brown` | 195 | Object | -4112.93,7.03,498.88 | 460,199,187 | Scale/Radius: 10.00 |
| 100 | `Roid_Sm_Brown` | 205 | Object | -4045.02,563.58,1133.43 | 414,149,185 | Scale/Radius: 10.00 |
| 101 | `Roid_Sm_Brown` | 213 | Object | -3623.08,760.01,3365.24 | 341,169,212 | Scale/Radius: 10.00 |
| 102 | `Roid_Sm_Brown` | 244 | Object | -3591.90,-145.75,3542.96 | 211,412,123 | Scale/Radius: 10.00 |
| 103 | `Roid_Sm_Brown` | 248 | Object | -4112.93,716.36,528.50 | 127,175,306 | Scale/Radius: 10.00 |
| 104 | `Roid_Sm_Brown` | 279 | Object | -4121.95,1545.73,2150.80 | 323,239,367 | Scale/Radius: 10.00 |
| 105 | `Roid_Sm_Brown` | 293 | Object | -3538.04,825.49,2680.59 | 408,311,44 | Scale/Radius: 10.00 |
| 106 | `Roid_Sm_Brown` | 318 | Object | 2084.06,890.97,-1576.99 | 289,450,372 | Scale/Radius: 10.00 |
| 107 | `Roid_Sm_Brown` | 331 | Object | -4518.27,378.07,1239.39 | 142,509,166 | Scale/Radius: 10.00 |
| 108 | `Roid_Sm_Brown` | 332 | Object | -4028.41,1174.70,3217.13 | 416,464,326 | Scale/Radius: 10.00 |
| 109 | `Roid_Sm_Brown` | 335 | Object | 1972.09,476.28,-1201.58 | 202,264,496 | Scale/Radius: 10.00 |
| 110 | `Roid_Sm_Brown` | 344 | Object | -4558.46,519.93,3098.65 | 501,0,8 | Scale/Radius: 10.00 |
| 111 | `Roid_Sm_Brown` | 370 | Object | -3061.85,749.10,3335.62 | 377,87,48 | Scale/Radius: 10.00 |
| 112 | `Roid_Sm_Brown` | 374 | Object | -1713.06,639.97,-1371.96 | 325,24,361 | Scale/Radius: 10.00 |
| 113 | `Roid_Sm_Brown` | 380 | Object | -334.85,1163.79,-1337.11 | 66,98,300 | Scale/Radius: 10.00 |
| 114 | `Roid_Sm_Brown2` | 351 | Object | -2407.09,-145.75,3513.34 | 429,479,108 | Scale/Radius: 10.00 |
| 115 | `Roid_Sm_Brown2` | 73 | Object | 237.95,94.33,-474.91 | 5,100,186 | Scale/Radius: 10.00 |
| 116 | `Roid_Sm_Brown2` | 78 | Object | -2812.42,901.88,2861.69 | 318,181,53 | Scale/Radius: 10.00 |
| 117 | `Roid_Sm_Brown2` | 95 | Object | -3576.83,181.64,225.26 | 446,370,308 | Scale/Radius: 10.00 |
| 118 | `Roid_Sm_Brown2` | 104 | Object | -4705.34,770.93,498.88 | 344,270,369 | Scale/Radius: 10.00 |
| 119 | `Roid_Sm_Brown2` | 116 | Object | -3872.52,345.33,3069.03 | 461,47,387 | Scale/Radius: 10.00 |
| 120 | `Roid_Sm_Brown2` | 120 | Object | 1522.83,1283.83,-2228.64 | 170,295,502 | Scale/Radius: 10.00 |
| 121 | `Roid_Sm_Brown2` | 130 | Object | 209.63,1687.60,-1194.29 | 432,200,320 | Scale/Radius: 10.00 |
| 122 | `Roid_Sm_Brown2` | 144 | Object | -2968.31,1054.66,3157.89 | 332,130,7 | Scale/Radius: 10.00 |
| 123 | `Roid_Sm_Brown2` | 146 | Object | 1348.50,378.07,-875.75 | 459,502,436 | Scale/Radius: 10.00 |
| 124 | `Roid_Sm_Brown2` | 165 | Object | -4611.81,-222.14,469.26 | 213,330,240 | Scale/Radius: 10.00 |
| 125 | `Roid_Sm_Brown2` | 170 | Object | -4455.91,410.80,1950.28 | 122,89,296 | Scale/Radius: 10.00 |
| 126 | `Roid_Sm_Brown2` | 174 | Object | 209.63,923.71,-1105.43 | 264,19,106 | Scale/Radius: 10.00 |
| 127 | `Roid_Sm_Brown2` | 186 | Object | -4424.73,574.50,1772.56 | 412,469,38 | Scale/Radius: 10.00 |
| 128 | `Roid_Sm_Brown2` | 190 | Object | -4121.42,1065.57,1061.67 | 25,158,381 | Scale/Radius: 10.00 |
| 129 | `Roid_Sm_Brown2` | 193 | Object | 550.99,618.15,-722.51 | 49,475,93 | Scale/Radius: 10.00 |
| 130 | `Roid_Sm_Brown2` | 198 | Object | -4580.63,-254.87,380.40 | 117,448,317 | Scale/Radius: 10.00 |
| 131 | `Roid_Sm_Brown2` | 210 | Object | -2968.31,312.59,3750.30 | 184,143,469 | Scale/Radius: 10.00 |
| 132 | `Roid_Sm_Brown2` | 224 | Object | -4487.09,530.85,410.02 | 321,410,13 | Scale/Radius: 10.00 |
| 133 | `Roid_Sm_Brown2` | 238 | Object | -213.73,1305.65,-1337.25 | 384,458,40 | Scale/Radius: 10.00 |
| 134 | `Roid_Sm_Brown2` | 246 | Object | -4589.64,1163.79,3128.27 | 448,129,458 | Scale/Radius: 10.00 |
| 135 | `Roid_Sm_Brown2` | 260 | Object | -4549.45,1676.69,1091.29 | 276,396,463 | Scale/Radius: 10.00 |
| 136 | `Roid_Sm_Brown2` | 271 | Object | -3061.85,-69.36,3305.99 | 174,467,215 | Scale/Radius: 10.00 |
| 137 | `Roid_Sm_Brown2` | 282 | Object | -4076.20,509.02,1251.91 | 277,66,171 | Scale/Radius: 10.00 |
| 138 | `Roid_Sm_Brown2` | 298 | Object | -26.65,388.98,-1426.11 | 380,22,195 | Scale/Radius: 10.00 |
| 139 | `Roid_Sm_Brown2` | 310 | Object | -3826.27,869.14,-70.94 | 491,220,335 | Scale/Radius: 10.00 |
| 140 | `Roid_Sm_Brown2` | 314 | Object | -4830.06,-80.27,-271.25 | 267,269,180 | Scale/Radius: 10.00 |
| 141 | `Roid_Sm_Brown2` | 320 | Object | -197.31,1054.66,-1729.60 | 352,129,508 | Scale/Radius: 10.00 |
| 142 | `Roid_Sm_Brown2` | 336 | Object | -415.57,61.60,-1788.84 | 196,90,196 | Scale/Radius: 10.00 |
| 143 | `Roid_Sm_Brown2` | 342 | Object | 404.11,-14.79,-986.77 | 310,506,170 | Scale/Radius: 10.00 |
| 144 | `Roid_Sm_Brown2` | 346 | Object | -3336.63,-113.01,2861.58 | 424,148,400 | Scale/Radius: 10.00 |
| 145 | `Roid_Sm_Brown2` | 350 | Object | 1834.62,683.62,-1576.99 | 298,213,358 | Scale/Radius: 10.00 |
| 146 | `Roid_Sm_Brown2` | 362 | Object | 911.99,1185.61,-1260.82 | 149,463,346 | Scale/Radius: 10.00 |
| 147 | `Roid_Sm_Brown2` | 368 | Object | 2755.77,1687.60,-591.68 | 406,425,483 | Scale/Radius: 10.00 |
| 148 | `Roid_Sm_Brown2` | 371 | Object | -1257.41,618.15,-900.23 | 226,237,87 | Scale/Radius: 10.00 |
| 149 | `Roid_Sm_Brown2` | 375 | Object | 643.28,-14.79,-386.05 | 34,97,349 | Scale/Radius: 10.00 |
| 150 | `Roid_Sm_Brown2` | 757 | Object | -4481.86,-80.27,183.09 | 267,269,180 | Scale/Radius: 10.00 |
| 151 | `Roid_Sm_Brown2` | 765 | Object | -4087.77,-80.27,122.04 | 267,269,180 | Scale/Radius: 10.00 |
| 152 | `Roid_Sm_Brown2` | 773 | Object | -1967.20,-80.27,-1811.02 | 267,269,180 | Scale/Radius: 10.00 |
| 153 | `Roid_Sm_Brown2` | 781 | Object | -1329.16,-80.27,-1749.98 | 267,269,180 | Scale/Radius: 10.00 |
| 154 | `Roid_Sm_Brown` | 201 | Object | -2423.82,858.23,3179.09 | 306,298,139 | Scale/Radius: 10.00 |
| 155 | `Roid_Sm_Brown` | 75 | Object | -4175.29,1087.40,1624.46 | 242,466,460 | Scale/Radius: 10.00 |
| 156 | `Roid_Sm_Brown` | 93 | Object | -1257.41,1141.96,-1314.91 | 125,498,347 | Scale/Radius: 10.00 |
| 157 | `Roid_Sm_Brown` | 96 | Object | -712.60,716.36,-1337.25 | 137,457,250 | Scale/Radius: 10.00 |
| 158 | `Roid_Sm_Brown` | 100 | Object | -4237.65,509.02,-182.39 | 282,477,183 | Scale/Radius: 10.00 |
| 159 | `Roid_Sm_Brown` | 118 | Object | -3217.75,1578.47,3691.06 | 469,404,486 | Scale/Radius: 10.00 |
| 160 | `Roid_Sm_Brown` | 121 | Object | 1304.58,148.90,-2199.02 | 391,60,288 | Scale/Radius: 10.00 |
| 161 | `Roid_Sm_Brown` | 123 | Object | 1709.91,312.59,-2702.56 | 331,492,213 | Scale/Radius: 10.00 |
| 162 | `Roid_Sm_Brown` | 125 | Object | 1117.50,705.45,-1517.75 | 137,510,324 | Scale/Radius: 10.00 |
| 163 | `Roid_Sm_Brown` | 129 | Object | -4455.91,203.46,-508.21 | 140,46,349 | Scale/Radius: 10.00 |
| 164 | `Roid_Sm_Brown` | 148 | Object | -4767.70,1622.12,1831.80 | 435,444,452 | Scale/Radius: 10.00 |
| 165 | `Roid_Sm_Brown` | 154 | Object | -1242.65,-200.31,-1248.39 | 37,457,192 | Scale/Radius: 10.00 |
| 166 | `Roid_Sm_Brown` | 156 | Object | 1211.04,1294.74,-1754.71 | 71,340,339 | Scale/Radius: 10.00 |
| 167 | `Roid_Sm_Brown` | 158 | Object | -1650.70,170.72,-1194.24 | 256,33,475 | Scale/Radius: 10.00 |
| 168 | `Roid_Sm_Brown` | 169 | Object | 769.25,923.71,-1226.05 | 6,36,140 | Scale/Radius: 10.00 |
| 169 | `Roid_Sm_Brown` | 178 | Object | -4611.81,847.32,1624.46 | 463,388,350 | Scale/Radius: 10.00 |
| 170 | `Roid_Sm_Brown` | 185 | Object | -3124.21,1414.78,3009.79 | 16,180,107 | Scale/Radius: 10.00 |
| 171 | `Roid_Sm_Brown` | 203 | Object | 1099.07,487.19,-549.93 | 187,13,280 | Scale/Radius: 10.00 |
| 172 | `Roid_Sm_Brown` | 217 | Object | 1585.19,541.76,-1695.47 | 149,273,46 | Scale/Radius: 10.00 |
| 173 | `Roid_Sm_Brown` | 219 | Object | -4611.80,432.63,-478.59 | 152,187,243 | Scale/Radius: 10.00 |
| 174 | `Roid_Sm_Brown` | 240 | Object | -1398.54,1589.39,-1307.63 | 139,223,121 | Scale/Radius: 10.00 |
| 175 | `Roid_Sm_Brown` | 251 | Object | -4549.45,1131.05,-1130.24 | 11,507,151 | Scale/Radius: 10.00 |
| 176 | `Roid_Sm_Brown` | 255 | Object | 1491.65,738.19,-1636.23 | 218,29,430 | Scale/Radius: 10.00 |
| 177 | `Roid_Sm_Brown` | 264 | Object | -4527.28,1087.40,2180.42 | 432,251,503 | Scale/Radius: 10.00 |
| 178 | `Roid_Sm_Brown` | 278 | Object | -415.57,880.05,-1137.19 | 346,310,242 | Scale/Radius: 10.00 |
| 179 | `Roid_Sm_Brown` | 286 | Object | -1009.23,1611.21,-1363.52 | 253,422,484 | Scale/Radius: 10.00 |
| 180 | `Roid_Sm_Brown` | 288 | Object | -4714.36,-134.83,2180.42 | 207,257,108 | Scale/Radius: 10.00 |
| 181 | `Roid_Sm_Brown` | 290 | Object | -3888.63,1032.83,-278.28 | 119,74,212 | Scale/Radius: 10.00 |
| 182 | `Roid_Sm_Brown` | 295 | Object | 1005.53,509.02,-283.34 | 318,102,198 | Scale/Radius: 10.00 |
| 183 | `Roid_Sm_Brown` | 302 | Object | -3966.05,83.42,2210.04 | 71,267,214 | Scale/Radius: 10.00 |
| 184 | `Roid_Sm_Brown` | 304 | Object | 2003.27,-254.87,-816.51 | 73,96,204 | Scale/Radius: 10.00 |
| 185 | `Roid_Sm_Brown` | 306 | Object | -665.00,1534.82,-2055.42 | 400,197,141 | Scale/Radius: 10.00 |
| 186 | `Roid_Sm_Brown` | 316 | Object | -3569.22,334.42,2680.59 | 135,269,6 | Scale/Radius: 10.00 |
| 187 | `Roid_Sm_Brown` | 322 | Object | -5734.26,749.10,291.54 | 227,112,153 | Scale/Radius: 10.00 |
| 188 | `Roid_Sm_Brown` | 329 | Object | -1086.75,672.71,-1278.01 | 98,298,472 | Scale/Radius: 10.00 |
| 189 | `Roid_Sm_Brown` | 334 | Object | -3030.67,1000.09,3572.58 | 394,346,48 | Scale/Radius: 10.00 |
| 190 | `Roid_Sm_Brown` | 359 | Object | -290.85,552.67,-1285.29 | 326,478,354 | Scale/Radius: 10.00 |
| 191 | `Roid_Sm_Brown` | 364 | Object | -5048.32,378.07,1269.01 | 325,461,64 | Scale/Radius: 10.00 |
| 192 | `Roid_Sm_Brown` | 379 | Object | -431.98,792.75,-1307.63 | 296,68,344 | Scale/Radius: 10.00 |
| 193 | `Roid_Sm_Brown` | 382 | Object | 1442.04,1687.60,-668.41 | 60,473,116 | Scale/Radius: 10.00 |
| 194 | `Roid_Sm_Brown` | 384 | Object | -5204.21,443.54,-93.53 | 465,144,148 | Scale/Radius: 10.00 |
| 195 | `Roid_Sm_Brown` | 387 | Object | 2221.52,-69.36,-816.51 | 133,382,28 | Scale/Radius: 10.00 |
| 196 | `Roid_Sm_Brown` | 750 | Object | -5082.38,509.02,264.48 | 282,477,183 | Scale/Radius: 10.00 |
| 197 | `Roid_Sm_Brown` | 751 | Object | -4857.19,203.46,-61.09 | 140,46,349 | Scale/Radius: 10.00 |
| 198 | `Roid_Sm_Brown` | 754 | Object | -4707.06,432.63,-20.39 | 152,187,243 | Scale/Radius: 10.00 |
| 199 | `Roid_Sm_Brown` | 756 | Object | -4763.35,1131.05,-671.53 | 11,507,151 | Scale/Radius: 10.00 |
| 200 | `Roid_Sm_Brown` | 758 | Object | -4688.29,509.02,203.43 | 282,477,183 | Scale/Radius: 10.00 |
| 201 | `Roid_Sm_Brown` | 759 | Object | -4463.10,203.46,-122.13 | 140,46,349 | Scale/Radius: 10.00 |
| 202 | `Roid_Sm_Brown` | 762 | Object | -4312.97,432.63,-81.44 | 152,187,243 | Scale/Radius: 10.00 |
| 203 | `Roid_Sm_Brown` | 764 | Object | -4369.27,1131.05,-732.57 | 11,507,151 | Scale/Radius: 10.00 |
| 204 | `Roid_Sm_Brown` | 767 | Object | -2342.52,203.46,-2055.20 | 140,46,349 | Scale/Radius: 10.00 |
| 205 | `Roid_Sm_Brown` | 770 | Object | -2192.40,432.63,-2014.50 | 152,187,243 | Scale/Radius: 10.00 |
| 206 | `Roid_Sm_Brown` | 772 | Object | -2248.69,1131.05,-2665.64 | 11,507,151 | Scale/Radius: 10.00 |
| 207 | `Roid_Sm_Brown` | 774 | Object | -1929.67,509.02,-1668.58 | 282,477,183 | Scale/Radius: 10.00 |
| 208 | `Roid_Sm_Brown` | 775 | Object | -1704.48,203.46,-1994.15 | 140,46,349 | Scale/Radius: 10.00 |
| 209 | `Roid_Sm_Brown` | 778 | Object | -1554.35,432.63,-1953.46 | 152,187,243 | Scale/Radius: 10.00 |
| 210 | `Roid_Sm_Brown` | 780 | Object | -1610.65,1131.05,-2604.59 | 11,507,151 | Scale/Radius: 10.00 |
| 211 | `Spcargo_Mining` | 1001 | Interactive | 1128.24,703.00,-1538.60 | 448,43,398 | secondary groups: CONT_027, none |
| 212 | `Bora_Frontier_Station` | 819 | Interactive | -477.26,0.00,1242.10 | 0,0,0 | None |
| 213 | `Mad_Pirate_Platform` | 820 | Interactive | -1224.04,-105.45,332.47 | 0,0,0 | None |
| 214 | `Bora_Frontier_Station_Pltform` | 891 | Interactive | -2354.04,845.97,1276.12 | 0,0,0 | secondary groups: none, BLANK |
