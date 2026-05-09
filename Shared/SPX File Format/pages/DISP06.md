# Tachyon: The Fringe DISP06.SPX - The Final Plan Unveiled

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP06.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `DISPUT6.BDF` |
| Region | 6 |
| Sector ID | 5 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 7 |
| Entities | 160 |
| Events | 8 |
| Waypoints | 0 |
| Child Sectors | 1 |
| Scripts | 0 |
| Scenes | 1 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Mad_Pirate_Platform`, `1: Gen_Pirate_Mercenary_Station`, `2: Spcargo_Art`, `3: Spcargo_Contraband`, `4: Roid_Sm_Brown`, `5: Roid_Sm_Brown2`, `6: Hyper_Gate` |
| Scripts | None |
| Scenes | `D6GC070A.SEN` |
| Labels | `obsidian`, `killer`, `BFGE_02`, `greyhound`, `quasar` |
| Aliases | `fake_2`, `fake_1`, `spy_1` |
| Groups | `CONT_030`, `CONT_061` |
| Child Sectors | [disp06A.spx](DISP06A.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 410; flags 6)
- Variable comparison: subject variable group 8, variable 27, op 1, value 1 (flags 4)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 700
- Set/add variable: variable group 8, variable 27, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 26
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 410; flags 6)
- Variable comparison: subject variable group 8, variable 27, op 1, value 2 (flags 4)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 1400
- Set/add variable: variable group 8, variable 27, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 26
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 410; flags 6)
- Variable comparison: subject variable group 8, variable 27, op 1, value 3 (flags 4)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 2100
- Set/add variable: variable group 8, variable 27, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 26
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 410; flags 6)
- Variable comparison: subject variable group 8, variable 27, op 1, value 4 (flags 4)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 2800
- Set/add variable: variable group 8, variable 27, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 26
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 410; flags 6)
- Variable comparison: subject variable group 8, variable 27, op 2, value 4 (flags 4)

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 3500
- Set/add variable: variable group 8, variable 27, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 26
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 32, op 2, value 10 (flags 4)

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 26
- Set/add variable: variable group 20, variable 32, subtype 0, value 0

### Event 6

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 411; flags 2)

**Action**

- Set/add variable: variable group 18, variable 800, subtype 0, value 1

### Event 7

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 412; flags 2)

**Action**

- Set/add variable: variable group 18, variable 801, subtype 0, value 1

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | 1239.07,0.00,-132.87 | 427,0,0 | Gate SPX: [disp03.spx](DISP03.md) |
| 1 | `Roid_Sm_Brown2` | 3 | Object | 2379.88,193.31,1275.33 | 384,473,282 | Scale/Radius: 8.00 |
| 2 | `Roid_Sm_Brown` | 6 | Object | 1388.95,268.14,474.96 | 62,363,219 | Scale/Radius: 8.00 |
| 3 | `Roid_Sm_Brown2` | 8 | Object | 2274.08,-106.01,1335.26 | 376,411,302 | Scale/Radius: 9.00 |
| 4 | `Roid_Sm_Brown2` | 15 | Object | 671.45,-193.31,-1569.68 | 318,210,13 | Scale/Radius: 7.00 |
| 5 | `Roid_Sm_Brown` | 21 | Object | 2143.36,-99.77,1749.74 | 451,155,440 | Scale/Radius: 7.00 |
| 6 | `Roid_Sm_Brown` | 22 | Object | 1874.92,249.43,2592.16 | 107,118,384 | Scale/Radius: 1.00 |
| 7 | `Roid_Sm_Brown` | 25 | Object | -1317.68,-118.48,-3163.08 | 490,26,370 | Scale/Radius: 9.00 |
| 8 | `Roid_Sm_Brown2` | 32 | Object | 1835.74,-187.08,2758.50 | 389,363,186 | Scale/Radius: 5.00 |
| 9 | `Roid_Sm_Brown` | 38 | Object | 1370.81,-274.38,-467.97 | 23,364,210 | Scale/Radius: 1.00 |
| 10 | `Roid_Sm_Brown` | 40 | Object | 1862.36,168.37,1500.41 | 42,112,47 | Scale/Radius: 3.00 |
| 11 | `Roid_Sm_Brown` | 41 | Object | 1311.89,-268.14,3094.87 | 298,139,363 | Scale/Radius: 7.00 |
| 12 | `Roid_Sm_Brown` | 43 | Object | 848.57,68.59,-1465.76 | 472,297,220 | Scale/Radius: 1.00 |
| 13 | `Roid_Sm_Brown` | 45 | Object | 1723.51,-261.91,1919.50 | 443,194,105 | Scale/Radius: 4.00 |
| 14 | `Roid_Sm_Brown` | 52 | Object | 2317.13,-74.83,1923.65 | 223,348,21 | Scale/Radius: 7.00 |
| 15 | `Roid_Sm_Brown` | 57 | Object | -1638.29,43.65,-3059.58 | 283,421,43 | Scale/Radius: 8.00 |
| 16 | `Roid_Sm_Brown` | 62 | Object | 1449.78,143.43,31.99 | 495,138,199 | Scale/Radius: 8.00 |
| 17 | `Roid_Sm_Brown` | 63 | Object | 1430.61,305.56,3095.70 | 12,395,491 | Scale/Radius: 7.00 |
| 18 | `Roid_Sm_Brown` | 66 | Object | 666.17,162.13,-1294.34 | 384,109,218 | Scale/Radius: 9.00 |
| 19 | `Roid_Sm_Brown2` | 67 | Object | 1739.01,31.18,3289.90 | 433,339,491 | Scale/Radius: 1.00 |
| 20 | `Roid_Sm_Brown2` | 70 | Object | -1878.95,-162.13,-2926.10 | 428,1,76 | Scale/Radius: 1.00 |
| 21 | `Roid_Sm_Brown` | 73 | Object | 1945.67,168.37,1248.96 | 89,433,206 | Scale/Radius: 6.00 |
| 22 | `Roid_Sm_Brown` | 78 | Object | 1384.67,56.12,68.87 | 24,433,209 | Scale/Radius: 7.00 |
| 23 | `Roid_Sm_Brown` | 80 | Object | -1573.68,-236.96,-2755.75 | 393,139,191 | Scale/Radius: 7.00 |
| 24 | `Roid_Sm_Brown2` | 81 | Object | -521.17,-236.96,-2539.28 | 457,498,441 | Scale/Radius: 5.00 |
| 25 | `Roid_Sm_Brown` | 85 | Object | -1430.54,-43.65,-2768.75 | 194,25,160 | Scale/Radius: 8.00 |
| 26 | `Roid_Sm_Brown2` | 88 | Object | -1047.24,-12.47,-2363.07 | 148,42,402 | Scale/Radius: 2.00 |
| 27 | `Roid_Sm_Brown` | 90 | Object | -1006.05,81.07,-2726.84 | 185,340,297 | Scale/Radius: 6.00 |
| 28 | `Roid_Sm_Brown` | 91 | Object | -787.82,-180.84,-2592.48 | 114,453,390 | Scale/Radius: 7.00 |
| 29 | `Roid_Sm_Brown` | 94 | Object | -732.28,205.78,-2760.12 | 149,51,456 | Scale/Radius: 4.00 |
| 30 | `Roid_Sm_Brown` | 96 | Object | 533.59,-93.54,-1832.01 | 25,229,176 | Scale/Radius: 5.00 |
| 31 | `Roid_Sm_Brown2` | 97 | Object | 1350.16,-199.55,3617.88 | 14,427,97 | Scale/Radius: 9.00 |
| 32 | `Roid_Sm_Brown` | 100 | Object | -830.85,-143.43,-2417.57 | 258,451,463 | Scale/Radius: 1.00 |
| 33 | `Roid_Sm_Brown` | 103 | Object | -1245.43,-243.20,-2523.15 | 367,380,413 | Scale/Radius: 3.00 |
| 34 | `Roid_Sm_Brown` | 104 | Object | -1830.11,193.31,-2953.77 | 116,294,266 | Scale/Radius: 8.00 |
| 35 | `Roid_Sm_Brown2` | 106 | Object | 1082.09,37.42,3866.21 | 321,38,129 | Scale/Radius: 9.00 |
| 36 | `Roid_Sm_Brown` | 109 | Object | 2395.66,143.43,1606.82 | 230,374,446 | Scale/Radius: 4.00 |
| 37 | `Roid_Sm_Brown2` | 115 | Object | 793.96,236.96,-822.05 | 36,477,114 | Scale/Radius: 7.00 |
| 38 | `Roid_Sm_Brown` | 118 | Object | 1691.17,168.37,2636.14 | 339,91,312 | Scale/Radius: 1.00 |
| 39 | `Roid_Sm_Brown2` | 123 | Object | 242.52,24.94,-1871.38 | 108,88,246 | Scale/Radius: 3.00 |
| 40 | `Roid_Sm_Brown2` | 126 | Object | -354.11,-162.13,-2225.40 | 339,327,277 | Scale/Radius: 7.00 |
| 41 | `Roid_Sm_Brown2` | 128 | Object | 911.76,-268.14,-1297.29 | 137,200,124 | Scale/Radius: 2.00 |
| 42 | `Roid_Sm_Brown` | 133 | Object | 198.97,174.60,-2119.06 | 303,201,349 | Scale/Radius: 8.00 |
| 43 | `Roid_Sm_Brown` | 134 | Object | 1426.76,112.25,3506.40 | 394,496,120 | Scale/Radius: 4.00 |
| 44 | `Roid_Sm_Brown` | 140 | Object | 2187.41,168.37,1656.70 | 101,467,230 | Scale/Radius: 1.00 |
| 45 | `Roid_Sm_Brown` | 144 | Object | 1857.64,-236.96,277.54 | 122,11,311 | Scale/Radius: 2.00 |
| 46 | `Roid_Sm_Brown` | 146 | Object | 1896.48,-155.90,2307.60 | 371,93,264 | Scale/Radius: 9.00 |
| 47 | `Roid_Sm_Brown2` | 147 | Object | 2351.61,168.37,1699.86 | 358,127,242 | Scale/Radius: 1.00 |
| 48 | `Roid_Sm_Brown2` | 153 | Object | 1981.58,-99.77,1160.53 | 138,124,320 | Scale/Radius: 8.00 |
| 49 | `Roid_Sm_Brown` | 155 | Object | 1812.14,299.32,3560.43 | 5,383,510 | Scale/Radius: 2.00 |
| 50 | `Roid_Sm_Brown` | 156 | Object | 1130.01,-143.43,-399.64 | 41,284,413 | Scale/Radius: 5.00 |
| 51 | `Roid_Sm_Brown` | 158 | Object | -1092.22,37.42,-2746.11 | 205,443,131 | Scale/Radius: 6.00 |
| 52 | `Roid_Sm_Brown` | 160 | Object | 1730.75,205.78,3606.54 | 71,386,26 | Scale/Radius: 2.00 |
| 53 | `Roid_Sm_Brown` | 163 | Object | 949.53,24.94,-433.57 | 152,79,433 | Scale/Radius: 6.00 |
| 54 | `Roid_Sm_Brown` | 164 | Object | 880.13,218.26,-802.78 | 133,136,276 | Scale/Radius: 1.00 |
| 55 | `Roid_Sm_Brown2` | 167 | Object | 1893.49,-236.96,1346.61 | 205,288,38 | Scale/Radius: 7.00 |
| 56 | `Roid_Sm_Brown` | 168 | Object | 243.46,-193.31,-1395.31 | 286,447,331 | Scale/Radius: 2.00 |
| 57 | `Roid_Sm_Brown2` | 169 | Object | 2264.51,249.43,1204.51 | 57,281,316 | Scale/Radius: 6.00 |
| 58 | `Roid_Sm_Brown2` | 172 | Object | 1776.84,174.60,2996.13 | 365,151,424 | Scale/Radius: 2.00 |
| 59 | `Roid_Sm_Brown` | 174 | Object | 1656.10,68.59,187.45 | 256,258,185 | Scale/Radius: 3.00 |
| 60 | `Roid_Sm_Brown` | 182 | Object | 1339.16,12.47,3351.77 | 420,72,155 | Scale/Radius: 9.00 |
| 61 | `Roid_Sm_Brown` | 183 | Object | -575.28,-93.54,-2236.28 | 151,472,152 | Scale/Radius: 7.00 |
| 62 | `Roid_Sm_Brown` | 184 | Object | 1370.81,268.14,-467.97 | 51,447,337 | Scale/Radius: 8.00 |
| 63 | `Roid_Sm_Brown2` | 185 | Object | 1207.11,155.90,-851.83 | 399,17,448 | Scale/Radius: 8.00 |
| 64 | `Roid_Sm_Brown` | 188 | Object | 546.01,193.31,-1430.53 | 123,481,369 | Scale/Radius: 3.00 |
| 65 | `Roid_Sm_Brown` | 191 | Object | -320.91,-43.65,-2505.41 | 77,91,368 | Scale/Radius: 9.00 |
| 66 | `Roid_Sm_Brown2` | 193 | Object | 1981.09,-31.18,1501.24 | 144,423,249 | Scale/Radius: 5.00 |
| 67 | `Roid_Sm_Brown2` | 196 | Object | 1437.76,112.25,3772.51 | 487,501,486 | Scale/Radius: 3.00 |
| 68 | `Roid_Sm_Brown` | 198 | Object | 572.36,-143.43,-1649.72 | 198,228,409 | Scale/Radius: 6.00 |
| 69 | `Roid_Sm_Brown` | 201 | Object | 1384.60,-187.08,1226.37 | 260,14,317 | Scale/Radius: 1.00 |
| 70 | `Roid_Sm_Brown` | 203 | Object | -1437.25,-236.96,-2628.78 | 499,445,465 | Scale/Radius: 8.00 |
| 71 | `Roid_Sm_Brown` | 206 | Object | 1641.84,24.94,3004.52 | 185,365,290 | Scale/Radius: 7.00 |
| 72 | `Roid_Sm_Brown` | 208 | Object | 1343.45,-212.02,3757.85 | 87,259,284 | Scale/Radius: 7.00 |
| 73 | `Roid_Sm_Brown` | 210 | Object | 1643.77,99.77,2799.17 | 452,161,37 | Scale/Radius: 3.00 |
| 74 | `Roid_Sm_Brown2` | 215 | Object | 1613.98,174.60,75.14 | 60,261,108 | Scale/Radius: 2.00 |
| 75 | `Roid_Sm_Brown` | 217 | Object | -1052.96,130.95,-2904.52 | 230,253,271 | Scale/Radius: 4.00 |
| 76 | `Roid_Sm_Brown2` | 219 | Object | 1095.53,174.60,-175.85 | 293,254,182 | Scale/Radius: 7.00 |
| 77 | `Roid_Sm_Brown` | 223 | Object | 478.98,-137.19,-1188.30 | 362,234,207 | Scale/Radius: 5.00 |
| 78 | `Roid_Sm_Brown` | 224 | Object | 1942.89,162.13,2826.00 | 247,371,92 | Scale/Radius: 6.00 |
| 79 | `Roid_Sm_Brown2` | 228 | Object | 1652.68,-124.72,1414.93 | 264,400,463 | Scale/Radius: 9.00 |
| 80 | `Roid_Sm_Brown` | 229 | Object | 235.81,-87.30,-1731.41 | 412,49,242 | Scale/Radius: 5.00 |
| 81 | `Roid_Sm_Brown2` | 232 | Object | 585.78,-62.36,-1929.66 | 141,4,122 | Scale/Radius: 4.00 |
| 82 | `Roid_Sm_Brown` | 233 | Object | 1274.99,-62.36,4301.62 | 448,458,416 | Scale/Radius: 5.00 |
| 83 | `Roid_Sm_Brown` | 237 | Object | -751.91,-112.25,-2680.91 | 36,71,221 | Scale/Radius: 4.00 |
| 84 | `Roid_Sm_Brown` | 240 | Object | 651.82,6.24,-1490.47 | 36,210,295 | Scale/Radius: 4.00 |
| 85 | `Roid_Sm_Brown` | 242 | Object | 1574.65,-162.13,1391.05 | 382,197,14 | Scale/Radius: 8.00 |
| 86 | `Roid_Sm_Brown` | 246 | Object | 1962.88,-106.01,1715.81 | 315,349,271 | Scale/Radius: 8.00 |
| 87 | `Roid_Sm_Brown2` | 249 | Object | 1192.67,-37.42,3871.65 | 231,206,453 | Scale/Radius: 3.00 |
| 88 | `Roid_Sm_Brown` | 250 | Object | 1386.59,-43.65,-136.48 | 437,201,507 | Scale/Radius: 5.00 |
| 89 | `Roid_Sm_Brown2` | 251 | Object | 1573.28,305.56,98.19 | 230,146,107 | Scale/Radius: 4.00 |
| 90 | `Roid_Sm_Brown` | 253 | Object | 2088.75,286.85,2393.45 | 354,429,471 | Scale/Radius: 7.00 |
| 91 | `Spcargo_Contraband` | 411 | Interactive | 65.40,85.85,1708.09 | 0,0,0 | secondary groups: CONT_030, none |
| 92 | `Spcargo_Art` | 412 | Interactive | -813.20,1300.02,2108.66 | 384,92,405 | secondary groups: CONT_061, none |
| 93 | `Roid_Sm_Brown2` | 31 | Object | 1323.38,-12.47,3020.27 | 184,254,405 | Scale/Radius: 1.00 |
| 94 | `Roid_Sm_Brown2` | 5 | Object | 1122.78,-143.43,3843.15 | 480,158,492 | Scale/Radius: 1.00 |
| 95 | `Roid_Sm_Brown2` | 12 | Object | 960.53,-274.38,-167.46 | 135,172,453 | Scale/Radius: 1.00 |
| 96 | `Roid_Sm_Brown2` | 14 | Object | 1760.57,-130.95,3005.35 | 63,219,237 | Scale/Radius: 1.00 |
| 97 | `Roid_Sm_Brown2` | 16 | Object | 2340.12,-236.96,1774.45 | 206,222,98 | Scale/Radius: 1.00 |
| 98 | `Roid_Sm_Brown2` | 19 | Object | -136.58,99.77,-2882.18 | 220,378,228 | Scale/Radius: 1.00 |
| 99 | `Roid_Sm_Brown2` | 27 | Object | 1464.13,311.79,228.11 | 194,15,339 | Scale/Radius: 1.00 |
| 100 | `Roid_Sm_Brown2` | 29 | Object | 1570.86,193.31,644.25 | 280,114,457 | Scale/Radius: 1.00 |
| 101 | `Roid_Sm_Brown2` | 36 | Object | 2289.86,180.84,1666.75 | 455,495,7 | Scale/Radius: 1.00 |
| 102 | `Roid_Sm_Brown2` | 47 | Object | 1844.22,43.65,557.48 | 174,125,280 | Scale/Radius: 1.00 |
| 103 | `Roid_Sm_Brown2` | 49 | Object | 861.00,106.01,-1064.28 | 370,247,57 | Scale/Radius: 1.00 |
| 104 | `Roid_Sm_Brown2` | 51 | Object | 884.92,74.83,-737.40 | 100,287,165 | Scale/Radius: 1.00 |
| 105 | `Roid_Sm_Brown2` | 56 | Object | -1666.06,-261.91,-2975.76 | 375,133,63 | Scale/Radius: 1.00 |
| 106 | `Roid_Sm_Brown2` | 59 | Object | 1951.45,-255.67,632.91 | 405,276,98 | Scale/Radius: 1.00 |
| 107 | `Roid_Sm_Brown2` | 60 | Object | 350.69,212.02,-1319.88 | 450,227,277 | Scale/Radius: 1.00 |
| 108 | `Roid_Sm_Brown2` | 61 | Object | 892.12,261.91,-1218.09 | 96,168,343 | Scale/Radius: 1.00 |
| 109 | `Roid_Sm_Brown2` | 65 | Object | 1084.01,130.95,3660.86 | 376,180,210 | Scale/Radius: 1.00 |
| 110 | `Roid_Sm_Brown2` | 69 | Object | -1377.42,-62.36,-2390.33 | 260,492,297 | Scale/Radius: 1.00 |
| 111 | `Roid_Sm_Brown2` | 74 | Object | 2005.00,68.59,1828.12 | 126,323,349 | Scale/Radius: 1.00 |
| 112 | `Roid_Sm_Brown2` | 77 | Object | -114.09,268.14,-2690.66 | 303,263,193 | Scale/Radius: 1.00 |
| 113 | `Roid_Sm_Brown2` | 79 | Object | 1591.49,-93.54,-116.38 | 489,344,168 | Scale/Radius: 1.00 |
| 114 | `Roid_Sm_Brown2` | 84 | Object | 1196.52,93.54,3460.95 | 181,204,449 | Scale/Radius: 1.00 |
| 115 | `Roid_Sm_Brown2` | 87 | Object | 1250.16,37.42,-263.45 | 415,452,358 | Scale/Radius: 1.00 |
| 116 | `Roid_Sm_Brown2` | 92 | Object | 560.37,-187.08,-1234.41 | 377,406,383 | Scale/Radius: 1.00 |
| 117 | `Roid_Sm_Brown2` | 93 | Object | 1138.64,-205.78,-744.96 | 461,23,162 | Scale/Radius: 1.00 |
| 118 | `Roid_Sm_Brown2` | 95 | Object | 1340.62,-162.13,161.91 | 112,465,72 | Scale/Radius: 1.00 |
| 119 | `Roid_Sm_Brown2` | 102 | Object | 2084.96,-212.02,1646.65 | 61,35,70 | Scale/Radius: 1.00 |
| 120 | `Roid_Sm_Brown2` | 108 | Object | 1061.03,118.48,3810.05 | 184,492,32 | Scale/Radius: 1.00 |
| 121 | `Roid_Sm_Brown2` | 114 | Object | 143.93,187.08,-2292.13 | 17,489,412 | Scale/Radius: 1.00 |
| 122 | `Roid_Sm_Brown2` | 117 | Object | 1427.72,-37.42,657.25 | 63,76,69 | Scale/Radius: 1.00 |
| 123 | `Roid_Sm_Brown2` | 120 | Object | -1645.00,-255.67,-2919.61 | 64,108,74 | Scale/Radius: 1.00 |
| 124 | `Roid_Sm_Brown2` | 125 | Object | 1757.71,81.07,2734.62 | 303,304,423 | Scale/Radius: 1.00 |
| 125 | `Roid_Sm_Brown2` | 129 | Object | 1571.83,218.26,3288.05 | 363,10,76 | Scale/Radius: 1.00 |
| 126 | `Roid_Sm_Brown2` | 132 | Object | 1238.15,236.96,3913.97 | 316,478,469 | Scale/Radius: 1.00 |
| 127 | `Roid_Sm_Brown2` | 137 | Object | -1246.36,-243.20,-2999.22 | 284,132,206 | Scale/Radius: 1.00 |
| 128 | `Roid_Sm_Brown2` | 139 | Object | 637.90,-93.54,-869.81 | 293,459,181 | Scale/Radius: 1.00 |
| 129 | `Roid_Sm_Brown2` | 145 | Object | 1847.51,-18.71,1644.99 | 502,235,255 | Scale/Radius: 1.00 |
| 130 | `Roid_Sm_Brown2` | 149 | Object | 1746.49,162.13,1770.31 | 251,388,89 | Scale/Radius: 1.00 |
| 131 | `Roid_Sm_Brown2` | 151 | Object | 1788.18,249.43,1065.83 | 242,510,76 | Scale/Radius: 1.00 |
| 132 | `Roid_Sm_Brown2` | 157 | Object | 714.01,243.20,-640.58 | 359,415,225 | Scale/Radius: 1.00 |
| 133 | `Roid_Sm_Brown2` | 166 | Object | 1163.06,-255.67,-758.80 | 68,159,359 | Scale/Radius: 1.00 |
| 134 | `Roid_Sm_Brown2` | 175 | Object | 566.14,81.07,-1850.45 | 271,48,55 | Scale/Radius: 1.00 |
| 135 | `Roid_Sm_Brown2` | 177 | Object | 1612.03,-249.43,3605.71 | 285,401,266 | Scale/Radius: 1.00 |
| 136 | `Roid_Sm_Brown2` | 178 | Object | 1118.51,-6.24,-325.05 | 73,509,305 | Scale/Radius: 1.00 |
| 137 | `Roid_Sm_Brown2` | 180 | Object | 1613.98,-143.43,75.14 | 307,500,446 | Scale/Radius: 1.00 |
| 138 | `Roid_Sm_Brown2` | 181 | Object | 624.98,-93.54,-930.58 | 486,433,210 | Scale/Radius: 1.00 |
| 139 | `Roid_Sm_Brown2` | 187 | Object | 1516.25,174.60,1287.96 | 139,466,34 | Scale/Radius: 1.00 |
| 140 | `Roid_Sm_Brown2` | 190 | Object | -747.13,162.13,-2615.53 | 421,478,392 | Scale/Radius: 1.00 |
| 141 | `Roid_Sm_Brown2` | 192 | Object | 1641.19,143.43,1489.53 | 5,95,28 | Scale/Radius: 1.00 |
| 142 | `Roid_Sm_Brown2` | 194 | Object | 2158.21,49.89,1605.16 | 22,142,502 | Scale/Radius: 1.00 |
| 143 | `Roid_Sm_Brown2` | 195 | Object | 1429.62,-193.31,3777.12 | 297,450,236 | Scale/Radius: 1.00 |
| 144 | `Roid_Sm_Brown2` | 200 | Object | 673.37,-143.43,-1775.03 | 92,154,177 | Scale/Radius: 1.00 |
| 145 | `Roid_Sm_Brown2` | 202 | Object | 2339.62,81.07,2115.17 | 369,277,284 | Scale/Radius: 1.00 |
| 146 | `Roid_Sm_Brown2` | 214 | Object | 921.32,-212.02,-1166.54 | 87,149,356 | Scale/Radius: 1.00 |
| 147 | `Roid_Sm_Brown2` | 216 | Object | 1914.11,37.42,585.98 | 88,369,342 | Scale/Radius: 1.00 |
| 148 | `Roid_Sm_Brown2` | 218 | Object | -200.26,37.42,-2709.93 | 262,185,372 | Scale/Radius: 1.00 |
| 149 | `Roid_Sm_Brown2` | 222 | Object | 2306.63,-249.43,1316.82 | 290,212,83 | Scale/Radius: 1.00 |
| 150 | `Roid_Sm_Brown2` | 227 | Object | 29.99,124.72,-2227.59 | 353,461,230 | Scale/Radius: 1.00 |
| 151 | `Roid_Sm_Brown2` | 231 | Object | 1098.86,-162.13,3516.27 | 366,156,138 | Scale/Radius: 1.00 |
| 152 | `Roid_Sm_Brown2` | 234 | Object | 411.01,-56.12,-1422.14 | 230,187,303 | Scale/Radius: 1.00 |
| 153 | `Roid_Sm_Brown2` | 236 | Object | 760.48,149.66,-1279.68 | 362,205,55 | Scale/Radius: 1.00 |
| 154 | `Roid_Sm_Brown2` | 239 | Object | 1959.53,56.12,1785.80 | 20,55,319 | Scale/Radius: 1.00 |
| 155 | `Roid_Sm_Brown2` | 245 | Object | 1163.97,137.19,3479.39 | 266,15,382 | Scale/Radius: 1.00 |
| 156 | `Roid_Sm_Brown2` | 252 | Object | 1809.40,-218.26,2977.68 | 107,145,155 | Scale/Radius: 1.00 |
| 157 | `Roid_Sm_Brown2` | 254 | Object | 1595.75,-74.83,3614.93 | 489,234,102 | Scale/Radius: 1.00 |
| 158 | `Gen_Pirate_Mercenary_Station` | 405 | Interactive | 197.69,798.25,1656.19 | 162,0,0 | None |
| 159 | `Mad_Pirate_Platform` | 410 | Interactive | 162.06,734.73,2469.64 | 418,0,0 | None |
