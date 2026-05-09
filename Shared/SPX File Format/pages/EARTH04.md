# Tachyon: The Fringe EARTH04.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH04.SPX` |
| Sector | `QUAD_04` |
| Backdrop | `EARTH04.BDF` |
| Region | 0 |
| Sector ID | 3 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 7 |
| Entities | 146 |
| Events | 3 |
| Waypoints | 0 |
| Child Sectors | 1 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Ganymede_Station`, `1: Spcargo_Goods`, `2: Spcargo_Credits`, `3: Roid_XL_Green`, `4: Roid_Med_Green2`, `5: Roid_Med_Green`, `6: Hyper_Gate` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `AGT Fighter` |
| Aliases | `danc_blowfish4`, `danc_blowfish3`, `danc_blowfish2`, `danc_blowfish1`, `danc_blowfish5`, `Jerome50` |
| Groups | `CONT_066`, `CONT_059` |
| Child Sectors | [earth04B.spx](EARTH04B.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 1334; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 135
- Set/add variable: variable group 0, variable 2, subtype 1, value 100
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 34
- Set/add variable: variable group 12, variable 303, subtype 0, value 1

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 32, op 2, value 10

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 34
- Set/add variable: variable group 20, variable 32, subtype 0, value 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 1337; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 132
- Set/add variable: variable group 12, variable 301, subtype 0, value 1

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 230 | Gate | 1254.21,0.00,2333.10 | 41,307,0 | Gate SPX: [Earth02.spx](EARTH02.md) |
| 1 | `Roid_Med_Green` | 1158 | Object | -3690.65,554.30,1223.85 | 203,254,291 | Scale/Radius: 1.00 |
| 2 | `Roid_Med_Green2` | 1160 | Object | -3448.14,-715.97,1705.02 | 262,199,303 | Scale/Radius: 9.00 |
| 3 | `Roid_XL_Green` | 1166 | Object | -1615.88,-161.67,2301.66 | 459,220,467 | Scale/Radius: 1.00 |
| 4 | `Roid_Med_Green2` | 1174 | Object | -3636.76,-669.78,1608.78 | 396,445,4 | Scale/Radius: 2.00 |
| 5 | `Roid_Med_Green2` | 1187 | Object | -1804.49,-715.97,1647.28 | 405,307,488 | Scale/Radius: 5.00 |
| 6 | `Roid_XL_Green` | 1193 | Object | -2666.74,-508.11,2705.84 | 239,136,41 | Scale/Radius: 2.00 |
| 7 | `Roid_Med_Green` | 1200 | Object | -3340.36,-184.77,1166.11 | 47,261,431 | Scale/Radius: 4.00 |
| 8 | `Roid_Med_Green2` | 1201 | Object | -2154.78,-1039.31,1146.87 | 323,218,241 | Scale/Radius: 6.00 |
| 9 | `Roid_Med_Green` | 1206 | Object | -3717.60,923.83,2186.18 | 359,392,257 | Scale/Radius: 7.00 |
| 10 | `Roid_Med_Green2` | 1216 | Object | -3151.75,554.30,2725.08 | 72,32,294 | Scale/Radius: 1.00 |
| 11 | `Roid_Med_Green` | 1223 | Object | -3636.76,993.12,1570.29 | 392,412,190 | Scale/Radius: 1.00 |
| 12 | `Roid_Med_Green` | 1232 | Object | -1723.66,1108.60,915.91 | 263,400,364 | Scale/Radius: 5.00 |
| 13 | `Roid_Med_Green2` | 1240 | Object | -2828.41,-415.72,1377.83 | 267,117,180 | Scale/Radius: 7.00 |
| 14 | `Roid_Med_Green2` | 1249 | Object | -1804.49,-1039.31,1974.47 | 378,234,487 | Scale/Radius: 8.00 |
| 15 | `Roid_Med_Green` | 1255 | Object | -3717.60,1016.22,915.91 | 420,98,59 | Scale/Radius: 4.00 |
| 16 | `Roid_XL_Green` | 1263 | Object | -1750.60,831.45,2282.41 | 56,433,182 | Scale/Radius: 4.00 |
| 17 | `Roid_Med_Green` | 1264 | Object | -1454.20,739.07,1762.76 | 233,105,438 | Scale/Radius: 5.00 |
| 18 | `Roid_Med_Green2` | 1265 | Object | -3421.20,-508.11,858.17 | 184,254,337 | Scale/Radius: 7.00 |
| 19 | `Roid_XL_Green` | 1272 | Object | -3744.54,831.45,1416.32 | 346,493,110 | Scale/Radius: 1.00 |
| 20 | `Roid_XL_Green` | 1280 | Object | -1993.11,1062.41,2705.84 | 364,108,502 | Scale/Radius: 1.00 |
| 21 | `Roid_Med_Green2` | 1288 | Object | -1211.70,1085.50,2513.37 | 402,395,158 | Scale/Radius: 6.00 |
| 22 | `Roid_Med_Green` | 1294 | Object | -1346.42,438.82,1628.03 | 414,265,135 | Scale/Radius: 2.00 |
| 23 | `Spcargo_Credits` | 1334 | Interactive | -1230.76,-2469.09,-1913.16 | 7,391,7 | secondary groups: CONT_066, none |
| 24 | `Spcargo_Goods` | 1337 | Interactive | -2039.85,3.00,1243.45 | 57,43,36 | secondary groups: CONT_059, none |
| 25 | `Roid_XL_Green` | 1208 | Object | -1508.10,138.57,2455.63 | 477,484,484 | Scale/Radius: 1.00 |
| 26 | `Roid_XL_Green` | 1186 | Object | -1642.82,0.00,1974.47 | 114,398,156 | Scale/Radius: 1.00 |
| 27 | `Roid_XL_Green` | 1194 | Object | -1527.72,-554.30,803.92 | 320,95,348 | Scale/Radius: 1.00 |
| 28 | `Roid_XL_Green` | 1215 | Object | -3340.36,-646.68,2417.14 | 13,505,362 | Scale/Radius: 1.00 |
| 29 | `Roid_XL_Green` | 1225 | Object | -2505.06,692.87,1281.59 | 39,243,142 | Scale/Radius: 1.00 |
| 30 | `Roid_XL_Green` | 1239 | Object | -3690.65,946.93,1166.11 | 352,462,152 | Scale/Radius: 1.00 |
| 31 | `Roid_XL_Green` | 1248 | Object | -1454.20,923.83,2320.91 | 457,451,377 | Scale/Radius: 1.00 |
| 32 | `Roid_XL_Green` | 1257 | Object | -2316.45,-762.16,2186.18 | 282,312,33 | Scale/Radius: 1.00 |
| 33 | `Roid_XL_Green` | 1273 | Object | -2612.85,531.20,1628.03 | 218,229,141 | Scale/Radius: 1.00 |
| 34 | `Roid_Med_Green2` | 1217 | Object | -1993.11,369.53,2744.33 | 277,192,387 | Scale/Radius: 1.00 |
| 35 | `Roid_Med_Green2` | 1167 | Object | -3636.76,-970.02,1320.09 | 73,394,93 | Scale/Radius: 1.00 |
| 36 | `Roid_Med_Green2` | 1188 | Object | -2020.05,461.92,2166.93 | 507,175,22 | Scale/Radius: 1.00 |
| 37 | `Roid_Med_Green2` | 1195 | Object | -2963.13,1062.41,2378.65 | 462,327,369 | Scale/Radius: 1.00 |
| 38 | `Roid_Med_Green2` | 1226 | Object | -3124.80,554.30,1243.10 | 205,90,158 | Scale/Radius: 1.00 |
| 39 | `Roid_Med_Green2` | 1241 | Object | -3448.14,-207.86,1685.77 | 137,326,355 | Scale/Radius: 1.00 |
| 40 | `Roid_Med_Green2` | 1250 | Object | -3367.31,-392.63,1955.22 | 190,432,333 | Scale/Radius: 1.00 |
| 41 | `Roid_Med_Green2` | 1266 | Object | -3879.27,-300.25,2609.60 | 353,418,137 | Scale/Radius: 1.00 |
| 42 | `Roid_Med_Green2` | 1274 | Object | -3259.53,-762.16,2089.95 | 378,508,222 | Scale/Radius: 1.00 |
| 43 | `Roid_Med_Green` | 1211 | Object | -1292.53,-946.93,2205.43 | 408,196,329 | Scale/Radius: 1.00 |
| 44 | `Roid_Med_Green` | 1154 | Object | -2397.28,-669.78,2263.17 | 423,186,205 | Scale/Radius: 1.00 |
| 45 | `Roid_Med_Green` | 1163 | Object | -3502.03,-923.83,954.40 | 506,289,257 | Scale/Radius: 1.00 |
| 46 | `Roid_Med_Green` | 1170 | Object | -2801.46,-1062.41,1782.00 | 25,3,7 | Scale/Radius: 1.00 |
| 47 | `Roid_Med_Green` | 1177 | Object | -2020.05,715.97,2301.66 | 221,315,50 | Scale/Radius: 1.00 |
| 48 | `Roid_Med_Green` | 1182 | Object | -3313.42,69.29,1647.28 | 348,0,247 | Scale/Radius: 1.00 |
| 49 | `Roid_Med_Green` | 1190 | Object | -3798.43,-300.25,935.16 | 440,144,452 | Scale/Radius: 1.00 |
| 50 | `Roid_Med_Green` | 1197 | Object | -2855.35,-715.97,1858.99 | 423,160,328 | Scale/Radius: 1.00 |
| 51 | `Roid_Med_Green` | 1203 | Object | -2127.83,-230.96,1705.02 | 30,104,456 | Scale/Radius: 1.00 |
| 52 | `Roid_Med_Green` | 1220 | Object | -2370.34,-1016.22,1050.64 | 62,28,174 | Scale/Radius: 1.00 |
| 53 | `Roid_Med_Green` | 1229 | Object | -3690.65,1131.70,1223.85 | 509,12,279 | Scale/Radius: 1.00 |
| 54 | `Roid_Med_Green` | 1235 | Object | -3286.47,-485.01,1377.83 | 389,316,181 | Scale/Radius: 1.00 |
| 55 | `Roid_Med_Green` | 1243 | Object | -2747.57,392.63,1858.99 | 91,80,41 | Scale/Radius: 1.00 |
| 56 | `Roid_Med_Green` | 1252 | Object | -2774.52,46.19,2320.91 | 185,209,3 | Scale/Radius: 1.00 |
| 57 | `Roid_Med_Green` | 1260 | Object | -1831.44,346.44,1281.59 | 288,60,357 | Scale/Radius: 1.00 |
| 58 | `Roid_Med_Green` | 1269 | Object | -3259.53,-346.44,1281.59 | 374,237,271 | Scale/Radius: 1.00 |
| 59 | `Roid_Med_Green` | 1277 | Object | -2478.12,-230.96,1955.22 | 125,20,369 | Scale/Radius: 1.00 |
| 60 | `Roid_Med_Green` | 1284 | Object | -3232.58,946.93,1416.32 | 369,148,245 | Scale/Radius: 1.00 |
| 61 | `Roid_Med_Green` | 1291 | Object | -1615.88,946.93,2628.85 | 309,453,433 | Scale/Radius: 1.00 |
| 62 | `Roid_Med_Green` | 1157 | Object | -3663.71,1062.41,1512.55 | 319,148,46 | Scale/Radius: 1.00 |
| 63 | `Roid_XL_Green` | 1205 | Object | -3151.75,161.67,896.66 | 243,6,494 | Scale/Radius: 1.00 |
| 64 | `Roid_XL_Green` | 1156 | Object | -2262.56,877.64,1705.02 | 177,114,259 | Scale/Radius: 1.00 |
| 65 | `Roid_XL_Green` | 1165 | Object | -2639.79,970.02,2340.15 | 269,358,247 | Scale/Radius: 1.00 |
| 66 | `Roid_XL_Green` | 1172 | Object | -3421.20,207.86,2609.60 | 21,438,365 | Scale/Radius: 1.00 |
| 67 | `Roid_XL_Green` | 1179 | Object | -3771.49,485.01,2725.08 | 342,350,175 | Scale/Radius: 1.00 |
| 68 | `Roid_XL_Green` | 1184 | Object | -2127.83,669.78,2436.39 | 41,289,132 | Scale/Radius: 1.00 |
| 69 | `Roid_XL_Green` | 1192 | Object | -2639.79,-785.26,1724.26 | 130,488,290 | Scale/Radius: 1.00 |
| 70 | `Roid_XL_Green` | 1199 | Object | -3043.97,600.49,2224.67 | 69,321,88 | Scale/Radius: 1.00 |
| 71 | `Roid_XL_Green` | 1213 | Object | -1454.20,-69.29,1108.38 | 230,227,410 | Scale/Radius: 1.00 |
| 72 | `Roid_XL_Green` | 1222 | Object | -3097.86,923.83,1724.26 | 455,451,33 | Scale/Radius: 1.00 |
| 73 | `Roid_XL_Green` | 1231 | Object | -1211.70,577.40,1820.50 | 41,67,254 | Scale/Radius: 1.00 |
| 74 | `Roid_XL_Green` | 1237 | Object | -3528.98,877.64,2109.19 | 453,361,500 | Scale/Radius: 1.00 |
| 75 | `Roid_XL_Green` | 1245 | Object | -2747.57,646.68,2186.18 | 24,138,501 | Scale/Radius: 1.00 |
| 76 | `Roid_XL_Green` | 1254 | Object | -2020.05,623.59,2705.84 | 188,204,354 | Scale/Radius: 1.00 |
| 77 | `Roid_XL_Green` | 1262 | Object | -2451.17,92.38,1397.07 | 260,96,441 | Scale/Radius: 1.00 |
| 78 | `Roid_XL_Green` | 1271 | Object | -2747.57,-808.35,1377.83 | 234,459,80 | Scale/Radius: 1.00 |
| 79 | `Roid_XL_Green` | 1279 | Object | -1696.71,346.44,1146.87 | 20,251,6 | Scale/Radius: 1.00 |
| 80 | `Roid_XL_Green` | 1286 | Object | -1400.31,-69.29,935.16 | 396,278,95 | Scale/Radius: 1.00 |
| 81 | `Roid_XL_Green` | 1293 | Object | -3636.76,230.96,1397.07 | 250,427,44 | Scale/Radius: 1.00 |
| 82 | `Roid_Med_Green` | 1168 | Object | -2505.06,669.78,1416.32 | 36,502,488 | Scale/Radius: 1.00 |
| 83 | `Roid_Med_Green` | 1161 | Object | -2720.63,69.29,1608.78 | 452,154,360 | Scale/Radius: 1.00 |
| 84 | `Roid_Med_Green` | 1175 | Object | -1939.22,-138.57,1916.73 | 377,387,325 | Scale/Radius: 1.00 |
| 85 | `Roid_Med_Green` | 1180 | Object | -3017.02,923.83,1146.87 | 48,272,50 | Scale/Radius: 1.00 |
| 86 | `Roid_Med_Green` | 1209 | Object | -2370.34,-23.10,2012.96 | 255,337,282 | Scale/Radius: 1.00 |
| 87 | `Roid_Med_Green` | 1218 | Object | -2774.52,1085.50,1724.26 | 208,2,296 | Scale/Radius: 1.00 |
| 88 | `Roid_Med_Green` | 1227 | Object | -1508.10,-970.02,2128.44 | 355,432,187 | Scale/Radius: 1.00 |
| 89 | `Roid_Med_Green` | 1233 | Object | -2181.72,854.55,2455.63 | 28,369,135 | Scale/Radius: 1.00 |
| 90 | `Roid_Med_Green` | 1258 | Object | -1211.70,-254.05,1320.09 | 247,8,66 | Scale/Radius: 1.00 |
| 91 | `Roid_Med_Green` | 1267 | Object | -1238.64,715.97,1974.47 | 276,256,350 | Scale/Radius: 1.00 |
| 92 | `Roid_Med_Green` | 1275 | Object | -1400.31,-415.72,1608.78 | 192,75,37 | Scale/Radius: 1.00 |
| 93 | `Roid_Med_Green` | 1282 | Object | -3448.14,-923.83,1146.87 | 44,432,178 | Scale/Radius: 1.00 |
| 94 | `Roid_Med_Green` | 1289 | Object | -3690.65,577.40,1743.51 | 508,139,484 | Scale/Radius: 1.00 |
| 95 | `Roid_Med_Green2` | 1164 | Object | -1966.16,-785.26,1916.73 | 5,251,270 | Scale/Radius: 1.00 |
| 96 | `Roid_Med_Green2` | 1155 | Object | -1723.66,669.78,2282.41 | 327,298,166 | Scale/Radius: 1.00 |
| 97 | `Roid_Med_Green2` | 1171 | Object | -1211.70,369.53,2224.67 | 455,51,421 | Scale/Radius: 1.00 |
| 98 | `Roid_Med_Green2` | 1178 | Object | -2612.85,69.29,1955.22 | 216,325,253 | Scale/Radius: 1.00 |
| 99 | `Roid_Med_Green2` | 1183 | Object | -1750.60,69.29,1300.84 | 475,234,216 | Scale/Radius: 1.00 |
| 100 | `Roid_Med_Green2` | 1191 | Object | -1642.82,-1016.22,1320.09 | 164,340,375 | Scale/Radius: 1.00 |
| 101 | `Roid_Med_Green2` | 1198 | Object | -3663.71,-854.55,2089.95 | 256,492,341 | Scale/Radius: 1.00 |
| 102 | `Roid_Med_Green2` | 1204 | Object | -2639.79,438.82,1762.76 | 481,12,490 | Scale/Radius: 1.00 |
| 103 | `Roid_Med_Green2` | 1212 | Object | -2043.97,6.68,1243.10 | 454,330,334 | Scale/Radius: 1.00 |
| 104 | `Roid_Med_Green2` | 1221 | Object | -2208.67,392.63,973.65 | 94,321,45 | Scale/Radius: 1.00 |
| 105 | `Roid_Med_Green2` | 1230 | Object | -1265.59,-415.72,1108.38 | 337,369,171 | Scale/Radius: 1.00 |
| 106 | `Roid_Med_Green2` | 1236 | Object | -3528.98,-300.25,2436.39 | 266,164,403 | Scale/Radius: 1.00 |
| 107 | `Roid_Med_Green2` | 1244 | Object | -2532.01,-785.26,1185.36 | 168,96,255 | Scale/Radius: 1.00 |
| 108 | `Roid_Med_Green2` | 1253 | Object | -3636.76,369.53,1339.33 | 90,179,399 | Scale/Radius: 1.00 |
| 109 | `Roid_Med_Green2` | 1261 | Object | -3421.20,461.92,954.40 | 500,420,243 | Scale/Radius: 1.00 |
| 110 | `Roid_Med_Green2` | 1270 | Object | -1238.64,1154.79,2032.21 | 493,444,348 | Scale/Radius: 1.00 |
| 111 | `Roid_Med_Green2` | 1278 | Object | -3286.47,277.15,2628.85 | 351,470,250 | Scale/Radius: 1.00 |
| 112 | `Roid_Med_Green2` | 1285 | Object | -3205.64,300.25,2359.40 | 62,151,245 | Scale/Radius: 1.00 |
| 113 | `Roid_Med_Green2` | 1292 | Object | -3825.38,739.07,1724.26 | 487,395,272 | Scale/Radius: 1.00 |
| 114 | `Roid_Med_Green2` | 1189 | Object | -3097.86,808.35,1127.62 | 270,453,96 | Scale/Radius: 1.00 |
| 115 | `Roid_Med_Green2` | 1153 | Object | -2612.85,46.19,2128.44 | 34,26,380 | Scale/Radius: 1.00 |
| 116 | `Roid_Med_Green2` | 1162 | Object | -3367.31,46.19,1512.55 | 384,301,127 | Scale/Radius: 1.00 |
| 117 | `Roid_Med_Green2` | 1169 | Object | -1723.66,1062.41,858.17 | 330,285,12 | Scale/Radius: 1.00 |
| 118 | `Roid_Med_Green2` | 1176 | Object | -3690.65,230.96,2725.08 | 109,389,93 | Scale/Radius: 1.00 |
| 119 | `Roid_Med_Green2` | 1181 | Object | -3502.03,-69.29,2147.69 | 340,457,43 | Scale/Radius: 1.00 |
| 120 | `Roid_Med_Green2` | 1196 | Object | -2262.56,300.25,1589.54 | 96,228,239 | Scale/Radius: 1.00 |
| 121 | `Roid_Med_Green2` | 1202 | Object | -1993.11,46.19,1493.31 | 205,203,362 | Scale/Radius: 1.00 |
| 122 | `Roid_Med_Green2` | 1210 | Object | -2262.56,0.00,1243.10 | 229,399,472 | Scale/Radius: 1.00 |
| 123 | `Roid_Med_Green2` | 1219 | Object | -2397.28,-1085.50,1512.55 | 291,95,104 | Scale/Radius: 1.00 |
| 124 | `Roid_Med_Green2` | 1228 | Object | -2774.52,923.83,1858.99 | 197,152,207 | Scale/Radius: 1.00 |
| 125 | `Roid_Med_Green2` | 1234 | Object | -3124.80,-877.64,1281.59 | 440,193,73 | Scale/Radius: 1.00 |
| 126 | `Roid_Med_Green2` | 1242 | Object | -2208.67,-1016.22,1858.99 | 337,164,386 | Scale/Radius: 1.00 |
| 127 | `Roid_Med_Green2` | 1251 | Object | -3205.64,-438.82,1012.14 | 83,71,334 | Scale/Radius: 1.00 |
| 128 | `Roid_Med_Green2` | 1259 | Object | -1642.82,-323.34,1185.36 | 281,76,464 | Scale/Radius: 1.00 |
| 129 | `Roid_Med_Green2` | 1268 | Object | -2181.72,-1131.70,1416.32 | 12,341,413 | Scale/Radius: 1.00 |
| 130 | `Roid_Med_Green2` | 1276 | Object | -1885.33,-1016.22,1608.78 | 271,349,233 | Scale/Radius: 1.00 |
| 131 | `Roid_Med_Green2` | 1283 | Object | -3178.69,923.83,954.40 | 219,440,439 | Scale/Radius: 1.00 |
| 132 | `Roid_Med_Green2` | 1290 | Object | -1319.48,-1062.41,1031.39 | 286,178,368 | Scale/Radius: 1.00 |
| 133 | `Roid_XL_Green` | 1224 | Object | -1588.93,1039.31,1185.36 | 120,506,293 | Scale/Radius: 1.00 |
| 134 | `Roid_XL_Green` | 1159 | Object | -2936.19,692.87,935.16 | 443,52,494 | Scale/Radius: 1.00 |
| 135 | `Roid_XL_Green` | 1173 | Object | -2343.39,-715.97,973.65 | 445,467,150 | Scale/Radius: 1.00 |
| 136 | `Roid_XL_Green` | 1185 | Object | -1454.20,-854.55,1570.29 | 250,105,136 | Scale/Radius: 1.00 |
| 137 | `Roid_XL_Green` | 1207 | Object | -3421.20,-600.49,1320.09 | 61,217,137 | Scale/Radius: 1.00 |
| 138 | `Roid_XL_Green` | 1214 | Object | -1346.42,-92.38,2609.60 | 143,217,422 | Scale/Radius: 1.00 |
| 139 | `Roid_XL_Green` | 1238 | Object | -3798.43,-46.19,1300.84 | 181,237,193 | Scale/Radius: 1.00 |
| 140 | `Roid_XL_Green` | 1247 | Object | -3636.76,-854.55,1185.36 | 91,417,272 | Scale/Radius: 1.00 |
| 141 | `Roid_XL_Green` | 1256 | Object | -3825.38,993.12,1281.59 | 154,216,278 | Scale/Radius: 1.00 |
| 142 | `Roid_XL_Green` | 1281 | Object | -1346.42,-808.35,915.91 | 357,46,137 | Scale/Radius: 1.00 |
| 143 | `Roid_XL_Green` | 1287 | Object | -2424.23,-946.93,1974.47 | 67,415,506 | Scale/Radius: 1.00 |
| 144 | `Roid_XL_Green` | 1295 | Object | -3017.02,946.93,1782.00 | 322,254,318 | Scale/Radius: 1.00 |
| 145 | `Ganymede_Station` | 229 | Interactive | -1210.84,-1633.68,-1396.00 | 3,64,0 | None |
