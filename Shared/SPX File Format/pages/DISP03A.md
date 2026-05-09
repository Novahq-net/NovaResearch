# Tachyon: The Fringe DISP03A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP03A.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 5 |
| Entities | 295 |
| Events | 23 |
| Waypoints | 4 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Minelayer`, `1: Ripstar_Gravity`, `2: Bora_Mine`, `3: Ripstar`, `4: KC2_Crystal` |
| Scripts | `PLAYER.SCR`, `WRNBC.SCR` |
| Scenes | None |
| Labels | `BFGE_02`, `BFBE_07`, `TNSA`, `BFBE_09`, `adder1`, `BFBF_07`, `ROSS`, `SPIKE`, `atkin`, `cruiser1` |
| Aliases | `fake_2`, `BC10_Waraxe`, `Coward`, `spy_1`, `fake_1`, `tnsa`, `BC10_Claymore4`, `BC10_Claymore3`, `BC10_Claymore2`, `BC10_Claymore1`, `BC10_Warhammer4`, `BC10_Warhammer3`, `BC10_Warhammer2`, `BC10_Warhammer1`, `BC10_Mace3`, `BC10_Mace4`, `BC10_Mace1`, `BC10_Mace2`, `Galileo`, `SPIKE`, `zeus`, `Stocks01` |
| Groups | None |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0
- Play dialog: PLAYER.SCR, line/variant 39
- Gate state/action: param 3, subtype 2, param 0
- Show/update HUD contact: contact/list 0, subtype 9, param 35
- Play scene: unknown index 0, param 0
- Object spawn/action: id 10701, subtype 14

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 500 (extra 1, 9938; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 500 (extra 1, 9940; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 500 (extra 1, 9939; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 500 (extra 1, 10102; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 500 (extra 1, 10101; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 500 (extra 1, 10121; join 2; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 43

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 9938; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 9939; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 9940; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 10101; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 10102; join 2; flags 2)
- Variable comparison: subject variable group 21, variable 21, op 0, value 1 (join 2)

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Broadcast HUD contact action: contact/list 0, subtype 0, param 11
- Play dialog: PLAYER.SCR, line/variant 44
- Hide/remove HUD contact: contact/list 0, subtype 9, param 10
- Set/add variable: variable group 21, variable 20, subtype 0, value 1
- Mission objective/state: param 393219, subtype 0, param 0

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 10121; flags 2)

**Action**

- Set/add variable: variable group 21, variable 21, subtype 0, value 1

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 900 (extra 1, 9074; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 900 (extra 1, 9107; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 900 (extra 1, 9094; join 2; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 42

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 1300 (extra 1, 10080; join 1; flags 2)
- Variable comparison: subject variable group 21, variable 24, op 1, value 1

**Action**

- Play dialog: WRNBC.SCR, line/variant 0
- Object spawn/action: Ripstar (object 39, id 10276), subtype 14
- Hide/remove HUD contact: contact/list 0, subtype 9, param 35
- Show/update HUD contact: contact/list 0, subtype 9, param 10
- Set/add variable: variable group 21, variable 24, subtype 0, value 1

### Event 6

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 1300 (extra 1, 9986; join 1; flags 2)
- Variable comparison: subject variable group 21, variable 24, op 1, value 1

**Action**

- Play dialog: WRNBC.SCR, line/variant 0
- Object spawn/action: Ripstar (object 17, id 10253), subtype 14
- Show/update HUD contact: contact/list 0, subtype 9, param 10
- Hide/remove HUD contact: contact/list 0, subtype 9, param 35
- Set/add variable: variable group 21, variable 24, subtype 0, value 1

### Event 7

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 1300 (extra 1, 9991; join 1; flags 2)
- Variable comparison: subject variable group 21, variable 24, op 1, value 1

**Action**

- Play dialog: WRNBC.SCR, line/variant 0
- Object spawn/action: Ripstar (object 56, id 10293), subtype 14
- Show/update HUD contact: contact/list 0, subtype 9, param 10
- Hide/remove HUD contact: contact/list 0, subtype 9, param 35
- Set/add variable: variable group 21, variable 24, subtype 0, value 1

### Event 8

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 1300 (extra 1, 10701; join 1; flags 2)
- Variable comparison: subject variable group 21, variable 24, op 1, value 1

**Action**

- Play dialog: WRNBC.SCR, line/variant 0
- Object spawn/action: Ripstar (object 69, id 10710), subtype 14
- Set/add variable: variable group 21, variable 24, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 35
- Show/update HUD contact: contact/list 0, subtype 9, param 10
- Object spawn/action: id 10701, subtype 15

### Event 9

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 1300 (extra 1, 10702; join 1; flags 2)
- Variable comparison: subject variable group 21, variable 24, op 1, value 1

**Action**

- Play dialog: WRNBC.SCR, line/variant 0
- Object spawn/action: Ripstar (object 65, id 10706), subtype 14
- Show/update HUD contact: contact/list 0, subtype 9, param 10
- Hide/remove HUD contact: contact/list 0, subtype 9, param 35
- Set/add variable: variable group 21, variable 24, subtype 0, value 1

### Event 10

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 120

**Action**

- Play dialog: PLAYER.SCR, line/variant 41

### Event 11

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 210

**Action**

- Play dialog: PLAYER.SCR, line/variant 45

### Event 12

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 300

**Action**

- Play dialog: PLAYER.SCR, line/variant 47

### Event 13

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 540

**Action**

- Play dialog: PLAYER.SCR, line/variant 46
- Set runtime trigger variable: variable group 20, variable 0, subtype 1, value 0

### Event 14

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 10279; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 10276; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 10277; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 10275; join 1; flags 2)
- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 4, param 10271
- Show/update HUD contact: contact/list 0, subtype 4, param 10265
- Play dialog: PLAYER.SCR, line/variant 217
- Object spawn/action: Ripstar (object 34, id 10271), subtype 14
- Object spawn/action: Ripstar (object 29, id 10265), subtype 14

### Event 15

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 10714; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 10712; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 10709; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 10713; join 1; flags 2)
- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 4, param 10288
- Play dialog: PLAYER.SCR, line/variant 217
- Object spawn/action: Ripstar (object 51, id 10288), subtype 14

### Event 16

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 10292; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 10293; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 10296; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 10295; join 1; flags 2)
- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 4, param 10285
- Play dialog: PLAYER.SCR, line/variant 217
- Object spawn/action: Ripstar (object 48, id 10285), subtype 14

### Event 17

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 10705; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 10707; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 10706; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 10704; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 10708; join 1; flags 2)
- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 4, param 10254
- Play dialog: PLAYER.SCR, line/variant 217
- Object spawn/action: Ripstar (object 18, id 10254), subtype 14

### Event 18

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 10248; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 10253; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 10247; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 10250; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 400 (extra 1, 10249; join 1; flags 2)
- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 4, param 10244
- Play dialog: PLAYER.SCR, line/variant 217
- Object spawn/action: Ripstar (object 8, id 10244), subtype 14

### Event 19

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 43

**Action**

- Set runtime trigger variable: variable group 20, variable 0, subtype 1, value 0

### Event 20

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 217

**Action**

- Object spawn/action: Ripstar (object 39, id 10276), subtype 15
- Object spawn/action: Ripstar (object 69, id 10710), subtype 15
- Object spawn/action: Ripstar (object 56, id 10293), subtype 15
- Object spawn/action: Ripstar (object 65, id 10706), subtype 15
- Object spawn/action: Ripstar (object 17, id 10253), subtype 15

### Event 21

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Object spawn/action: Ripstar (object 34, id 10271), subtype 15
- Object spawn/action: Ripstar (object 29, id 10265), subtype 15
- Object spawn/action: Ripstar (object 51, id 10288), subtype 15
- Object spawn/action: Ripstar (object 48, id 10285), subtype 15
- Object spawn/action: Ripstar (object 18, id 10254), subtype 15
- Object spawn/action: Ripstar (object 8, id 10244), subtype 15

### Event 22

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 10101; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 10102; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 10121; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 9938; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 9939; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 9940; join 2; flags 2)

**Action**

- Object spawn/action: Ripstar (object 34, id 10271), subtype 15
- Object spawn/action: Ripstar (object 29, id 10265), subtype 15
- Object spawn/action: Ripstar (object 51, id 10288), subtype 15
- Object spawn/action: Ripstar (object 48, id 10285), subtype 15
- Object spawn/action: Ripstar (object 18, id 10254), subtype 15
- Object spawn/action: Ripstar (object 8, id 10244), subtype 15

## Waypoints

### Waypoint 0

- Tag: `104`
- Members: `Bora_Minelayer (object 294, id 9107, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (236.31, 0.00, 13734.17) | None |
| 1 | (-433.18, 0.00, 12385.01) | None |
| 2 | (-1052.36, 0.00, 10177.88) | None |
| 3 | (-3376.63, 0.00, 9055.05) | None |
| 4 | (-2714.14, 0.00, 6730.77) | None |
| 5 | (-779.68, 0.00, 6504.91) | None |
| 6 | (1236.79, 0.00, 6546.21) | None |
| 7 | (3383.21, 0.00, 6956.78) | None |
| 8 | (3581.02, 0.00, 8922.70) | None |
| 9 | (2061.46, 0.00, 10308.55) | None |
| 10 | (1056.38, 0.00, 12074.41) | on arrival redirect to Waypoint 0 (tag 104), point 0 |

### Waypoint 1

- Tag: `103`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1381.57, 0.00, -7697.67) | None |
| 1 | (-398.39, 0.00, -8108.23) | None |
| 2 | (-2492.45, 0.00, -8577.45) | None |
| 3 | (-3040.90, 0.00, -7041.31) | None |
| 4 | (-4611.45, 0.00, -7393.22) | None |
| 5 | (-6222.33, 0.00, -5082.51) | None |
| 6 | (-9178.07, 0.00, -5469.92) | None |
| 7 | (-10044.53, 0.00, -2964.47) | on arrival redirect to Waypoint 3 (tag 101), point 0 |

### Waypoint 2

- Tag: `102`
- Members: `Bora_Minelayer (object 293, id 9094, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (3632.69, 0.00, -8049.58) | None |
| 1 | (5307.94, 0.00, -8988.01) | None |
| 2 | (7506.71, 0.00, -7463.06) | None |
| 3 | (9894.72, 0.00, -2158.77) | None |
| 4 | (10010.04, 0.00, 4444.73) | None |
| 5 | (5868.42, 0.00, 4127.04) | None |
| 6 | (5544.77, 0.00, -2006.22) | None |
| 7 | (3197.08, 0.00, -3919.62) | None |
| 8 | (1888.29, 0.00, -5620.53) | on arrival redirect to Waypoint 1 (tag 103), point 0 |

### Waypoint 3

- Tag: `101`
- Members: `Bora_Minelayer (object 292, id 9074, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-8388.03, 0.00, -844.11) | None |
| 1 | (-8557.64, 0.00, 3350.15) | None |
| 2 | (-6331.46, 0.00, 4044.07) | None |
| 3 | (-5685.02, 0.00, -2278.39) | None |
| 4 | (-1445.42, 0.00, -4941.01) | None |
| 5 | (-974.26, 0.00, -6700.58) | None |
| 6 | (648.65, 0.00, -6641.93) | on arrival redirect to Waypoint 2 (tag 102), point 0 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `KC2_Crystal` | 9938 | Interactive | 864.34,858.90,10111.91 | 0,0,0 | None |
| 1 | `KC2_Crystal` | 9939 | Interactive | 4242.37,157.77,-7384.22 | 0,0,0 | None |
| 2 | `KC2_Crystal` | 9940 | Interactive | -9670.32,176.53,1124.01 | 0,0,0 | None |
| 3 | `KC2_Crystal` | 10101 | Interactive | 6083.71,-458.68,-5100.26 | 0,0,0 | None |
| 4 | `KC2_Crystal` | 10102 | Interactive | 7214.02,-471.40,208.77 | 0,0,0 | None |
| 5 | `KC2_Crystal` | 10121 | Interactive | -4907.47,2072.15,-4065.02 | 0,0,0 | None |
| 6 | `Ripstar` | 10242 | Interactive | -4933.73,2268.69,-3982.72 | 0,0,0 | None |
| 7 | `Ripstar` | 10243 | Interactive | -4916.08,2264.80,-3970.19 | 0,0,0 | None |
| 8 | `Ripstar` | 10244 | Interactive | -4824.43,1900.76,-3997.74 | 0,0,0 | None |
| 9 | `Ripstar` | 10245 | Interactive | -5025.61,2075.27,-4208.62 | 0,0,0 | None |
| 10 | `Ripstar` | 10246 | Interactive | -4837.35,1910.62,-4135.06 | 0,0,0 | None |
| 11 | `Ripstar` | 10247 | Interactive | -6146.31,-162.96,-3720.48 | 0,0,0 | None |
| 12 | `Ripstar` | 10248 | Interactive | -6146.31,-186.76,-3765.75 | 0,0,0 | None |
| 13 | `Ripstar` | 10249 | Interactive | -6146.31,-247.75,-3741.06 | 0,0,0 | None |
| 14 | `Ripstar` | 10250 | Interactive | -6146.31,-209.08,-3691.67 | 0,0,0 | None |
| 15 | `Ripstar` | 10251 | Interactive | -6146.31,-209.08,-3764.38 | 0,0,0 | None |
| 16 | `Ripstar` | 10252 | Interactive | -6146.31,-159.99,-3745.17 | 0,0,0 | None |
| 17 | `Ripstar` | 10253 | Interactive | -6146.31,-215.03,-3721.85 | 0,0,0 | None |
| 18 | `Ripstar` | 10254 | Interactive | -9731.89,9.54,1125.85 | 0,0,0 | None |
| 19 | `Ripstar` | 10255 | Interactive | -9602.29,276.31,1195.80 | 0,0,0 | None |
| 20 | `Ripstar` | 10256 | Interactive | -9566.16,329.39,1099.22 | 0,0,0 | None |
| 21 | `Ripstar` | 10257 | Interactive | -9619.81,18.98,1154.27 | 0,0,0 | None |
| 22 | `Ripstar` | 10258 | Interactive | -9775.26,251.38,1026.35 | 0,0,0 | None |
| 23 | `Ripstar` | 10259 | Interactive | -9647.21,26.24,934.26 | 0,0,0 | None |
| 24 | `Ripstar` | 10260 | Interactive | -9746.33,326.70,1057.42 | 0,0,0 | None |
| 25 | `Ripstar` | 10261 | Interactive | -9728.15,308.31,1022.14 | 0,0,0 | None |
| 26 | `Ripstar` | 10262 | Interactive | 4192.60,20.28,-7338.92 | 0,0,0 | None |
| 27 | `Ripstar` | 10263 | Interactive | 4173.19,14.17,-7378.46 | 0,0,0 | None |
| 28 | `Ripstar` | 10264 | Interactive | 4347.71,116.86,-7492.96 | 0,0,0 | None |
| 29 | `Ripstar` | 10265 | Interactive | 4351.40,286.90,-7387.46 | 0,0,0 | None |
| 30 | `Ripstar` | 10267 | Interactive | 4348.63,170.93,-7269.62 | 0,0,0 | None |
| 31 | `Ripstar` | 10268 | Interactive | 6018.57,-306.32,-4975.42 | 0,0,0 | None |
| 32 | `Ripstar` | 10269 | Interactive | 6071.15,-299.53,-5230.30 | 0,0,0 | None |
| 33 | `Ripstar` | 10270 | Interactive | 6147.22,-264.29,-5138.92 | 0,0,0 | None |
| 34 | `Ripstar` | 10271 | Interactive | 6131.05,-606.89,-4975.11 | 0,0,0 | None |
| 35 | `Ripstar` | 10272 | Interactive | 6126.65,-640.48,-5232.08 | 0,0,0 | None |
| 36 | `Ripstar` | 10273 | Interactive | 6021.67,-669.79,-5131.61 | 0,0,0 | None |
| 37 | `Ripstar` | 10274 | Interactive | 6108.23,-681.20,-4987.99 | 0,0,0 | None |
| 38 | `Ripstar` | 10275 | Interactive | 3965.37,-969.45,-4129.82 | 0,0,0 | None |
| 39 | `Ripstar` | 10276 | Interactive | 3964.12,-973.01,-4158.98 | 0,0,0 | None |
| 40 | `Ripstar` | 10277 | Interactive | 3964.12,-973.01,-4198.76 | 0,0,0 | None |
| 41 | `Ripstar` | 10278 | Interactive | 3964.74,-1022.76,-4206.78 | 0,0,0 | None |
| 42 | `Ripstar` | 10279 | Interactive | 3964.12,-1026.31,-4167.56 | 0,0,0 | None |
| 43 | `Ripstar` | 10280 | Interactive | 3965.37,-1022.76,-4129.82 | 0,0,0 | None |
| 44 | `Ripstar` | 10281 | Interactive | 807.90,1146.50,10225.31 | 0,0,0 | None |
| 45 | `Ripstar` | 10282 | Interactive | 738.16,666.32,9999.29 | 0,0,0 | None |
| 46 | `Ripstar` | 10283 | Interactive | 915.60,1076.49,10264.18 | 0,0,0 | None |
| 47 | `Ripstar` | 10284 | Interactive | 769.12,1097.28,10039.52 | 0,0,0 | None |
| 48 | `Ripstar` | 10285 | Interactive | 914.99,1074.15,10264.71 | 0,0,0 | None |
| 49 | `Ripstar` | 10286 | Interactive | 7324.56,-218.54,150.56 | 0,0,0 | None |
| 50 | `Ripstar` | 10287 | Interactive | 7273.54,-345.72,432.54 | 0,0,0 | None |
| 51 | `Ripstar` | 10288 | Interactive | 7164.80,-611.95,425.07 | 0,0,0 | None |
| 52 | `Ripstar` | 10289 | Interactive | 7257.95,-654.40,-23.68 | 0,0,0 | None |
| 53 | `Ripstar` | 10290 | Interactive | 7184.93,-592.69,-76.42 | 0,0,0 | None |
| 54 | `Ripstar` | 10291 | Interactive | 7242.10,-208.34,58.26 | 0,0,0 | None |
| 55 | `Ripstar` | 10292 | Interactive | -368.68,63.90,7949.11 | 0,0,0 | None |
| 56 | `Ripstar` | 10293 | Interactive | -368.68,17.71,7804.07 | 0,0,0 | None |
| 57 | `Ripstar` | 10294 | Interactive | -368.68,-245.76,7776.25 | 0,0,0 | None |
| 58 | `Ripstar` | 10295 | Interactive | -368.68,-72.79,7998.96 | 0,0,0 | None |
| 59 | `Ripstar` | 10296 | Interactive | -368.68,-164.86,7935.93 | 0,0,0 | None |
| 60 | `Ripstar` | 10297 | Interactive | -368.68,-71.38,7745.53 | 0,0,0 | None |
| 61 | `Ripstar` | 10298 | Interactive | -368.68,149.69,7856.81 | 0,0,0 | None |
| 62 | `Ripstar` | 10703 | Interactive | -7181.73,1487.60,2604.93 | 0,0,0 | None |
| 63 | `Ripstar` | 10704 | Interactive | -7126.68,1410.99,2556.93 | 0,0,0 | None |
| 64 | `Ripstar` | 10705 | Interactive | -7231.12,1515.87,2640.21 | 0,0,0 | None |
| 65 | `Ripstar` | 10706 | Interactive | -7172.93,1515.12,2710.29 | 0,0,0 | None |
| 66 | `Ripstar` | 10707 | Interactive | -7126.68,1330.17,2660.16 | 0,0,0 | None |
| 67 | `Ripstar` | 10708 | Interactive | -7281.87,1421.90,2727.80 | 0,0,0 | None |
| 68 | `Ripstar` | 10709 | Interactive | 4644.50,75.29,529.56 | 0,0,0 | None |
| 69 | `Ripstar` | 10710 | Interactive | 4866.99,147.60,553.44 | 0,0,0 | None |
| 70 | `Ripstar` | 10711 | Interactive | 4797.36,94.63,602.74 | 0,0,0 | None |
| 71 | `Ripstar` | 10712 | Interactive | 4658.10,229.34,546.69 | 0,0,0 | None |
| 72 | `Ripstar` | 10713 | Interactive | 4704.58,113.64,633.36 | 0,0,0 | None |
| 73 | `Ripstar` | 10714 | Interactive | 4901.80,145.87,611.38 | 0,0,0 | None |
| 74 | `Bora_Mine` | 10716 | Interactive | 83.68,323.34,7470.62 | 347,191,29 | None |
| 75 | `Bora_Mine` | 10717 | Interactive | -678.48,-254.05,7320.50 | 82,85,72 | None |
| 76 | `Bora_Mine` | 10718 | Interactive | -262.76,531.20,7412.88 | 11,348,87 | None |
| 77 | `Bora_Mine` | 10719 | Interactive | -863.25,150.12,7482.17 | 474,268,434 | None |
| 78 | `Bora_Mine` | 10720 | Interactive | -770.87,-103.93,7620.74 | 417,33,124 | None |
| 79 | `Bora_Mine` | 10721 | Interactive | -886.35,-184.77,7736.22 | 181,249,368 | None |
| 80 | `Bora_Mine` | 10722 | Interactive | -459.07,577.40,7874.80 | 290,406,189 | None |
| 81 | `Bora_Mine` | 10723 | Interactive | -759.32,-127.03,8094.21 | 401,54,208 | None |
| 82 | `Bora_Mine` | 10724 | Interactive | -701.58,-427.27,8013.37 | 282,338,394 | None |
| 83 | `Bora_Mine` | 10725 | Interactive | -401.33,-531.20,8048.02 | 230,70,56 | None |
| 84 | `Bora_Mine` | 10726 | Interactive | -66.44,-369.53,8417.55 | 302,466,445 | None |
| 85 | `Bora_Mine` | 10727 | Interactive | -320.50,254.05,7308.95 | 367,239,423 | None |
| 86 | `Bora_Mine` | 10728 | Interactive | -170.38,496.56,7840.15 | 505,437,49 | None |
| 87 | `Bora_Mine` | 10729 | Interactive | -597.65,-161.67,7447.53 | 287,320,90 | None |
| 88 | `Bora_Mine` | 10730 | Interactive | -586.10,-173.22,7747.77 | 170,222,147 | None |
| 89 | `Bora_Mine` | 10731 | Interactive | 187.61,311.79,8267.43 | 102,480,445 | None |
| 90 | `Bora_Mine` | 10732 | Interactive | -308.95,161.67,8059.56 | 222,234,360 | None |
| 91 | `Bora_Mine` | 10733 | Interactive | -262.76,115.48,7805.51 | 421,153,404 | None |
| 92 | `Bora_Mine` | 10734 | Interactive | -366.69,-473.46,7770.87 | 186,212,351 | None |
| 93 | `Bora_Mine` | 10735 | Interactive | -586.10,-485.01,7701.58 | 238,292,361 | None |
| 94 | `Bora_Mine` | 10737 | Interactive | 1331.99,1296.39,9593.47 | 40,490,478 | None |
| 95 | `Bora_Mine` | 10738 | Interactive | 962.46,1619.73,9847.53 | 299,42,209 | None |
| 96 | `Bora_Mine` | 10739 | Interactive | 535.18,892.21,10217.06 | 450,236,311 | None |
| 97 | `Bora_Mine` | 10740 | Interactive | 1308.89,1492.70,9558.83 | 127,386,478 | None |
| 98 | `Bora_Mine` | 10741 | Interactive | 1366.63,1273.29,9639.66 | 275,238,165 | None |
| 99 | `Bora_Mine` | 10742 | Interactive | 1343.54,1007.69,10101.58 | 352,43,330 | None |
| 100 | `Bora_Mine` | 10743 | Interactive | 1389.73,1088.53,9639.66 | 171,41,391 | None |
| 101 | `Bora_Mine` | 10744 | Interactive | 1239.61,1307.94,9685.86 | 496,51,369 | None |
| 102 | `Bora_Mine` | 10745 | Interactive | 488.99,1458.06,10297.89 | 209,187,86 | None |
| 103 | `Bora_Mine` | 10746 | Interactive | 835.43,1631.28,9986.10 | 152,457,403 | None |
| 104 | `Bora_Mine` | 10748 | Interactive | 1498.43,-608.26,7477.12 | 280,212,363 | None |
| 105 | `Bora_Mine` | 10749 | Interactive | 1764.03,-804.57,7430.93 | 27,273,38 | None |
| 106 | `Bora_Mine` | 10750 | Interactive | 2202.85,-1127.92,7384.74 | 273,122,342 | None |
| 107 | `Bora_Mine` | 10751 | Interactive | 1844.86,-689.10,8216.19 | 506,215,315 | None |
| 108 | `Bora_Mine` | 10752 | Interactive | 2122.01,-700.64,7881.30 | 244,161,208 | None |
| 109 | `Bora_Mine` | 10753 | Interactive | 1394.49,-1312.68,7892.85 | 190,262,371 | None |
| 110 | `Bora_Mine` | 10754 | Interactive | 1198.18,-700.64,7731.18 | 107,61,388 | None |
| 111 | `Bora_Mine` | 10755 | Interactive | 1775.57,-954.70,8308.57 | 115,492,474 | None |
| 112 | `Bora_Mine` | 10756 | Interactive | 1117.34,-296.47,8019.88 | 348,142,354 | None |
| 113 | `Bora_Mine` | 10757 | Interactive | 1948.79,-458.14,8297.03 | 182,30,331 | None |
| 114 | `Bora_Mine` | 10759 | Interactive | 6486.60,-402.34,453.13 | 267,413,264 | None |
| 115 | `Bora_Mine` | 10760 | Interactive | 6417.31,-21.26,464.68 | 232,472,476 | None |
| 116 | `Bora_Mine` | 10761 | Interactive | 6405.76,-564.01,441.58 | 48,170,3 | None |
| 117 | `Bora_Mine` | 10762 | Interactive | 6936.97,-968.19,-366.77 | 465,141,322 | None |
| 118 | `Bora_Mine` | 10763 | Interactive | 7179.47,-425.44,522.42 | 511,314,98 | None |
| 119 | `Bora_Mine` | 10764 | Interactive | 7329.60,-656.40,326.10 | 489,11,114 | None |
| 120 | `Bora_Mine` | 10765 | Interactive | 6717.56,-587.11,129.79 | 492,225,313 | None |
| 121 | `Bora_Mine` | 10766 | Interactive | 7352.69,-818.07,-147.36 | 80,358,199 | None |
| 122 | `Bora_Mine` | 10767 | Interactive | 6717.56,-656.40,-297.49 | 248,396,364 | None |
| 123 | `Bora_Mine` | 10768 | Interactive | 6717.56,-229.13,-412.96 | 135,395,123 | None |
| 124 | `Bora_Mine` | 10770 | Interactive | 6176.87,660.71,2326.65 | 322,27,202 | None |
| 125 | `Bora_Mine` | 10771 | Interactive | 7054.51,-170.74,3158.10 | 233,340,110 | None |
| 126 | `Bora_Mine` | 10772 | Interactive | 6754.27,-159.19,2349.75 | 99,72,368 | None |
| 127 | `Bora_Mine` | 10773 | Interactive | 6985.22,-78.35,2384.39 | 119,158,455 | None |
| 128 | `Bora_Mine` | 10774 | Interactive | 6338.54,672.26,2176.53 | 293,474,158 | None |
| 129 | `Bora_Mine` | 10775 | Interactive | 6777.36,660.71,2950.24 | 292,110,82 | None |
| 130 | `Bora_Mine` | 10776 | Interactive | 6581.05,25.58,2973.34 | 92,455,202 | None |
| 131 | `Bora_Mine` | 10777 | Interactive | 6407.83,-9.07,2661.54 | 59,210,475 | None |
| 132 | `Bora_Mine` | 10778 | Interactive | 6696.53,372.01,2349.75 | 249,427,178 | None |
| 133 | `Bora_Mine` | 10779 | Interactive | 6788.91,672.26,2118.79 | 298,111,121 | None |
| 134 | `Bora_Mine` | 10781 | Interactive | 5090.90,804.36,539.30 | 195,17,123 | None |
| 135 | `Bora_Mine` | 10782 | Interactive | 4906.13,792.81,1301.47 | 119,286,154 | None |
| 136 | `Bora_Mine` | 10783 | Interactive | 5194.83,-27.09,562.40 | 392,317,8 | None |
| 137 | `Bora_Mine` | 10784 | Interactive | 5310.31,307.80,1382.30 | 360,437,27 | None |
| 138 | `Bora_Mine` | 10785 | Interactive | 5229.47,515.66,1405.40 | 44,309,462 | None |
| 139 | `Bora_Mine` | 10786 | Interactive | 5137.09,665.79,493.11 | 468,378,467 | None |
| 140 | `Bora_Mine` | 10787 | Interactive | 5021.61,250.06,1220.63 | 463,67,486 | None |
| 141 | `Bora_Mine` | 10788 | Interactive | 4802.20,-73.28,1082.05 | 60,278,60 | None |
| 142 | `Bora_Mine` | 10789 | Interactive | 4617.43,504.11,793.36 | 393,466,27 | None |
| 143 | `Bora_Mine` | 10790 | Interactive | 5113.99,457.92,1220.63 | 135,5,260 | None |
| 144 | `Bora_Mine` | 10792 | Interactive | 5788.53,-724.71,-5043.37 | 395,383,27 | None |
| 145 | `Bora_Mine` | 10793 | Interactive | 5626.86,-1290.56,-4893.25 | 405,308,97 | None |
| 146 | `Bora_Mine` | 10794 | Interactive | 6181.16,-505.30,-4720.03 | 415,392,461 | None |
| 147 | `Bora_Mine` | 10795 | Interactive | 6007.94,-493.75,-4315.85 | 164,465,62 | None |
| 148 | `Bora_Mine` | 10796 | Interactive | 5638.41,-840.19,-5412.90 | 275,330,497 | None |
| 149 | `Bora_Mine` | 10797 | Interactive | 5730.79,-574.59,-4523.71 | 503,305,245 | None |
| 150 | `Bora_Mine` | 10798 | Interactive | 6134.97,-228.15,-4512.16 | 69,83,143 | None |
| 151 | `Bora_Mine` | 10799 | Interactive | 5880.91,-574.59,-4650.74 | 83,48,489 | None |
| 152 | `Bora_Mine` | 10800 | Interactive | 6158.06,-574.59,-4754.67 | 168,2,420 | None |
| 153 | `Bora_Mine` | 10801 | Interactive | 6146.52,-1244.37,-4835.51 | 160,75,30 | None |
| 154 | `Bora_Mine` | 10803 | Interactive | 4460.75,-1490.43,-3843.12 | 481,26,463 | None |
| 155 | `Bora_Mine` | 10804 | Interactive | 3975.74,-1224.83,-4443.61 | 371,77,157 | None |
| 156 | `Bora_Mine` | 10805 | Interactive | 4310.63,-1374.95,-3669.90 | 445,152,381 | None |
| 157 | `Bora_Mine` | 10806 | Interactive | 3975.74,-1744.49,-3958.60 | 250,333,174 | None |
| 158 | `Bora_Mine` | 10807 | Interactive | 3975.74,-843.75,-4420.52 | 414,239,154 | None |
| 159 | `Bora_Mine` | 10808 | Interactive | 4229.79,-1698.30,-4385.87 | 174,60,159 | None |
| 160 | `Bora_Mine` | 10809 | Interactive | 4206.70,-1605.91,-4270.39 | 142,20,266 | None |
| 161 | `Bora_Mine` | 10810 | Interactive | 4079.67,-1144.00,-4305.04 | 186,347,140 | None |
| 162 | `Bora_Mine` | 10811 | Interactive | 3652.40,-1040.06,-3843.12 | 71,186,146 | None |
| 163 | `Bora_Mine` | 10812 | Interactive | 3871.81,-1698.30,-4293.49 | 354,410,327 | None |
| 164 | `Bora_Mine` | 10814 | Interactive | 3947.59,-152.50,-7194.55 | 373,206,375 | None |
| 165 | `Bora_Mine` | 10815 | Interactive | 4259.39,20.72,-7514.66 | 235,127,145 | None |
| 166 | `Bora_Mine` | 10816 | Interactive | 4698.21,344.06,-6405.71 | 382,302,66 | None |
| 167 | `Bora_Mine` | 10817 | Interactive | 4594.28,-48.57,-7434.63 | 267,0,415 | None |
| 168 | `Bora_Mine` | 10818 | Interactive | 4432.61,-94.76,-7000.20 | 378,73,486 | None |
| 169 | `Bora_Mine` | 10819 | Interactive | 4444.15,413.35,-6474.31 | 490,398,158 | None |
| 170 | `Bora_Mine` | 10820 | Interactive | 4016.88,-533.58,-7526.09 | 198,186,358 | None |
| 171 | `Bora_Mine` | 10821 | Interactive | 4143.91,575.02,-7160.25 | 197,167,201 | None |
| 172 | `Bora_Mine` | 10822 | Interactive | 4340.22,263.23,-7148.82 | 1,84,437 | None |
| 173 | `Bora_Mine` | 10823 | Interactive | 3809.02,-452.74,-7388.90 | 423,343,365 | None |
| 174 | `Bora_Mine` | 10825 | Interactive | -4619.48,517.28,-5067.57 | 215,167,310 | None |
| 175 | `Bora_Mine` | 10826 | Interactive | -4861.98,240.13,-5044.47 | 156,172,274 | None |
| 176 | `Bora_Mine` | 10827 | Interactive | -3915.05,-337.26,-5240.79 | 185,177,151 | None |
| 177 | `Bora_Mine` | 10828 | Interactive | -4654.12,9.17,-5899.02 | 76,428,7 | None |
| 178 | `Bora_Mine` | 10829 | Interactive | -3938.15,494.19,-6118.43 | 196,366,400 | None |
| 179 | `Bora_Mine` | 10830 | Interactive | -4469.35,344.06,-5113.76 | 45,320,90 | None |
| 180 | `Bora_Mine` | 10831 | Interactive | -4850.44,-106.31,-5795.09 | 118,115,285 | None |
| 181 | `Bora_Mine` | 10832 | Interactive | -4169.11,-487.39,-6002.95 | 127,321,380 | None |
| 182 | `Bora_Mine` | 10833 | Interactive | -4561.74,263.23,-5079.12 | 1,354,386 | None |
| 183 | `Bora_Mine` | 10834 | Interactive | -4423.16,-314.17,-5806.63 | 353,31,425 | None |
| 184 | `Bora_Mine` | 10836 | Interactive | -4845.62,2136.68,-4538.03 | 315,94,262 | None |
| 185 | `Bora_Mine` | 10837 | Interactive | -4325.96,2171.33,-3879.80 | 42,183,501 | None |
| 186 | `Bora_Mine` | 10838 | Interactive | -5342.18,1640.12,-3798.96 | 453,215,377 | None |
| 187 | `Bora_Mine` | 10839 | Interactive | -5469.21,1605.48,-3683.48 | 490,442,281 | None |
| 188 | `Bora_Mine` | 10840 | Interactive | -4499.18,1813.34,-3718.13 | 312,376,162 | None |
| 189 | `Bora_Mine` | 10841 | Interactive | -4360.61,2113.59,-4307.07 | 63,283,235 | None |
| 190 | `Bora_Mine` | 10842 | Interactive | -4464.54,1443.81,-3452.52 | 380,59,88 | None |
| 191 | `Bora_Mine` | 10843 | Interactive | -5284.44,1640.12,-4376.36 | 385,0,499 | None |
| 192 | `Bora_Mine` | 10844 | Interactive | -4556.92,2125.14,-4480.29 | 14,345,65 | None |
| 193 | `Bora_Mine` | 10845 | Interactive | -4995.74,2182.87,-3822.06 | 13,133,270 | None |
| 194 | `Bora_Mine` | 10847 | Interactive | -5608.32,-172.89,-3946.32 | 276,199,211 | None |
| 195 | `Bora_Mine` | 10848 | Interactive | -6093.33,-149.80,-4119.54 | 214,414,196 | None |
| 196 | `Bora_Mine` | 10849 | Interactive | -6070.24,150.45,-3357.37 | 154,219,254 | None |
| 197 | `Bora_Mine` | 10850 | Interactive | -6382.03,-103.61,-3449.76 | 202,201,135 | None |
| 198 | `Bora_Mine` | 10851 | Interactive | -6024.05,531.53,-3311.18 | 216,424,382 | None |
| 199 | `Bora_Mine` | 10852 | Interactive | -5700.71,242.83,-3403.57 | 155,280,464 | None |
| 200 | `Bora_Mine` | 10853 | Interactive | -6428.22,473.79,-3403.57 | 132,251,251 | None |
| 201 | `Bora_Mine` | 10854 | Interactive | -6451.32,323.67,-4038.70 | 453,133,474 | None |
| 202 | `Bora_Mine` | 10855 | Interactive | -6035.60,-34.32,-3241.90 | 442,370,166 | None |
| 203 | `Bora_Mine` | 10856 | Interactive | -5723.80,231.28,-3784.65 | 181,77,166 | None |
| 204 | `Bora_Mine` | 10858 | Interactive | -9428.45,150.12,680.14 | 461,308,157 | None |
| 205 | `Bora_Mine` | 10859 | Interactive | -9451.54,496.56,1696.35 | 453,266,391 | None |
| 206 | `Bora_Mine` | 10860 | Interactive | -9416.90,277.15,1315.27 | 438,202,433 | None |
| 207 | `Bora_Mine` | 10861 | Interactive | -9405.35,-254.05,1095.86 | 415,11,352 | None |
| 208 | `Bora_Mine` | 10862 | Interactive | -9878.82,381.08,1153.60 | 403,187,366 | None |
| 209 | `Bora_Mine` | 10863 | Interactive | -9024.27,311.79,1165.15 | 189,400,26 | None |
| 210 | `Bora_Mine` | 10864 | Interactive | -9636.31,-161.67,1245.99 | 469,41,359 | None |
| 211 | `Bora_Mine` | 10865 | Interactive | -9636.31,173.22,818.71 | 93,210,303 | None |
| 212 | `Bora_Mine` | 10866 | Interactive | -9682.50,473.46,1234.44 | 68,295,108 | None |
| 213 | `Bora_Mine` | 10867 | Interactive | -10052.04,334.89,657.04 | 443,9,113 | None |
| 214 | `Bora_Mine` | 10869 | Interactive | -6958.80,986.86,3141.37 | 369,233,26 | None |
| 215 | `Bora_Mine` | 10870 | Interactive | -7778.70,1494.97,3014.34 | 363,487,126 | None |
| 216 | `Bora_Mine` | 10871 | Interactive | -7755.60,1575.80,2367.66 | 114,444,393 | None |
| 217 | `Bora_Mine` | 10872 | Interactive | -6970.34,1333.29,2633.26 | 23,407,412 | None |
| 218 | `Bora_Mine` | 10873 | Interactive | -7813.34,1056.14,3002.79 | 323,487,469 | None |
| 219 | `Bora_Mine` | 10874 | Interactive | -7328.33,1229.36,2864.22 | 266,366,247 | None |
| 220 | `Bora_Mine` | 10875 | Interactive | -7062.73,1725.92,2217.53 | 275,393,106 | None |
| 221 | `Bora_Mine` | 10876 | Interactive | -6970.34,1033.05,2217.53 | 19,50,326 | None |
| 222 | `Bora_Mine` | 10877 | Interactive | -7709.41,1979.98,2090.51 | 31,155,345 | None |
| 223 | `Bora_Mine` | 10878 | Interactive | -7120.47,1425.68,2275.27 | 441,380,171 | None |
| 224 | `Bora_Mine` | 10880 | Interactive | -4986.39,-1450.61,781.44 | 225,478,502 | None |
| 225 | `Bora_Mine` | 10881 | Interactive | -5263.54,-1912.52,1220.26 | 204,262,423 | None |
| 226 | `Bora_Mine` | 10882 | Interactive | -5321.28,-2120.39,885.37 | 156,85,271 | None |
| 227 | `Bora_Mine` | 10883 | Interactive | -5563.79,-2409.08,1070.14 | 161,469,165 | None |
| 228 | `Bora_Mine` | 10884 | Interactive | -5228.90,-2316.70,781.44 | 30,63,208 | None |
| 229 | `Bora_Mine` | 10885 | Interactive | -5298.18,-1508.35,735.25 | 441,316,415 | None |
| 230 | `Bora_Mine` | 10886 | Interactive | -5344.38,-1854.78,1185.61 | 352,290,331 | None |
| 231 | `Bora_Mine` | 10887 | Interactive | -5251.99,-1577.63,1174.07 | 148,424,335 | None |
| 232 | `Bora_Mine` | 10888 | Interactive | -5448.31,-1450.61,1647.53 | 26,71,253 | None |
| 233 | `Bora_Mine` | 10889 | Interactive | -5148.06,-2004.91,1405.03 | 121,59,472 | None |
| 234 | `Ripstar_Gravity` | 11281 | Object | -4916.91,2266.85,-3970.42 | 0,0,0 | Scale/Radius: 1.00 |
| 235 | `Ripstar_Gravity` | 11282 | Object | -4934.02,2267.02,-3983.00 | 0,0,0 | Scale/Radius: 1.00 |
| 236 | `Ripstar_Gravity` | 11283 | Object | -4824.53,1902.96,-3997.62 | 0,0,0 | Scale/Radius: 1.00 |
| 237 | `Ripstar_Gravity` | 11284 | Object | -4837.45,1909.67,-4134.59 | 0,0,0 | Scale/Radius: 1.00 |
| 238 | `Ripstar_Gravity` | 11285 | Object | -5025.99,2073.17,-4208.93 | 0,0,0 | Scale/Radius: 1.00 |
| 239 | `Ripstar_Gravity` | 11286 | Object | -6146.78,-167.18,-3718.07 | 0,0,0 | Scale/Radius: 1.00 |
| 240 | `Ripstar_Gravity` | 11287 | Object | -6146.78,-218.75,-3724.59 | 0,0,0 | Scale/Radius: 1.00 |
| 241 | `Ripstar_Gravity` | 11288 | Object | -6146.15,-250.98,-3739.19 | 0,0,0 | Scale/Radius: 1.00 |
| 242 | `Ripstar_Gravity` | 11289 | Object | -6145.80,-214.45,-3766.12 | 0,0,0 | Scale/Radius: 1.00 |
| 243 | `Ripstar_Gravity` | 11290 | Object | -6146.17,-212.31,-3692.90 | 0,0,0 | Scale/Radius: 1.00 |
| 244 | `Ripstar_Gravity` | 11291 | Object | -6146.78,-162.88,-3746.44 | 0,0,0 | Scale/Radius: 1.00 |
| 245 | `Ripstar_Gravity` | 11292 | Object | -6146.45,-182.22,-3763.90 | 0,0,0 | Scale/Radius: 1.00 |
| 246 | `Ripstar_Gravity` | 11293 | Object | 3963.90,-1032.01,-4128.46 | 0,0,0 | Scale/Radius: 1.00 |
| 247 | `Ripstar_Gravity` | 11294 | Object | 3963.90,-1022.34,-4167.10 | 0,0,0 | Scale/Radius: 1.00 |
| 248 | `Ripstar_Gravity` | 11295 | Object | 3963.90,-973.99,-4161.16 | 0,0,0 | Scale/Radius: 1.00 |
| 249 | `Ripstar_Gravity` | 11296 | Object | 3963.90,-1015.89,-4205.74 | 0,0,0 | Scale/Radius: 1.00 |
| 250 | `Ripstar_Gravity` | 11297 | Object | 3963.90,-967.54,-4196.83 | 0,0,0 | Scale/Radius: 1.00 |
| 251 | `Ripstar_Gravity` | 11298 | Object | 3963.90,-967.54,-4128.46 | 0,0,0 | Scale/Radius: 1.00 |
| 252 | `Ripstar_Gravity` | 11299 | Object | 6147.67,-262.61,-5137.13 | 0,0,0 | Scale/Radius: 1.00 |
| 253 | `Ripstar_Gravity` | 11300 | Object | 6019.49,-304.27,-4973.05 | 0,0,0 | Scale/Radius: 1.00 |
| 254 | `Ripstar_Gravity` | 11301 | Object | 6127.57,-642.36,-5232.11 | 0,0,0 | Scale/Radius: 1.00 |
| 255 | `Ripstar_Gravity` | 11302 | Object | 6023.07,-666.93,-5132.46 | 0,0,0 | Scale/Radius: 1.00 |
| 256 | `Ripstar_Gravity` | 11306 | Object | 4352.20,284.92,-7386.26 | 0,0,0 | Scale/Radius: 1.00 |
| 257 | `Ripstar_Gravity` | 11309 | Object | 4349.82,168.84,-7270.37 | 0,0,0 | Scale/Radius: 1.00 |
| 258 | `Ripstar_Gravity` | 11311 | Object | 4348.91,119.46,-7493.81 | 0,0,0 | Scale/Radius: 1.00 |
| 259 | `Ripstar_Gravity` | 11313 | Object | 7241.95,-212.14,56.93 | 0,0,0 | Scale/Radius: 1.00 |
| 260 | `Ripstar_Gravity` | 11317 | Object | 7184.78,-592.35,-74.63 | 0,0,0 | Scale/Radius: 1.00 |
| 261 | `Ripstar_Gravity` | 11318 | Object | 4705.21,119.87,639.08 | 0,0,0 | Scale/Radius: 1.00 |
| 262 | `Ripstar_Gravity` | 11319 | Object | 4894.51,150.28,611.11 | 0,0,0 | Scale/Radius: 1.00 |
| 263 | `Ripstar_Gravity` | 11320 | Object | 4662.53,233.92,556.80 | 0,0,0 | Scale/Radius: 1.00 |
| 264 | `Ripstar_Gravity` | 11321 | Object | 4645.92,85.65,523.61 | 0,0,0 | Scale/Radius: 1.00 |
| 265 | `Ripstar_Gravity` | 11322 | Object | 4788.21,70.44,597.01 | 0,0,0 | Scale/Radius: 1.00 |
| 266 | `Ripstar_Gravity` | 11323 | Object | 4864.78,150.28,559.03 | 0,0,0 | Scale/Radius: 1.00 |
| 267 | `Ripstar_Gravity` | 11325 | Object | -9620.50,20.79,1153.52 | 0,0,0 | Scale/Radius: 1.00 |
| 268 | `Ripstar_Gravity` | 11326 | Object | -9777.71,252.78,1026.88 | 0,0,0 | Scale/Radius: 1.00 |
| 269 | `Ripstar_Gravity` | 11327 | Object | -9748.12,328.90,1055.73 | 0,0,0 | Scale/Radius: 1.00 |
| 270 | `Ripstar_Gravity` | 11328 | Object | -9728.30,310.79,1022.02 | 0,0,0 | Scale/Radius: 1.00 |
| 271 | `Ripstar_Gravity` | 11329 | Object | -9733.68,6.49,1126.14 | 0,0,0 | Scale/Radius: 1.00 |
| 272 | `Ripstar_Gravity` | 11330 | Object | -9566.76,332.00,1099.01 | 0,0,0 | Scale/Radius: 1.00 |
| 273 | `Ripstar_Gravity` | 11331 | Object | -9647.61,23.94,935.06 | 0,0,0 | Scale/Radius: 1.00 |
| 274 | `Ripstar_Gravity` | 11334 | Object | -7279.02,1421.43,2725.04 | 0,0,0 | Scale/Radius: 1.00 |
| 275 | `Ripstar_Gravity` | 11335 | Object | -7177.18,1486.72,2607.91 | 0,0,0 | Scale/Radius: 1.00 |
| 276 | `Ripstar_Gravity` | 11336 | Object | -7133.00,1408.37,2558.81 | 0,0,0 | Scale/Radius: 1.00 |
| 277 | `Ripstar_Gravity` | 11338 | Object | -7123.58,1332.97,2657.34 | 0,0,0 | Scale/Radius: 1.00 |
| 278 | `Ripstar_Gravity` | 11339 | Object | -7226.87,1514.45,2642.09 | 0,0,0 | Scale/Radius: 1.00 |
| 279 | `Ripstar_Gravity` | 11340 | Object | -7170.29,1512.40,2714.41 | 0,0,0 | Scale/Radius: 1.00 |
| 280 | `Ripstar_Gravity` | 11341 | Object | -368.19,-171.75,7933.86 | 0,0,0 | Scale/Radius: 1.00 |
| 281 | `Ripstar_Gravity` | 11342 | Object | -366.17,-248.11,7780.48 | 0,0,0 | Scale/Radius: 1.00 |
| 282 | `Ripstar_Gravity` | 11343 | Object | -366.17,-67.62,7998.17 | 0,0,0 | Scale/Radius: 1.00 |
| 283 | `Ripstar_Gravity` | 11344 | Object | -368.19,59.82,7948.34 | 0,0,0 | Scale/Radius: 1.00 |
| 284 | `Ripstar_Gravity` | 11345 | Object | -366.17,-74.56,7748.47 | 0,0,0 | Scale/Radius: 1.00 |
| 285 | `Ripstar_Gravity` | 11346 | Object | -368.19,140.65,7859.21 | 0,0,0 | Scale/Radius: 1.00 |
| 286 | `Ripstar_Gravity` | 11347 | Object | -367.18,22.63,7802.02 | 0,0,0 | Scale/Radius: 1.00 |
| 287 | `Ripstar_Gravity` | 11348 | Object | 963.14,589.27,10077.10 | 0,0,0 | Scale/Radius: 1.00 |
| 288 | `Ripstar_Gravity` | 11349 | Object | 964.36,590.81,10088.07 | 0,0,0 | Scale/Radius: 1.00 |
| 289 | `Ripstar_Gravity` | 11350 | Object | 737.10,668.12,10000.73 | 0,0,0 | Scale/Radius: 1.00 |
| 290 | `Ripstar_Gravity` | 11351 | Object | 807.37,1144.70,10226.85 | 0,0,0 | Scale/Radius: 1.00 |
| 291 | `Ripstar_Gravity` | 11352 | Object | 768.05,1099.31,10039.15 | 0,0,0 | Scale/Radius: 1.00 |
| 292 | `Bora_Minelayer` | 9074 | Interactive | -9033.05,0.00,-2216.40 | 64,0,0 | waypoint: Waypoint 3 (tag 101, 7 point(s)), starting point 0, arrival event value 6619136 |
| 293 | `Bora_Minelayer` | 9094 | Interactive | 2742.71,0.00,-7228.45 | 171,0,0 | waypoint: Waypoint 2 (tag 102, 9 point(s)), starting point 0, arrival event value 6684672 |
| 294 | `Bora_Minelayer` | 9107 | Interactive | 1219.83,0.00,14427.60 | 388,0,0 | waypoint: Waypoint 0 (tag 104, 11 point(s)), starting point 0, arrival event value 6815744 |
