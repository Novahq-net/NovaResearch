# Tachyon: The Fringe FRON10.SPX - Arena Gambit - Onrald's Champion; Arena Qualifier Round 2; Arena Tier I; Arena Tier II; Arena Tier III; Arena Tier IV; Arena Tier V; Arena Bonus Round

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON10.SPX` |
| Sector | `QUAD_10` |
| Backdrop | `FRONTI10.BDF` |
| Region | 4 |
| Sector ID | 9 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 9 |
| Entities | 351 |
| Events | 6 |
| Waypoints | 1 |
| Child Sectors | 2 |
| Scripts | 1 |
| Scenes | 1 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Mad_Pirate_Platform`, `1: Malkar_Station`, `2: Accelerator_Ring`, `3: Asteroid_1`, `4: Asteroid_2`, `5: Roid_Sm_Brown2`, `6: Roid_Sm_Brown`, `7: Ice_Roid_1`, `8: Hyper_Gate` |
| Scripts | `MALKR.SCR` |
| Scenes | `F10GC03A.SEN` |
| Labels | `Susan`, `BFGE_01`, `BFGE_1`, `Malkar1` |
| Aliases | `BC05_sistine_chapel`, `Susan Bradley` |
| Groups | None |
| Child Sectors | [fron10A.spx](FRON10A.md), [fron10B.spx](FRON10B.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1183; flags 6)
- Variable comparison: subject variable group 8, variable 24, op 1, value 1 (flags 4)

**Action**

- Play dialog: MALKR.SCR, line/variant 8
- Set/add variable: variable group 0, variable 2, subtype 1, value 1000
- Show/update HUD contact: contact/list 0, subtype 9, param 40
- Set/add variable: variable group 8, variable 24, subtype 0, value 0
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1183; flags 6)
- Variable comparison: subject variable group 8, variable 24, op 1, value 2 (flags 4)

**Action**

- Play dialog: MALKR.SCR, line/variant 8
- Set/add variable: variable group 0, variable 2, subtype 1, value 2000
- Show/update HUD contact: contact/list 0, subtype 9, param 40
- Set/add variable: variable group 8, variable 24, subtype 0, value 0
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1183; flags 6)
- Variable comparison: subject variable group 8, variable 24, op 1, value 3 (flags 4)

**Action**

- Play dialog: MALKR.SCR, line/variant 8
- Set/add variable: variable group 0, variable 2, subtype 1, value 3000
- Show/update HUD contact: contact/list 0, subtype 9, param 40
- Set/add variable: variable group 8, variable 24, subtype 0, value 0
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 1183; flags 6)
- Variable comparison: subject variable group 8, variable 24, op 2, value 3 (flags 4)

**Action**

- Play dialog: MALKR.SCR, line/variant 8
- Set/add variable: variable group 0, variable 2, subtype 1, value 4000
- Show/update HUD contact: contact/list 0, subtype 9, param 40
- Set/add variable: variable group 8, variable 24, subtype 0, value 0
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 32, op 2, value 10

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 40
- Set/add variable: variable group 20, variable 32, subtype 0, value 0

### Event 5

**Trigger**

- Variable comparison: subject variable group 21, variable 24, op 1, value 1
- Variable comparison: subject variable group 0, variable 4, op 1, value 3002

**Action**

- Group/spawn-list action: spawn list/group 117, subtype 4, param 1

## Waypoints

### Waypoint 0

- Tag: `3`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (816.20, -350.00, -2481.56) | None |
| 1 | (816.20, -1400.00, -1954.56) | None |
| 2 | (816.20, -1400.00, -103.38) | None |
| 3 | (816.20, -825.34, 123.45) | None |
| 4 | (816.20, -205.08, -282.25) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | -478.95,0.00,474.49 | 192,491,0 | Gate SPX: [fron11.spx](FRON11.md) |
| 1 | `Ice_Roid_1` | 83 | Object | -978.99,866.09,381.46 | 125,190,137 | Scale/Radius: 6.00 |
| 2 | `Roid_Sm_Brown` | 617 | Object | 1247.76,-346.44,1317.39 | 404,194,142 | Scale/Radius: 5.00 |
| 3 | `Roid_Sm_Brown2` | 622 | Object | -1200.47,577.40,30.00 | 293,472,414 | Scale/Radius: 1.00 |
| 4 | `Roid_Sm_Brown` | 625 | Object | 957.91,558.15,878.07 | 303,356,80 | Scale/Radius: 9.00 |
| 5 | `Roid_Sm_Brown2` | 630 | Object | 593.37,-19.25,1398.23 | 284,209,341 | Scale/Radius: 4.00 |
| 6 | `Roid_Sm_Brown` | 632 | Object | -1450.06,-384.93,290.42 | 504,149,32 | Scale/Radius: 3.00 |
| 7 | `Roid_Sm_Brown` | 640 | Object | -671.65,-904.59,1087.98 | 148,289,99 | Scale/Radius: 4.00 |
| 8 | `Roid_Sm_Brown` | 649 | Object | -671.65,115.48,1111.07 | 382,85,106 | Scale/Radius: 2.00 |
| 9 | `Roid_Sm_Brown` | 658 | Object | -1131.45,596.64,701.71 | 428,482,382 | Scale/Radius: 7.00 |
| 10 | `Roid_Sm_Brown2` | 663 | Object | -687.92,-538.90,580.35 | 124,468,263 | Scale/Radius: 5.00 |
| 11 | `Roid_Sm_Brown` | 667 | Object | 1266.91,866.09,547.11 | 428,305,229 | Scale/Radius: 2.00 |
| 12 | `Roid_Sm_Brown2` | 672 | Object | -1450.06,-211.71,163.40 | 414,300,21 | Scale/Radius: 6.00 |
| 13 | `Roid_Sm_Brown2` | 681 | Object | -423.01,-866.09,880.98 | 239,101,228 | Scale/Radius: 3.00 |
| 14 | `Roid_Sm_Brown` | 684 | Object | -61.01,-558.15,1201.91 | 454,234,436 | Scale/Radius: 8.00 |
| 15 | `Roid_Sm_Brown2` | 689 | Object | -363.71,-461.92,1018.69 | 9,313,314 | Scale/Radius: 7.00 |
| 16 | `Roid_Sm_Brown` | 693 | Object | -253.47,173.22,1421.32 | 69,18,278 | Scale/Radius: 3.00 |
| 17 | `Roid_Sm_Brown` | 700 | Object | -633.16,-827.60,1180.36 | 474,208,106 | Scale/Radius: 3.00 |
| 18 | `Roid_Sm_Brown` | 707 | Object | 362.42,346.44,1513.71 | 304,336,373 | Scale/Radius: 6.00 |
| 19 | `Roid_Sm_Brown2` | 719 | Object | -1161.98,692.87,18.45 | 140,317,443 | Scale/Radius: 8.00 |
| 20 | `Roid_Sm_Brown` | 722 | Object | -1229.19,-134.73,794.10 | 2,186,326 | Scale/Radius: 1.00 |
| 21 | `Roid_Sm_Brown` | 731 | Object | -253.47,692.87,1386.68 | 312,77,197 | Scale/Radius: 4.00 |
| 22 | `Roid_Sm_Brown2` | 736 | Object | 842.43,-346.44,1039.74 | 481,52,181 | Scale/Radius: 3.00 |
| 23 | `Roid_Sm_Brown` | 739 | Object | -234.32,885.34,1066.76 | 368,81,258 | Scale/Radius: 5.00 |
| 24 | `Roid_Sm_Brown2` | 744 | Object | 824.33,-423.42,1525.25 | 100,507,199 | Scale/Radius: 6.00 |
| 25 | `Roid_Sm_Brown` | 747 | Object | -368.95,-827.60,1190.36 | 227,22,101 | Scale/Radius: 7.00 |
| 26 | `Roid_Sm_Brown` | 751 | Object | -1893.66,-26.46,-1600.17 | 393,39,74 | Scale/Radius: 1.00 |
| 27 | `Roid_Sm_Brown` | 758 | Object | -1886.44,4.81,-1888.87 | 56,303,195 | Scale/Radius: 7.00 |
| 28 | `Roid_Sm_Brown2` | 763 | Object | -1872.48,-36.09,-1384.61 | 398,211,489 | Scale/Radius: 7.00 |
| 29 | `Roid_Sm_Brown` | 766 | Object | -1911.94,-81.80,-1677.15 | 364,86,481 | Scale/Radius: 1.00 |
| 30 | `Roid_Sm_Brown2` | 771 | Object | -1865.27,-43.30,-991.98 | 400,14,440 | Scale/Radius: 5.00 |
| 31 | `Ice_Roid_1` | 772 | Object | -1866.23,36.09,-1376.91 | 125,147,280 | Scale/Radius: 2.00 |
| 32 | `Roid_Sm_Brown` | 774 | Object | -1917.23,-134.73,-1307.62 | 149,116,139 | Scale/Radius: 6.00 |
| 33 | `Roid_Sm_Brown2` | 779 | Object | -1897.99,-185.25,-1338.41 | 203,128,294 | Scale/Radius: 3.00 |
| 34 | `Roid_Sm_Brown` | 781 | Object | -1900.87,-72.17,-1053.57 | 472,126,211 | Scale/Radius: 8.00 |
| 35 | `Roid_Sm_Brown2` | 786 | Object | -1891.25,-39.70,-1119.00 | 439,5,285 | Scale/Radius: 4.00 |
| 36 | `Asteroid_2` | 787 | Object | -1847.94,-133.52,-1338.41 | 506,356,486 | Scale/Radius: 2.00 |
| 37 | `Roid_Sm_Brown` | 790 | Object | -1865.27,-101.04,-1500.09 | 98,345,210 | Scale/Radius: 1.00 |
| 38 | `Roid_Sm_Brown2` | 795 | Object | -1872.48,292.31,-2112.12 | 468,17,505 | Scale/Radius: 3.00 |
| 39 | `Roid_Sm_Brown2` | 803 | Object | -1859.49,341.63,-1900.41 | 123,243,370 | Scale/Radius: 5.00 |
| 40 | `Asteroid_2` | 804 | Object | -1803.68,173.22,-1392.30 | 401,109,27 | Scale/Radius: 4.00 |
| 41 | `Roid_Sm_Brown` | 806 | Object | -2059.66,-259.83,-1885.02 | 266,101,271 | Scale/Radius: 6.00 |
| 42 | `Roid_Sm_Brown2` | 811 | Object | -1978.82,-43.30,-1900.41 | 286,173,278 | Scale/Radius: 7.00 |
| 43 | `Roid_Sm_Brown` | 815 | Object | -2012.98,276.67,-3035.96 | 3,154,314 | Scale/Radius: 9.00 |
| 44 | `Roid_Sm_Brown2` | 820 | Object | -486.79,30.07,-4022.45 | 240,413,148 | Scale/Radius: 5.00 |
| 45 | `Asteroid_1` | 821 | Object | -1818.11,-282.68,-610.90 | 305,270,194 | Scale/Radius: 7.00 |
| 46 | `Asteroid_2` | 822 | Object | -1892.69,-120.29,-360.69 | 382,395,282 | Scale/Radius: 1.00 |
| 47 | `Roid_Sm_Brown2` | 831 | Object | -2099.11,57.74,-1453.89 | 219,242,484 | Scale/Radius: 5.00 |
| 48 | `Roid_Sm_Brown` | 834 | Object | -2182.83,252.61,-891.90 | 300,445,180 | Scale/Radius: 9.00 |
| 49 | `Roid_Sm_Brown2` | 839 | Object | -1768.55,-303.13,24.24 | 178,150,497 | Scale/Radius: 7.00 |
| 50 | `Roid_Sm_Brown` | 842 | Object | -1622.76,163.60,-1376.91 | 370,45,474 | Scale/Radius: 2.00 |
| 51 | `Roid_Sm_Brown2` | 847 | Object | -1846.02,-153.97,-945.79 | 433,115,432 | Scale/Radius: 4.00 |
| 52 | `Ice_Roid_1` | 848 | Object | -1255.73,238.18,-270.34 | 79,132,222 | Scale/Radius: 4.00 |
| 53 | `Roid_Sm_Brown` | 851 | Object | -1882.59,-313.96,-2146.77 | 76,16,141 | Scale/Radius: 5.00 |
| 54 | `Roid_Sm_Brown2` | 856 | Object | -821.24,613.48,638.09 | 503,20,303 | Scale/Radius: 8.00 |
| 55 | `Roid_Sm_Brown` | 859 | Object | -1664.14,-601.45,-14.25 | 55,511,491 | Scale/Radius: 4.00 |
| 56 | `Roid_Sm_Brown2` | 864 | Object | -1905.20,13.23,-914.99 | 331,234,39 | Scale/Radius: 5.00 |
| 57 | `Roid_Sm_Brown2` | 872 | Object | -1517.96,922.63,-1254.15 | 438,360,186 | Scale/Radius: 5.00 |
| 58 | `Roid_Sm_Brown2` | 880 | Object | -1838.32,-866.09,-1530.88 | 12,413,253 | Scale/Radius: 3.00 |
| 59 | `Roid_Sm_Brown` | 882 | Object | -1883.55,-163.60,-2966.67 | 472,182,352 | Scale/Radius: 8.00 |
| 60 | `Roid_Sm_Brown2` | 887 | Object | -1625.65,-342.83,-1885.02 | 304,151,436 | Scale/Radius: 5.00 |
| 61 | `Asteroid_2` | 888 | Object | -975.21,-240.58,176.18 | 26,458,311 | Scale/Radius: 1.00 |
| 62 | `Roid_Sm_Brown` | 890 | Object | -2123.52,-820.38,-1238.55 | 227,415,204 | Scale/Radius: 9.00 |
| 63 | `Roid_Sm_Brown2` | 894 | Object | -1588.12,779.48,-3463.23 | 75,171,207 | Scale/Radius: 4.00 |
| 64 | `Roid_Sm_Brown2` | 900 | Object | -1965.35,-572.58,-414.58 | 176,75,162 | Scale/Radius: 4.00 |
| 65 | `Roid_Sm_Brown` | 902 | Object | -821.31,1390.35,955.19 | 287,104,260 | Scale/Radius: 3.00 |
| 66 | `Roid_Sm_Brown2` | 905 | Object | 1963.05,1174.79,-2023.95 | 271,423,399 | Scale/Radius: 3.00 |
| 67 | `Roid_Sm_Brown` | 906 | Object | 2655.92,1228.68,-1562.03 | 395,255,369 | Scale/Radius: 1.00 |
| 68 | `Roid_Sm_Brown2` | 909 | Object | -1174.29,1194.04,-231.76 | 271,354,5 | Scale/Radius: 8.00 |
| 69 | `Roid_Sm_Brown` | 913 | Object | 288.60,1101.66,-1100.11 | 113,362,83 | Scale/Radius: 4.00 |
| 70 | `Roid_Sm_Brown2` | 916 | Object | -981.67,1178.64,-2331.89 | 91,296,152 | Scale/Radius: 6.00 |
| 71 | `Roid_Sm_Brown` | 920 | Object | -231.05,1120.90,131.66 | 225,173,2 | Scale/Radius: 7.00 |
| 72 | `Roid_Sm_Brown2` | 923 | Object | -635.23,1244.08,-1177.10 | 173,346,315 | Scale/Radius: 9.00 |
| 73 | `Roid_Sm_Brown` | 926 | Object | 2598.18,1382.65,-1254.09 | 100,455,63 | Scale/Radius: 5.00 |
| 74 | `Roid_Sm_Brown2` | 929 | Object | -1154.89,1340.31,-4410.52 | 152,510,84 | Scale/Radius: 4.00 |
| 75 | `Roid_Sm_Brown2` | 933 | Object | -557.10,1421.15,584.11 | 311,401,272 | Scale/Radius: 3.00 |
| 76 | `Roid_Sm_Brown2` | 940 | Object | 635.04,1109.35,-1716.00 | 211,509,3 | Scale/Radius: 6.00 |
| 77 | `Roid_Sm_Brown2` | 946 | Object | -500.93,1436.54,831.34 | 388,120,205 | Scale/Radius: 3.00 |
| 78 | `Roid_Sm_Brown` | 951 | Object | 3175.58,1247.93,-1331.07 | 383,44,110 | Scale/Radius: 7.00 |
| 79 | `Roid_Sm_Brown2` | 954 | Object | 3348.80,1224.83,-638.20 | 397,144,241 | Scale/Radius: 2.00 |
| 80 | `Roid_Sm_Brown2` | 962 | Object | 1674.35,1324.91,-1177.10 | 209,149,103 | Scale/Radius: 3.00 |
| 81 | `Roid_Sm_Brown` | 964 | Object | 713.17,1117.05,1200.00 | 46,354,298 | Scale/Radius: 5.00 |
| 82 | `Roid_Sm_Brown` | 969 | Object | -1578.47,1078.56,-308.75 | 474,363,76 | Scale/Radius: 8.00 |
| 83 | `Roid_Sm_Brown2` | 972 | Object | -788.06,1317.22,353.15 | 184,471,393 | Scale/Radius: 9.00 |
| 84 | `Roid_Sm_Brown` | 975 | Object | -1058.81,1140.15,-3927.10 | 385,121,181 | Scale/Radius: 9.00 |
| 85 | `Roid_Sm_Brown2` | 978 | Object | 1616.61,1101.66,-407.24 | 103,194,308 | Scale/Radius: 9.00 |
| 86 | `Roid_Sm_Brown` | 986 | Object | 1501.13,1232.53,-484.23 | 210,160,99 | Scale/Radius: 2.00 |
| 87 | `Roid_Sm_Brown2` | 989 | Object | 2251.75,1363.41,-2100.93 | 196,191,336 | Scale/Radius: 4.00 |
| 88 | `Roid_Sm_Brown2` | 996 | Object | -1636.21,1336.46,-3388.19 | 387,454,497 | Scale/Radius: 5.00 |
| 89 | `Roid_Sm_Brown` | 999 | Object | 3233.32,1205.59,-1562.03 | 176,391,94 | Scale/Radius: 3.00 |
| 90 | `Roid_Sm_Brown2` | 1002 | Object | -404.27,1359.56,-407.24 | 247,229,397 | Scale/Radius: 4.00 |
| 91 | `Roid_Sm_Brown` | 1008 | Object | 2367.23,1274.87,-3409.70 | 507,4,427 | Scale/Radius: 5.00 |
| 92 | `Roid_Sm_Brown2` | 1011 | Object | 1983.44,1321.07,1123.01 | 354,412,169 | Scale/Radius: 5.00 |
| 93 | `Roid_Sm_Brown` | 1014 | Object | -879.05,1374.96,955.19 | 136,232,297 | Scale/Radius: 3.00 |
| 94 | `Roid_Sm_Brown2` | 1017 | Object | -1001.08,1271.02,76.18 | 295,135,365 | Scale/Radius: 4.00 |
| 95 | `Roid_Sm_Brown` | 1020 | Object | 1270.17,1136.30,670.57 | 256,354,192 | Scale/Radius: 3.00 |
| 96 | `Roid_Sm_Brown2` | 1023 | Object | 2194.01,1340.31,-792.17 | 274,72,34 | Scale/Radius: 4.00 |
| 97 | `Roid_Sm_Brown` | 1027 | Object | -499.37,1059.31,1200.00 | 150,123,477 | Scale/Radius: 7.00 |
| 98 | `Roid_Sm_Brown2` | 1030 | Object | 115.38,1409.60,-4564.49 | 295,261,244 | Scale/Radius: 3.00 |
| 99 | `Roid_Sm_Brown` | 1032 | Object | 1212.43,1120.90,-3332.71 | 298,342,141 | Scale/Radius: 5.00 |
| 100 | `Roid_Sm_Brown2` | 1035 | Object | 866.00,1097.81,-1792.99 | 269,258,153 | Scale/Radius: 4.00 |
| 101 | `Roid_Sm_Brown` | 1038 | Object | -970.45,1297.97,280.60 | 299,215,210 | Scale/Radius: 3.00 |
| 102 | `Roid_Sm_Brown` | 1043 | Object | 866.00,1336.46,-1792.99 | 64,400,366 | Scale/Radius: 6.00 |
| 103 | `Roid_Sm_Brown` | 1050 | Object | 1983.44,1398.05,738.08 | 419,133,508 | Scale/Radius: 5.00 |
| 104 | `Roid_Sm_Brown2` | 1053 | Object | -827.86,1090.11,-1771.48 | 167,484,88 | Scale/Radius: 8.00 |
| 105 | `Roid_Sm_Brown` | 1055 | Object | 1096.96,1259.48,-407.24 | 151,294,189 | Scale/Radius: 3.00 |
| 106 | `Roid_Sm_Brown2` | 1058 | Object | 2309.49,1124.75,-3717.64 | 465,473,380 | Scale/Radius: 2.00 |
| 107 | `Roid_Sm_Brown` | 1060 | Object | 346.34,1382.65,-1946.96 | 413,36,347 | Scale/Radius: 1.00 |
| 108 | `Roid_Sm_Brown2` | 1063 | Object | 1290.56,1074.71,1046.03 | 451,393,295 | Scale/Radius: 3.00 |
| 109 | `Roid_Sm_Brown` | 1067 | Object | 866.00,1205.59,362.62 | 82,435,134 | Scale/Radius: 9.00 |
| 110 | `Roid_Sm_Brown2` | 1070 | Object | 115.38,1290.27,-2177.92 | 467,296,137 | Scale/Radius: 8.00 |
| 111 | `Roid_Sm_Brown` | 1073 | Object | -1405.25,1374.96,-1771.48 | 251,101,189 | Scale/Radius: 2.00 |
| 112 | `Accelerator_Ring` | 1151 | Interactive | 916.46,-372.56,-1952.21 | 256,0,0 | None |
| 113 | `Accelerator_Ring` | 1152 | Interactive | 916.46,-372.56,-2002.21 | 256,0,0 | None |
| 114 | `Accelerator_Ring` | 1153 | Interactive | 916.46,-372.56,-2052.21 | 256,0,0 | None |
| 115 | `Accelerator_Ring` | 1154 | Interactive | 916.46,-372.56,-2102.21 | 256,0,0 | None |
| 116 | `Accelerator_Ring` | 1155 | Interactive | 916.46,-372.56,-2152.21 | 256,0,0 | None |
| 117 | `Accelerator_Ring` | 1157 | Interactive | 916.46,-372.56,-2202.21 | 256,0,0 | None |
| 118 | `Accelerator_Ring` | 1158 | Interactive | 916.46,-372.56,-2252.21 | 256,0,0 | None |
| 119 | `Accelerator_Ring` | 1159 | Interactive | 916.46,-372.56,-2302.21 | 256,0,0 | None |
| 120 | `Accelerator_Ring` | 1160 | Interactive | 916.46,-372.56,-2352.21 | 256,0,0 | None |
| 121 | `Accelerator_Ring` | 1161 | Interactive | 916.46,-372.56,-2402.21 | 256,0,0 | None |
| 122 | `Accelerator_Ring` | 1163 | Interactive | 916.46,-372.56,-2452.21 | 256,0,0 | None |
| 123 | `Accelerator_Ring` | 1164 | Interactive | 916.46,-372.56,-2502.21 | 256,0,0 | None |
| 124 | `Accelerator_Ring` | 1165 | Interactive | 916.46,-372.56,-2552.21 | 256,0,0 | None |
| 125 | `Accelerator_Ring` | 1167 | Interactive | 916.46,-372.56,-2602.21 | 256,0,0 | None |
| 126 | `Accelerator_Ring` | 1168 | Interactive | 916.46,-372.56,-2652.21 | 256,0,0 | None |
| 127 | `Accelerator_Ring` | 1169 | Interactive | 916.46,-372.56,-2702.21 | 256,0,0 | None |
| 128 | `Accelerator_Ring` | 1170 | Interactive | 916.46,-372.56,-2752.21 | 256,0,0 | None |
| 129 | `Accelerator_Ring` | 1172 | Interactive | 916.46,-372.56,-2802.21 | 256,0,0 | None |
| 130 | `Accelerator_Ring` | 1173 | Interactive | 916.46,-372.56,-2852.21 | 256,0,0 | None |
| 131 | `Accelerator_Ring` | 1174 | Interactive | 916.46,-372.56,-2902.21 | 256,0,0 | None |
| 132 | `Asteroid_2` | 942 | Object | 2251.75,1405.75,1209.47 | 210,247,80 | Scale/Radius: 10.00 |
| 133 | `Asteroid_2` | 35 | Object | -800.52,923.83,979.92 | 502,312,87 | Scale/Radius: 10.00 |
| 134 | `Asteroid_2` | 624 | Object | -1196.65,885.34,477.82 | 312,204,451 | Scale/Radius: 10.00 |
| 135 | `Asteroid_2` | 631 | Object | 611.47,-731.37,1062.84 | 257,348,306 | Scale/Radius: 10.00 |
| 136 | `Asteroid_2` | 639 | Object | -556.17,365.68,1168.81 | 340,280,402 | Scale/Radius: 10.00 |
| 137 | `Asteroid_2` | 648 | Object | 1709.67,346.44,1432.87 | 465,319,327 | Scale/Radius: 10.00 |
| 138 | `Asteroid_2` | 657 | Object | -556.17,230.96,1238.10 | 341,428,287 | Scale/Radius: 10.00 |
| 139 | `Asteroid_2` | 666 | Object | -253.47,-346.44,1490.61 | 203,384,105 | Scale/Radius: 10.00 |
| 140 | `Asteroid_2` | 675 | Object | 111.06,269.45,947.36 | 367,114,431 | Scale/Radius: 10.00 |
| 141 | `Asteroid_2` | 683 | Object | 862.83,-673.63,1421.32 | 77,501,436 | Scale/Radius: 10.00 |
| 142 | `Asteroid_2` | 699 | Object | 92.97,596.64,1536.80 | 455,149,159 | Scale/Radius: 10.00 |
| 143 | `Asteroid_2` | 706 | Object | -499.99,-846.85,904.08 | 427,436,354 | Scale/Radius: 10.00 |
| 144 | `Asteroid_2` | 713 | Object | -40.46,-615.89,945.71 | 400,315,222 | Scale/Radius: 10.00 |
| 145 | `Asteroid_2` | 721 | Object | 1209.26,-327.19,1213.46 | 380,213,245 | Scale/Radius: 10.00 |
| 146 | `Asteroid_2` | 730 | Object | -402.20,76.99,1445.96 | 486,208,285 | Scale/Radius: 10.00 |
| 147 | `Asteroid_2` | 746 | Object | -1488.56,808.35,-67.56 | 202,437,297 | Scale/Radius: 10.00 |
| 148 | `Asteroid_2` | 750 | Object | -1899.43,30.07,-1561.67 | 376,473,257 | Scale/Radius: 10.00 |
| 149 | `Asteroid_2` | 757 | Object | -1887.40,86.61,-1423.10 | 488,398,78 | Scale/Radius: 10.00 |
| 150 | `Asteroid_2` | 765 | Object | -1886.44,93.83,-1642.51 | 0,493,21 | Scale/Radius: 10.00 |
| 151 | `Asteroid_2` | 773 | Object | -1965.35,-64.96,-1638.66 | 401,14,505 | Scale/Radius: 10.00 |
| 152 | `Asteroid_2` | 780 | Object | -1831.59,45.71,-1623.26 | 107,395,474 | Scale/Radius: 10.00 |
| 153 | `Asteroid_2` | 789 | Object | -1917.23,-36.09,-1777.24 | 145,165,505 | Scale/Radius: 10.00 |
| 154 | `Asteroid_2` | 797 | Object | -1888.36,126.31,-1592.47 | 221,79,142 | Scale/Radius: 10.00 |
| 155 | `Asteroid_2` | 805 | Object | -1926.86,230.96,-1669.45 | 503,157,103 | Scale/Radius: 10.00 |
| 156 | `Asteroid_2` | 814 | Object | -1774.81,102.25,-1919.66 | 357,35,130 | Scale/Radius: 10.00 |
| 157 | `Asteroid_2` | 833 | Object | -872.24,-75.78,206.97 | 100,437,496 | Scale/Radius: 10.00 |
| 158 | `Asteroid_2` | 841 | Object | -2023.09,-134.73,-2393.12 | 72,405,260 | Scale/Radius: 10.00 |
| 159 | `Asteroid_2` | 858 | Object | -1659.33,-336.81,-861.10 | 16,197,178 | Scale/Radius: 10.00 |
| 160 | `Asteroid_2` | 866 | Object | -1738.24,519.66,-2701.07 | 431,466,133 | Scale/Radius: 10.00 |
| 161 | `Asteroid_2` | 874 | Object | -1899.91,-185.25,-3424.74 | 99,241,72 | Scale/Radius: 10.00 |
| 162 | `Asteroid_2` | 881 | Object | -1522.68,442.67,-2762.66 | 152,97,35 | Scale/Radius: 10.00 |
| 163 | `Asteroid_2` | 889 | Object | -1849.39,555.74,-3128.34 | 133,217,445 | Scale/Radius: 10.00 |
| 164 | `Asteroid_2` | 895 | Object | -1711.29,808.35,-3748.08 | 241,383,258 | Scale/Radius: 10.00 |
| 165 | `Asteroid_2` | 925 | Object | -1462.99,1309.52,307.14 | 407,414,331 | Scale/Radius: 10.00 |
| 166 | `Asteroid_2` | 936 | Object | 2136.27,1255.63,593.58 | 1,222,372 | Scale/Radius: 10.00 |
| 167 | `Asteroid_2` | 950 | Object | -57.84,1328.76,-2100.93 | 4,5,472 | Scale/Radius: 10.00 |
| 168 | `Asteroid_2` | 958 | Object | -346.53,1417.30,-99.30 | 179,449,182 | Scale/Radius: 10.00 |
| 169 | `Asteroid_2` | 1026 | Object | 886.38,1409.60,430.14 | 35,163,0 | Scale/Radius: 10.00 |
| 170 | `Asteroid_2` | 1059 | Object | 2136.27,1394.20,-2408.88 | 117,71,134 | Scale/Radius: 10.00 |
| 171 | `Asteroid_2` | 1066 | Object | 288.60,1309.52,-1485.05 | 100,50,291 | Scale/Radius: 10.00 |
| 172 | `Roid_Sm_Brown` | 992 | Object | 2424.97,1398.05,593.58 | 56,103,462 | Scale/Radius: 10.00 |
| 173 | `Roid_Sm_Brown` | 620 | Object | 303.53,384.93,1363.09 | 234,74,288 | Scale/Radius: 10.00 |
| 174 | `Roid_Sm_Brown` | 628 | Object | -368.95,615.89,1305.84 | 274,48,198 | Scale/Radius: 10.00 |
| 175 | `Roid_Sm_Brown` | 635 | Object | -582.22,-153.97,740.86 | 37,248,4 | Scale/Radius: 10.00 |
| 176 | `Roid_Sm_Brown` | 643 | Object | 1671.18,-673.63,1617.64 | 469,142,447 | Scale/Radius: 10.00 |
| 177 | `Roid_Sm_Brown` | 652 | Object | 1324.74,-404.18,1375.13 | 157,38,27 | Scale/Radius: 10.00 |
| 178 | `Roid_Sm_Brown` | 661 | Object | 1632.69,-211.71,1640.73 | 322,350,17 | Scale/Radius: 10.00 |
| 179 | `Roid_Sm_Brown` | 670 | Object | -1036.72,-173.22,724.81 | 122,311,417 | Scale/Radius: 10.00 |
| 180 | `Roid_Sm_Brown` | 679 | Object | 957.91,134.73,1074.39 | 125,478,337 | Scale/Radius: 10.00 |
| 181 | `Roid_Sm_Brown` | 687 | Object | -844.26,750.61,909.58 | 487,411,85 | Scale/Radius: 10.00 |
| 182 | `Roid_Sm_Brown` | 703 | Object | -1527.05,-76.99,232.68 | 233,224,36 | Scale/Radius: 10.00 |
| 183 | `Roid_Sm_Brown` | 710 | Object | -1131.45,134.73,320.63 | 491,386,165 | Scale/Radius: 10.00 |
| 184 | `Roid_Sm_Brown` | 717 | Object | -1246.93,-577.40,158.96 | 118,58,461 | Scale/Radius: 10.00 |
| 185 | `Roid_Sm_Brown` | 725 | Object | 285.43,673.63,1259.65 | 361,116,286 | Scale/Radius: 10.00 |
| 186 | `Roid_Sm_Brown` | 734 | Object | -1267.68,442.67,701.71 | 350,183,58 | Scale/Radius: 10.00 |
| 187 | `Roid_Sm_Brown` | 742 | Object | -998.23,19.25,805.64 | 178,79,113 | Scale/Radius: 10.00 |
| 188 | `Roid_Sm_Brown` | 754 | Object | -1931.19,33.68,-1430.80 | 52,499,393 | Scale/Radius: 10.00 |
| 189 | `Roid_Sm_Brown` | 761 | Object | -1904.24,7.22,-1646.36 | 46,421,395 | Scale/Radius: 10.00 |
| 190 | `Roid_Sm_Brown` | 769 | Object | -1917.23,-180.44,-1569.37 | 202,70,377 | Scale/Radius: 10.00 |
| 191 | `Roid_Sm_Brown` | 777 | Object | -1905.68,-55.33,-2223.75 | 373,125,345 | Scale/Radius: 10.00 |
| 192 | `Roid_Sm_Brown` | 793 | Object | -1840.73,61.35,-1338.41 | 267,105,480 | Scale/Radius: 10.00 |
| 193 | `Roid_Sm_Brown` | 801 | Object | -2065.43,-33.68,-1561.67 | 404,288,398 | Scale/Radius: 10.00 |
| 194 | `Roid_Sm_Brown` | 809 | Object | -2013.46,-269.45,-868.80 | 237,324,198 | Scale/Radius: 10.00 |
| 195 | `Roid_Sm_Brown` | 818 | Object | -1907.13,246.60,-687.88 | 434,238,202 | Scale/Radius: 10.00 |
| 196 | `Roid_Sm_Brown` | 837 | Object | -2000.95,429.44,-1834.97 | 70,152,505 | Scale/Radius: 10.00 |
| 197 | `Roid_Sm_Brown` | 862 | Object | -1910.50,-277.87,-1507.78 | 434,354,408 | Scale/Radius: 10.00 |
| 198 | `Roid_Sm_Brown` | 870 | Object | -1543.37,-344.03,-241.36 | 399,78,414 | Scale/Radius: 10.00 |
| 199 | `Roid_Sm_Brown` | 878 | Object | -1596.78,667.61,-784.11 | 161,24,421 | Scale/Radius: 10.00 |
| 200 | `Roid_Sm_Brown` | 885 | Object | -2101.39,476.35,-1153.86 | 500,260,410 | Scale/Radius: 10.00 |
| 201 | `Roid_Sm_Brown` | 912 | Object | -1058.81,1147.85,-2772.30 | 261,326,438 | Scale/Radius: 10.00 |
| 202 | `Roid_Sm_Brown` | 1025 | Object | 923.74,1244.08,285.63 | 400,19,447 | Scale/Radius: 10.00 |
| 203 | `Roid_Sm_Brown` | 1049 | Object | 1212.43,1213.28,-2023.95 | 345,111,413 | Scale/Radius: 10.00 |
| 204 | `Roid_Sm_Brown2` | 952 | Object | 1867.96,1093.96,1430.96 | 274,324,392 | Scale/Radius: 10.00 |
| 205 | `Roid_Sm_Brown2` | 13 | Object | -772.13,943.08,718.97 | 167,345,244 | Scale/Radius: 10.00 |
| 206 | `Roid_Sm_Brown2` | 69 | Object | -1371.97,962.33,665.46 | 131,255,144 | Scale/Radius: 10.00 |
| 207 | `Roid_Sm_Brown2` | 618 | Object | -1131.45,-96.23,251.34 | 99,212,466 | Scale/Radius: 10.00 |
| 208 | `Roid_Sm_Brown2` | 626 | Object | -402.20,-134.73,1053.33 | 473,267,244 | Scale/Radius: 10.00 |
| 209 | `Roid_Sm_Brown2` | 633 | Object | -1161.98,-827.60,572.75 | 229,98,123 | Scale/Radius: 10.00 |
| 210 | `Roid_Sm_Brown2` | 641 | Object | 362.42,-173.22,1652.28 | 352,249,19 | Scale/Radius: 10.00 |
| 211 | `Roid_Sm_Brown2` | 650 | Object | -1113.71,346.44,794.10 | 275,229,2 | Scale/Radius: 10.00 |
| 212 | `Roid_Sm_Brown2` | 668 | Object | -1362.41,654.38,551.59 | 405,204,16 | Scale/Radius: 10.00 |
| 213 | `Roid_Sm_Brown2` | 677 | Object | -4.42,230.96,1339.99 | 62,177,231 | Scale/Radius: 10.00 |
| 214 | `Roid_Sm_Brown2` | 685 | Object | -1411.57,-923.83,128.75 | 213,302,298 | Scale/Radius: 10.00 |
| 215 | `Roid_Sm_Brown2` | 694 | Object | 400.91,-654.38,1190.36 | 65,448,441 | Scale/Radius: 10.00 |
| 216 | `Roid_Sm_Brown2` | 701 | Object | 111.06,404.18,982.00 | 305,314,408 | Scale/Radius: 10.00 |
| 217 | `Roid_Sm_Brown2` | 708 | Object | 72.57,-481.16,982.00 | 358,357,293 | Scale/Radius: 10.00 |
| 218 | `Roid_Sm_Brown2` | 715 | Object | 1170.77,288.70,1190.36 | 313,414,125 | Scale/Radius: 10.00 |
| 219 | `Roid_Sm_Brown2` | 723 | Object | 1324.74,-692.87,1617.64 | 407,82,92 | Scale/Radius: 10.00 |
| 220 | `Roid_Sm_Brown2` | 740 | Object | -1161.98,-904.59,-120.12 | 390,355,229 | Scale/Radius: 10.00 |
| 221 | `Roid_Sm_Brown2` | 752 | Object | -1890.77,-48.12,-1831.13 | 85,76,322 | Scale/Radius: 10.00 |
| 222 | `Roid_Sm_Brown2` | 759 | Object | -1925.89,-8.42,-1619.41 | 235,323,432 | Scale/Radius: 10.00 |
| 223 | `Roid_Sm_Brown2` | 767 | Object | -1906.65,-60.15,-1557.83 | 71,154,47 | Scale/Radius: 10.00 |
| 224 | `Roid_Sm_Brown2` | 775 | Object | -1836.40,187.65,-1438.50 | 144,96,379 | Scale/Radius: 10.00 |
| 225 | `Roid_Sm_Brown2` | 782 | Object | -1835.43,146.75,-1592.47 | 66,127,431 | Scale/Radius: 10.00 |
| 226 | `Roid_Sm_Brown2` | 791 | Object | -1837.84,-50.52,-1465.44 | 415,256,126 | Scale/Radius: 10.00 |
| 227 | `Roid_Sm_Brown2` | 807 | Object | -1911.46,0.00,-2177.56 | 450,50,243 | Scale/Radius: 10.00 |
| 228 | `Roid_Sm_Brown2` | 835 | Object | -1758.45,25.26,-2212.21 | 123,247,110 | Scale/Radius: 10.00 |
| 229 | `Roid_Sm_Brown2` | 843 | Object | -1822.92,529.28,-1808.03 | 99,130,479 | Scale/Radius: 10.00 |
| 230 | `Roid_Sm_Brown2` | 852 | Object | -1674.73,281.48,-3393.94 | 75,253,403 | Scale/Radius: 10.00 |
| 231 | `Roid_Sm_Brown2` | 860 | Object | -1873.45,185.25,-3878.96 | 28,34,281 | Scale/Radius: 10.00 |
| 232 | `Roid_Sm_Brown2` | 868 | Object | -1971.48,418.61,-2424.13 | 496,265,396 | Scale/Radius: 10.00 |
| 233 | `Roid_Sm_Brown2` | 876 | Object | -1459.74,920.22,-491.99 | 476,72,436 | Scale/Radius: 10.00 |
| 234 | `Roid_Sm_Brown2` | 883 | Object | -2145.30,-347.64,-1854.22 | 434,444,501 | Scale/Radius: 10.00 |
| 235 | `Roid_Sm_Brown2` | 903 | Object | -808.45,1398.05,-2177.92 | 115,202,488 | Scale/Radius: 10.00 |
| 236 | `Roid_Sm_Brown2` | 907 | Object | -404.27,1409.60,-2870.79 | 373,158,346 | Scale/Radius: 10.00 |
| 237 | `Roid_Sm_Brown2` | 914 | Object | -1058.81,1321.07,-231.76 | 144,192,61 | Scale/Radius: 10.00 |
| 238 | `Roid_Sm_Brown2` | 938 | Object | -635.23,1190.19,-484.23 | 253,470,486 | Scale/Radius: 10.00 |
| 239 | `Roid_Sm_Brown2` | 960 | Object | 2482.71,1321.07,-3178.74 | 409,246,502 | Scale/Radius: 10.00 |
| 240 | `Roid_Sm_Brown2` | 965 | Object | -1615.39,1224.83,-3496.19 | 411,3,18 | Scale/Radius: 10.00 |
| 241 | `Roid_Sm_Brown2` | 976 | Object | 115.38,1170.94,-3178.74 | 91,286,438 | Scale/Radius: 10.00 |
| 242 | `Roid_Sm_Brown2` | 981 | Object | -1636.21,1394.20,-2387.37 | 113,277,238 | Scale/Radius: 10.00 |
| 243 | `Roid_Sm_Brown2` | 994 | Object | -1212.63,1097.81,-4410.52 | 37,17,72 | Scale/Radius: 10.00 |
| 244 | `Roid_Sm_Brown2` | 1000 | Object | 1501.13,1144.00,-1100.11 | 118,174,478 | Scale/Radius: 10.00 |
| 245 | `Roid_Sm_Brown2` | 1009 | Object | -1270.37,1382.65,-330.25 | 124,335,306 | Scale/Radius: 10.00 |
| 246 | `Roid_Sm_Brown2` | 1015 | Object | 461.82,1309.52,-4102.57 | 99,60,300 | Scale/Radius: 10.00 |
| 247 | `Roid_Sm_Brown2` | 1021 | Object | -620.28,1190.19,-3354.33 | 58,30,334 | Scale/Radius: 10.00 |
| 248 | `Roid_Sm_Brown2` | 1028 | Object | 635.04,1182.49,-2023.95 | 277,320,40 | Scale/Radius: 10.00 |
| 249 | `Roid_Sm_Brown2` | 1033 | Object | -288.79,1247.93,-1869.98 | 366,375,193 | Scale/Radius: 10.00 |
| 250 | `Roid_Sm_Brown2` | 1044 | Object | 1327.91,1432.70,-1023.13 | 460,115,476 | Scale/Radius: 10.00 |
| 251 | `Roid_Sm_Brown2` | 1051 | Object | 2194.01,1217.13,1286.45 | 182,223,97 | Scale/Radius: 10.00 |
| 252 | `Roid_Sm_Brown2` | 1056 | Object | -37.45,1105.50,584.11 | 36,144,306 | Scale/Radius: 10.00 |
| 253 | `Roid_Sm_Brown2` | 1074 | Object | -672.58,1182.49,199.18 | 378,287,179 | Scale/Radius: 10.00 |
| 254 | `Roid_Sm_Brown` | 1052 | Object | 1752.48,1278.72,892.05 | 167,147,415 | Scale/Radius: 10.00 |
| 255 | `Roid_Sm_Brown` | 627 | Object | -1323.92,-596.64,355.27 | 482,412,117 | Scale/Radius: 10.00 |
| 256 | `Roid_Sm_Brown` | 634 | Object | -1334.58,-654.38,-90.66 | 332,111,105 | Scale/Radius: 10.00 |
| 257 | `Roid_Sm_Brown` | 651 | Object | 824.33,-327.19,1236.56 | 351,280,459 | Scale/Radius: 10.00 |
| 258 | `Roid_Sm_Brown` | 678 | Object | -726.41,-538.90,603.45 | 322,148,49 | Scale/Radius: 10.00 |
| 259 | `Roid_Sm_Brown` | 686 | Object | 208.44,115.48,1606.09 | 194,11,430 | Scale/Radius: 10.00 |
| 260 | `Roid_Sm_Brown` | 695 | Object | 785.84,-885.34,1490.61 | 494,13,248 | Scale/Radius: 10.00 |
| 261 | `Roid_Sm_Brown` | 702 | Object | -764.90,-943.08,580.35 | 412,448,217 | Scale/Radius: 10.00 |
| 262 | `Roid_Sm_Brown` | 709 | Object | -1477.89,-943.08,470.75 | 334,415,15 | Scale/Radius: 10.00 |
| 263 | `Roid_Sm_Brown` | 724 | Object | -1180.61,0.00,82.56 | 421,159,353 | Scale/Radius: 10.00 |
| 264 | `Roid_Sm_Brown` | 733 | Object | 226.54,96.23,901.17 | 260,476,311 | Scale/Radius: 10.00 |
| 265 | `Roid_Sm_Brown` | 741 | Object | 1132.28,192.47,1594.54 | 331,484,135 | Scale/Radius: 10.00 |
| 266 | `Roid_Sm_Brown` | 753 | Object | -1889.32,31.28,-1781.08 | 497,432,366 | Scale/Radius: 10.00 |
| 267 | `Roid_Sm_Brown` | 760 | Object | -1890.77,40.90,-1696.40 | 330,337,129 | Scale/Radius: 10.00 |
| 268 | `Roid_Sm_Brown` | 776 | Object | -1900.87,-33.68,-1292.22 | 36,165,177 | Scale/Radius: 10.00 |
| 269 | `Roid_Sm_Brown` | 792 | Object | -1895.58,173.22,-2192.96 | 462,102,147 | Scale/Radius: 10.00 |
| 270 | `Roid_Sm_Brown` | 800 | Object | -1923.01,4.81,-1253.73 | 18,233,142 | Scale/Radius: 10.00 |
| 271 | `Roid_Sm_Brown` | 808 | Object | -2017.31,120.29,-1284.52 | 500,27,134 | Scale/Radius: 10.00 |
| 272 | `Roid_Sm_Brown` | 817 | Object | -1690.60,-66.16,-2073.63 | 266,71,31 | Scale/Radius: 10.00 |
| 273 | `Roid_Sm_Brown` | 828 | Object | -1934.55,368.09,-1315.32 | 338,286,272 | Scale/Radius: 10.00 |
| 274 | `Roid_Sm_Brown` | 836 | Object | -1987.48,-134.73,-541.61 | 273,360,214 | Scale/Radius: 10.00 |
| 275 | `Roid_Sm_Brown` | 853 | Object | -1899.91,-335.61,-2389.27 | 503,17,460 | Scale/Radius: 10.00 |
| 276 | `Roid_Sm_Brown` | 861 | Object | -1746.42,224.94,-1042.02 | 113,271,173 | Scale/Radius: 10.00 |
| 277 | `Roid_Sm_Brown` | 884 | Object | -2066.75,-433.05,-1708.16 | 92,360,173 | Scale/Radius: 10.00 |
| 278 | `Roid_Sm_Brown` | 898 | Object | -1323.00,-522.06,-3003.83 | 102,8,68 | Scale/Radius: 10.00 |
| 279 | `Roid_Sm_Brown` | 904 | Object | 230.86,1386.50,-561.21 | 165,11,51 | Scale/Radius: 10.00 |
| 280 | `Roid_Sm_Brown` | 915 | Object | -1097.15,1351.86,208.65 | 504,326,192 | Scale/Radius: 10.00 |
| 281 | `Roid_Sm_Brown` | 922 | Object | 1963.05,1301.82,-3024.77 | 369,365,9 | Scale/Radius: 10.00 |
| 282 | `Roid_Sm_Brown` | 928 | Object | 2540.44,1401.90,-3101.75 | 204,504,155 | Scale/Radius: 10.00 |
| 283 | `Roid_Sm_Brown` | 932 | Object | 1789.83,1344.16,-1408.06 | 430,45,408 | Scale/Radius: 10.00 |
| 284 | `Roid_Sm_Brown` | 945 | Object | 2156.65,1209.44,1353.97 | 449,362,328 | Scale/Radius: 10.00 |
| 285 | `Roid_Sm_Brown` | 953 | Object | 1154.69,1059.31,-330.25 | 101,84,2 | Scale/Radius: 10.00 |
| 286 | `Roid_Sm_Brown` | 961 | Object | 288.60,1093.96,-1254.09 | 284,227,483 | Scale/Radius: 10.00 |
| 287 | `Roid_Sm_Brown` | 966 | Object | 2424.97,1421.15,-2331.89 | 370,2,204 | Scale/Radius: 10.00 |
| 288 | `Roid_Sm_Brown` | 971 | Object | 1327.91,1232.53,-2639.84 | 396,254,450 | Scale/Radius: 10.00 |
| 289 | `Roid_Sm_Brown` | 982 | Object | 923.74,1328.76,901.52 | 63,345,88 | Scale/Radius: 10.00 |
| 290 | `Roid_Sm_Brown` | 988 | Object | 173.12,1355.71,-1716.00 | 177,48,146 | Scale/Radius: 10.00 |
| 291 | `Roid_Sm_Brown` | 995 | Object | 808.26,1067.01,-4333.53 | 189,81,285 | Scale/Radius: 10.00 |
| 292 | `Roid_Sm_Brown` | 1001 | Object | -1520.73,1294.12,-4466.00 | 11,25,384 | Scale/Radius: 10.00 |
| 293 | `Roid_Sm_Brown` | 1010 | Object | 1674.35,1251.78,-3101.75 | 384,103,366 | Scale/Radius: 10.00 |
| 294 | `Roid_Sm_Brown` | 1016 | Object | 3175.58,1297.97,-1716.00 | 317,242,299 | Scale/Radius: 10.00 |
| 295 | `Roid_Sm_Brown` | 1022 | Object | -1244.12,1409.60,407.25 | 352,383,294 | Scale/Radius: 10.00 |
| 296 | `Roid_Sm_Brown` | 1029 | Object | 1963.05,1182.49,-3717.64 | 506,65,3 | Scale/Radius: 10.00 |
| 297 | `Roid_Sm_Brown` | 1040 | Object | 692.78,1394.20,-2947.78 | 12,167,33 | Scale/Radius: 10.00 |
| 298 | `Roid_Sm_Brown` | 1045 | Object | 923.74,1178.64,-1485.05 | 95,64,250 | Scale/Radius: 10.00 |
| 299 | `Roid_Sm_Brown` | 1057 | Object | 3348.80,1290.27,-1716.00 | 207,262,38 | Scale/Radius: 10.00 |
| 300 | `Roid_Sm_Brown` | 1069 | Object | 577.30,1313.37,-2947.78 | 247,493,23 | Scale/Radius: 10.00 |
| 301 | `Roid_Sm_Brown` | 1075 | Object | 577.30,1271.02,362.62 | 399,77,119 | Scale/Radius: 10.00 |
| 302 | `Roid_Sm_Brown` | 655 | Object | 649.97,673.63,1005.10 | 234,252,27 | Scale/Radius: 10.00 |
| 303 | `Roid_Sm_Brown` | 638 | Object | -368.95,404.18,1271.20 | 461,4,274 | Scale/Radius: 10.00 |
| 304 | `Roid_Sm_Brown` | 673 | Object | -1334.58,558.15,186.49 | 374,461,474 | Scale/Radius: 10.00 |
| 305 | `Roid_Sm_Brown` | 737 | Object | 400.91,-635.14,1467.51 | 419,401,329 | Scale/Radius: 10.00 |
| 306 | `Roid_Sm_Brown` | 745 | Object | -882.75,346.44,609.33 | 136,156,69 | Scale/Radius: 10.00 |
| 307 | `Roid_Sm_Brown` | 849 | Object | -1653.07,43.30,-137.43 | 367,483,289 | Scale/Radius: 10.00 |
| 308 | `Roid_Sm_Brown` | 957 | Object | 1096.96,1186.34,-1023.13 | 477,299,218 | Scale/Radius: 10.00 |
| 309 | `Roid_Sm_Brown` | 985 | Object | -1751.69,1278.72,-4081.07 | 501,273,122 | Scale/Radius: 10.00 |
| 310 | `Roid_Sm_Brown` | 1019 | Object | -152.93,1263.33,661.10 | 464,48,217 | Scale/Radius: 10.00 |
| 311 | `Roid_Sm_Brown` | 1037 | Object | 1096.96,1309.52,-869.16 | 56,285,472 | Scale/Radius: 10.00 |
| 312 | `Roid_Sm_Brown` | 1065 | Object | -1328.11,1440.39,-792.17 | 159,344,159 | Scale/Radius: 10.00 |
| 313 | `Roid_Sm_Brown2` | 664 | Object | 495.99,558.15,820.33 | 469,210,24 | Scale/Radius: 10.00 |
| 314 | `Roid_Sm_Brown2` | 647 | Object | -440.69,-404.18,1111.07 | 123,356,226 | Scale/Radius: 10.00 |
| 315 | `Roid_Sm_Brown2` | 674 | Object | -1488.56,423.42,-148.40 | 495,182,333 | Scale/Radius: 10.00 |
| 316 | `Roid_Sm_Brown2` | 720 | Object | -773.22,885.34,396.98 | 13,453,187 | Scale/Radius: 10.00 |
| 317 | `Roid_Sm_Brown2` | 823 | Object | -1637.20,79.39,-1869.62 | 398,461,173 | Scale/Radius: 10.00 |
| 318 | `Roid_Sm_Brown2` | 924 | Object | -115.58,1278.72,1132.48 | 76,502,497 | Scale/Radius: 10.00 |
| 319 | `Roid_Sm_Brown2` | 934 | Object | -1328.11,1274.87,439.61 | 280,459,110 | Scale/Radius: 10.00 |
| 320 | `Roid_Sm_Brown2` | 968 | Object | -692.97,1328.76,-2331.89 | 258,336,330 | Scale/Radius: 10.00 |
| 321 | `Roid_Sm_Brown2` | 1003 | Object | -1270.37,1190.19,-1408.06 | 414,187,236 | Scale/Radius: 10.00 |
| 322 | `Roid_Sm_Brown2` | 1012 | Object | 981.48,1348.01,-1946.96 | 149,69,285 | Scale/Radius: 10.00 |
| 323 | `Asteroid_2` | 998 | Object | 57.64,1059.31,-1177.10 | 185,226,357 | Scale/Radius: 1.00 |
| 324 | `Asteroid_2` | 623 | Object | -40.46,-943.08,1038.10 | 180,113,320 | Scale/Radius: 1.00 |
| 325 | `Asteroid_2` | 656 | Object | -214.98,-38.49,1352.04 | 233,298,398 | Scale/Radius: 1.00 |
| 326 | `Asteroid_2` | 665 | Object | 901.32,230.96,1548.35 | 218,500,24 | Scale/Radius: 1.00 |
| 327 | `Asteroid_2` | 682 | Object | 149.56,-269.45,1016.65 | 412,176,346 | Scale/Radius: 1.00 |
| 328 | `Asteroid_2` | 691 | Object | -1631.86,423.42,158.96 | 157,244,287 | Scale/Radius: 1.00 |
| 329 | `Asteroid_2` | 729 | Object | 534.49,230.96,1201.42 | 434,50,250 | Scale/Radius: 1.00 |
| 330 | `Asteroid_2` | 764 | Object | -1922.04,86.61,-1546.28 | 142,176,293 | Scale/Radius: 1.00 |
| 331 | `Asteroid_2` | 788 | Object | -2002.40,108.26,-1823.43 | 497,487,257 | Scale/Radius: 1.00 |
| 332 | `Asteroid_2` | 796 | Object | -1901.35,-122.70,-2516.30 | 203,8,206 | Scale/Radius: 1.00 |
| 333 | `Asteroid_2` | 813 | Object | -1837.36,66.16,-322.20 | 241,430,166 | Scale/Radius: 1.00 |
| 334 | `Asteroid_2` | 824 | Object | -1816.19,-223.74,-3186.08 | 73,222,361 | Scale/Radius: 1.00 |
| 335 | `Asteroid_2` | 832 | Object | -1862.38,-512.44,-1015.07 | 329,400,164 | Scale/Radius: 1.00 |
| 336 | `Asteroid_2` | 840 | Object | -1872.97,126.31,-1269.13 | 343,358,235 | Scale/Radius: 1.00 |
| 337 | `Asteroid_2` | 857 | Object | -826.05,96.23,445.63 | 80,507,24 | Scale/Radius: 1.00 |
| 338 | `Asteroid_2` | 873 | Object | -2073.48,-471.54,-984.49 | 38,336,68 | Scale/Radius: 1.00 |
| 339 | `Asteroid_2` | 910 | Object | -37.45,1251.78,1123.01 | 211,362,170 | Scale/Radius: 1.00 |
| 340 | `Asteroid_2` | 918 | Object | 1732.09,1297.97,-253.27 | 477,168,226 | Scale/Radius: 1.00 |
| 341 | `Asteroid_2` | 948 | Object | 1154.69,1274.87,-1946.96 | 277,145,10 | Scale/Radius: 1.00 |
| 342 | `Asteroid_2` | 955 | Object | -1751.69,1386.50,-770.67 | 322,439,283 | Scale/Radius: 1.00 |
| 343 | `Asteroid_2` | 963 | Object | -462.01,1194.04,-1639.02 | 221,218,163 | Scale/Radius: 1.00 |
| 344 | `Asteroid_2` | 973 | Object | -1578.47,1132.45,-2695.32 | 412,128,251 | Scale/Radius: 1.00 |
| 345 | `Asteroid_2` | 984 | Object | 2886.88,1213.28,-2177.92 | 417,381,305 | Scale/Radius: 1.00 |
| 346 | `Asteroid_2` | 990 | Object | -1232.03,1209.44,-2079.43 | 175,253,322 | Scale/Radius: 1.00 |
| 347 | `Asteroid_2` | 1004 | Object | -635.23,1090.11,-2177.92 | 76,295,482 | Scale/Radius: 1.00 |
| 348 | `Asteroid_2` | 1071 | Object | 1789.83,1078.56,208.65 | 467,383,269 | Scale/Radius: 1.00 |
| 349 | `Malkar_Station` | 1076 | Interactive | 917.89,-831.73,-283.21 | 0,0,0 | None |
| 350 | `Mad_Pirate_Platform` | 1183 | Interactive | 917.84,-498.56,-1489.60 | 0,0,0 | None |
