# Tachyon: The Fringe FRON07.SPX - Freedom and Humiliation

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON07.SPX` |
| Sector | `QUAD_07` |
| Backdrop | `FRONTI7.BDF` |
| Region | 4 |
| Sector ID | 6 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 7 |
| Entities | 117 |
| Events | 2 |
| Waypoints | 0 |
| Child Sectors | 2 |
| Scripts | 1 |
| Scenes | 2 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Baron_Onrald_Station`, `1: Spcargo_Contraband`, `2: Spcargo_Art`, `3: Junk_10`, `4: Junk_05`, `5: Junk_04`, `6: Hyper_Gate` |
| Scripts | `PLAYER.SCR` |
| Scenes | `F7BC020A.SEN`, `F7GC051A.SEN` |
| Labels | `BFGE_01`, `alexander`, `BFGF_01`, `baronhajod` |
| Aliases | `jumbo`, `jumbo_1`, `egg`, `egg_1`, `Hajod_1` |
| Groups | `CONT_061`, `CONT_031` |
| Child Sectors | [fron07A.spx](FRON07A.md), [fron07B.spx](FRON07B.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 1226; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 212
- Set/add variable: variable group 16, variable 803, subtype 0, value 1

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 1225; flags 2)

**Action**

- Set/add variable: variable group 16, variable 805, subtype 0, value 1

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | 728.61,0.00,-1423.22 | 0,0,0 | Gate SPX: [fron12.spx](FRON12.md) |
| 1 | `Hyper_Gate` | 2 | Gate | -2919.47,0.00,1778.39 | 128,0,0 | Gate SPX: [fron12.spx](FRON12.md) |
| 2 | `Junk_04` | 953 | Object | 1128.53,30.55,245.59 | 486,300,405 | Scale/Radius: 10.00 |
| 3 | `Junk_04` | 955 | Object | 1710.85,139.55,1492.86 | 44,238,447 | Scale/Radius: 10.00 |
| 4 | `Junk_04` | 956 | Object | 976.49,151.39,2531.08 | 247,0,0 | Scale/Radius: 9.85 |
| 5 | `Junk_04` | 958 | Object | -1020.89,214.12,1087.28 | 205,314,432 | Scale/Radius: 3.85 |
| 6 | `Junk_04` | 960 | Object | 1318.09,-392.73,-159.64 | 267,304,428 | Scale/Radius: 5.07 |
| 7 | `Junk_04` | 961 | Object | 810.44,-66.99,-124.84 | 142,44,431 | Scale/Radius: 10.00 |
| 8 | `Junk_04` | 963 | Object | -83.07,-245.31,1329.99 | 243,397,474 | Scale/Radius: 3.30 |
| 9 | `Junk_05` | 968 | Object | 1240.91,-118.53,2.60 | 394,31,186 | Scale/Radius: 3.49 |
| 10 | `Junk_05` | 969 | Object | 1392.30,425.29,699.04 | 441,402,38 | Scale/Radius: 3.49 |
| 11 | `Junk_05` | 971 | Object | -446.29,-229.09,875.38 | 485,172,391 | Scale/Radius: 3.49 |
| 12 | `Junk_05` | 972 | Object | -715.33,-166.08,1732.38 | 471,78,348 | Scale/Radius: 3.49 |
| 13 | `Junk_05` | 973 | Object | 15.95,156.79,2394.40 | 63,158,303 | Scale/Radius: 3.49 |
| 14 | `Junk_05` | 974 | Object | 107.69,-93.57,2045.39 | 220,331,141 | Scale/Radius: 3.49 |
| 15 | `Junk_05` | 976 | Object | 880.59,130.26,2155.70 | 316,67,447 | Scale/Radius: 3.49 |
| 16 | `Junk_05` | 977 | Object | 263.11,216.20,2522.69 | 474,316,144 | Scale/Radius: 3.49 |
| 17 | `Junk_05` | 978 | Object | 156.77,-323.64,2214.92 | 284,420,128 | Scale/Radius: 3.49 |
| 18 | `Junk_05` | 979 | Object | 263.15,50.74,1881.15 | 442,354,174 | Scale/Radius: 3.49 |
| 19 | `Junk_05` | 980 | Object | -214.41,158.68,1087.32 | 444,78,410 | Scale/Radius: 3.49 |
| 20 | `Junk_05` | 981 | Object | -192.10,-148.10,200.26 | 452,316,85 | Scale/Radius: 3.49 |
| 21 | `Junk_05` | 982 | Object | 1556.72,-103.01,5.79 | 152,78,46 | Scale/Radius: 4.10 |
| 22 | `Junk_05` | 983 | Object | 1684.17,63.47,1799.75 | 431,158,155 | Scale/Radius: 3.49 |
| 23 | `Junk_10` | 1029 | Object | -787.61,-123.54,2463.01 | 347,84,30 | Scale/Radius: 2.22 |
| 24 | `Junk_10` | 1030 | Object | -961.55,577.94,1907.29 | 441,417,158 | Scale/Radius: 7.26 |
| 25 | `Junk_10` | 1032 | Object | -100.15,-384.40,546.37 | 252,44,327 | Scale/Radius: 2.58 |
| 26 | `Junk_10` | 1033 | Object | 1293.40,-151.39,240.46 | 324,448,212 | Scale/Radius: 4.06 |
| 27 | `Junk_10` | 1034 | Object | 462.70,368.03,1230.44 | 63,158,417 | Scale/Radius: 2.93 |
| 28 | `Junk_10` | 1036 | Object | -70.89,-380.48,1577.73 | 101,158,363 | Scale/Radius: 3.24 |
| 29 | `Junk_10` | 1037 | Object | 787.43,205.81,581.70 | 410,224,225 | Scale/Radius: 3.02 |
| 30 | `Junk_10` | 1038 | Object | 1061.21,-173.21,719.49 | 245,304,410 | Scale/Radius: 1.98 |
| 31 | `Junk_10` | 1041 | Object | -610.70,-116.78,1235.58 | 31,218,68 | Scale/Radius: 3.01 |
| 32 | `Junk_10` | 1042 | Object | 1420.53,35.21,897.42 | 169,132,292 | Scale/Radius: 3.70 |
| 33 | `Junk_10` | 1043 | Object | 1887.39,-85.67,1589.69 | 158,64,472 | Scale/Radius: 2.27 |
| 34 | `Junk_10` | 1045 | Object | -875.18,293.85,685.79 | 100,205,431 | Scale/Radius: 5.08 |
| 35 | `Junk_10` | 1046 | Object | 1016.03,98.93,1520.16 | 94,70,405 | Scale/Radius: 3.97 |
| 36 | `Junk_05` | 1096 | Object | -793.70,131.44,920.77 | 313,31,162 | Scale/Radius: 3.49 |
| 37 | `Junk_05` | 1097 | Object | -718.43,309.92,104.76 | 158,408,284 | Scale/Radius: 3.49 |
| 38 | `Junk_05` | 1098 | Object | -544.96,287.19,467.90 | 158,432,31 | Scale/Radius: 3.49 |
| 39 | `Junk_05` | 1099 | Object | 649.67,176.86,429.28 | 141,102,218 | Scale/Radius: 3.49 |
| 40 | `Junk_05` | 1100 | Object | 952.68,304.13,385.93 | 151,316,425 | Scale/Radius: 3.49 |
| 41 | `Junk_05` | 1101 | Object | 1227.88,211.83,992.47 | 427,16,394 | Scale/Radius: 3.49 |
| 42 | `Junk_05` | 1102 | Object | 1320.64,71.65,1906.87 | 408,92,100 | Scale/Radius: 3.49 |
| 43 | `Junk_05` | 1103 | Object | 1192.71,368.78,2053.26 | 395,347,448 | Scale/Radius: 3.49 |
| 44 | `Junk_04` | 1104 | Object | 417.62,91.24,2317.11 | 205,368,427 | Scale/Radius: 4.79 |
| 45 | `Junk_04` | 1105 | Object | 22.13,-62.99,1010.30 | 78,158,438 | Scale/Radius: 6.07 |
| 46 | `Junk_10` | 1132 | Object | -569.85,92.56,1597.40 | 371,471,171 | Scale/Radius: 1.64 |
| 47 | `Junk_10` | 1133 | Object | -685.58,-120.91,392.80 | 228,191,141 | Scale/Radius: 3.51 |
| 48 | `Junk_10` | 1134 | Object | -236.36,439.17,-129.41 | 58,91,304 | Scale/Radius: 4.25 |
| 49 | `Junk_10` | 1135 | Object | 91.50,67.12,367.30 | 283,141,82 | Scale/Radius: 2.16 |
| 50 | `Junk_10` | 1136 | Object | 718.43,44.63,1020.54 | 94,412,189 | Scale/Radius: 1.44 |
| 51 | `Junk_10` | 1137 | Object | 234.67,-139.90,867.38 | 78,94,110 | Scale/Radius: 3.51 |
| 52 | `Junk_10` | 1138 | Object | 824.28,142.69,1345.79 | 347,142,73 | Scale/Radius: 5.68 |
| 53 | `Junk_10` | 1140 | Object | 1541.44,67.34,2273.91 | 141,78,31 | Scale/Radius: 6.37 |
| 54 | `Junk_10` | 1142 | Object | 93.07,-310.91,1440.31 | 158,114,107 | Scale/Radius: 1.27 |
| 55 | `Junk_10` | 1143 | Object | -13.71,-270.74,1793.10 | 408,186,394 | Scale/Radius: 4.01 |
| 56 | `Junk_10` | 1144 | Object | -313.48,-53.44,2290.40 | 267,110,437 | Scale/Radius: 2.41 |
| 57 | `Junk_10` | 1127 | Object | 1930.25,-344.96,1175.01 | 404,92,274 | Scale/Radius: 6.73 |
| 58 | `Junk_10` | 1019 | Object | -760.45,191.36,550.04 | 202,46,368 | Scale/Radius: 6.73 |
| 59 | `Junk_10` | 1020 | Object | -263.73,-255.42,1672.57 | 0,0,402 | Scale/Radius: 6.73 |
| 60 | `Junk_10` | 1021 | Object | 1604.05,-222.15,938.12 | 213,50,425 | Scale/Radius: 6.73 |
| 61 | `Junk_10` | 1022 | Object | 746.46,-167.82,2579.18 | 65,425,142 | Scale/Radius: 6.73 |
| 62 | `Junk_10` | 1023 | Object | -113.48,174.50,2620.24 | 252,442,469 | Scale/Radius: 6.73 |
| 63 | `Junk_10` | 1024 | Object | -425.06,208.26,1152.33 | 148,316,68 | Scale/Radius: 6.73 |
| 64 | `Junk_10` | 1025 | Object | 1089.88,-287.85,2343.08 | 0,0,77 | Scale/Radius: 6.73 |
| 65 | `Junk_10` | 1026 | Object | 1257.31,156.08,1432.54 | 347,110,213 | Scale/Radius: 6.73 |
| 66 | `Junk_10` | 1027 | Object | 1333.80,-514.76,543.27 | 127,30,14 | Scale/Radius: 6.73 |
| 67 | `Junk_10` | 1123 | Object | -555.85,442.31,1435.35 | 486,302,64 | Scale/Radius: 6.73 |
| 68 | `Junk_10` | 1124 | Object | -704.87,200.83,1979.48 | 210,245,412 | Scale/Radius: 6.73 |
| 69 | `Junk_10` | 1125 | Object | 1605.86,368.93,1308.51 | 329,280,229 | Scale/Radius: 6.73 |
| 70 | `Junk_10` | 1126 | Object | 1839.91,318.18,628.23 | 449,316,149 | Scale/Radius: 6.73 |
| 71 | `Junk_10` | 1128 | Object | 284.07,213.22,617.74 | 16,31,442 | Scale/Radius: 6.73 |
| 72 | `Junk_05` | 997 | Object | -6.92,271.44,776.99 | 110,270,466 | Scale/Radius: 7.09 |
| 73 | `Junk_05` | 984 | Object | 1198.54,238.31,2503.90 | 175,158,466 | Scale/Radius: 7.09 |
| 74 | `Junk_05` | 985 | Object | -565.20,714.88,2244.90 | 299,457,47 | Scale/Radius: 7.09 |
| 75 | `Junk_05` | 989 | Object | -1065.84,0.00,247.37 | 154,474,299 | Scale/Radius: 7.09 |
| 76 | `Junk_05` | 990 | Object | 399.12,-165.62,354.35 | 286,164,449 | Scale/Radius: 7.09 |
| 77 | `Junk_05` | 991 | Object | 1031.57,233.72,-17.99 | 78,449,239 | Scale/Radius: 7.09 |
| 78 | `Junk_05` | 992 | Object | 645.12,-111.77,594.60 | 499,30,439 | Scale/Radius: 7.09 |
| 79 | `Junk_05` | 995 | Object | 153.52,70.81,1696.38 | 141,427,360 | Scale/Radius: 7.09 |
| 80 | `Junk_05` | 996 | Object | -470.53,154.26,132.59 | 63,414,158 | Scale/Radius: 7.09 |
| 81 | `Junk_05` | 998 | Object | 347.06,194.13,1532.14 | 441,399,464 | Scale/Radius: 7.09 |
| 82 | `Junk_05` | 1106 | Object | -467.61,0.00,2557.25 | 30,158,299 | Scale/Radius: 7.09 |
| 83 | `Junk_05` | 1107 | Object | -524.64,278.68,1740.27 | 141,314,202 | Scale/Radius: 7.09 |
| 84 | `Junk_05` | 1108 | Object | 259.69,406.12,-154.57 | 390,266,107 | Scale/Radius: 7.09 |
| 85 | `Junk_04` | 1115 | Object | -106.64,109.34,393.47 | 0,101,0 | Scale/Radius: 5.24 |
| 86 | `Junk_04` | 999 | Object | 903.73,-174.86,1176.29 | 102,188,373 | Scale/Radius: 5.24 |
| 87 | `Junk_04` | 1000 | Object | -294.53,403.09,2055.13 | 125,16,363 | Scale/Radius: 5.24 |
| 88 | `Junk_04` | 1002 | Object | 59.13,-144.17,-55.82 | 442,329,31 | Scale/Radius: 5.24 |
| 89 | `Junk_04` | 1003 | Object | 1099.48,73.93,567.33 | 302,302,410 | Scale/Radius: 5.24 |
| 90 | `Junk_04` | 1004 | Object | 633.96,0.00,827.27 | 71,273,363 | Scale/Radius: 5.24 |
| 91 | `Junk_04` | 1005 | Object | 50.11,-102.84,2558.65 | 320,442,125 | Scale/Radius: 5.24 |
| 92 | `Junk_04` | 1007 | Object | 936.82,-133.64,1007.13 | 453,381,477 | Scale/Radius: 5.24 |
| 93 | `Junk_04` | 1110 | Object | 744.21,-535.45,2209.71 | 280,393,427 | Scale/Radius: 5.24 |
| 94 | `Junk_04` | 1111 | Object | 941.88,156.55,2700.12 | 169,67,141 | Scale/Radius: 5.24 |
| 95 | `Junk_04` | 1112 | Object | 1384.99,397.34,2387.57 | 141,110,156 | Scale/Radius: 5.24 |
| 96 | `Junk_04` | 1113 | Object | 1057.23,-174.55,1699.12 | 205,44,333 | Scale/Radius: 5.24 |
| 97 | `Junk_04` | 1114 | Object | -824.67,-77.27,1154.33 | 31,158,407 | Scale/Radius: 5.24 |
| 98 | `Junk_04` | 1116 | Object | 73.46,-68.66,199.55 | 316,63,442 | Scale/Radius: 5.24 |
| 99 | `Junk_05` | 1014 | Object | 208.42,572.73,1198.53 | 142,107,442 | Scale/Radius: 3.49 |
| 100 | `Junk_05` | 1008 | Object | -497.27,-96.20,2079.87 | 110,102,100 | Scale/Radius: 3.49 |
| 101 | `Junk_05` | 1009 | Object | -962.81,-384.30,1593.76 | 0,0,0 | Scale/Radius: 3.49 |
| 102 | `Junk_05` | 1011 | Object | -407.62,128.55,591.01 | 107,434,455 | Scale/Radius: 3.49 |
| 103 | `Junk_05` | 1013 | Object | 86.06,111.27,478.26 | 47,63,427 | Scale/Radius: 3.49 |
| 104 | `Junk_05` | 1117 | Object | 469.19,0.00,1774.46 | 142,284,441 | Scale/Radius: 3.49 |
| 105 | `Junk_05` | 1119 | Object | -854.52,73.19,1308.51 | 100,14,383 | Scale/Radius: 3.49 |
| 106 | `Junk_05` | 1120 | Object | -1034.85,-275.70,1392.49 | 309,55,486 | Scale/Radius: 3.49 |
| 107 | `Junk_05` | 1121 | Object | 471.53,-248.03,176.67 | 30,354,158 | Scale/Radius: 3.49 |
| 108 | `Junk_05` | 1122 | Object | 852.80,-285.62,255.47 | 499,202,215 | Scale/Radius: 3.49 |
| 109 | `Junk_04` | 967 | Object | -431.21,464.43,1933.16 | 405,91,432 | Scale/Radius: 10.00 |
| 110 | `Junk_04` | 950 | Object | -394.42,348.91,1318.07 | 427,78,415 | Scale/Radius: 10.00 |
| 111 | `Junk_04` | 964 | Object | 1619.37,-280.56,665.61 | 412,270,317 | Scale/Radius: 10.00 |
| 112 | `Junk_04` | 965 | Object | 524.99,185.95,-179.29 | 125,410,31 | Scale/Radius: 10.00 |
| 113 | `Junk_04` | 966 | Object | 1329.11,-183.47,2224.12 | 158,292,110 | Scale/Radius: 10.00 |
| 114 | `Spcargo_Art` | 1225 | Interactive | 1469.99,0.00,518.92 | 178,455,43 | secondary groups: CONT_061, none |
| 115 | `Spcargo_Contraband` | 1226 | Interactive | 1227.65,299.49,2583.34 | 0,0,0 | secondary groups: CONT_031, none |
| 116 | `Baron_Onrald_Station` | 896 | Interactive | -2045.68,0.00,-337.77 | 0,0,0 | None |
