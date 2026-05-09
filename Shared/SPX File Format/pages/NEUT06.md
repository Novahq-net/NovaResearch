# Tachyon: The Fringe NEUT06.SPX - Withdraw from Independence; Taking away Independence; Hub Escort; The Blockade

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT06.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `NEUTRA6.BDF` |
| Region | 1 |
| Sector ID | 5 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 24 |
| Entities | 371 |
| Events | 4 |
| Waypoints | 0 |
| Child Sectors | 8 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Mad_Pirate_Platform`, `1: Generic_Colony_Station`, `2: Spcargo_Credits`, `3: Spcargo_Contraband`, `4: Spcargo_Parts`, `5: Roid_XL_Green`, `6: Ice_Roid_2`, `7: Roid_Lrg_Grey`, `8: Ice_Roid_1`, `9: Roid_Med_Green2`, `10: Roid_Med_Green`, `11: Roid_Sm_Brown2`, `12: Roid_Sm_Grey`, `13: Roid_Sm_Brown`, `14: Junk_03`, `15: Junk_04`, `16: Junk_05`, `17: Junk_06`, `18: Junk_07`, `19: Junk_08`, `20: Junk_09`, `21: Junk_10`, `22: Mega_Gate`, `23: Hyper_Gate` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `BFNE_02`, `bfbe_08`, `BFNE_01`, `bfne_09`, `bfbe_01`, `BLACK`, `repar` |
| Aliases | `Todd08`, `Todd09`, `Todd10`, `oside`, `oside_1`, `oside_2`, `bagel`, `bagel_1`, `bagel_2`, `kwB10_01`, `kwB10_02`, `Todd13`, `Todd12`, `Todd02`, `Todd03`, `Todd04`, `Todd05`, `Todd06`, `Todd07`, `will_01`, `kevin01`, `SHIP1_HYPER`, `SHIP2_HYPER`, `SHIP3_HYPER`, `ohshit` |
| Groups | `CONT_060`, `CONT_062`, `CONT_067`, `WRECKTOWN` |
| Child Sectors | [neut06A.spx](NEUT06A.md), [neut06B.spx](NEUT06B.md), [neut06C.spx](NEUT06C.md), [neut06D.spx](NEUT06D.md), [neut06E.spx](NEUT06E.md), [neut06F.spx](NEUT06F.md), [neut06G.spx](NEUT06G.md), [neut06H.spx](NEUT06H.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 6758; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 194
- Set/add variable: variable group 13, variable 803, subtype 0, value 1

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 6757; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 197
- Set/add variable: variable group 13, variable 808, subtype 0, value 1

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 6768; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 196
- Set/add variable: variable group 0, variable 2, subtype 1, value 250
- Show/update HUD contact: contact/list 0, subtype 9, param 36
- Set/add variable: variable group 13, variable 809, subtype 0, value 1
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 32, op 2, value 10

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 36
- Set/add variable: variable group 20, variable 32, subtype 0, value 0

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 4689 | Gate | 0.36,0.00,2239.73 | 64,256,0 | Gate SPX: [neut07.spx](NEUT07.md) |
| 1 | `Hyper_Gate` | 4690 | Gate | -12.59,-243.54,-1836.08 | 508,0,0 | Gate SPX: [neut05.spx](NEUT05.md) |
| 2 | `Mega_Gate` | 4691 | Gate | -2175.05,0.00,-30.77 | 128,0,0 | Gate SPX: [fron01.spx](FRON01.md) |
| 3 | `Junk_10` | 5651 | Object | 888.21,361.83,71.74 | 499,489,192 | Scale/Radius: 5.00 |
| 4 | `Junk_09` | 5652 | Object | 68.93,-76.99,-633.23 | 276,108,64 | Scale/Radius: 3.00 |
| 5 | `Junk_08` | 5653 | Object | 839.22,238.66,-107.90 | 444,68,101 | Scale/Radius: 2.00 |
| 6 | `Junk_07` | 5654 | Object | 229.52,254.05,-831.92 | 420,376,376 | Scale/Radius: 4.00 |
| 7 | `Junk_06` | 5655 | Object | -359.21,-536.68,-2126.76 | 51,372,70 | Scale/Radius: 3.00 |
| 8 | `Junk_05` | 5656 | Object | 1228.45,192.47,-649.56 | 460,133,218 | Scale/Radius: 3.00 |
| 9 | `Junk_04` | 5657 | Object | 534.37,-338.74,-984.35 | 436,181,39 | Scale/Radius: 1.00 |
| 10 | `Junk_03` | 5658 | Object | 194.14,-69.29,-263.05 | 172,316,187 | Scale/Radius: 7.00 |
| 11 | `Junk_10` | 5659 | Object | 605.14,146.27,164.28 | 271,106,84 | Scale/Radius: 7.00 |
| 12 | `Junk_09` | 5660 | Object | -34.50,169.37,-1063.28 | 474,440,392 | Scale/Radius: 1.00 |
| 13 | `Junk_08` | 5661 | Object | -116.96,-744.54,-2064.16 | 189,217,32 | Scale/Radius: 8.00 |
| 14 | `Junk_07` | 5662 | Object | 58.04,-123.18,-774.76 | 366,167,320 | Scale/Radius: 5.00 |
| 15 | `Junk_06` | 5663 | Object | 651.41,-46.19,-720.33 | 33,174,281 | Scale/Radius: 4.00 |
| 16 | `Junk_05` | 5664 | Object | 108.91,736.17,-1365.02 | 318,162,59 | Scale/Radius: 4.00 |
| 17 | `Junk_04` | 5665 | Object | 217.79,174.17,-1207.15 | 223,203,432 | Scale/Radius: 5.00 |
| 18 | `Junk_03` | 5666 | Object | -315.66,-590.57,-2017.88 | 408,89,160 | Scale/Radius: 1.00 |
| 19 | `Junk_10` | 5667 | Object | 353.88,343.54,-1495.67 | 247,467,377 | Scale/Radius: 4.00 |
| 20 | `Junk_09` | 5668 | Object | 403.72,377.23,-625.06 | 145,280,318 | Scale/Radius: 4.00 |
| 21 | `Junk_08` | 5669 | Object | 335.68,-269.45,-823.76 | 293,118,504 | Scale/Radius: 9.00 |
| 22 | `Junk_07` | 5670 | Object | 716.74,-331.04,128.90 | 270,72,313 | Scale/Radius: 8.00 |
| 23 | `Junk_06` | 5671 | Object | 594.25,-269.45,-1463.40 | 461,233,333 | Scale/Radius: 1.00 |
| 24 | `Junk_05` | 5672 | Object | -95.10,-613.67,-1433.12 | 176,206,186 | Scale/Radius: 6.00 |
| 25 | `Junk_04` | 5673 | Object | 1097.18,-1231.97,-1770.19 | 465,244,481 | Scale/Radius: 2.00 |
| 26 | `Junk_03` | 5674 | Object | 278.52,-130.88,-652.28 | 429,94,76 | Scale/Radius: 2.00 |
| 27 | `Junk_10` | 5675 | Object | 460.08,-259.53,-1307.48 | 467,237,30 | Scale/Radius: 8.00 |
| 28 | `Junk_09` | 5676 | Object | 624.94,60.79,-295.26 | 244,489,493 | Scale/Radius: 5.00 |
| 29 | `Junk_08` | 5677 | Object | 722.18,-100.08,-257.61 | 427,83,123 | Scale/Radius: 4.00 |
| 30 | `Junk_07` | 5678 | Object | 269.50,682.28,-1792.35 | 496,73,279 | Scale/Radius: 9.00 |
| 31 | `Junk_06` | 5679 | Object | 65.40,-690.65,-1408.19 | 302,46,192 | Scale/Radius: 5.00 |
| 32 | `Junk_05` | 5680 | Object | 1157.68,-184.77,-769.32 | 93,391,363 | Scale/Radius: 7.00 |
| 33 | `Junk_04` | 5681 | Object | -152.34,-521.28,-2295.51 | 258,90,494 | Scale/Radius: 9.00 |
| 34 | `Junk_03` | 5682 | Object | -317.57,246.36,-970.74 | 9,418,96 | Scale/Radius: 1.00 |
| 35 | `Junk_10` | 5683 | Object | 575.20,61.59,-453.58 | 320,316,488 | Scale/Radius: 1.00 |
| 36 | `Junk_09` | 5684 | Object | 700.41,161.67,-1186.59 | 133,480,19 | Scale/Radius: 5.00 |
| 37 | `Junk_08` | 5685 | Object | 490.02,-139.60,-1684.19 | 316,234,418 | Scale/Radius: 4.00 |
| 38 | `Junk_07` | 5686 | Object | 285.83,158.78,-1808.69 | 165,455,253 | Scale/Radius: 2.00 |
| 39 | `Junk_06` | 5687 | Object | 471.77,123.18,-1112.27 | 64,316,10 | Scale/Radius: 4.00 |
| 40 | `Junk_05` | 5688 | Object | 877.33,-331.04,158.84 | 2,216,116 | Scale/Radius: 6.00 |
| 41 | `Junk_04` | 5689 | Object | 1299.22,-192.47,-758.43 | 251,195,388 | Scale/Radius: 1.00 |
| 42 | `Junk_03` | 5690 | Object | 639.72,-236.44,-1258.48 | 24,74,261 | Scale/Radius: 1.00 |
| 43 | `Junk_10` | 5691 | Object | -282.19,-15.40,-853.70 | 167,479,194 | Scale/Radius: 8.00 |
| 44 | `Junk_09` | 5692 | Object | 405.59,274.26,-1052.01 | 257,103,113 | Scale/Radius: 2.00 |
| 45 | `Junk_08` | 5693 | Object | 225.99,-505.89,-1606.88 | 427,111,367 | Scale/Radius: 1.00 |
| 46 | `Junk_07` | 5694 | Object | 1154.96,-354.14,-118.79 | 156,241,329 | Scale/Radius: 1.00 |
| 47 | `Junk_06` | 5695 | Object | -127.85,-182.55,-1519.78 | 73,472,170 | Scale/Radius: 9.00 |
| 48 | `Junk_05` | 5696 | Object | 877.33,-323.34,-412.75 | 157,490,469 | Scale/Radius: 5.00 |
| 49 | `Junk_04` | 5697 | Object | 717.48,476.52,-349.70 | 23,367,252 | Scale/Radius: 1.00 |
| 50 | `Junk_03` | 5698 | Object | 771.17,277.15,-420.92 | 503,16,252 | Scale/Radius: 6.00 |
| 51 | `Junk_10` | 5699 | Object | 234.12,204.97,-1680.76 | 112,495,86 | Scale/Radius: 8.00 |
| 52 | `Junk_09` | 5700 | Object | -165.95,-636.76,-1329.25 | 319,302,78 | Scale/Radius: 3.00 |
| 53 | `Junk_08` | 5701 | Object | 206.90,582.20,-1577.33 | 326,218,463 | Scale/Radius: 6.00 |
| 54 | `Junk_07` | 5702 | Object | 937.21,0.00,-91.57 | 273,22,304 | Scale/Radius: 2.00 |
| 55 | `Junk_06` | 5703 | Object | 364.77,143.38,-1582.77 | 37,358,24 | Scale/Radius: 2.00 |
| 56 | `Junk_05` | 5704 | Object | -32.58,-182.55,-1996.11 | 368,490,69 | Scale/Radius: 6.00 |
| 57 | `Junk_04` | 5705 | Object | -225.84,-398.11,-1536.11 | 90,503,404 | Scale/Radius: 3.00 |
| 58 | `Junk_03` | 5706 | Object | 394.75,-382.71,-1928.06 | 196,148,470 | Scale/Radius: 8.00 |
| 59 | `Junk_10` | 5707 | Object | -92.46,-767.64,-1631.38 | 170,429,295 | Scale/Radius: 2.00 |
| 60 | `Junk_09` | 5708 | Object | 1240.55,-268.15,860.84 | 71,36,301 | Scale/Radius: 7.00 |
| 61 | `Junk_08` | 5709 | Object | 558.06,-247.16,-1759.09 | 156,17,59 | Scale/Radius: 8.00 |
| 62 | `Junk_07` | 5710 | Object | -206.78,-482.79,-1288.42 | 361,67,359 | Scale/Radius: 2.00 |
| 63 | `Junk_06` | 5711 | Object | 10.97,-813.83,-1887.23 | 191,507,388 | Scale/Radius: 5.00 |
| 64 | `Junk_05` | 5712 | Object | 32.74,-259.53,-2290.07 | 85,504,340 | Scale/Radius: 1.00 |
| 65 | `Junk_04` | 5713 | Object | 915.43,115.48,-374.65 | 232,488,245 | Scale/Radius: 8.00 |
| 66 | `Junk_03` | 5714 | Object | 90.71,-23.10,-350.15 | 143,281,365 | Scale/Radius: 2.00 |
| 67 | `Junk_10` | 5715 | Object | 379.97,507.31,-164.61 | 374,178,324 | Scale/Radius: 2.00 |
| 68 | `Junk_09` | 5716 | Object | 1013.42,315.64,-358.32 | 404,477,267 | Scale/Radius: 1.00 |
| 69 | `Junk_08` | 5717 | Object | 302.21,-351.92,-1302.03 | 310,304,244 | Scale/Radius: 6.00 |
| 70 | `Junk_07` | 5718 | Object | 89.86,597.60,-1612.71 | 431,507,43 | Scale/Radius: 4.00 |
| 71 | `Junk_06` | 5719 | Object | 462.75,389.73,-994.85 | 94,18,71 | Scale/Radius: 4.00 |
| 72 | `Junk_05` | 5720 | Object | 92.62,-482.79,-1740.25 | 255,1,408 | Scale/Radius: 6.00 |
| 73 | `Junk_04` | 5721 | Object | -309.41,192.47,-750.27 | 402,52,269 | Scale/Radius: 2.00 |
| 74 | `Junk_10` | 5940 | Object | 24.06,-2144.36,1773.96 | 248,380,200 | Scale/Radius: 1.00 |
| 75 | `Junk_09` | 5941 | Object | -69.97,-2096.21,1591.12 | 211,256,93 | Scale/Radius: 4.00 |
| 76 | `Junk_08` | 5942 | Object | 126.71,-2096.24,1604.59 | 392,255,424 | Scale/Radius: 6.00 |
| 77 | `Junk_07` | 5943 | Object | 89.82,-2152.70,1787.44 | 440,351,58 | Scale/Radius: 1.00 |
| 78 | `Junk_06` | 5944 | Object | 125.10,-2133.45,1874.05 | 500,484,504 | Scale/Radius: 6.00 |
| 79 | `Junk_05` | 5945 | Object | -114.88,-2139.83,1856.72 | 198,133,137 | Scale/Radius: 7.00 |
| 80 | `Junk_04` | 5946 | Object | 266.24,-2091.11,1889.44 | 171,233,495 | Scale/Radius: 7.00 |
| 81 | `Junk_03` | 5947 | Object | -68.36,-2100.06,1431.38 | 319,169,468 | Scale/Radius: 2.00 |
| 82 | `Roid_Sm_Brown` | 5948 | Object | 80.19,-2234.82,1573.80 | 50,306,202 | Scale/Radius: 6.00 |
| 83 | `Roid_Sm_Grey` | 5949 | Object | -119.69,-2078.24,1527.61 | 337,288,229 | Scale/Radius: 2.00 |
| 84 | `Roid_Sm_Brown2` | 5950 | Object | -248.00,-2127.00,1646.94 | 251,279,192 | Scale/Radius: 9.00 |
| 85 | `Junk_10` | 5951 | Object | 192.47,-2097.53,1346.69 | 477,165,409 | Scale/Radius: 4.00 |
| 86 | `Junk_09` | 5952 | Object | 250.20,-2286.14,1779.74 | 91,257,418 | Scale/Radius: 1.00 |
| 87 | `Junk_08` | 5953 | Object | -73.17,-2223.88,1664.26 | 390,58,88 | Scale/Radius: 5.00 |
| 88 | `Junk_07` | 5954 | Object | -92.42,-1939.03,1415.98 | 205,346,16 | Scale/Radius: 4.00 |
| 89 | `Junk_06` | 5955 | Object | -392.35,-1985.86,1962.58 | 236,41,93 | Scale/Radius: 2.00 |
| 90 | `Junk_05` | 5956 | Object | 449.09,-2065.45,1169.62 | 209,227,307 | Scale/Radius: 6.00 |
| 91 | `Junk_04` | 5957 | Object | -347.44,-2214.25,1415.98 | 205,181,503 | Scale/Radius: 7.00 |
| 92 | `Junk_03` | 5958 | Object | 173.22,-2178.36,2131.95 | 183,34,410 | Scale/Radius: 5.00 |
| 93 | `Roid_Sm_Brown` | 5959 | Object | 80.19,-2218.78,2085.76 | 129,158,52 | Scale/Radius: 2.00 |
| 94 | `Roid_Sm_Grey` | 5960 | Object | -225.54,-2268.14,1797.06 | 317,28,44 | Scale/Radius: 2.00 |
| 95 | `Roid_Sm_Brown2` | 5961 | Object | 617.49,-2003.86,1902.92 | 346,321,455 | Scale/Radius: 3.00 |
| 96 | `Junk_10` | 5962 | Object | 567.77,-2055.18,1138.83 | 212,110,471 | Scale/Radius: 2.00 |
| 97 | `Junk_09` | 5963 | Object | 317.57,-2124.47,1381.33 | 1,258,73 | Scale/Radius: 2.00 |
| 98 | `Junk_08` | 5964 | Object | -635.14,-1982.05,1138.83 | 482,425,36 | Scale/Radius: 2.00 |
| 99 | `Junk_07` | 5965 | Object | 696.08,-2419.58,2426.42 | 379,471,373 | Scale/Radius: 1.00 |
| 100 | `Junk_06` | 5966 | Object | 606.27,-1849.25,1631.54 | 327,497,422 | Scale/Radius: 4.00 |
| 101 | `Junk_05` | 5967 | Object | -898.17,-2270.74,2339.81 | 91,19,71 | Scale/Radius: 1.00 |
| 102 | `Junk_04` | 5968 | Object | -450.09,-1980.73,1877.89 | 354,404,355 | Scale/Radius: 5.00 |
| 103 | `Junk_03` | 5969 | Object | 360.87,-2201.46,907.87 | 417,417,187 | Scale/Radius: 2.00 |
| 104 | `Roid_Sm_Brown` | 5970 | Object | -817.98,-2157.83,873.23 | 47,460,133 | Scale/Radius: 8.00 |
| 105 | `Roid_Sm_Grey` | 5971 | Object | 441.07,-2308.60,2692.02 | 213,322,398 | Scale/Radius: 7.00 |
| 106 | `Roid_Sm_Brown2` | 5972 | Object | -769.86,-1870.42,1046.45 | 151,331,267 | Scale/Radius: 4.00 |
| 107 | `Junk_10` | 5973 | Object | -646.36,-1823.58,663.44 | 441,47,265 | Scale/Radius: 4.00 |
| 108 | `Junk_08` | 5975 | Object | -264.64,-1833.85,1335.14 | 124,427,82 | Scale/Radius: 2.00 |
| 109 | `Junk_07` | 5976 | Object | 102.65,-2039.79,2878.71 | 186,427,322 | Scale/Radius: 7.00 |
| 110 | `Junk_06` | 5977 | Object | 708.91,-2099.45,2230.11 | 483,476,147 | Scale/Radius: 5.00 |
| 111 | `Junk_05` | 5978 | Object | -606.27,-2143.72,2328.26 | 67,91,406 | Scale/Radius: 5.00 |
| 112 | `Junk_04` | 5979 | Object | 213.32,-1949.33,715.41 | 26,406,388 | Scale/Radius: 9.00 |
| 113 | `Junk_03` | 5974 | Object | 179.63,-1763.92,1766.27 | 71,468,255 | Scale/Radius: 1.00 |
| 114 | `Junk_10` | 5982 | Object | -4934.15,425.35,269.45 | 412,146,51 | Scale/Radius: 8.00 |
| 115 | `Junk_09` | 5983 | Object | -3775.51,565.85,-53.89 | 59,374,443 | Scale/Radius: 2.00 |
| 116 | `Junk_08` | 5984 | Object | -2347.42,448.45,80.84 | 318,71,306 | Scale/Radius: 7.00 |
| 117 | `Junk_07` | 5985 | Object | -4691.65,585.10,835.30 | 413,15,399 | Scale/Radius: 8.00 |
| 118 | `Junk_06` | 5986 | Object | -3991.07,592.80,835.30 | 5,160,415 | Scale/Radius: 8.00 |
| 119 | `Junk_05` | 5987 | Object | -4233.58,486.94,-700.57 | 76,171,390 | Scale/Radius: 6.00 |
| 120 | `Junk_04` | 5988 | Object | -3748.57,531.21,296.40 | 144,360,354 | Scale/Radius: 6.00 |
| 121 | `Junk_03` | 5989 | Object | -2374.36,546.61,1185.59 | 372,371,55 | Scale/Radius: 3.00 |
| 122 | `Roid_Sm_Brown` | 5990 | Object | -3236.61,483.09,-970.02 | 255,182,490 | Scale/Radius: 4.00 |
| 123 | `Roid_Med_Green` | 5991 | Object | -2859.38,434.98,673.63 | 272,424,92 | Scale/Radius: 6.00 |
| 124 | `Roid_Med_Green2` | 5992 | Object | -3155.77,598.57,538.90 | 6,46,38 | Scale/Radius: 2.00 |
| 125 | `Roid_Sm_Brown2` | 5993 | Object | -2374.36,490.79,-1212.53 | 251,108,182 | Scale/Radius: 5.00 |
| 126 | `Ice_Roid_1` | 5994 | Object | -3748.57,448.45,-808.35 | 138,267,362 | Scale/Radius: 6.00 |
| 127 | `Junk_10` | 5995 | Object | -2940.21,594.72,-107.78 | 3,487,388 | Scale/Radius: 2.00 |
| 128 | `Junk_09` | 5996 | Object | -3991.07,567.78,-458.07 | 239,415,348 | Scale/Radius: 1.00 |
| 129 | `Junk_08` | 5997 | Object | -2967.16,560.08,-700.57 | 204,490,173 | Scale/Radius: 5.00 |
| 130 | `Junk_07` | 5998 | Object | -3425.22,440.75,269.45 | 333,486,416 | Scale/Radius: 4.00 |
| 131 | `Junk_06` | 5999 | Object | -2670.76,538.91,-242.51 | 204,496,126 | Scale/Radius: 8.00 |
| 132 | `Junk_05` | 6000 | Object | -3209.66,592.80,-592.79 | 498,131,456 | Scale/Radius: 5.00 |
| 133 | `Junk_04` | 6001 | Object | -4853.32,431.13,-619.74 | 221,348,455 | Scale/Radius: 5.00 |
| 134 | `Junk_03` | 6002 | Object | -3155.77,519.66,-80.84 | 453,235,39 | Scale/Radius: 1.00 |
| 135 | `Roid_Sm_Brown` | 6003 | Object | -3047.99,469.62,-1077.81 | 431,444,354 | Scale/Radius: 3.00 |
| 136 | `Roid_Med_Green` | 6004 | Object | -3398.28,587.03,1212.53 | 352,299,377 | Scale/Radius: 7.00 |
| 137 | `Roid_Med_Green2` | 6005 | Object | -4476.08,463.85,-1293.37 | 362,331,283 | Scale/Radius: 2.00 |
| 138 | `Roid_Sm_Brown2` | 6006 | Object | -2670.76,429.20,1077.81 | 458,417,332 | Scale/Radius: 2.00 |
| 139 | `Ice_Roid_1` | 6007 | Object | -3371.33,519.66,-1104.75 | 110,416,466 | Scale/Radius: 1.00 |
| 140 | `Junk_10` | 6008 | Object | -2832.43,560.08,323.34 | 172,49,233 | Scale/Radius: 5.00 |
| 141 | `Junk_09` | 6009 | Object | -4314.41,575.48,889.19 | 3,161,278 | Scale/Radius: 2.00 |
| 142 | `Junk_08` | 6010 | Object | -4260.52,413.81,-80.84 | 313,27,465 | Scale/Radius: 2.00 |
| 143 | `Junk_07` | 6011 | Object | -4503.03,475.40,808.35 | 9,140,211 | Scale/Radius: 1.00 |
| 144 | `Junk_06` | 6012 | Object | -2751.60,529.29,404.18 | 172,102,22 | Scale/Radius: 4.00 |
| 145 | `Junk_05` | 6013 | Object | -2374.36,429.20,-350.29 | 437,48,88 | Scale/Radius: 8.00 |
| 146 | `Junk_04` | 6014 | Object | -2428.25,461.92,619.74 | 173,192,264 | Scale/Radius: 6.00 |
| 147 | `Junk_03` | 6015 | Object | -4961.10,556.23,-646.68 | 499,375,305 | Scale/Radius: 6.00 |
| 148 | `Roid_Sm_Brown` | 6016 | Object | -3344.39,413.81,1104.75 | 198,229,12 | Scale/Radius: 6.00 |
| 149 | `Roid_Med_Green` | 6017 | Object | -4934.15,554.31,1104.75 | 273,407,321 | Scale/Radius: 3.00 |
| 150 | `Roid_Med_Green2` | 6018 | Object | -4314.41,442.68,-862.24 | 441,74,348 | Scale/Radius: 5.00 |
| 151 | `Roid_Sm_Brown2` | 6019 | Object | -3021.05,411.88,565.85 | 17,435,158 | Scale/Radius: 1.00 |
| 152 | `Ice_Roid_1` | 6020 | Object | -4206.63,556.23,-1131.70 | 472,251,133 | Scale/Radius: 3.00 |
| 153 | `Junk_10` | 6021 | Object | -2805.49,596.65,-592.79 | 486,179,255 | Scale/Radius: 3.00 |
| 154 | `Junk_09` | 6022 | Object | -4233.58,485.02,970.02 | 121,423,140 | Scale/Radius: 3.00 |
| 155 | `Junk_08` | 6023 | Object | -4395.25,558.16,1185.59 | 328,223,26 | Scale/Radius: 6.00 |
| 156 | `Junk_07` | 6024 | Object | -4799.43,483.09,-404.18 | 127,467,113 | Scale/Radius: 4.00 |
| 157 | `Junk_06` | 6025 | Object | -2347.42,488.87,-646.68 | 393,356,334 | Scale/Radius: 1.00 |
| 158 | `Junk_05` | 6026 | Object | -3910.24,494.64,-188.62 | 326,182,193 | Scale/Radius: 2.00 |
| 159 | `Junk_04` | 6027 | Object | -4718.59,550.46,646.68 | 350,308,23 | Scale/Radius: 4.00 |
| 160 | `Junk_03` | 6028 | Object | -2589.93,490.79,458.07 | 374,89,341 | Scale/Radius: 2.00 |
| 161 | `Roid_Sm_Brown` | 6029 | Object | -3452.17,508.11,242.51 | 93,480,24 | Scale/Radius: 8.00 |
| 162 | `Roid_Med_Green` | 6030 | Object | -2293.53,477.32,-1212.53 | 374,76,111 | Scale/Radius: 7.00 |
| 163 | `Roid_Med_Green2` | 6031 | Object | -3856.35,552.38,-1104.75 | 497,263,273 | Scale/Radius: 4.00 |
| 164 | `Roid_Sm_Brown2` | 6032 | Object | -3236.61,560.08,1131.70 | 105,34,434 | Scale/Radius: 5.00 |
| 165 | `Ice_Roid_1` | 6033 | Object | -4206.63,529.29,1158.64 | 388,447,480 | Scale/Radius: 4.00 |
| 166 | `Junk_10` | 6034 | Object | -2428.25,517.74,-458.07 | 26,389,184 | Scale/Radius: 5.00 |
| 167 | `Junk_08` | 6036 | Object | -2616.87,485.02,808.35 | 206,45,99 | Scale/Radius: 1.00 |
| 168 | `Junk_07` | 6037 | Object | -4395.25,502.34,-754.46 | 8,485,457 | Scale/Radius: 3.00 |
| 169 | `Junk_06` | 6038 | Object | -4179.69,521.59,862.24 | 485,336,471 | Scale/Radius: 2.00 |
| 170 | `Junk_05` | 6039 | Object | -2886.32,454.22,-1266.42 | 123,397,445 | Scale/Radius: 6.00 |
| 171 | `Junk_04` | 6040 | Object | -4314.41,600.50,-700.57 | 21,239,298 | Scale/Radius: 7.00 |
| 172 | `Junk_03` | 6041 | Object | -4287.47,510.04,-1293.37 | 238,27,86 | Scale/Radius: 7.00 |
| 173 | `Roid_Sm_Brown` | 6042 | Object | -3317.44,587.03,592.79 | 29,7,180 | Scale/Radius: 5.00 |
| 174 | `Roid_Med_Green` | 6043 | Object | -2616.87,583.18,673.63 | 510,133,83 | Scale/Radius: 5.00 |
| 175 | `Roid_Med_Green2` | 6044 | Object | -4449.14,500.42,-996.97 | 482,157,44 | Scale/Radius: 1.00 |
| 176 | `Roid_Sm_Brown2` | 6045 | Object | -4503.03,510.04,1131.70 | 321,207,70 | Scale/Radius: 7.00 |
| 177 | `Ice_Roid_1` | 6046 | Object | -2616.87,423.43,-808.35 | 470,491,97 | Scale/Radius: 6.00 |
| 178 | `Junk_10` | 6047 | Object | -4449.14,496.57,700.57 | 353,349,415 | Scale/Radius: 7.00 |
| 179 | `Junk_09` | 6048 | Object | -3473.62,847.18,1495.99 | 99,103,181 | Scale/Radius: 8.00 |
| 180 | `Junk_08` | 6049 | Object | -4745.54,594.72,-215.56 | 423,37,506 | Scale/Radius: 9.00 |
| 181 | `Junk_07` | 6050 | Object | -2536.03,411.88,215.56 | 332,305,503 | Scale/Radius: 1.00 |
| 182 | `Junk_06` | 6051 | Object | -3506.06,552.38,-889.19 | 421,267,276 | Scale/Radius: 5.00 |
| 183 | `Junk_05` | 6052 | Object | -3748.57,429.20,-458.07 | 92,508,406 | Scale/Radius: 2.00 |
| 184 | `Junk_03` | 6035 | Object | -4179.69,506.19,431.12 | 132,246,10 | Scale/Radius: 1.00 |
| 185 | `Roid_Lrg_Grey` | 6277 | Object | 2274.15,-33.87,-4318.73 | 131,151,421 | Scale/Radius: 1.00 |
| 186 | `Ice_Roid_2` | 6278 | Object | 2123.25,89.30,-3725.94 | 67,186,165 | Scale/Radius: 3.00 |
| 187 | `Ice_Roid_1` | 6279 | Object | 1966.07,58.51,-3963.06 | 503,280,166 | Scale/Radius: 2.00 |
| 188 | `Roid_Med_Green` | 6280 | Object | 2519.35,-181.69,-3810.63 | 228,485,49 | Scale/Radius: 3.00 |
| 189 | `Ice_Roid_2` | 6284 | Object | 2127.60,53.97,-3816.33 | 383,409,139 | Scale/Radius: 3.00 |
| 190 | `Ice_Roid_1` | 6285 | Object | 2337.02,-117.02,-3596.09 | 415,270,180 | Scale/Radius: 1.00 |
| 191 | `Roid_Med_Green2` | 6287 | Object | 2343.31,104.70,-3663.84 | 186,350,444 | Scale/Radius: 3.00 |
| 192 | `Ice_Roid_1` | 6291 | Object | 2003.80,261.75,-3788.04 | 451,338,379 | Scale/Radius: 3.00 |
| 193 | `Roid_Med_Green2` | 6293 | Object | 2121.32,7.78,-3788.10 | 251,508,443 | Scale/Radius: 5.00 |
| 194 | `Ice_Roid_2` | 6296 | Object | 2544.50,153.97,-4143.72 | 184,165,64 | Scale/Radius: 3.00 |
| 195 | `Ice_Roid_1` | 6297 | Object | 2506.77,-98.54,-3895.31 | 372,452,294 | Scale/Radius: 3.00 |
| 196 | `Roid_Med_Green` | 6298 | Object | 2425.04,639.24,-4088.30 | 182,232,407 | Scale/Radius: 7.00 |
| 197 | `Ice_Roid_2` | 6302 | Object | 1828.31,-61.59,-2735.67 | 107,412,173 | Scale/Radius: 5.00 |
| 198 | `Ice_Roid_1` | 6303 | Object | 1991.22,-224.80,-4290.51 | 443,468,331 | Scale/Radius: 2.00 |
| 199 | `Roid_Med_Green` | 6304 | Object | 2695.39,-194.00,-4188.88 | 302,259,67 | Scale/Radius: 6.00 |
| 200 | `Roid_Lrg_Grey` | 6307 | Object | 1972.36,-129.34,-4301.80 | 285,336,131 | Scale/Radius: 2.00 |
| 201 | `Ice_Roid_2` | 6308 | Object | 1802.61,61.59,-3799.33 | 502,94,88 | Scale/Radius: 3.00 |
| 202 | `Ice_Roid_1` | 6309 | Object | 2670.24,120.10,-4482.46 | 405,248,409 | Scale/Radius: 6.00 |
| 203 | `Ice_Roid_2` | 6314 | Object | 2072.30,-126.26,-2825.27 | 387,476,232 | Scale/Radius: 3.00 |
| 204 | `Ice_Roid_1` | 6315 | Object | 2016.37,209.40,-4380.84 | 462,454,32 | Scale/Radius: 1.00 |
| 205 | `Roid_Med_Green` | 6316 | Object | 1947.21,-15.40,-3494.47 | 270,380,214 | Scale/Radius: 2.00 |
| 206 | `Roid_Med_Green2` | 6317 | Object | 2330.73,107.78,-3833.21 | 448,24,96 | Scale/Radius: 5.00 |
| 207 | `Roid_Lrg_Grey` | 6318 | Object | 1953.50,157.05,-4121.14 | 419,493,469 | Scale/Radius: 2.00 |
| 208 | `Ice_Roid_1` | 6320 | Object | 1978.65,166.29,-4155.01 | 436,222,256 | Scale/Radius: 3.00 |
| 209 | `Roid_XL_Green` | 6323 | Object | 2714.25,-110.86,-4245.34 | 141,233,306 | Scale/Radius: 2.00 |
| 210 | `Ice_Roid_1` | 6326 | Object | 1314.86,-58.94,-2486.92 | 437,220,391 | Scale/Radius: 5.00 |
| 211 | `Roid_Med_Green` | 6327 | Object | 1934.64,-187.85,-4284.86 | 319,99,319 | Scale/Radius: 3.00 |
| 212 | `Roid_XL_Green` | 6329 | Object | 1953.50,135.50,-4211.47 | 345,134,461 | Scale/Radius: 1.00 |
| 213 | `Ice_Roid_1` | 6332 | Object | 2663.95,181.69,-3579.15 | 169,445,171 | Scale/Radius: 1.00 |
| 214 | `Roid_Med_Green` | 6333 | Object | 2160.98,-40.03,-3686.42 | 105,480,86 | Scale/Radius: 4.00 |
| 215 | `Roid_Med_Green2` | 6334 | Object | 2624.34,24.64,-4634.26 | 391,1,80 | Scale/Radius: 6.00 |
| 216 | `Roid_Lrg_Grey` | 6335 | Object | 2594.79,-67.75,-4019.51 | 458,364,289 | Scale/Radius: 3.00 |
| 217 | `Ice_Roid_1` | 6337 | Object | 2519.35,18.48,-3833.21 | 215,505,102 | Scale/Radius: 1.00 |
| 218 | `Roid_XL_Green` | 6340 | Object | 2500.49,-150.89,-3635.61 | 459,328,12 | Scale/Radius: 1.00 |
| 219 | `Roid_Lrg_Grey` | 6341 | Object | 2764.55,15.40,-4205.82 | 451,141,504 | Scale/Radius: 5.00 |
| 220 | `Ice_Roid_2` | 6342 | Object | 2462.76,252.51,-3709.00 | 487,296,82 | Scale/Radius: 1.00 |
| 221 | `Roid_Med_Green` | 6344 | Object | 1953.50,-58.51,-3923.54 | 120,356,89 | Scale/Radius: 7.00 |
| 222 | `Roid_Lrg_Grey` | 6346 | Object | 1865.48,-117.02,-4442.94 | 367,57,324 | Scale/Radius: 7.00 |
| 223 | `Ice_Roid_2` | 6347 | Object | 1299.63,80.07,-3189.60 | 113,411,216 | Scale/Radius: 6.00 |
| 224 | `Roid_Med_Green` | 6349 | Object | 3097.77,-61.59,-4815.55 | 406,173,54 | Scale/Radius: 1.00 |
| 225 | `Roid_Lrg_Grey` | 6352 | Object | 2343.31,-314.10,-3788.04 | 352,503,78 | Scale/Radius: 4.00 |
| 226 | `Ice_Roid_2` | 6353 | Object | 2167.26,-49.27,-4488.10 | 271,395,20 | Scale/Radius: 3.00 |
| 227 | `Ice_Roid_1` | 6354 | Object | 1350.03,135.50,-2394.12 | 72,159,481 | Scale/Radius: 2.00 |
| 228 | `Roid_Med_Green` | 6355 | Object | 3122.92,221.72,-4431.65 | 53,13,175 | Scale/Radius: 4.00 |
| 229 | `Roid_Med_Green2` | 6356 | Object | 1685.70,-8.40,-3053.17 | 369,323,432 | Scale/Radius: 6.00 |
| 230 | `Roid_Lrg_Grey` | 6358 | Object | 2318.16,388.01,-3031.53 | 208,380,333 | Scale/Radius: 3.00 |
| 231 | `Ice_Roid_2` | 6359 | Object | 2016.37,-209.40,-4668.76 | 331,446,148 | Scale/Radius: 5.00 |
| 232 | `Ice_Roid_1` | 6360 | Object | 2720.54,-449.60,-3833.21 | 205,133,143 | Scale/Radius: 6.00 |
| 233 | `Roid_Med_Green2` | 6362 | Object | 2016.37,30.79,-4363.90 | 185,60,171 | Scale/Radius: 4.00 |
| 234 | `Roid_Lrg_Grey` | 6364 | Object | 2632.52,67.75,-4815.55 | 255,201,134 | Scale/Radius: 5.00 |
| 235 | `Ice_Roid_2` | 6365 | Object | 2293.01,-12.32,-4713.93 | 507,292,173 | Scale/Radius: 3.00 |
| 236 | `Ice_Roid_1` | 6366 | Object | 1953.50,277.15,-4262.28 | 481,103,115 | Scale/Radius: 1.00 |
| 237 | `Roid_Med_Green` | 6367 | Object | 2406.18,461.92,-3957.41 | 157,16,46 | Scale/Radius: 5.00 |
| 238 | `Roid_Med_Green2` | 6368 | Object | 3198.36,234.04,-3844.50 | 174,108,202 | Scale/Radius: 4.00 |
| 239 | `Roid_XL_Green` | 6369 | Object | 1890.63,344.90,-3754.17 | 202,144,105 | Scale/Radius: 1.00 |
| 240 | `Roid_Lrg_Grey` | 6370 | Object | 1940.92,80.07,-4036.45 | 266,54,459 | Scale/Radius: 4.00 |
| 241 | `Ice_Roid_2` | 6371 | Object | 1601.42,541.98,-4239.69 | 451,469,251 | Scale/Radius: 6.00 |
| 242 | `Ice_Roid_1` | 6372 | Object | 1651.71,369.53,-4284.86 | 456,237,490 | Scale/Radius: 3.00 |
| 243 | `Roid_Med_Green` | 6373 | Object | 1852.90,-55.43,-4951.05 | 15,502,431 | Scale/Radius: 8.00 |
| 244 | `Roid_Med_Green2` | 6374 | Object | 2142.11,-301.79,-3246.06 | 18,182,195 | Scale/Radius: 6.00 |
| 245 | `Roid_XL_Green` | 6375 | Object | 3135.49,246.36,-3438.01 | 154,309,192 | Scale/Radius: 1.00 |
| 246 | `Roid_Lrg_Grey` | 6376 | Object | 2758.26,-197.08,-4002.58 | 55,169,7 | Scale/Radius: 1.00 |
| 247 | `Ice_Roid_2` | 6377 | Object | 3135.49,-234.04,-3957.41 | 237,386,420 | Scale/Radius: 2.00 |
| 248 | `Ice_Roid_1` | 6378 | Object | 2116.97,234.04,-3212.19 | 450,38,381 | Scale/Radius: 6.00 |
| 249 | `Roid_Med_Green` | 6379 | Object | 2443.90,314.10,-4544.56 | 353,258,155 | Scale/Radius: 4.00 |
| 250 | `Roid_Med_Green2` | 6380 | Object | 1299.63,-30.79,-4284.86 | 303,426,176 | Scale/Radius: 3.00 |
| 251 | `Roid_XL_Green` | 6381 | Object | 2431.33,-461.92,-4059.03 | 152,44,330 | Scale/Radius: 1.00 |
| 252 | `Roid_Lrg_Grey` | 6382 | Object | 1136.68,-43.11,-2556.70 | 40,350,218 | Scale/Radius: 1.00 |
| 253 | `Ice_Roid_2` | 6383 | Object | 3298.96,-338.74,-4680.05 | 203,115,11 | Scale/Radius: 6.00 |
| 254 | `Ice_Roid_1` | 6384 | Object | 1886.24,-3.69,-3502.45 | 288,64,433 | Scale/Radius: 5.00 |
| 255 | `Roid_Med_Green` | 6385 | Object | 1412.80,-36.95,-3844.50 | 294,78,132 | Scale/Radius: 9.00 |
| 256 | `Roid_Med_Green2` | 6386 | Object | 2569.64,461.92,-3483.18 | 183,476,464 | Scale/Radius: 1.00 |
| 257 | `Ice_Roid_2` | 6389 | Object | 2393.60,18.48,-4510.69 | 127,70,511 | Scale/Radius: 1.00 |
| 258 | `Ice_Roid_1` | 6390 | Object | 2884.00,-98.54,-3325.10 | 180,279,44 | Scale/Radius: 2.00 |
| 259 | `Roid_Med_Green` | 6391 | Object | 2506.77,498.87,-3810.63 | 3,262,0 | Scale/Radius: 1.00 |
| 260 | `Roid_Med_Green2` | 6392 | Object | 1073.29,138.57,-4584.08 | 380,359,257 | Scale/Radius: 3.00 |
| 261 | `Ice_Roid_2` | 6395 | Object | 1337.35,101.62,-3025.88 | 469,435,384 | Scale/Radius: 3.00 |
| 262 | `Ice_Roid_1` | 6396 | Object | 658.34,-508.11,-3533.99 | 416,407,185 | Scale/Radius: 4.00 |
| 263 | `Roid_Med_Green` | 6397 | Object | 1959.79,-101.62,-5075.25 | 355,340,422 | Scale/Radius: 4.00 |
| 264 | `Roid_Med_Green2` | 6398 | Object | 3011.59,147.81,-2935.64 | 48,282,355 | Scale/Radius: 1.00 |
| 265 | `Roid_XL_Green` | 6399 | Object | 809.23,64.67,-4228.40 | 325,442,270 | Scale/Radius: 1.00 |
| 266 | `Roid_Lrg_Grey` | 6400 | Object | 1954.43,27.71,-3110.02 | 109,364,498 | Scale/Radius: 5.00 |
| 267 | `Ice_Roid_2` | 6401 | Object | 2186.13,221.72,-4990.57 | 388,258,85 | Scale/Radius: 1.00 |
| 268 | `Ice_Roid_1` | 6402 | Object | 1922.06,-461.92,-5329.30 | 46,118,51 | Scale/Radius: 2.00 |
| 269 | `Roid_Med_Green` | 6403 | Object | 1205.32,-332.58,-5210.75 | 186,316,466 | Scale/Radius: 2.00 |
| 270 | `Roid_Med_Green2` | 6404 | Object | 1299.63,249.43,-4330.02 | 406,365,189 | Scale/Radius: 3.00 |
| 271 | `Ice_Roid_1` | 6408 | Object | 1205.32,-55.43,-2754.89 | 260,140,465 | Scale/Radius: 3.00 |
| 272 | `Roid_Med_Green` | 6409 | Object | 2619.94,-129.34,-2958.13 | 254,149,58 | Scale/Radius: 8.00 |
| 273 | `Roid_Med_Green2` | 6410 | Object | 2978.31,323.34,-4516.33 | 444,51,302 | Scale/Radius: 6.00 |
| 274 | `Roid_XL_Green` | 6411 | Object | 2223.85,702.11,-4719.57 | 258,185,308 | Scale/Radius: 1.00 |
| 275 | `Roid_Lrg_Grey` | 6412 | Object | 1620.28,332.58,-3855.79 | 325,74,180 | Scale/Radius: 7.00 |
| 276 | `Ice_Roid_2` | 6413 | Object | 1205.32,-147.81,-4143.72 | 245,195,322 | Scale/Radius: 5.00 |
| 277 | `Ice_Roid_1` | 6414 | Object | 2072.96,-36.95,-4516.33 | 470,175,136 | Scale/Radius: 5.00 |
| 278 | `Roid_Lrg_Grey` | 6418 | Object | 2601.08,-369.53,-3178.31 | 263,462,142 | Scale/Radius: 2.00 |
| 279 | `Ice_Roid_2` | 6419 | Object | 2186.13,-184.77,-4584.08 | 431,434,250 | Scale/Radius: 6.00 |
| 280 | `Roid_Med_Green` | 6421 | Object | 2450.19,267.91,-3313.81 | 38,389,126 | Scale/Radius: 3.00 |
| 281 | `Ice_Roid_2` | 6424 | Object | 991.62,-160.13,-3288.49 | 47,359,251 | Scale/Radius: 1.00 |
| 282 | `Ice_Roid_1` | 6425 | Object | 3399.55,788.34,-3934.83 | 493,356,371 | Scale/Radius: 2.00 |
| 283 | `Roid_Med_Green2` | 6427 | Object | 2720.54,-36.95,-4657.47 | 134,16,153 | Scale/Radius: 5.00 |
| 284 | `Roid_XL_Green` | 6428 | Object | 952.09,-125.44,-4907.05 | 409,370,80 | Scale/Radius: 1.00 |
| 285 | `Roid_Lrg_Grey` | 6429 | Object | 3625.89,24.64,-4025.16 | 373,210,83 | Scale/Radius: 3.00 |
| 286 | `Ice_Roid_2` | 6430 | Object | 2972.02,-591.25,-4138.07 | 213,487,489 | Scale/Radius: 6.00 |
| 287 | `Ice_Roid_1` | 6431 | Object | 1261.91,73.91,-3731.59 | 82,479,424 | Scale/Radius: 1.00 |
| 288 | `Roid_Med_Green` | 6432 | Object | 1437.95,36.95,-3550.93 | 55,408,326 | Scale/Radius: 5.00 |
| 289 | `Roid_Med_Green2` | 6433 | Object | 1480.62,429.39,-4725.22 | 200,344,83 | Scale/Radius: 6.00 |
| 290 | `Roid_XL_Green` | 6434 | Object | 2997.17,-369.53,-3460.60 | 109,329,39 | Scale/Radius: 2.00 |
| 291 | `Roid_Lrg_Grey` | 6435 | Object | 708.63,357.22,-5267.20 | 159,338,164 | Scale/Radius: 2.00 |
| 292 | `Ice_Roid_2` | 6436 | Object | 2318.16,-99.76,-5497.82 | 190,268,341 | Scale/Radius: 4.00 |
| 293 | `Ice_Roid_1` | 6437 | Object | 2318.16,862.24,-3686.42 | 463,306,48 | Scale/Radius: 2.00 |
| 294 | `Roid_Med_Green` | 6438 | Object | 2393.60,172.45,-4657.47 | 266,124,387 | Scale/Radius: 5.00 |
| 295 | `Roid_Med_Green2` | 6439 | Object | 3952.83,210.43,-2873.45 | 176,345,441 | Scale/Radius: 6.00 |
| 296 | `Roid_Lrg_Grey` | 6441 | Object | 2670.24,628.21,-3957.41 | 248,243,80 | Scale/Radius: 2.00 |
| 297 | `Ice_Roid_2` | 6442 | Object | 3084.98,-86.22,-5299.47 | 8,123,101 | Scale/Radius: 5.00 |
| 298 | `Ice_Roid_1` | 6443 | Object | 1136.16,541.98,-3302.52 | 362,154,476 | Scale/Radius: 5.00 |
| 299 | `Roid_Med_Green` | 6444 | Object | 884.14,-400.33,-3041.70 | 204,351,190 | Scale/Radius: 5.00 |
| 300 | `Roid_Med_Green2` | 6445 | Object | 970.63,-631.29,-3560.75 | 347,406,334 | Scale/Radius: 8.00 |
| 301 | `Roid_XL_Green` | 6446 | Object | 3057.19,84.11,-5502.80 | 372,221,203 | Scale/Radius: 1.00 |
| 302 | `Roid_Lrg_Grey` | 6447 | Object | 2462.76,138.57,-3799.33 | 411,9,428 | Scale/Radius: 7.00 |
| 303 | `Ice_Roid_2` | 6448 | Object | 922.40,-716.68,-4358.77 | 194,155,489 | Scale/Radius: 6.00 |
| 304 | `Ice_Roid_1` | 6449 | Object | 3563.02,508.11,-4872.01 | 92,319,112 | Scale/Radius: 5.00 |
| 305 | `Roid_Med_Green` | 6450 | Object | 2179.84,384.93,-3375.91 | 470,95,187 | Scale/Radius: 6.00 |
| 306 | `Roid_Lrg_Grey` | 6453 | Object | 2871.43,-445.98,-3292.27 | 414,315,171 | Scale/Radius: 3.00 |
| 307 | `Ice_Roid_2` | 6454 | Object | 545.17,107.18,-5149.05 | 422,116,291 | Scale/Radius: 1.00 |
| 308 | `Ice_Roid_1` | 6455 | Object | 608.04,230.96,-4250.99 | 251,358,55 | Scale/Radius: 3.00 |
| 309 | `Roid_Lrg_Grey` | 6458 | Object | 1416.61,-444.20,-3855.79 | 482,244,234 | Scale/Radius: 4.00 |
| 310 | `Ice_Roid_2` | 6459 | Object | 1601.42,184.77,-2941.20 | 15,14,211 | Scale/Radius: 1.00 |
| 311 | `Ice_Roid_1` | 6460 | Object | 3248.09,203.24,-3156.64 | 25,230,312 | Scale/Radius: 3.00 |
| 312 | `Roid_Med_Green` | 6461 | Object | 953.57,184.77,-3914.32 | 118,424,229 | Scale/Radius: 8.00 |
| 313 | `Roid_Med_Green2` | 6462 | Object | 319.28,-110.86,-4567.69 | 242,90,383 | Scale/Radius: 5.00 |
| 314 | `Roid_XL_Green` | 6463 | Object | 1865.48,-424.96,-4059.03 | 33,107,388 | Scale/Radius: 1.00 |
| 315 | `Roid_Lrg_Grey` | 6464 | Object | 3261.99,94.88,-5729.35 | 376,64,420 | Scale/Radius: 2.00 |
| 316 | `Ice_Roid_2` | 6465 | Object | 1261.91,-110.86,-3821.92 | 194,54,504 | Scale/Radius: 1.00 |
| 317 | `Ice_Roid_1` | 6466 | Object | 2770.83,-560.46,-3946.12 | 197,401,378 | Scale/Radius: 4.00 |
| 318 | `Roid_Med_Green` | 6467 | Object | 1494.53,-215.56,-3037.17 | 223,447,206 | Scale/Radius: 1.00 |
| 319 | `Roid_Med_Green2` | 6468 | Object | 2154.69,-83.53,-2589.27 | 35,203,405 | Scale/Radius: 1.00 |
| 320 | `Roid_Lrg_Grey` | 6469 | Object | 2154.69,452.68,-5210.75 | 475,481,479 | Scale/Radius: 6.00 |
| 321 | `Ice_Roid_2` | 6470 | Object | 1758.60,-86.22,-3076.69 | 166,486,190 | Scale/Radius: 1.00 |
| 322 | `Ice_Roid_1` | 6471 | Object | 3461.85,29.21,-3031.80 | 320,223,81 | Scale/Radius: 5.00 |
| 323 | `Roid_Med_Green` | 6472 | Object | 1236.76,285.60,-2773.91 | 93,275,3 | Scale/Radius: 3.00 |
| 324 | `Ice_Roid_2` | 6476 | Object | 3657.33,831.45,-4736.51 | 90,275,197 | Scale/Radius: 4.00 |
| 325 | `Ice_Roid_1` | 6477 | Object | 1111.01,-332.58,-4838.13 | 277,166,493 | Scale/Radius: 4.00 |
| 326 | `Roid_Med_Green` | 6478 | Object | 298.06,-677.48,-3669.83 | 51,284,310 | Scale/Radius: 8.00 |
| 327 | `Roid_Med_Green2` | 6479 | Object | 1111.01,30.79,-2952.49 | 378,395,340 | Scale/Radius: 5.00 |
| 328 | `Roid_Lrg_Grey` | 6481 | Object | 3600.74,-233.80,-5385.54 | 181,384,344 | Scale/Radius: 1.00 |
| 329 | `Ice_Roid_2` | 6482 | Object | 2978.31,189.75,-5404.11 | 44,0,144 | Scale/Radius: 1.00 |
| 330 | `Ice_Roid_1` | 6483 | Object | 2066.67,862.24,-3709.00 | 34,139,437 | Scale/Radius: 5.00 |
| 331 | `Roid_XL_Green` | 6493 | Object | 1440.21,0.00,-4103.79 | 0,0,0 | Scale/Radius: 1.00 |
| 332 | `Roid_XL_Green` | 6495 | Object | 1656.60,0.00,-4136.90 | 0,0,0 | Scale/Radius: 1.00 |
| 333 | `Roid_XL_Green` | 6505 | Object | 1649.26,0.00,-4448.51 | 0,0,0 | Scale/Radius: 1.00 |
| 334 | `Roid_XL_Green` | 6506 | Object | 2822.65,0.00,-4343.98 | 57,85,78 | Scale/Radius: 1.00 |
| 335 | `Roid_XL_Green` | 6507 | Object | 2197.39,0.00,-4848.72 | 441,427,384 | Scale/Radius: 1.00 |
| 336 | `Roid_Lrg_Grey` | 6519 | Object | 2805.60,7.19,-5711.06 | 5,168,176 | Scale/Radius: 1.00 |
| 337 | `Ice_Roid_1` | 6521 | Object | 3172.94,76.46,-5584.63 | 245,80,147 | Scale/Radius: 3.00 |
| 338 | `Roid_XL_Green` | 6522 | Object | 2503.61,40.42,-5238.96 | 78,100,4 | Scale/Radius: 1.00 |
| 339 | `Ice_Roid_2` | 6524 | Object | 3114.58,-31.44,-5918.20 | 422,333,445 | Scale/Radius: 4.00 |
| 340 | `Ice_Roid_1` | 6525 | Object | 3332.47,-0.90,-5598.18 | 23,143,124 | Scale/Radius: 4.00 |
| 341 | `Roid_XL_Green` | 6526 | Object | 3039.75,-38.62,-5726.08 | 497,451,268 | Scale/Radius: 1.00 |
| 342 | `Roid_Lrg_Grey` | 6527 | Object | 2270.30,5.39,-5698.83 | 23,310,379 | Scale/Radius: 1.00 |
| 343 | `Ice_Roid_1` | 6529 | Object | 1796.80,-8.98,-4177.52 | 60,27,507 | Scale/Radius: 5.00 |
| 344 | `Roid_XL_Green` | 6530 | Object | 3486.50,-8.98,-6465.73 | 445,445,350 | Scale/Radius: 1.00 |
| 345 | `Ice_Roid_2` | 6532 | Object | 3671.27,163.47,-6390.28 | 54,456,47 | Scale/Radius: 6.00 |
| 346 | `Ice_Roid_1` | 6533 | Object | 3542.96,-55.69,-6207.06 | 336,36,425 | Scale/Radius: 4.00 |
| 347 | `Roid_XL_Green` | 6534 | Object | 3774.99,94.22,-5600.98 | 441,259,156 | Scale/Radius: 2.00 |
| 348 | `Roid_Lrg_Grey` | 6535 | Object | 2854.13,-5.39,-6018.03 | 187,26,142 | Scale/Radius: 5.00 |
| 349 | `Ice_Roid_2` | 6536 | Object | 739.81,-220.95,-3295.16 | 432,299,51 | Scale/Radius: 2.00 |
| 350 | `Ice_Roid_1` | 6537 | Object | 3318.42,-202.09,-6309.45 | 68,167,326 | Scale/Radius: 6.00 |
| 351 | `Roid_XL_Green` | 6538 | Object | 3286.39,165.26,-5209.90 | 503,292,68 | Scale/Radius: 1.00 |
| 352 | `Roid_Lrg_Grey` | 6539 | Object | 3360.76,-53.89,-6223.23 | 159,382,476 | Scale/Radius: 1.00 |
| 353 | `Ice_Roid_2` | 6540 | Object | 2568.71,-111.37,-5532.93 | 138,171,389 | Scale/Radius: 1.00 |
| 354 | `Ice_Roid_1` | 6541 | Object | 2514.35,134.73,-5796.50 | 343,129,446 | Scale/Radius: 4.00 |
| 355 | `Roid_XL_Green` | 6542 | Object | 3881.70,-51.89,-5572.12 | 479,169,471 | Scale/Radius: 1.00 |
| 356 | `Roid_Lrg_Grey` | 6543 | Object | 3768.79,-161.67,-5856.77 | 230,340,118 | Scale/Radius: 2.00 |
| 357 | `Ice_Roid_2` | 6544 | Object | 3691.80,226.34,-6452.26 | 56,182,44 | Scale/Radius: 6.00 |
| 358 | `Ice_Roid_1` | 6545 | Object | 2357.83,143.71,-5042.42 | 308,162,355 | Scale/Radius: 6.00 |
| 359 | `Roid_Lrg_Grey` | 6546 | Object | 2455.34,179.63,-4925.44 | 462,205,355 | Scale/Radius: 2.00 |
| 360 | `Roid_Med_Green` | 6558 | Object | 2645.38,56.38,-4731.60 | 71,249,36 | Scale/Radius: 1.00 |
| 361 | `Roid_XL_Green` | 6560 | Object | 3609.68,111.20,-6332.37 | 128,85,192 | Scale/Radius: 1.00 |
| 362 | `Roid_Lrg_Grey` | 6282 | Object | 2313.69,27.93,-4416.59 | 365,351,321 | Scale/Radius: 1.00 |
| 363 | `Roid_Lrg_Grey` | 6300 | Object | 2119.60,-15.40,-3929.43 | 118,310,323 | Scale/Radius: 1.00 |
| 364 | `Roid_Med_Green` | 6393 | Object | 1638.33,-27.71,-3126.84 | 509,8,455 | Scale/Radius: 1.00 |
| 365 | `Roid_Lrg_Grey` | 6288 | Object | 2551.93,43.11,-4603.35 | 327,332,89 | Scale/Radius: 1.00 |
| 366 | `Spcargo_Parts` | 6757 | Interactive | -4471.20,-30.71,-837.25 | 0,0,0 | secondary groups: CONT_060, none |
| 367 | `Spcargo_Contraband` | 6758 | Interactive | 2820.05,-30.71,-5960.26 | 284,284,286 | secondary groups: CONT_062, none |
| 368 | `Spcargo_Credits` | 6768 | Interactive | -3697.89,-1250.84,313.82 | 0,158,158 | secondary groups: CONT_067, none |
| 369 | `Generic_Colony_Station` | 5649 | Interactive | -3189.79,-1145.14,-10.44 | 384,0,0 | secondary groups: none, WRECKTOWN |
| 370 | `Mad_Pirate_Platform` | 6264 | Interactive | -2142.93,-1038.84,-10.31 | 128,0,0 | None |
