# Tachyon: The Fringe BORA01.SPX - Aftermath of Destruction

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `BORA01.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `BORA1.BDF` |
| Region | 3 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 6 |
| Entities | 260 |
| Events | 12 |
| Waypoints | 0 |
| Child Sectors | 6 |
| Scripts | 2 |
| Scenes | 3 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Base_Mine`, `1: Bora_StarBase`, `2: Roid_Sm_Brown`, `3: Navigational_Bouy`, `4: Roid_Sm_Brown2`, `5: Hyper_Gate` |
| Scripts | `PLAYER.SCR`, `ANNAH.SCR` |
| Scenes | `BORA2HUB.SEN`, `BOR2RIP.SEN`, `BOR2FRON.SEN` |
| Labels | `chaas` |
| Aliases | `frank01`, `frank04`, `frank03`, `frank02` |
| Groups | `FREEDOM_STARBASE` |
| Child Sectors | [bora01A.spx](BORA01A.md), [bora01B.spx](BORA01B.md), [bora01C.spx](BORA01C.md), [bora01D.spx](BORA01D.md), [bora01E.spx](BORA01E.md), [bora01F.spx](BORA01F.md) |

## Events

### Event 0

**Trigger**

- Variable comparison: subject variable group 0, variable 4, op 0, value 2001
- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Mission objective/state: param 196613, subtype 0, param 0
- Set runtime trigger variable: variable group 20, variable 18, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 0, variable 4, op 1, value 2001
- Variable comparison: subject variable group 20, variable 18, op 1, value 4

**Action**

- Play dialog: PLAYER.SCR, line/variant 0

### Event 2

**Trigger**

- Variable comparison: subject variable group 0, variable 4, op 0, value 2008
- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Area/player/sector/dock/time event: subject 0, op 9, value 0

**Action**

- Play dialog: ANNAH.SCR, line/variant 7
- Mission objective/state: param 196609, subtype 0, param 0
- Broadcast HUD contact action: contact/list 0, subtype 0, param 10
- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0
- Set/add variable: variable group 21, variable 20, subtype 0, value 1
- Set/add variable: variable group 21, variable 21, subtype 0, value 1

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 2005

**Action**

- Mission objective/state: param 196610, subtype 0, param 0

### Event 4

**Trigger**

- Variable comparison: subject variable group 0, variable 4, op 0, value 4017
- Area/player/sector/dock/time event: subject 0, op 9, value 0

**Action**

- Mission objective/state: param 196609, subtype 0, param 0
- Show/update HUD contact: contact/list 0, subtype 9, param 16
- Play dialog: PLAYER.SCR, line/variant 36

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 24, op 1, value 1

**Action**

- Set/add variable: variable group 15, variable 408, subtype 0, value 1
- Set/add variable: variable group 15, variable 409, subtype 0, value 3
- Hide/remove HUD contact: contact/list 0, subtype 9, param 16

### Event 6

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 24, op 1, value 2

**Action**

- Set/add variable: variable group 15, variable 408, subtype 0, value 1
- Set/add variable: variable group 15, variable 409, subtype 0, value 2
- Hide/remove HUD contact: contact/list 0, subtype 9, param 16
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 7

**Trigger**

- Variable comparison: subject variable group 0, variable 4, op 1, value 4030
- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Mission objective/state: param 196609, subtype 0, param 0

### Event 8

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4023

**Action**

- Mission objective/state: param 196615, subtype 0, param 0

### Event 9

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4004
- Area/player/sector/dock/time event: subject 0, op 9, value 0

**Action**

- Mission objective/state: param 196612, subtype 0, param 0
- Play dialog: ANNAH.SCR, line/variant 8

### Event 10

**Trigger**

- Variable comparison: subject variable group 15, variable 403, op 0, value 2

**Action**

- Set/add variable: variable group 22, variable 22, subtype 0, value 1

### Event 11

**Trigger**

- Variable comparison: subject variable group 15, variable 405, op 0, value 2

**Action**

- Set/add variable: variable group 22, variable 24, subtype 0, value 1

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1004 | Gate | -508.30,213.30,-2790.30 | 498,0,0 | Gate SPX: [bora02.spx](BORA02.md) |
| 1 | `Hyper_Gate` | 1005 | Gate | 1247.06,-76.68,-2580.48 | 0,0,0 | Gate SPX: [bora04.spx](BORA04.md) |
| 2 | `Hyper_Gate` | 1006 | Gate | 2221.63,251.95,-1899.29 | 0,0,0 | Gate SPX: [bora07.spx](BORA07.md) |
| 3 | `Hyper_Gate` | 1007 | Gate | -1712.42,-76.68,-2166.69 | 0,0,0 | Gate SPX: [bora05.spx](BORA05.md) |
| 4 | `Roid_Sm_Brown2` | 1106 | Object | 430.90,1087.64,4673.51 | 108,115,320 | Scale/Radius: 5.00 |
| 5 | `Roid_Sm_Brown2` | 1108 | Object | -4162.82,-342.97,-879.32 | 480,69,237 | Scale/Radius: 3.00 |
| 6 | `Roid_Sm_Brown2` | 1127 | Object | -3373.51,-670.36,-756.07 | 129,28,306 | Scale/Radius: 5.00 |
| 7 | `Roid_Sm_Brown2` | 1129 | Object | -3774.22,-623.59,-496.73 | 457,84,117 | Scale/Radius: 7.00 |
| 8 | `Roid_Sm_Brown2` | 1137 | Object | -4209.83,639.18,349.41 | 117,227,472 | Scale/Radius: 3.00 |
| 9 | `Roid_Sm_Brown2` | 1139 | Object | -3545.48,-623.59,-839.85 | 395,505,410 | Scale/Radius: 3.00 |
| 10 | `Roid_Sm_Brown2` | 1146 | Object | -3338.24,-109.13,-279.85 | 154,449,428 | Scale/Radius: 4.00 |
| 11 | `Roid_Sm_Brown2` | 1147 | Object | -2855.40,-311.79,643.93 | 258,434,335 | Scale/Radius: 1.00 |
| 12 | `Roid_Sm_Brown2` | 1149 | Object | -4096.67,592.41,-945.46 | 230,37,414 | Scale/Radius: 4.00 |
| 13 | `Roid_Sm_Brown2` | 1150 | Object | -3668.69,249.43,-1176.21 | 480,408,294 | Scale/Radius: 7.00 |
| 14 | `Roid_Sm_Brown2` | 1153 | Object | -3610.90,732.72,229.81 | 120,315,159 | Scale/Radius: 2.00 |
| 15 | `Roid_Sm_Brown2` | 1155 | Object | 15.11,1477.38,4836.41 | 232,267,26 | Scale/Radius: 5.00 |
| 16 | `Roid_Sm_Brown2` | 1162 | Object | 93.77,2334.81,4611.43 | 142,87,19 | Scale/Radius: 4.00 |
| 17 | `Roid_Sm_Brown2` | 1164 | Object | 2319.13,-2290.77,2944.57 | 406,150,211 | Scale/Radius: 3.00 |
| 18 | `Roid_Sm_Brown2` | 1171 | Object | -5143.64,623.59,119.90 | 196,336,224 | Scale/Radius: 6.00 |
| 19 | `Roid_Sm_Brown2` | 1175 | Object | -3386.74,296.20,24.40 | 347,114,71 | Scale/Radius: 3.00 |
| 20 | `Roid_Sm_Brown2` | 1178 | Object | -3267.69,-592.41,-606.15 | 145,354,315 | Scale/Radius: 6.00 |
| 21 | `Roid_Sm_Brown2` | 1183 | Object | -4223.98,46.77,-814.21 | 300,89,301 | Scale/Radius: 8.00 |
| 22 | `Roid_Sm_Brown2` | 1188 | Object | -4556.73,-763.89,705.83 | 424,109,67 | Scale/Radius: 4.00 |
| 23 | `Roid_Sm_Brown2` | 1197 | Object | -2788.12,-389.74,1050.30 | 116,359,339 | Scale/Radius: 4.00 |
| 24 | `Roid_Sm_Brown2` | 1203 | Object | -3897.68,296.20,-884.76 | 171,224,100 | Scale/Radius: 1.00 |
| 25 | `Roid_Sm_Brown2` | 1209 | Object | -4657.86,342.97,203.44 | 274,414,508 | Scale/Radius: 8.00 |
| 26 | `Roid_Sm_Brown2` | 1213 | Object | -5189.94,-109.13,294.07 | 400,238,181 | Scale/Radius: 4.00 |
| 27 | `Roid_Sm_Brown2` | 1219 | Object | 486.21,2054.20,4474.74 | 185,185,254 | Scale/Radius: 2.00 |
| 28 | `Roid_Sm_Brown2` | 1223 | Object | -2715.81,732.72,-312.95 | 318,281,113 | Scale/Radius: 3.00 |
| 29 | `Roid_Sm_Brown2` | 1224 | Object | -2654.78,530.05,315.42 | 104,458,490 | Scale/Radius: 8.00 |
| 30 | `Roid_Sm_Brown2` | 1229 | Object | 2079.03,-1729.55,2967.62 | 43,73,497 | Scale/Radius: 6.00 |
| 31 | `Roid_Sm_Brown2` | 1247 | Object | -5583.56,701.54,194.77 | 84,446,468 | Scale/Radius: 2.00 |
| 32 | `Roid_Sm_Brown2` | 1249 | Object | -3983.50,-218.26,474.53 | 402,379,141 | Scale/Radius: 8.00 |
| 33 | `Roid_Sm_Brown2` | 1255 | Object | 2398.50,-2618.16,3376.69 | 35,161,33 | Scale/Radius: 1.00 |
| 34 | `Roid_Sm_Brown2` | 1268 | Object | -4536.88,-93.54,813.86 | 124,469,314 | Scale/Radius: 2.00 |
| 35 | `Roid_Sm_Brown2` | 1270 | Object | -2545.45,608.00,668.35 | 119,86,381 | Scale/Radius: 2.00 |
| 36 | `Roid_Sm_Brown2` | 1280 | Object | -3811.53,-62.36,558.31 | 9,489,458 | Scale/Radius: 9.00 |
| 37 | `Roid_Sm_Brown2` | 1281 | Object | -3785.07,452.10,276.11 | 414,56,412 | Scale/Radius: 8.00 |
| 38 | `Roid_Sm_Brown2` | 1282 | Object | -2524.70,685.95,313.22 | 456,352,152 | Scale/Radius: 2.00 |
| 39 | `Roid_Sm_Brown2` | 1294 | Object | 1902.65,-2072.52,3144.00 | 450,327,310 | Scale/Radius: 4.00 |
| 40 | `Roid_Sm_Brown2` | 1297 | Object | -3878.41,-467.69,-1035.85 | 245,287,366 | Scale/Radius: 9.00 |
| 41 | `Roid_Sm_Brown2` | 1298 | Object | -3214.77,389.74,108.18 | 121,277,412 | Scale/Radius: 1.00 |
| 42 | `Roid_Sm_Brown2` | 1301 | Object | -3119.97,-202.67,-370.24 | 304,42,250 | Scale/Radius: 8.00 |
| 43 | `Roid_Sm_Brown2` | 1304 | Object | -3547.04,265.02,-451.14 | 106,391,417 | Scale/Radius: 2.00 |
| 44 | `Roid_Sm_Brown2` | 1306 | Object | 264.82,1118.82,4248.94 | 507,455,508 | Scale/Radius: 7.00 |
| 45 | `Roid_Sm_Brown2` | 1309 | Object | -5601.19,654.77,-43.34 | 271,505,367 | Scale/Radius: 7.00 |
| 46 | `Roid_Sm_Brown2` | 1311 | Object | -4510.82,-311.79,99.56 | 452,233,157 | Scale/Radius: 5.00 |
| 47 | `Roid_Sm_Brown2` | 1317 | Object | -3231.38,15.59,782.74 | 209,201,189 | Scale/Radius: 4.00 |
| 48 | `Roid_Sm_Brown2` | 1319 | Object | -112.40,1181.18,4674.58 | 162,484,182 | Scale/Radius: 4.00 |
| 49 | `Roid_Sm_Brown2` | 1323 | Object | -3446.02,-46.77,-1526.76 | 94,472,140 | Scale/Radius: 3.00 |
| 50 | `Roid_Sm_Brown2` | 1332 | Object | 442.11,2069.79,4518.84 | 52,92,363 | Scale/Radius: 6.00 |
| 51 | `Roid_Sm_Brown2` | 1334 | Object | -4680.92,358.56,-1000.58 | 289,234,385 | Scale/Radius: 8.00 |
| 52 | `Roid_Sm_Brown2` | 1336 | Object | -4189.99,-763.89,457.44 | 265,31,9 | Scale/Radius: 2.00 |
| 53 | `Roid_Sm_Brown2` | 1344 | Object | -837.96,2023.02,4615.28 | 226,309,118 | Scale/Radius: 3.00 |
| 54 | `Roid_Sm_Brown2` | 1348 | Object | 2259.60,-2041.34,2620.47 | 396,59,253 | Scale/Radius: 5.00 |
| 55 | `Roid_Sm_Brown2` | 1354 | Object | -4165.74,202.67,305.31 | 274,253,97 | Scale/Radius: 7.00 |
| 56 | `Roid_Sm_Brown2` | 1356 | Object | -4380.51,-296.20,-529.80 | 413,321,397 | Scale/Radius: 1.00 |
| 57 | `Roid_Sm_Brown2` | 1359 | Object | -3143.19,202.67,694.55 | 3,316,90 | Scale/Radius: 3.00 |
| 58 | `Roid_Sm_Brown2` | 1360 | Object | -3630.82,265.02,-623.11 | 2,508,510 | Scale/Radius: 3.00 |
| 59 | `Roid_Sm_Brown2` | 1365 | Object | 1818.87,-2477.85,2972.03 | 176,170,479 | Scale/Radius: 1.00 |
| 60 | `Roid_Sm_Brown2` | 1370 | Object | -2501.95,763.89,-143.19 | 494,479,351 | Scale/Radius: 9.00 |
| 61 | `Roid_Sm_Brown2` | 1376 | Object | -4679.91,31.18,225.49 | 291,171,474 | Scale/Radius: 2.00 |
| 62 | `Roid_Sm_Brown2` | 1380 | Object | -2916.11,608.00,1362.58 | 291,29,369 | Scale/Radius: 8.00 |
| 63 | `Roid_Sm_Brown2` | 1381 | Object | -2918.20,732.72,1052.51 | 388,277,442 | Scale/Radius: 2.00 |
| 64 | `Roid_Sm_Brown2` | 1386 | Object | -4100.52,-233.85,-426.18 | 68,471,298 | Scale/Radius: 6.00 |
| 65 | `Roid_Sm_Brown2` | 1390 | Object | 2195.66,-2244.00,2556.54 | 400,388,137 | Scale/Radius: 6.00 |
| 66 | `Roid_Sm_Brown2` | 1391 | Object | -2672.41,452.10,77.31 | 454,406,278 | Scale/Radius: 7.00 |
| 67 | `Roid_Sm_Brown2` | 1392 | Object | 19.52,2272.46,4576.25 | 308,403,291 | Scale/Radius: 1.00 |
| 68 | `Roid_Sm_Brown2` | 1395 | Object | 157.71,1290.31,4675.37 | 52,102,154 | Scale/Radius: 8.00 |
| 69 | `Roid_Sm_Brown2` | 1401 | Object | 562.86,1337.07,3955.96 | 406,479,233 | Scale/Radius: 4.00 |
| 70 | `Roid_Sm_Brown2` | 1412 | Object | 2510.94,-1729.55,3136.38 | 170,72,386 | Scale/Radius: 2.00 |
| 71 | `Roid_Sm_Brown2` | 1414 | Object | 2301.49,-2867.59,2706.46 | 380,503,195 | Scale/Radius: 5.00 |
| 72 | `Roid_Sm_Brown2` | 1419 | Object | -4973.14,-311.79,-376.40 | 63,190,366 | Scale/Radius: 2.00 |
| 73 | `Roid_Sm_Brown2` | 1420 | Object | -3387.92,-233.85,1067.14 | 52,392,147 | Scale/Radius: 4.00 |
| 74 | `Roid_Sm_Brown2` | 1421 | Object | -3771.84,124.72,774.37 | 386,321,48 | Scale/Radius: 1.00 |
| 75 | `Roid_Sm_Brown2` | 1426 | Object | -5495.37,-62.36,106.58 | 10,292,294 | Scale/Radius: 4.00 |
| 76 | `Roid_Sm_Brown2` | 1428 | Object | 24.29,2459.53,4282.14 | 458,113,359 | Scale/Radius: 4.00 |
| 77 | `Roid_Sm_Brown2` | 1429 | Object | -3534.20,-763.89,-1438.57 | 96,483,265 | Scale/Radius: 8.00 |
| 78 | `Roid_Sm_Brown2` | 1443 | Object | -3375.72,-233.85,-625.99 | 148,412,393 | Scale/Radius: 6.00 |
| 79 | `Roid_Sm_Brown2` | 1444 | Object | 1430.18,-2696.11,3261.24 | 7,435,77 | Scale/Radius: 4.00 |
| 80 | `Roid_Sm_Brown2` | 1447 | Object | 555.26,1087.64,4935.62 | 434,28,81 | Scale/Radius: 6.00 |
| 81 | `Roid_Sm_Brown2` | 1448 | Object | 2358.81,-2883.18,3160.63 | 294,445,365 | Scale/Radius: 4.00 |
| 82 | `Roid_Sm_Brown2` | 1450 | Object | 1928.89,-2244.00,2951.18 | 234,193,438 | Scale/Radius: 2.00 |
| 83 | `Roid_Sm_Brown2` | 1452 | Object | -884.26,1087.64,4789.45 | 230,313,190 | Scale/Radius: 1.00 |
| 84 | `Roid_Sm_Brown2` | 1453 | Object | -4641.24,-654.77,-784.51 | 204,420,131 | Scale/Radius: 4.00 |
| 85 | `Roid_Sm_Brown2` | 1462 | Object | -2892.88,-109.13,297.79 | 77,270,508 | Scale/Radius: 5.00 |
| 86 | `Roid_Sm_Brown2` | 1464 | Object | -3591.06,-233.85,337.84 | 477,91,218 | Scale/Radius: 3.00 |
| 87 | `Roid_Sm_Brown2` | 1467 | Object | 1717.99,-2477.85,3504.96 | 242,475,279 | Scale/Radius: 5.00 |
| 88 | `Roid_Sm_Brown2` | 1469 | Object | -3683.66,748.30,686.18 | 434,243,117 | Scale/Radius: 2.00 |
| 89 | `Roid_Sm_Brown2` | 1477 | Object | -2761.66,-311.79,768.10 | 46,262,123 | Scale/Radius: 7.00 |
| 90 | `Roid_Sm_Brown2` | 1479 | Object | 31.65,1025.28,5018.76 | 310,319,269 | Scale/Radius: 4.00 |
| 91 | `Roid_Sm_Brown2` | 1482 | Object | 505.14,2132.15,4136.50 | 277,92,139 | Scale/Radius: 7.00 |
| 92 | `Roid_Sm_Brown2` | 1486 | Object | 41.56,2319.22,4554.20 | 186,74,434 | Scale/Radius: 6.00 |
| 93 | `Roid_Sm_Brown2` | 1493 | Object | -3898.25,654.77,-1143.88 | 356,367,494 | Scale/Radius: 9.00 |
| 94 | `Roid_Sm_Brown2` | 1497 | Object | -4616.65,-670.36,-50.36 | 266,225,428 | Scale/Radius: 4.00 |
| 95 | `Roid_Sm_Brown2` | 1499 | Object | -4721.05,-374.15,-134.26 | 198,363,486 | Scale/Radius: 7.00 |
| 96 | `Roid_Sm_Brown2` | 1502 | Object | -184.41,1368.25,4979.07 | 81,74,381 | Scale/Radius: 1.00 |
| 97 | `Roid_Sm_Brown2` | 1516 | Object | -2695.52,-436.51,701.96 | 378,485,86 | Scale/Radius: 6.00 |
| 98 | `Roid_Sm_Brown2` | 1518 | Object | 312.04,1758.00,4521.04 | 378,110,76 | Scale/Radius: 7.00 |
| 99 | `Roid_Sm_Brown2` | 1521 | Object | 2180.23,-1589.24,3467.09 | 236,342,99 | Scale/Radius: 1.00 |
| 100 | `Roid_Sm_Brown2` | 1526 | Object | -375.24,1695.64,4972.52 | 439,297,148 | Scale/Radius: 4.00 |
| 101 | `Roid_Sm_Brown2` | 1529 | Object | -608.77,1898.30,4769.06 | 480,408,12 | Scale/Radius: 5.00 |
| 102 | `Roid_Sm_Brown2` | 1530 | Object | -221.89,2397.17,4632.93 | 299,31,361 | Scale/Radius: 1.00 |
| 103 | `Roid_Sm_Brown2` | 1531 | Object | -5186.99,155.90,-546.16 | 222,212,240 | Scale/Radius: 2.00 |
| 104 | `Roid_Sm_Brown2` | 1532 | Object | -181.82,1461.79,4247.65 | 438,203,488 | Scale/Radius: 4.00 |
| 105 | `Roid_Sm_Brown2` | 1537 | Object | 1887.00,-2618.16,2865.20 | 6,161,62 | Scale/Radius: 5.00 |
| 106 | `Roid_Sm_Brown2` | 1540 | Object | -4749.27,327.38,-804.36 | 199,434,154 | Scale/Radius: 4.00 |
| 107 | `Roid_Sm_Brown2` | 1547 | Object | -3451.38,-280.61,874.42 | 299,212,434 | Scale/Radius: 7.00 |
| 108 | `Roid_Sm_Brown2` | 1548 | Object | -3963.82,561.23,-818.62 | 440,350,184 | Scale/Radius: 7.00 |
| 109 | `Roid_Sm_Brown2` | 1552 | Object | -4018.95,311.79,-184.85 | 456,433,155 | Scale/Radius: 8.00 |
| 110 | `Roid_Sm_Brown2` | 1557 | Object | -5427.02,-701.54,-89.64 | 318,330,44 | Scale/Radius: 9.00 |
| 111 | `Roid_Sm_Brown2` | 1559 | Object | 180.72,2334.81,4658.15 | 240,366,406 | Scale/Radius: 2.00 |
| 112 | `Roid_Sm_Brown2` | 1561 | Object | -4807.78,-296.20,97.62 | 475,0,500 | Scale/Radius: 3.00 |
| 113 | `Roid_Sm_Brown2` | 1565 | Object | -366.25,2054.20,4526.54 | 123,423,368 | Scale/Radius: 7.00 |
| 114 | `Roid_Sm_Brown2` | 1567 | Object | -5085.58,15.59,-136.08 | 493,432,382 | Scale/Radius: 4.00 |
| 115 | `Roid_Sm_Brown2` | 1569 | Object | -4077.55,-685.95,217.12 | 200,355,201 | Scale/Radius: 1.00 |
| 116 | `Roid_Sm_Brown2` | 1570 | Object | 392.70,1103.23,4376.81 | 225,71,241 | Scale/Radius: 5.00 |
| 117 | `Roid_Sm_Brown2` | 1572 | Object | -3740.98,-452.10,232.02 | 408,382,214 | Scale/Radius: 8.00 |
| 118 | `Roid_Sm_Brown2` | 1579 | Object | -3406.58,-93.54,-83.63 | 19,48,193 | Scale/Radius: 9.00 |
| 119 | `Roid_Sm_Brown2` | 1582 | Object | -5077.50,-608.00,53.76 | 167,502,230 | Scale/Radius: 3.00 |
| 120 | `Roid_Sm_Brown2` | 1586 | Object | -510.71,1212.36,5049.62 | 354,412,199 | Scale/Radius: 3.00 |
| 121 | `Roid_Sm_Brown2` | 1591 | Object | -2783.83,685.95,1230.29 | 429,213,8 | Scale/Radius: 3.00 |
| 122 | `Roid_Sm_Brown2` | 1595 | Object | -350.99,2537.48,4820.40 | 345,1,0 | Scale/Radius: 6.00 |
| 123 | `Roid_Sm_Brown2` | 1598 | Object | -4574.53,-249.43,-591.54 | 498,376,472 | Scale/Radius: 2.00 |
| 124 | `Roid_Sm_Brown2` | 1608 | Object | -3845.34,358.56,-429.56 | 270,98,391 | Scale/Radius: 8.00 |
| 125 | `Roid_Sm_Brown2` | 1618 | Object | -3723.34,233.85,470.12 | 479,183,349 | Scale/Radius: 1.00 |
| 126 | `Roid_Sm_Brown2` | 1621 | Object | -2623.21,-530.05,-661.30 | 248,261,333 | Scale/Radius: 5.00 |
| 127 | `Roid_Sm_Brown2` | 1623 | Object | -5192.14,-358.56,424.15 | 17,121,362 | Scale/Radius: 2.00 |
| 128 | `Roid_Sm_Brown2` | 1630 | Object | -4464.86,670.36,-960.89 | 11,278,480 | Scale/Radius: 9.00 |
| 129 | `Roid_Sm_Brown2` | 1640 | Object | -4768.10,-608.00,313.68 | 443,13,76 | Scale/Radius: 1.00 |
| 130 | `none` | 2260 | Marker | -983.75,0.00,-1171.14 | 0,0,0 | None |
| 131 | `Navigational_Bouy` | 2265 | Interactive | -775.34,0.00,-1144.70 | 0,0,0 | secondary groups: none, FREEDOM_STARBASE |
| 132 | `Roid_Sm_Brown` | 1507 | Object | -5382.93,576.82,-133.73 | 413,356,454 | Scale/Radius: 10.00 |
| 133 | `Roid_Sm_Brown` | 1107 | Object | -3347.06,-187.08,240.46 | 295,481,511 | Scale/Radius: 10.00 |
| 134 | `Roid_Sm_Brown` | 1111 | Object | -3404.38,530.05,-213.71 | 269,420,502 | Scale/Radius: 10.00 |
| 135 | `Roid_Sm_Brown` | 1121 | Object | -3610.90,-202.67,229.81 | 1,508,395 | Scale/Radius: 10.00 |
| 136 | `Roid_Sm_Brown` | 1126 | Object | -3514.36,311.79,-1330.54 | 117,410,11 | Scale/Radius: 10.00 |
| 137 | `Roid_Sm_Brown` | 1132 | Object | 664.27,1664.46,4366.04 | 438,481,16 | Scale/Radius: 10.00 |
| 138 | `Roid_Sm_Brown` | 1135 | Object | 1840.70,-1916.62,3039.37 | 151,315,187 | Scale/Radius: 10.00 |
| 139 | `Roid_Sm_Brown` | 1138 | Object | 1840.92,-2758.46,2949.98 | 408,405,100 | Scale/Radius: 10.00 |
| 140 | `Roid_Sm_Brown` | 1140 | Object | -105.79,2069.79,4284.35 | 392,335,481 | Scale/Radius: 10.00 |
| 141 | `Roid_Sm_Brown` | 1142 | Object | -5038.99,-654.77,33.83 | 297,234,58 | Scale/Radius: 10.00 |
| 142 | `Roid_Sm_Brown` | 1151 | Object | -842.37,1555.33,4875.44 | 250,462,334 | Scale/Radius: 10.00 |
| 143 | `Roid_Sm_Brown` | 1152 | Object | -4077.46,-405.33,617.48 | 38,446,118 | Scale/Radius: 10.00 |
| 144 | `Roid_Sm_Brown` | 1154 | Object | 577.31,1960.66,4913.57 | 460,76,217 | Scale/Radius: 10.00 |
| 145 | `Roid_Sm_Brown` | 1157 | Object | -162.36,1680.05,4957.03 | 247,219,418 | Scale/Radius: 10.00 |
| 146 | `Roid_Sm_Brown` | 1159 | Object | -3622.39,623.59,-1350.39 | 419,499,208 | Scale/Radius: 10.00 |
| 147 | `Roid_Sm_Brown` | 1160 | Object | -2919.34,-202.67,579.99 | 496,438,206 | Scale/Radius: 10.00 |
| 148 | `Roid_Sm_Brown` | 1165 | Object | -2935.95,-498.87,1254.54 | 314,218,393 | Scale/Radius: 10.00 |
| 149 | `Roid_Sm_Brown` | 1180 | Object | -572.44,1867.12,4855.61 | 129,435,217 | Scale/Radius: 10.00 |
| 150 | `Roid_Sm_Brown` | 1181 | Object | -670.50,1477.38,4575.05 | 314,331,331 | Scale/Radius: 10.00 |
| 151 | `Roid_Sm_Brown` | 1184 | Object | -2756.19,467.69,1184.08 | 498,165,76 | Scale/Radius: 10.00 |
| 152 | `Roid_Sm_Brown` | 1200 | Object | 409.75,1539.74,4569.64 | 180,280,214 | Scale/Radius: 10.00 |
| 153 | `Roid_Sm_Brown` | 1204 | Object | -2720.92,140.31,381.56 | 491,476,291 | Scale/Radius: 10.00 |
| 154 | `Roid_Sm_Brown` | 1206 | Object | -3430.58,732.72,-1158.58 | 218,495,328 | Scale/Radius: 10.00 |
| 155 | `Roid_Sm_Brown` | 1216 | Object | 106.80,1492.97,4613.98 | 181,377,432 | Scale/Radius: 10.00 |
| 156 | `Roid_Sm_Brown` | 1218 | Object | -3772.01,561.23,-626.81 | 137,226,476 | Scale/Radius: 10.00 |
| 157 | `Roid_Sm_Brown` | 1220 | Object | 2484.48,-1370.98,3418.58 | 183,33,353 | Scale/Radius: 10.00 |
| 158 | `Roid_Sm_Brown` | 1230 | Object | -54.33,1929.48,4703.64 | 405,399,451 | Scale/Radius: 10.00 |
| 159 | `Roid_Sm_Brown` | 1246 | Object | -3369.10,670.36,262.51 | 147,280,510 | Scale/Radius: 10.00 |
| 160 | `Roid_Sm_Brown` | 1250 | Object | -206.07,2537.48,4399.78 | 200,470,87 | Scale/Radius: 10.00 |
| 161 | `Roid_Sm_Brown` | 1258 | Object | -3165.24,-576.82,716.60 | 182,244,460 | Scale/Radius: 10.00 |
| 162 | `Roid_Sm_Brown` | 1260 | Object | -26.42,1477.38,4716.47 | 253,68,420 | Scale/Radius: 10.00 |
| 163 | `Roid_Sm_Brown` | 1263 | Object | -4701.96,62.36,247.54 | 239,464,67 | Scale/Radius: 10.00 |
| 164 | `Roid_Sm_Brown` | 1264 | Object | -2559.27,-109.13,-597.36 | 436,349,164 | Scale/Radius: 10.00 |
| 165 | `Roid_Sm_Brown` | 1269 | Object | -3127.76,654.77,1062.73 | 56,121,490 | Scale/Radius: 10.00 |
| 166 | `Roid_Sm_Brown` | 1272 | Object | 135.66,2210.10,4697.42 | 353,38,268 | Scale/Radius: 10.00 |
| 167 | `Roid_Sm_Brown` | 1275 | Object | -3448.47,-717.13,-169.61 | 29,300,197 | Scale/Radius: 10.00 |
| 168 | `Roid_Sm_Brown` | 1276 | Object | -540.42,1492.97,4572.84 | 364,243,451 | Scale/Radius: 10.00 |
| 169 | `Roid_Sm_Brown` | 1277 | Object | -4206.34,763.89,-576.10 | 196,507,257 | Scale/Radius: 10.00 |
| 170 | `Roid_Sm_Brown` | 1279 | Object | -110.56,1399.43,4578.45 | 60,453,215 | Scale/Radius: 10.00 |
| 171 | `Roid_Sm_Brown` | 1285 | Object | 1548.23,-1370.98,3291.11 | 215,248,65 | Scale/Radius: 10.00 |
| 172 | `Roid_Sm_Brown` | 1302 | Object | 662.07,1570.92,4496.12 | 456,51,431 | Scale/Radius: 10.00 |
| 173 | `Roid_Sm_Brown` | 1308 | Object | -5214.63,779.48,-499.95 | 104,445,120 | Scale/Radius: 10.00 |
| 174 | `Roid_Sm_Brown` | 1313 | Object | -3926.34,265.02,-472.48 | 118,151,268 | Scale/Radius: 10.00 |
| 175 | `Roid_Sm_Brown` | 1315 | Object | -3615.39,171.49,-254.92 | 296,406,123 | Scale/Radius: 10.00 |
| 176 | `Roid_Sm_Brown` | 1320 | Object | -3919.56,140.31,538.47 | 505,238,169 | Scale/Radius: 10.00 |
| 177 | `Roid_Sm_Brown` | 1324 | Object | -3015.65,-62.36,-524.61 | 484,15,467 | Scale/Radius: 10.00 |
| 178 | `Roid_Sm_Brown` | 1325 | Object | -824.83,2100.97,4729.38 | 39,130,211 | Scale/Radius: 10.00 |
| 179 | `Roid_Sm_Brown` | 1327 | Object | 364.76,1352.66,4739.65 | 199,381,338 | Scale/Radius: 10.00 |
| 180 | `Roid_Sm_Brown` | 1331 | Object | 414.74,2100.97,4354.77 | 227,494,122 | Scale/Radius: 10.00 |
| 181 | `Roid_Sm_Brown` | 1343 | Object | -4181.17,748.30,-62.87 | 464,13,417 | Scale/Radius: 10.00 |
| 182 | `Roid_Sm_Brown` | 1346 | Object | -2841.47,-452.10,-570.90 | 491,173,72 | Scale/Radius: 10.00 |
| 183 | `Roid_Sm_Brown` | 1349 | Object | 2195.66,-2462.26,2556.54 | 382,84,46 | Scale/Radius: 10.00 |
| 184 | `Roid_Sm_Brown` | 1355 | Object | -2568.09,452.10,-77.05 | 30,255,89 | Scale/Radius: 10.00 |
| 185 | `Roid_Sm_Brown` | 1362 | Object | -3353.67,124.72,630.70 | 176,184,125 | Scale/Radius: 10.00 |
| 186 | `Roid_Sm_Brown` | 1363 | Object | -3688.53,280.61,-1284.24 | 465,90,461 | Scale/Radius: 10.00 |
| 187 | `Roid_Sm_Brown` | 1364 | Object | -4462.66,109.13,-1090.97 | 345,233,17 | Scale/Radius: 10.00 |
| 188 | `Roid_Sm_Brown` | 1366 | Object | -4011.31,732.72,551.34 | 217,130,39 | Scale/Radius: 10.00 |
| 189 | `Roid_Sm_Brown` | 1367 | Object | 1616.57,-1433.34,3094.89 | 499,292,212 | Scale/Radius: 10.00 |
| 190 | `Roid_Sm_Brown` | 1375 | Object | -209.52,1695.64,4664.76 | 155,130,205 | Scale/Radius: 10.00 |
| 191 | `Roid_Sm_Brown` | 1377 | Object | 162.12,1492.97,4415.21 | 245,404,447 | Scale/Radius: 10.00 |
| 192 | `Roid_Sm_Brown` | 1378 | Object | -2621.00,-405.33,-791.38 | 333,353,66 | Scale/Radius: 10.00 |
| 193 | `Roid_Sm_Brown` | 1379 | Object | -4889.36,-498.87,-204.43 | 425,278,380 | Scale/Radius: 10.00 |
| 194 | `Roid_Sm_Brown` | 1382 | Object | -3624.60,31.18,-1220.31 | 133,26,306 | Scale/Radius: 10.00 |
| 195 | `Roid_Sm_Brown` | 1383 | Object | -4957.70,-140.31,-8.21 | 285,53,212 | Scale/Radius: 10.00 |
| 196 | `Roid_Sm_Brown` | 1394 | Object | -4767.09,561.23,-539.66 | 182,74,481 | Scale/Radius: 10.00 |
| 197 | `Roid_Sm_Brown` | 1396 | Object | -134.81,1851.53,4730.58 | 400,120,347 | Scale/Radius: 10.00 |
| 198 | `Roid_Sm_Brown` | 1398 | Object | -4605.23,639.18,-268.66 | 151,274,488 | Scale/Radius: 10.00 |
| 199 | `Roid_Sm_Brown` | 1400 | Object | -3988.08,155.90,-666.50 | 243,36,64 | Scale/Radius: 10.00 |
| 200 | `Roid_Sm_Brown` | 1403 | Object | -4836.73,545.64,602.21 | 304,335,257 | Scale/Radius: 10.00 |
| 201 | `Roid_Sm_Brown` | 1405 | Object | -4797.04,-701.54,818.27 | 254,171,337 | Scale/Radius: 10.00 |
| 202 | `Roid_Sm_Brown` | 1406 | Object | -335.19,2428.35,4406.81 | 191,329,20 | Scale/Radius: 10.00 |
| 203 | `Roid_Sm_Brown` | 1408 | Object | -2828.95,-420.92,361.72 | 102,152,76 | Scale/Radius: 10.00 |
| 204 | `Roid_Sm_Brown` | 1410 | Object | -10.23,1773.59,4659.55 | 434,146,357 | Scale/Radius: 10.00 |
| 205 | `Roid_Sm_Brown` | 1413 | Object | -5010.90,109.13,648.50 | 406,453,311 | Scale/Radius: 10.00 |
| 206 | `Roid_Sm_Brown` | 1416 | Object | -4424.84,77.95,141.45 | 389,306,1 | Scale/Radius: 10.00 |
| 207 | `Roid_Sm_Brown` | 1431 | Object | -4338.62,15.59,-443.82 | 306,326,219 | Scale/Radius: 10.00 |
| 208 | `Roid_Sm_Brown` | 1440 | Object | -628.61,2459.53,4661.03 | 252,474,472 | Scale/Radius: 10.00 |
| 209 | `Roid_Sm_Brown` | 1446 | Object | -4644.91,514.46,794.02 | 209,106,150 | Scale/Radius: 10.00 |
| 210 | `Roid_Sm_Brown` | 1449 | Object | -3384.54,-436.51,-105.68 | 373,236,238 | Scale/Radius: 10.00 |
| 211 | `Roid_Sm_Brown` | 1454 | Object | -3368.07,498.87,1175.18 | 479,494,251 | Scale/Radius: 10.00 |
| 212 | `Roid_Sm_Brown` | 1458 | Object | -3610.90,-467.69,229.81 | 453,347,162 | Scale/Radius: 10.00 |
| 213 | `Roid_Sm_Brown` | 1463 | Object | -2948.00,-452.10,-286.46 | 428,282,89 | Scale/Radius: 10.00 |
| 214 | `Roid_Sm_Brown` | 1465 | Object | -4558.93,46.77,835.91 | 123,326,22 | Scale/Radius: 10.00 |
| 215 | `Roid_Sm_Brown` | 1468 | Object | 516.56,1134.41,4130.13 | 146,79,314 | Scale/Radius: 10.00 |
| 216 | `Roid_Sm_Brown` | 1470 | Object | -229.36,1461.79,4556.73 | 5,190,453 | Scale/Radius: 10.00 |
| 217 | `Roid_Sm_Brown` | 1473 | Object | -3647.60,265.02,942.77 | 60,342,198 | Scale/Radius: 10.00 |
| 218 | `Roid_Sm_Brown` | 1476 | Object | -4079.75,-311.79,347.20 | 319,277,225 | Scale/Radius: 10.00 |
| 219 | `Roid_Sm_Brown` | 1478 | Object | -3582.71,-420.92,-1134.32 | 270,58,275 | Scale/Radius: 10.00 |
| 220 | `Roid_Sm_Brown` | 1485 | Object | 2109.68,-2820.82,2514.65 | 465,57,56 | Scale/Radius: 10.00 |
| 221 | `Roid_Sm_Brown` | 1494 | Object | -3147.60,109.13,954.70 | 463,222,471 | Scale/Radius: 10.00 |
| 222 | `Roid_Sm_Brown` | 1498 | Object | -3148.63,249.43,42.04 | 453,396,229 | Scale/Radius: 10.00 |
| 223 | `Roid_Sm_Brown` | 1501 | Object | -4328.04,717.13,644.48 | 296,418,72 | Scale/Radius: 10.00 |
| 224 | `Roid_Sm_Brown` | 1504 | Object | -2455.65,-623.59,-317.36 | 467,12,78 | Scale/Radius: 10.00 |
| 225 | `Roid_Sm_Brown` | 1505 | Object | -3408.68,-109.13,-1254.54 | 248,31,165 | Scale/Radius: 10.00 |
| 226 | `Roid_Sm_Brown` | 1511 | Object | -3338.24,-592.41,-279.85 | 120,28,246 | Scale/Radius: 10.00 |
| 227 | `Roid_Sm_Brown` | 1513 | Object | -3435.24,-654.77,328.65 | 136,340,184 | Scale/Radius: 10.00 |
| 228 | `Roid_Sm_Brown` | 1522 | Object | -2833.36,-561.23,621.88 | 392,266,33 | Scale/Radius: 10.00 |
| 229 | `Roid_Sm_Brown` | 1523 | Object | 1914.21,-2477.85,3436.62 | 15,70,493 | Scale/Radius: 10.00 |
| 230 | `Roid_Sm_Brown` | 1528 | Object | -4440.61,265.02,-1113.02 | 91,79,397 | Scale/Radius: 10.00 |
| 231 | `Roid_Sm_Brown` | 1535 | Object | -4244.39,389.74,-1181.36 | 28,129,399 | Scale/Radius: 10.00 |
| 232 | `Roid_Sm_Brown` | 1542 | Object | -2718.71,-701.54,251.49 | 197,474,109 | Scale/Radius: 10.00 |
| 233 | `Roid_Sm_Brown` | 1549 | Object | -4771.32,140.31,-782.31 | 459,207,452 | Scale/Radius: 10.00 |
| 234 | `Roid_Sm_Brown` | 1551 | Object | -4951.83,-202.67,311.71 | 481,428,401 | Scale/Radius: 10.00 |
| 235 | `Roid_Sm_Brown` | 1571 | Object | 439.00,1867.12,4202.64 | 188,242,439 | Scale/Radius: 10.00 |
| 236 | `Roid_Sm_Brown` | 1575 | Object | -3951.16,-280.61,-579.48 | 376,149,194 | Scale/Radius: 10.00 |
| 237 | `Roid_Sm_Brown` | 1583 | Object | -5169.07,-280.61,36.03 | 154,424,297 | Scale/Radius: 10.00 |
| 238 | `Roid_Sm_Brown` | 1587 | Object | 2510.94,-2306.36,3136.38 | 346,114,414 | Scale/Radius: 10.00 |
| 239 | `Roid_Sm_Brown` | 1589 | Object | -5296.94,280.61,-91.84 | 344,423,281 | Scale/Radius: 10.00 |
| 240 | `Roid_Sm_Brown` | 1590 | Object | -3860.50,-109.13,-1368.02 | 165,271,168 | Scale/Radius: 10.00 |
| 241 | `Roid_Sm_Brown` | 1599 | Object | -4539.09,-327.38,-334.80 | 503,244,278 | Scale/Radius: 10.00 |
| 242 | `Roid_Sm_Brown` | 1602 | Object | 2019.28,-2680.52,2732.92 | 501,80,355 | Scale/Radius: 10.00 |
| 243 | `Roid_Sm_Brown` | 1604 | Object | -3299.73,483.28,978.96 | 140,409,79 | Scale/Radius: 10.00 |
| 244 | `Roid_Sm_Brown` | 1609 | Object | -968.04,2506.30,4617.49 | 11,466,354 | Scale/Radius: 10.00 |
| 245 | `Roid_Sm_Brown` | 1611 | Object | -3598.25,-187.08,-1015.64 | 236,418,14 | Scale/Radius: 10.00 |
| 246 | `Roid_Sm_Brown` | 1612 | Object | -292.06,1758.00,4357.89 | 431,394,180 | Scale/Radius: 10.00 |
| 247 | `Roid_Sm_Brown` | 1614 | Object | -2762.81,-62.36,295.58 | 175,34,144 | Scale/Radius: 10.00 |
| 248 | `Roid_Sm_Brown` | 1615 | Object | 2140.54,-2727.28,3251.02 | 137,498,501 | Scale/Radius: 10.00 |
| 249 | `Roid_Sm_Brown` | 1619 | Object | 2010.68,-2586.98,3163.84 | 176,134,318 | Scale/Radius: 10.00 |
| 250 | `Roid_Sm_Brown` | 1622 | Object | -4681.10,545.64,-497.77 | 399,130,385 | Scale/Radius: 10.00 |
| 251 | `Roid_Sm_Brown` | 1624 | Object | -2475.49,748.30,-425.39 | 55,133,441 | Scale/Radius: 10.00 |
| 252 | `Roid_Sm_Brown` | 1633 | Object | -3882.82,-93.54,-775.70 | 235,392,291 | Scale/Radius: 10.00 |
| 253 | `Roid_Sm_Brown` | 1635 | Object | -3446.27,-77.95,-299.69 | 365,104,203 | Scale/Radius: 10.00 |
| 254 | `Roid_Sm_Brown` | 1639 | Object | -4167.10,-623.59,99.92 | 148,431,266 | Scale/Radius: 10.00 |
| 255 | `Roid_Sm_Brown` | 1643 | Object | -4935.66,576.82,-30.26 | 70,289,306 | Scale/Radius: 10.00 |
| 256 | `Roid_Sm_Brown` | 1644 | Object | -3576.09,-748.30,-1524.56 | 236,140,71 | Scale/Radius: 10.00 |
| 257 | `Roid_Sm_Brown` | 1645 | Object | -3699.09,-389.74,318.00 | 83,306,366 | Scale/Radius: 10.00 |
| 258 | `Bora_StarBase` | 1008 | Interactive | 63.71,-340.34,-2.44 | 0,0,0 | None |
| 259 | `Bora_Base_Mine` | 2254 | Interactive | -3005.63,0.00,-1092.04 | 63,0,0 | None |
