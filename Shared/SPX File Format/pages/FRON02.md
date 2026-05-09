# Tachyon: The Fringe FRON02.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON02.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `FRONTI2.BDF` |
| Region | 4 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 7 |
| Entities | 207 |
| Events | 8 |
| Waypoints | 0 |
| Child Sectors | 1 |
| Scripts | 1 |
| Scenes | 1 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Armon_Patroli_Black_Market_Ship`, `1: Asteroid_2`, `2: Roid_XL_Green`, `3: Roid_Sm_Brown2`, `4: Roid_Sm_Brown`, `5: Mega_Gate`, `6: Hyper_Gate` |
| Scripts | `ARMAN.SCR` |
| Scenes | `F2GC030A.SEN` |
| Labels | `SPIKE`, `Arman` |
| Aliases | `Arman` |
| Groups | `OPPORTUNITY`, `CONT_062` |
| Child Sectors | [fron02A.spx](FRON02A.md) |

## Events

### Event 0

**Trigger**

- Object event: subject Armon_Patroli_Black_Market_Ship (object 206, id 265), op 0, value 0 (flags 2)
- Variable comparison: subject variable group 16, variable 418, op 0, value 1

**Action**

- Play dialog: ARMAN.SCR, line/variant 4

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 265; flags 6)
- Variable comparison: subject variable group 8, variable 26, op 1, value 1 (flags 4)

**Action**

- Play dialog: ARMAN.SCR, line/variant 8
- Set/add variable: variable group 0, variable 2, subtype 1, value 850
- Set/add variable: variable group 8, variable 26, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 40
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 265; flags 6)
- Variable comparison: subject variable group 8, variable 26, op 1, value 2 (flags 4)

**Action**

- Play dialog: ARMAN.SCR, line/variant 8
- Set/add variable: variable group 0, variable 2, subtype 1, value 1700
- Set/add variable: variable group 8, variable 26, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 40
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 265; flags 6)
- Variable comparison: subject variable group 8, variable 26, op 1, value 3 (flags 4)

**Action**

- Play dialog: ARMAN.SCR, line/variant 8
- Set/add variable: variable group 0, variable 2, subtype 1, value 2550
- Set/add variable: variable group 8, variable 26, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 40
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 265; flags 6)
- Variable comparison: subject variable group 8, variable 26, op 1, value 4 (flags 4)

**Action**

- Play dialog: ARMAN.SCR, line/variant 8
- Set/add variable: variable group 0, variable 2, subtype 1, value 3400
- Set/add variable: variable group 8, variable 26, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 40
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 265; flags 6)
- Variable comparison: subject variable group 8, variable 26, op 2, value 4 (flags 4)

**Action**

- Play dialog: ARMAN.SCR, line/variant 8
- Set/add variable: variable group 0, variable 2, subtype 1, value 4250
- Set/add variable: variable group 8, variable 26, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 40
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 32, op 2, value 10 (flags 4)

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 40
- Set/add variable: variable group 20, variable 32, subtype 0, value 0

### Event 7

**Trigger**

- Variable comparison: subject variable group 0, variable 4, op 1, value 3002

**Action**

- Object spawn/action: Armon_Patroli_Black_Market_Ship (object 206, id 265), subtype 19

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | -1488.67,0.00,1434.73 | 192,0,0 | Gate SPX: [fron01.spx](FRON01.md) |
| 1 | `Mega_Gate` | 2 | Gate | 7.53,1396.40,-2155.04 | 0,469,384 | Gate SPX: [myst06.spx](MYST06.md) |
| 2 | `Roid_Sm_Brown` | 48 | Object | -2694.51,-2017.94,-2617.53 | 502,62,116 | Scale/Radius: 10.00 |
| 3 | `Roid_Sm_Brown2` | 53 | Object | 230.96,60.68,692.87 | 23,125,332 | Scale/Radius: 10.00 |
| 4 | `Roid_Sm_Brown` | 56 | Object | 2925.47,291.64,-769.86 | 415,90,36 | Scale/Radius: 10.00 |
| 5 | `Roid_Sm_Brown2` | 61 | Object | -3387.39,2909.17,-384.93 | 234,158,393 | Scale/Radius: 10.00 |
| 6 | `Roid_XL_Green` | 63 | Object | -2925.47,1677.39,-1924.65 | 182,353,358 | Scale/Radius: 1.00 |
| 7 | `Roid_Sm_Brown` | 65 | Object | 230.96,1600.40,-3387.39 | 313,228,190 | Scale/Radius: 10.00 |
| 8 | `Roid_Sm_Brown2` | 70 | Object | -2837.37,-2864.79,-757.01 | 159,396,374 | Scale/Radius: 10.00 |
| 9 | `Roid_Sm_Brown` | 73 | Object | -2694.51,-1017.12,-1847.67 | 236,29,393 | Scale/Radius: 10.00 |
| 10 | `Roid_Sm_Brown2` | 78 | Object | 3695.33,2370.26,76.99 | 117,22,406 | Scale/Radius: 10.00 |
| 11 | `Asteroid_2` | 80 | Object | -1616.71,-478.22,-3464.37 | 349,169,4 | Scale/Radius: 10.00 |
| 12 | `Roid_Sm_Brown` | 83 | Object | 1924.65,2062.32,1924.65 | 99,425,117 | Scale/Radius: 10.00 |
| 13 | `Roid_Sm_Brown2` | 88 | Object | 2463.55,3602.04,3387.39 | 43,392,373 | Scale/Radius: 10.00 |
| 14 | `Asteroid_2` | 89 | Object | 2771.50,-2787.80,-2925.47 | 85,505,18 | Scale/Radius: 10.00 |
| 15 | `Roid_XL_Green` | 90 | Object | -1770.68,3140.12,1385.75 | 202,19,511 | Scale/Radius: 1.00 |
| 16 | `Roid_Sm_Brown` | 92 | Object | -3310.40,-1940.96,-769.86 | 112,8,14 | Scale/Radius: 10.00 |
| 17 | `Roid_Sm_Brown2` | 97 | Object | 461.92,2909.17,-2155.61 | 149,274,435 | Scale/Radius: 10.00 |
| 18 | `Roid_XL_Green` | 100 | Object | 615.89,1138.49,-384.93 | 159,376,176 | Scale/Radius: 2.00 |
| 19 | `Roid_Sm_Brown` | 102 | Object | -1924.65,368.63,2078.62 | 423,128,11 | Scale/Radius: 10.00 |
| 20 | `Roid_Sm_Brown2` | 107 | Object | -1462.74,-170.28,3002.46 | 155,368,111 | Scale/Radius: 10.00 |
| 21 | `Roid_Sm_Brown` | 111 | Object | -76.99,-2094.93,3002.46 | 262,443,250 | Scale/Radius: 10.00 |
| 22 | `Roid_Sm_Brown2` | 116 | Object | 2463.55,1446.43,-769.86 | 338,408,369 | Scale/Radius: 10.00 |
| 23 | `Roid_Sm_Brown` | 118 | Object | 230.96,4063.96,-3387.39 | 378,409,283 | Scale/Radius: 10.00 |
| 24 | `Roid_Sm_Brown2` | 123 | Object | -384.93,3909.99,-3233.42 | 455,289,325 | Scale/Radius: 10.00 |
| 25 | `Asteroid_2` | 124 | Object | 2309.58,4217.93,-2155.61 | 61,158,268 | Scale/Radius: 10.00 |
| 26 | `Roid_XL_Green` | 125 | Object | 3233.42,-2171.91,-692.87 | 445,310,406 | Scale/Radius: 2.00 |
| 27 | `Roid_Sm_Brown` | 127 | Object | 3156.43,4448.89,384.93 | 113,136,355 | Scale/Radius: 10.00 |
| 28 | `Roid_Sm_Brown2` | 132 | Object | -230.96,1600.40,3156.43 | 135,24,395 | Scale/Radius: 10.00 |
| 29 | `Roid_Sm_Brown` | 136 | Object | 1385.75,-3095.75,2925.47 | 382,395,143 | Scale/Radius: 10.00 |
| 30 | `Roid_Sm_Brown2` | 141 | Object | -846.85,2216.29,-1308.76 | 161,101,309 | Scale/Radius: 10.00 |
| 31 | `Roid_Sm_Brown` | 145 | Object | -3695.33,1523.42,-1462.74 | 24,173,362 | Scale/Radius: 10.00 |
| 32 | `Roid_Sm_Brown2` | 150 | Object | 1077.81,4140.94,3695.33 | 200,163,59 | Scale/Radius: 10.00 |
| 33 | `Roid_XL_Green` | 151 | Object | 2309.58,-709.18,1308.76 | 156,319,0 | Scale/Radius: 3.00 |
| 34 | `Roid_Sm_Brown` | 153 | Object | -461.92,1292.46,1077.81 | 219,11,259 | Scale/Radius: 10.00 |
| 35 | `Roid_Sm_Brown2` | 158 | Object | 3233.42,445.61,-2078.62 | 273,91,504 | Scale/Radius: 10.00 |
| 36 | `Roid_Sm_Brown` | 160 | Object | 461.92,-1325.07,2463.55 | 487,467,174 | Scale/Radius: 10.00 |
| 37 | `Roid_Sm_Brown2` | 165 | Object | -923.83,-2017.94,3618.35 | 198,299,403 | Scale/Radius: 10.00 |
| 38 | `Asteroid_2` | 167 | Object | -1847.67,-2787.80,-76.99 | 195,43,46 | Scale/Radius: 10.00 |
| 39 | `Roid_Sm_Brown` | 170 | Object | -1154.79,3602.04,1154.79 | 469,185,117 | Scale/Radius: 10.00 |
| 40 | `Roid_Sm_Brown2` | 175 | Object | -3849.30,2062.32,-923.83 | 7,2,291 | Scale/Radius: 10.00 |
| 41 | `Asteroid_2` | 176 | Object | 692.87,-2787.80,923.83 | 356,350,480 | Scale/Radius: 10.00 |
| 42 | `Roid_Sm_Brown` | 178 | Object | 1154.79,2524.24,384.93 | 476,73,266 | Scale/Radius: 10.00 |
| 43 | `Roid_Sm_Brown2` | 183 | Object | -1000.82,2216.29,-3387.39 | 449,229,161 | Scale/Radius: 10.00 |
| 44 | `Roid_XL_Green` | 185 | Object | -1847.67,2524.24,1308.76 | 210,35,357 | Scale/Radius: 2.00 |
| 45 | `Roid_Sm_Brown` | 187 | Object | 2001.64,-1710.00,3541.36 | 6,181,245 | Scale/Radius: 10.00 |
| 46 | `Roid_Sm_Brown2` | 192 | Object | 538.90,-2710.82,-923.83 | 510,378,372 | Scale/Radius: 10.00 |
| 47 | `Roid_Sm_Brown` | 196 | Object | 3772.32,1985.33,-461.92 | 256,79,28 | Scale/Radius: 10.00 |
| 48 | `Roid_Sm_Brown2` | 201 | Object | 1770.68,-93.29,1154.79 | 381,6,18 | Scale/Radius: 10.00 |
| 49 | `Roid_Sm_Brown` | 203 | Object | 153.97,-940.14,384.93 | 322,160,40 | Scale/Radius: 10.00 |
| 50 | `Roid_Sm_Brown2` | 208 | Object | 1077.81,445.61,3002.46 | 237,310,66 | Scale/Radius: 10.00 |
| 51 | `Asteroid_2` | 209 | Object | 1693.69,4525.87,3464.37 | 368,336,467 | Scale/Radius: 10.00 |
| 52 | `Roid_XL_Green` | 210 | Object | 1385.75,522.60,-769.86 | 370,118,472 | Scale/Radius: 1.00 |
| 53 | `Roid_Sm_Brown` | 212 | Object | 692.87,2832.18,-615.89 | 165,108,231 | Scale/Radius: 10.00 |
| 54 | `Roid_Sm_Brown2` | 217 | Object | -1770.68,2986.15,2232.60 | 298,18,257 | Scale/Radius: 10.00 |
| 55 | `Asteroid_2` | 218 | Object | -3772.32,4525.87,-846.85 | 450,297,43 | Scale/Radius: 10.00 |
| 56 | `Roid_XL_Green` | 219 | Object | -2232.60,-1402.05,846.85 | 371,471,485 | Scale/Radius: 2.00 |
| 57 | `Roid_Sm_Brown` | 221 | Object | 384.93,-2633.83,-3541.36 | 466,456,331 | Scale/Radius: 10.00 |
| 58 | `Roid_Sm_Brown2` | 226 | Object | 158.27,4140.94,221.02 | 486,388,267 | Scale/Radius: 10.00 |
| 59 | `Roid_Sm_Brown` | 228 | Object | -692.87,-2787.80,-3233.42 | 180,449,142 | Scale/Radius: 10.00 |
| 60 | `Roid_Sm_Brown2` | 233 | Object | 2617.53,1600.40,-384.93 | 258,500,285 | Scale/Radius: 10.00 |
| 61 | `Roid_Sm_Brown` | 236 | Object | 692.87,3833.00,3464.37 | 25,217,242 | Scale/Radius: 10.00 |
| 62 | `Roid_Sm_Brown2` | 241 | Object | -2001.64,2986.15,-1308.76 | 377,224,152 | Scale/Radius: 10.00 |
| 63 | `Roid_Sm_Brown` | 243 | Object | 230.96,3371.08,-3002.46 | 145,351,340 | Scale/Radius: 10.00 |
| 64 | `Roid_Sm_Brown2` | 248 | Object | -538.90,3525.06,-769.86 | 423,162,188 | Scale/Radius: 10.00 |
| 65 | `Roid_Sm_Brown` | 250 | Object | -1308.76,3371.08,2463.55 | 129,304,61 | Scale/Radius: 10.00 |
| 66 | `Asteroid_2` | 52 | Object | 3397.91,4207.68,-3024.27 | 140,96,171 | Scale/Radius: 10.00 |
| 67 | `Asteroid_2` | 60 | Object | 2551.06,127.42,671.06 | 332,498,465 | Scale/Radius: 10.00 |
| 68 | `Asteroid_2` | 69 | Object | -682.36,3129.88,2133.79 | 78,178,384 | Scale/Radius: 10.00 |
| 69 | `Asteroid_2` | 77 | Object | 1935.17,2513.99,2980.64 | 248,112,170 | Scale/Radius: 10.00 |
| 70 | `Asteroid_2` | 87 | Object | 1781.20,1051.25,-1946.47 | 220,98,321 | Scale/Radius: 10.00 |
| 71 | `Asteroid_2` | 96 | Object | -3684.81,50.43,132.15 | 145,184,232 | Scale/Radius: 10.00 |
| 72 | `Asteroid_2` | 106 | Object | 2166.13,4053.71,3442.56 | 280,344,359 | Scale/Radius: 10.00 |
| 73 | `Asteroid_2` | 115 | Object | -451.40,589.34,3057.63 | 27,142,319 | Scale/Radius: 10.00 |
| 74 | `Asteroid_2` | 122 | Object | 3474.89,1128.24,-560.72 | 226,203,286 | Scale/Radius: 10.00 |
| 75 | `Asteroid_2` | 131 | Object | -451.40,1667.14,-1715.51 | 433,364,306 | Scale/Radius: 10.00 |
| 76 | `Asteroid_2` | 140 | Object | -2453.04,127.42,2903.65 | 426,453,198 | Scale/Radius: 10.00 |
| 77 | `Asteroid_2` | 149 | Object | -2760.98,358.38,-2408.39 | 73,333,171 | Scale/Radius: 10.00 |
| 78 | `Asteroid_2` | 157 | Object | 3300.39,4053.71,2277.38 | 346,431,245 | Scale/Radius: 10.00 |
| 79 | `Asteroid_2` | 164 | Object | -1221.26,3899.74,2903.65 | 26,10,212 | Scale/Radius: 10.00 |
| 80 | `Asteroid_2` | 174 | Object | 2166.13,-1027.37,55.17 | 261,320,91 | Scale/Radius: 10.00 |
| 81 | `Asteroid_2` | 182 | Object | 1242.30,1282.21,517.08 | 435,263,321 | Scale/Radius: 10.00 |
| 82 | `Asteroid_2` | 191 | Object | -3761.80,4438.64,1055.99 | 505,424,476 | Scale/Radius: 10.00 |
| 83 | `Asteroid_2` | 200 | Object | 2166.13,-1104.36,1671.88 | 12,286,388 | Scale/Radius: 10.00 |
| 84 | `Asteroid_2` | 207 | Object | 2859.00,-1797.23,1748.86 | 226,163,302 | Scale/Radius: 10.00 |
| 85 | `Asteroid_2` | 216 | Object | -3299.88,-873.40,-1099.62 | 375,42,358 | Scale/Radius: 10.00 |
| 86 | `Asteroid_2` | 225 | Object | -2222.08,-2721.06,-3409.21 | 79,189,181 | Scale/Radius: 10.00 |
| 87 | `Asteroid_2` | 232 | Object | -2837.97,358.38,-2716.33 | 450,206,295 | Scale/Radius: 10.00 |
| 88 | `Asteroid_2` | 240 | Object | 3705.85,1513.17,-868.66 | 134,382,344 | Scale/Radius: 10.00 |
| 89 | `Asteroid_2` | 247 | Object | 3012.97,589.34,-1946.47 | 237,445,213 | Scale/Radius: 10.00 |
| 90 | `Roid_Sm_Brown` | 85 | Object | 3772.32,-1248.08,-2540.54 | 320,493,470 | Scale/Radius: 10.00 |
| 91 | `Roid_Sm_Brown` | 50 | Object | 307.94,445.61,-2386.57 | 131,447,90 | Scale/Radius: 10.00 |
| 92 | `Roid_Sm_Brown` | 58 | Object | 1077.81,907.53,-2078.62 | 256,94,308 | Scale/Radius: 10.00 |
| 93 | `Roid_Sm_Brown` | 67 | Object | 1924.65,-1863.97,-2617.53 | 419,270,97 | Scale/Radius: 10.00 |
| 94 | `Roid_Sm_Brown` | 75 | Object | -615.89,291.64,1693.69 | 477,64,83 | Scale/Radius: 10.00 |
| 95 | `Roid_Sm_Brown` | 94 | Object | 1770.68,4525.87,-3156.43 | 122,490,123 | Scale/Radius: 10.00 |
| 96 | `Roid_Sm_Brown` | 104 | Object | -2771.50,-1786.98,-1770.68 | 8,374,157 | Scale/Radius: 10.00 |
| 97 | `Roid_Sm_Brown` | 113 | Object | 3156.43,-2171.91,-1847.67 | 72,462,470 | Scale/Radius: 10.00 |
| 98 | `Roid_Sm_Brown` | 120 | Object | -2760.39,1138.49,-757.01 | 200,365,161 | Scale/Radius: 10.00 |
| 99 | `Roid_Sm_Brown` | 129 | Object | -846.85,-555.21,-2925.47 | 106,290,222 | Scale/Radius: 10.00 |
| 100 | `Roid_Sm_Brown` | 138 | Object | 3772.32,60.68,1231.78 | 236,350,370 | Scale/Radius: 10.00 |
| 101 | `Roid_Sm_Brown` | 147 | Object | -1924.65,4063.96,3156.43 | 462,507,81 | Scale/Radius: 10.00 |
| 102 | `Roid_Sm_Brown` | 155 | Object | 461.92,4140.94,307.94 | 90,302,323 | Scale/Radius: 10.00 |
| 103 | `Roid_Sm_Brown` | 162 | Object | 2232.60,1061.50,3233.42 | 302,285,143 | Scale/Radius: 10.00 |
| 104 | `Roid_Sm_Brown` | 172 | Object | 76.99,-2171.91,3695.33 | 78,78,159 | Scale/Radius: 10.00 |
| 105 | `Roid_Sm_Brown` | 180 | Object | 2694.51,-2402.87,2463.55 | 95,340,330 | Scale/Radius: 10.00 |
| 106 | `Roid_Sm_Brown` | 189 | Object | 1847.67,4371.90,-2617.53 | 264,319,82 | Scale/Radius: 10.00 |
| 107 | `Roid_Sm_Brown` | 198 | Object | -2309.58,214.65,2155.61 | 500,43,278 | Scale/Radius: 10.00 |
| 108 | `Roid_Sm_Brown` | 205 | Object | 3233.42,-324.25,-2078.62 | 297,292,267 | Scale/Radius: 10.00 |
| 109 | `Roid_Sm_Brown` | 214 | Object | -1616.71,-2094.93,-2694.51 | 347,232,65 | Scale/Radius: 10.00 |
| 110 | `Roid_Sm_Brown` | 223 | Object | 2617.53,-1402.05,-615.89 | 367,374,232 | Scale/Radius: 10.00 |
| 111 | `Roid_Sm_Brown` | 230 | Object | 2309.58,-1479.04,1308.76 | 156,244,206 | Scale/Radius: 10.00 |
| 112 | `Roid_Sm_Brown` | 238 | Object | 384.93,368.63,538.90 | 391,92,265 | Scale/Radius: 10.00 |
| 113 | `Roid_Sm_Brown` | 245 | Object | 1231.78,-2325.89,76.99 | 190,388,217 | Scale/Radius: 10.00 |
| 114 | `Roid_Sm_Brown2` | 166 | Object | 3618.35,1446.43,-2001.64 | 65,23,266 | Scale/Radius: 10.00 |
| 115 | `Roid_Sm_Brown2` | 71 | Object | -1231.78,-2402.87,769.86 | 239,67,115 | Scale/Radius: 10.00 |
| 116 | `Roid_Sm_Brown2` | 79 | Object | 1924.65,291.64,-615.89 | 403,232,428 | Scale/Radius: 10.00 |
| 117 | `Roid_Sm_Brown2` | 98 | Object | 3772.32,4371.90,-1770.68 | 191,315,20 | Scale/Radius: 10.00 |
| 118 | `Roid_Sm_Brown2` | 108 | Object | -3233.42,-786.17,538.90 | 326,223,475 | Scale/Radius: 10.00 |
| 119 | `Roid_Sm_Brown2` | 234 | Object | 2001.64,753.56,-1847.67 | 166,133,455 | Scale/Radius: 10.00 |
| 120 | `Roid_Sm_Brown` | 177 | Object | 3233.42,2216.29,-1385.75 | 329,41,387 | Scale/Radius: 10.00 |
| 121 | `Roid_Sm_Brown` | 47 | Object | 1077.81,4525.87,-3156.43 | 485,373,304 | Scale/Radius: 10.00 |
| 122 | `Roid_Sm_Brown` | 55 | Object | -3374.35,1523.42,1965.25 | 153,132,446 | Scale/Radius: 10.00 |
| 123 | `Roid_Sm_Brown` | 64 | Object | -3310.40,676.57,-1231.78 | 302,294,407 | Scale/Radius: 10.00 |
| 124 | `Roid_Sm_Brown` | 72 | Object | 3464.37,3063.14,2463.55 | 89,72,314 | Scale/Radius: 10.00 |
| 125 | `Roid_Sm_Brown` | 82 | Object | -846.85,1908.35,230.96 | 422,366,177 | Scale/Radius: 10.00 |
| 126 | `Roid_Sm_Brown` | 91 | Object | -1924.65,1138.49,-769.86 | 24,505,392 | Scale/Radius: 10.00 |
| 127 | `Roid_Sm_Brown` | 101 | Object | -3156.43,-1786.98,1847.67 | 503,487,449 | Scale/Radius: 10.00 |
| 128 | `Roid_Sm_Brown` | 110 | Object | -692.87,2370.26,1385.75 | 299,480,368 | Scale/Radius: 10.00 |
| 129 | `Roid_Sm_Brown` | 117 | Object | 461.92,984.51,-769.86 | 166,433,86 | Scale/Radius: 10.00 |
| 130 | `Roid_Sm_Brown` | 126 | Object | 1693.69,-786.17,-3464.37 | 362,328,258 | Scale/Radius: 10.00 |
| 131 | `Roid_Sm_Brown` | 135 | Object | -1462.74,-478.22,-1385.75 | 126,196,327 | Scale/Radius: 10.00 |
| 132 | `Roid_Sm_Brown` | 144 | Object | 769.86,-2787.80,-2386.57 | 11,457,451 | Scale/Radius: 10.00 |
| 133 | `Roid_Sm_Brown` | 152 | Object | 846.85,1831.36,2386.57 | 317,79,377 | Scale/Radius: 10.00 |
| 134 | `Roid_Sm_Brown` | 159 | Object | 3289.88,-1171.10,2376.18 | 475,82,27 | Scale/Radius: 10.00 |
| 135 | `Roid_Sm_Brown` | 169 | Object | 2694.51,522.60,3772.32 | 355,86,501 | Scale/Radius: 10.00 |
| 136 | `Roid_Sm_Brown` | 186 | Object | -538.90,368.63,-1924.65 | 338,417,280 | Scale/Radius: 10.00 |
| 137 | `Roid_Sm_Brown` | 195 | Object | -461.92,-863.15,384.93 | 98,115,319 | Scale/Radius: 10.00 |
| 138 | `Roid_Sm_Brown` | 202 | Object | -2694.51,3986.97,1308.76 | 485,368,405 | Scale/Radius: 10.00 |
| 139 | `Roid_Sm_Brown` | 211 | Object | -230.96,1292.46,2848.48 | 95,129,94 | Scale/Radius: 10.00 |
| 140 | `Roid_Sm_Brown` | 220 | Object | 2617.53,-1402.05,615.89 | 385,88,268 | Scale/Radius: 10.00 |
| 141 | `Roid_Sm_Brown` | 227 | Object | 307.94,-124.25,307.94 | 58,297,239 | Scale/Radius: 10.00 |
| 142 | `Roid_Sm_Brown` | 235 | Object | -2232.60,-555.21,76.99 | 263,178,485 | Scale/Radius: 10.00 |
| 143 | `Roid_Sm_Brown` | 242 | Object | -769.86,2062.32,2001.64 | 264,508,156 | Scale/Radius: 10.00 |
| 144 | `Roid_Sm_Brown` | 249 | Object | 307.94,-1402.05,-2309.58 | 420,456,374 | Scale/Radius: 10.00 |
| 145 | `Roid_Sm_Brown2` | 171 | Object | 3387.39,-2864.79,-628.05 | 386,257,472 | Scale/Radius: 10.00 |
| 146 | `Roid_Sm_Brown2` | 49 | Object | -2078.62,-2094.93,603.72 | 84,257,311 | Scale/Radius: 10.00 |
| 147 | `Roid_Sm_Brown2` | 57 | Object | -692.87,1831.36,-166.14 | 149,505,133 | Scale/Radius: 10.00 |
| 148 | `Roid_Sm_Brown2` | 66 | Object | 1847.67,1215.47,-936.00 | 243,145,20 | Scale/Radius: 10.00 |
| 149 | `Roid_Sm_Brown2` | 74 | Object | -1077.81,2447.25,-3091.61 | 404,455,328 | Scale/Radius: 10.00 |
| 150 | `Roid_Sm_Brown2` | 84 | Object | -384.93,-1940.96,757.70 | 362,353,172 | Scale/Radius: 10.00 |
| 151 | `Roid_Sm_Brown2` | 93 | Object | 461.92,-2633.83,-782.03 | 125,352,120 | Scale/Radius: 10.00 |
| 152 | `Roid_Sm_Brown2` | 103 | Object | -2912.43,3294.10,2568.98 | 203,16,100 | Scale/Radius: 10.00 |
| 153 | `Roid_Sm_Brown2` | 112 | Object | 2001.64,3294.10,1142.63 | 490,356,365 | Scale/Radius: 10.00 |
| 154 | `Roid_Sm_Brown2` | 119 | Object | 1462.74,2370.26,-243.12 | 109,25,450 | Scale/Radius: 10.00 |
| 155 | `Roid_Sm_Brown2` | 128 | Object | -2386.57,753.56,64.82 | 339,124,472 | Scale/Radius: 10.00 |
| 156 | `Roid_Sm_Brown2` | 137 | Object | 1231.78,-1248.08,1758.51 | 423,465,352 | Scale/Radius: 10.00 |
| 157 | `Roid_Sm_Brown2` | 146 | Object | 1154.79,-1248.08,-89.15 | 388,90,508 | Scale/Radius: 10.00 |
| 158 | `Roid_Sm_Brown2` | 154 | Object | 538.90,3371.08,1835.50 | 182,88,433 | Scale/Radius: 10.00 |
| 159 | `Roid_Sm_Brown2` | 161 | Object | 3772.32,-2864.79,1604.54 | 300,59,481 | Scale/Radius: 10.00 |
| 160 | `Roid_Sm_Brown2` | 179 | Object | -2694.51,-1556.03,1758.51 | 274,125,40 | Scale/Radius: 10.00 |
| 161 | `Roid_Sm_Brown2` | 188 | Object | 2001.64,-1479.04,3529.19 | 252,124,11 | Scale/Radius: 10.00 |
| 162 | `Roid_Sm_Brown2` | 197 | Object | 2001.64,3371.08,-2167.78 | 388,245,477 | Scale/Radius: 10.00 |
| 163 | `Roid_Sm_Brown2` | 204 | Object | 923.83,-632.19,-2244.76 | 42,436,248 | Scale/Radius: 10.00 |
| 164 | `Roid_Sm_Brown2` | 213 | Object | 1385.75,4448.89,-1859.83 | 24,309,20 | Scale/Radius: 10.00 |
| 165 | `Roid_Sm_Brown2` | 222 | Object | 3618.35,-1171.10,-705.04 | 188,453,28 | Scale/Radius: 10.00 |
| 166 | `Roid_Sm_Brown2` | 229 | Object | 2386.57,3525.06,-859.01 | 46,250,6 | Scale/Radius: 10.00 |
| 167 | `Roid_Sm_Brown2` | 237 | Object | 2848.48,-1633.01,2451.39 | 259,392,389 | Scale/Radius: 10.00 |
| 168 | `Roid_Sm_Brown2` | 244 | Object | 2309.58,291.64,3221.25 | 19,369,317 | Scale/Radius: 10.00 |
| 169 | `Roid_Sm_Brown2` | 59 | Object | 2617.53,3602.04,-230.96 | 40,23,413 | Scale/Radius: 10.00 |
| 170 | `Roid_Sm_Brown2` | 51 | Object | -2232.60,2601.22,-692.87 | 508,137,68 | Scale/Radius: 10.00 |
| 171 | `Roid_Sm_Brown2` | 68 | Object | 2309.58,3063.14,-692.87 | 420,128,441 | Scale/Radius: 10.00 |
| 172 | `Roid_Sm_Brown2` | 76 | Object | 1616.71,-2171.91,2309.58 | 94,18,82 | Scale/Radius: 10.00 |
| 173 | `Roid_Sm_Brown2` | 86 | Object | -2155.61,1215.47,-3849.30 | 384,499,67 | Scale/Radius: 10.00 |
| 174 | `Roid_Sm_Brown2` | 95 | Object | -76.99,-1633.01,307.94 | 426,297,223 | Scale/Radius: 10.00 |
| 175 | `Roid_Sm_Brown2` | 105 | Object | 3695.33,599.58,1616.71 | 393,389,42 | Scale/Radius: 10.00 |
| 176 | `Roid_Sm_Brown2` | 114 | Object | -1924.65,4140.94,-3156.43 | 417,21,362 | Scale/Radius: 10.00 |
| 177 | `Roid_Sm_Brown2` | 121 | Object | -615.89,3756.01,1616.71 | 238,70,498 | Scale/Radius: 10.00 |
| 178 | `Roid_Sm_Brown2` | 130 | Object | -769.86,2755.19,-1231.78 | 374,406,240 | Scale/Radius: 10.00 |
| 179 | `Roid_Sm_Brown2` | 139 | Object | 1693.69,-3095.75,2386.57 | 91,453,267 | Scale/Radius: 10.00 |
| 180 | `Roid_Sm_Brown2` | 148 | Object | -1231.78,3063.14,1462.74 | 449,259,147 | Scale/Radius: 10.00 |
| 181 | `Roid_Sm_Brown2` | 156 | Object | -307.94,1215.47,692.87 | 403,264,345 | Scale/Radius: 10.00 |
| 182 | `Roid_Sm_Brown2` | 163 | Object | 1385.75,-2402.87,2617.53 | 391,343,29 | Scale/Radius: 10.00 |
| 183 | `Roid_Sm_Brown2` | 173 | Object | 2078.62,4525.87,-2617.53 | 218,272,451 | Scale/Radius: 10.00 |
| 184 | `Roid_Sm_Brown2` | 181 | Object | -2078.62,2755.19,1000.82 | 362,464,453 | Scale/Radius: 10.00 |
| 185 | `Roid_Sm_Brown2` | 190 | Object | -2386.57,522.60,3002.46 | 54,194,89 | Scale/Radius: 10.00 |
| 186 | `Roid_Sm_Brown2` | 199 | Object | 3156.43,60.68,1385.75 | 245,508,255 | Scale/Radius: 10.00 |
| 187 | `Roid_Sm_Brown2` | 206 | Object | 3310.40,2447.25,-2771.50 | 422,192,231 | Scale/Radius: 10.00 |
| 188 | `Roid_Sm_Brown2` | 215 | Object | 1616.71,-2017.94,-923.83 | 282,464,334 | Scale/Radius: 10.00 |
| 189 | `Roid_Sm_Brown2` | 224 | Object | -3143.39,1061.50,2966.07 | 378,87,395 | Scale/Radius: 10.00 |
| 190 | `Roid_Sm_Brown2` | 231 | Object | -1154.79,1061.50,-3002.46 | 464,183,258 | Scale/Radius: 10.00 |
| 191 | `Roid_Sm_Brown2` | 239 | Object | 1462.74,-16.30,1308.76 | 374,26,364 | Scale/Radius: 10.00 |
| 192 | `Roid_Sm_Brown2` | 246 | Object | -1770.68,2139.31,-2386.57 | 323,433,120 | Scale/Radius: 10.00 |
| 193 | `Roid_Sm_Brown` | 62 | Object | -384.93,984.51,-76.99 | 136,504,301 | Scale/Radius: 10.00 |
| 194 | `Roid_Sm_Brown` | 142 | Object | -1693.69,4140.94,-2232.60 | 113,146,441 | Scale/Radius: 10.00 |
| 195 | `Roid_Sm_Brown` | 193 | Object | 153.97,-3018.76,76.99 | 199,338,193 | Scale/Radius: 10.00 |
| 196 | `Roid_Sm_Brown` | 133 | Object | -2463.55,3525.06,2155.61 | 336,335,310 | Scale/Radius: 10.00 |
| 197 | `Roid_Sm_Brown` | 134 | Object | 307.94,-1325.07,-307.94 | 353,18,272 | Scale/Radius: 10.00 |
| 198 | `Roid_Sm_Brown` | 54 | Object | 1231.78,2601.22,2694.51 | 206,468,414 | Scale/Radius: 10.00 |
| 199 | `Roid_Sm_Brown` | 81 | Object | 153.97,-1094.11,2001.64 | 238,147,336 | Scale/Radius: 10.00 |
| 200 | `Roid_Sm_Brown` | 99 | Object | -461.92,2447.25,2309.58 | 49,453,341 | Scale/Radius: 10.00 |
| 201 | `Roid_Sm_Brown` | 109 | Object | -2001.64,-863.15,-1077.81 | 362,308,67 | Scale/Radius: 10.00 |
| 202 | `Roid_Sm_Brown` | 143 | Object | -3541.36,-1248.08,-692.87 | 147,38,105 | Scale/Radius: 10.00 |
| 203 | `Roid_Sm_Brown` | 168 | Object | 2540.54,1061.50,1000.82 | 278,310,170 | Scale/Radius: 10.00 |
| 204 | `Roid_Sm_Brown` | 184 | Object | 2694.51,3679.03,2540.54 | 445,251,201 | Scale/Radius: 10.00 |
| 205 | `Roid_Sm_Brown` | 194 | Object | 2386.57,445.61,3310.40 | 154,220,148 | Scale/Radius: 10.00 |
| 206 | `Armon_Patroli_Black_Market_Ship` | 265 | Interactive | 108.51,-350.00,239.40 | 256,0,0 | secondary groups: CONT_062, OPPORTUNITY |
