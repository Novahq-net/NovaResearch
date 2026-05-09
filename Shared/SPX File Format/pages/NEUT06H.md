# Tachyon: The Fringe NEUT06H.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT06H.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 5 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 7 |
| Entities | 68 |
| Events | 11 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Medical_Frigate`, `1: Ice_Roid_1`, `2: Roid_XL_Green`, `3: Ice_Roid_2`, `4: Roid_Med_Green`, `5: Roid_Lrg_Grey`, `6: Roid_Med_Green2` |
| Scripts | `PLAYER.SCR`, `BLACK.SCR` |
| Scenes | None |
| Labels | `BFNE_02`, `bfbe_08`, `BFNE_01`, `bfne_09`, `bfbe_01`, `BLACK`, `repar` |
| Aliases | `Todd08`, `Todd09`, `Todd10`, `oside`, `oside_1`, `oside_2`, `bagel`, `bagel_1`, `bagel_2`, `kwB10_01`, `kwB10_02`, `Todd13`, `Todd12`, `Todd02`, `Todd03`, `Todd04`, `Todd05`, `Todd06`, `Todd07`, `will_01`, `kevin01`, `SHIP1_HYPER`, `SHIP2_HYPER`, `SHIP3_HYPER`, `ohshit` |
| Groups | `BLACKWELL`, `CONT_002` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Gate state/action: param 4691, subtype 3, param 0
- Set runtime trigger variable: variable group 20, variable 17, subtype 0, value 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 17
- Object spawn/action: Medical_Frigate (object 67, id 6168), subtype 14

### Event 2

**Trigger**

- Variable comparison: subject variable group 21, variable 28, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 93
- Set/add variable: variable group 13, variable 414, subtype 0, value 1
- Set/add variable: variable group 13, variable 415, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 11, param 34
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 17, op 1, value 4

**Action**

- Set runtime trigger variable: variable group 20, variable 17, subtype 1, value 0
- Play dialog: BLACK.SCR, line/variant 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 17
- Show/update HUD contact: contact/list 0, subtype 9, param 30

### Event 4

**Trigger**

- Object event: subject Medical_Frigate (object 67, id 6168), op 14, value 4

**Action**

- Set runtime trigger variable: variable group 20, variable 17, subtype 0, value 0
- Object spawn/action: Medical_Frigate (object 67, id 6168), subtype 15
- Hide/remove HUD contact: contact/list 0, subtype 9, param 42
- Hide/remove HUD contact: contact/list 0, subtype 9, param 31
- Hide/remove HUD contact: contact/list 0, subtype 9, param 30
- Set/add variable: variable group 21, variable 23, subtype 0, value 1

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 17, op 1, value 9 (join 1)
- Object event: subject Medical_Frigate (object 67, id 6168), op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 17, subtype 1, value 0
- Play dialog: BLACK.SCR, line/variant 3
- Set/add variable: variable group 13, variable 414, subtype 0, value 1
- Set/add variable: variable group 13, variable 415, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 33

### Event 6

**Trigger**

- Object arrival: Medical_Frigate (object 67, id 6168) reached Waypoint 0 (tag 451), point 1 (raw value 29556737)

**Action**

- Object spawn/action: Medical_Frigate (object 67, id 6168), subtype 7
- Hide/remove HUD contact: contact/list 0, subtype 9, param 42
- Hide/remove HUD contact: contact/list 0, subtype 9, param 31
- Show/update HUD contact: contact/list 0, subtype 11, param 34
- Set/add variable: variable group 13, variable 415, subtype 0, value 1
- Set/add variable: variable group 13, variable 414, subtype 0, value 1

### Event 7

**Trigger**

- Object arrival: Medical_Frigate (object 67, id 6168) reached Waypoint 0 (tag 451), point 0 (raw value 29556736)
- Variable comparison: subject variable group 21, variable 23, op 1, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 18, subtype 0, value 0

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 18, op 1, value 35 (flags 1)
- Variable comparison: subject variable group 21, variable 23, op 1, value 0
- Variable comparison: subject variable group 21, variable 28, op 1, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 91
- Hide/remove HUD contact: contact/list 0, subtype 9, param 30
- Show/update HUD contact: contact/list 0, subtype 9, param 42
- Show/update HUD contact: contact/list 0, subtype 9, param 31

### Event 9

**Trigger**

- Variable comparison: subject variable group 20, variable 18, op 1, value 36

**Action**

- Set runtime trigger variable: variable group 20, variable 18, subtype 1, value 0

### Event 10

**Trigger**

- Object event: subject Medical_Frigate (object 67, id 6168), op 2, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Set/add variable: variable group 21, variable 28, subtype 0, value 1

## Waypoints

### Waypoint 0

- Tag: `451`
- Members: `Medical_Frigate (object 67, id 6168, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1184.84, -66.61, -2314.50) | None; listened by Event 7 for Medical_Frigate (object 67, id 6168) |
| 1 | (8751.91, 540.32, -14972.17) | None; listened by Event 6 for Medical_Frigate (object 67, id 6168) |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Roid_Med_Green2` | 6281 | Object | 2255.28,-33.87,-4194.53 | 321,216,6 | Scale/Radius: 8.00 |
| 1 | `Roid_Lrg_Grey` | 6283 | Object | 2412.46,-160.13,-3788.04 | 417,465,92 | Scale/Radius: 9.00 |
| 2 | `Roid_Med_Green` | 6286 | Object | 2146.92,16.95,-4044.07 | 378,55,75 | Scale/Radius: 8.00 |
| 3 | `Roid_Lrg_Grey` | 6289 | Object | 1727.16,18.48,-3709.00 | 0,28,82 | Scale/Radius: 9.00 |
| 4 | `Ice_Roid_2` | 6290 | Object | 2500.49,-64.67,-4426.00 | 93,242,269 | Scale/Radius: 3.00 |
| 5 | `Roid_Med_Green` | 6292 | Object | 2021.86,-123.18,-3675.36 | 368,378,21 | Scale/Radius: 2.00 |
| 6 | `Roid_XL_Green` | 6294 | Object | 2261.57,-58.51,-3675.13 | 307,388,331 | Scale/Radius: 2.00 |
| 7 | `Roid_Lrg_Grey` | 6295 | Object | 2311.87,-80.07,-4059.03 | 111,408,363 | Scale/Radius: 4.00 |
| 8 | `Roid_Med_Green2` | 6299 | Object | 2368.45,-153.97,-4431.65 | 0,108,492 | Scale/Radius: 5.00 |
| 9 | `Roid_Lrg_Grey` | 6301 | Object | 2047.23,-117.02,-4038.34 | 100,29,374 | Scale/Radius: 7.00 |
| 10 | `Roid_Med_Green2` | 6305 | Object | 2394.44,12.94,-4208.81 | 297,162,355 | Scale/Radius: 9.00 |
| 11 | `Roid_XL_Green` | 6306 | Object | 2252.71,255.59,-3862.96 | 345,227,455 | Scale/Radius: 2.00 |
| 12 | `Roid_Med_Green` | 6310 | Object | 2242.71,36.95,-4217.11 | 213,484,358 | Scale/Radius: 1.00 |
| 13 | `Roid_Med_Green2` | 6311 | Object | 1495.73,-38.55,-2724.06 | 170,49,272 | Scale/Radius: 7.00 |
| 14 | `Roid_XL_Green` | 6312 | Object | 2330.73,-58.51,-4442.94 | 443,349,372 | Scale/Radius: 1.00 |
| 15 | `Roid_Lrg_Grey` | 6313 | Object | 2186.13,-141.65,-3827.56 | 386,120,112 | Scale/Radius: 3.00 |
| 16 | `Ice_Roid_2` | 6319 | Object | 2293.01,9.24,-4025.16 | 320,167,332 | Scale/Radius: 1.00 |
| 17 | `Roid_Med_Green` | 6321 | Object | 2318.16,-76.99,-4115.49 | 305,504,273 | Scale/Radius: 2.00 |
| 18 | `Roid_Med_Green2` | 6322 | Object | 2356.17,24.64,-4351.06 | 228,267,283 | Scale/Radius: 9.00 |
| 19 | `Roid_Lrg_Grey` | 6324 | Object | 1301.13,-34.75,-2638.71 | 81,262,48 | Scale/Radius: 9.00 |
| 20 | `Ice_Roid_2` | 6325 | Object | 2198.70,-212.48,-3793.69 | 497,68,94 | Scale/Radius: 2.00 |
| 21 | `Roid_Med_Green2` | 6328 | Object | 2487.91,249.43,-4267.92 | 449,112,182 | Scale/Radius: 3.00 |
| 22 | `Roid_Lrg_Grey` | 6330 | Object | 2204.99,160.13,-4171.95 | 105,275,453 | Scale/Radius: 3.00 |
| 23 | `Ice_Roid_2` | 6331 | Object | 2236.42,-120.10,-3720.29 | 60,42,214 | Scale/Radius: 5.00 |
| 24 | `Ice_Roid_2` | 6336 | Object | 2192.41,-6.16,-4030.81 | 438,77,12 | Scale/Radius: 2.00 |
| 25 | `Roid_Med_Green` | 6338 | Object | 2204.84,19.19,-4110.64 | 376,278,254 | Scale/Radius: 9.00 |
| 26 | `Roid_Med_Green2` | 6339 | Object | 2079.36,-15.40,-4207.78 | 124,168,385 | Scale/Radius: 8.00 |
| 27 | `Ice_Roid_1` | 6343 | Object | 2418.75,120.10,-4245.34 | 369,301,168 | Scale/Radius: 4.00 |
| 28 | `Roid_Med_Green2` | 6345 | Object | 2330.73,36.95,-4126.78 | 352,246,249 | Scale/Radius: 2.00 |
| 29 | `Ice_Roid_1` | 6348 | Object | 2230.14,86.22,-4183.24 | 169,355,373 | Scale/Radius: 5.00 |
| 30 | `Roid_Med_Green2` | 6350 | Object | 2267.86,-277.15,-4465.52 | 290,441,279 | Scale/Radius: 8.00 |
| 31 | `Roid_XL_Green` | 6351 | Object | 2192.41,-511.19,-3912.25 | 22,86,501 | Scale/Radius: 1.00 |
| 32 | `Roid_XL_Green` | 6357 | Object | 2756.01,301.79,-3681.54 | 268,494,349 | Scale/Radius: 3.00 |
| 33 | `Roid_Med_Green` | 6361 | Object | 1990.42,36.95,-3709.23 | 487,44,266 | Scale/Radius: 8.00 |
| 34 | `Roid_XL_Green` | 6363 | Object | 2539.38,227.88,-4409.97 | 414,215,123 | Scale/Radius: 2.00 |
| 35 | `Roid_XL_Green` | 6387 | Object | 1194.73,-63.50,-2393.54 | 64,2,41 | Scale/Radius: 1.00 |
| 36 | `Roid_Lrg_Grey` | 6388 | Object | 1473.04,-38.41,-2901.82 | 325,293,451 | Scale/Radius: 8.00 |
| 37 | `Roid_Lrg_Grey` | 6394 | Object | 1714.59,27.71,-3432.37 | 167,494,50 | Scale/Radius: 8.00 |
| 38 | `Roid_XL_Green` | 6405 | Object | 1920.34,-160.00,-3375.63 | 383,393,159 | Scale/Radius: 3.00 |
| 39 | `Roid_Lrg_Grey` | 6406 | Object | 1680.83,159.02,-3279.64 | 1,202,453 | Scale/Radius: 9.00 |
| 40 | `Ice_Roid_2` | 6407 | Object | 2167.26,-415.72,-3991.29 | 310,171,69 | Scale/Radius: 3.00 |
| 41 | `Roid_Med_Green` | 6415 | Object | 3864.15,133.36,-6720.26 | 458,7,38 | Scale/Radius: 8.00 |
| 42 | `Roid_Med_Green2` | 6416 | Object | 3344.08,62.35,-5773.35 | 248,71,302 | Scale/Radius: 5.00 |
| 43 | `Roid_XL_Green` | 6417 | Object | 2223.85,-535.82,-3804.98 | 18,30,222 | Scale/Radius: 1.00 |
| 44 | `Ice_Roid_1` | 6420 | Object | 1752.31,-304.86,-3669.48 | 303,141,329 | Scale/Radius: 5.00 |
| 45 | `Roid_Med_Green2` | 6422 | Object | 3329.12,133.33,-6064.86 | 227,509,61 | Scale/Radius: 9.00 |
| 46 | `Roid_Lrg_Grey` | 6423 | Object | 1426.04,-431.12,-3299.63 | 58,236,154 | Scale/Radius: 7.00 |
| 47 | `Roid_Med_Green` | 6426 | Object | 4059.36,143.96,-7023.77 | 481,386,289 | Scale/Radius: 9.00 |
| 48 | `Roid_XL_Green` | 6440 | Object | 2293.01,-615.89,-4476.81 | 369,50,220 | Scale/Radius: 1.00 |
| 49 | `Roid_Med_Green2` | 6451 | Object | 2929.76,-515.98,-5073.72 | 73,143,379 | Scale/Radius: 8.00 |
| 50 | `Roid_XL_Green` | 6452 | Object | 2780.02,248.48,-5566.06 | 396,10,93 | Scale/Radius: 3.00 |
| 51 | `Roid_Med_Green` | 6456 | Object | 2337.02,523.51,-4025.16 | 180,136,166 | Scale/Radius: 9.00 |
| 52 | `Roid_Med_Green2` | 6457 | Object | 2792.51,62.98,-4951.67 | 59,116,160 | Scale/Radius: 6.00 |
| 53 | `Roid_Med_Green2` | 6473 | Object | 3874.76,145.67,-6906.21 | 243,502,375 | Scale/Radius: 7.00 |
| 54 | `Roid_Lrg_Grey` | 6475 | Object | 1861.26,-15.36,-3349.46 | 278,441,209 | Scale/Radius: 2.00 |
| 55 | `Roid_XL_Green` | 6480 | Object | 1416.61,335.32,-2969.42 | 146,311,59 | Scale/Radius: 1.00 |
| 56 | `Roid_XL_Green` | 6494 | Object | 2250.84,0.00,-4442.66 | 0,0,0 | Scale/Radius: 1.00 |
| 57 | `Roid_XL_Green` | 6518 | Object | 3648.33,132.52,-6547.51 | 301,337,326 | Scale/Radius: 2.00 |
| 58 | `Ice_Roid_2` | 6520 | Object | 2823.57,-37.72,-5689.50 | 305,32,208 | Scale/Radius: 5.00 |
| 59 | `Roid_Lrg_Grey` | 6523 | Object | 3722.59,42.21,-6624.71 | 488,106,249 | Scale/Radius: 3.00 |
| 60 | `Ice_Roid_2` | 6528 | Object | 3653.46,-79.04,-6518.43 | 25,101,419 | Scale/Radius: 4.00 |
| 61 | `Roid_Lrg_Grey` | 6531 | Object | 1171.09,156.82,-3080.22 | 417,145,277 | Scale/Radius: 9.00 |
| 62 | `Roid_XL_Green` | 6556 | Object | 4036.49,148.99,-7179.77 | 0,0,0 | Scale/Radius: 1.00 |
| 63 | `Roid_XL_Green` | 6557 | Object | 1109.49,-76.51,-2225.50 | 462,420,64 | Scale/Radius: 1.00 |
| 64 | `Roid_XL_Green` | 6559 | Object | 2805.49,86.93,-5154.23 | 0,441,0 | Scale/Radius: 1.00 |
| 65 | `Roid_Lrg_Grey` | 6474 | Object | 2773.12,43.98,-4913.48 | 62,226,18 | Scale/Radius: 1.00 |
| 66 | `Roid_Lrg_Grey` | 6276 | Object | 1967.02,-221.72,-3643.52 | 77,507,343 | Scale/Radius: 1.00 |
| 67 | `Medical_Frigate` | 6168 | Interactive | 820.87,-92.86,-1682.37 | 212,6,28 | label: BLACK; secondary groups: CONT_002, BLACKWELL; waypoint: Waypoint 0 (tag 451, 2 point(s)), starting point 0, arrival event value 29556736 |
