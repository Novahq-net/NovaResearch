# Tachyon: The Fringe DISP03F.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP03F.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 18 |
| Entities | 80 |
| Events | 18 |
| Waypoints | 17 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bflat03_GC10_Only`, `1: Bflat04_GC10_Only`, `2: GalSpan_Cruiser`, `3: Zeus_GalSpan_Carrier`, `4: Roid_Med_Brown`, `5: Bora_Mace`, `6: Mars_Billboard_GC10_Cinematic`, `7: Bora_Shuttle_Medium`, `8: GalSpan_Pegasus`, `9: GalSpan_Poseidon`, `10: GalSpan_Archangel`, `11: Roid_Sm_Brown2`, `12: Roid_Sm_Brown`, `13: Bora_Warhammer`, `14: Bora_Battleaxe`, `15: TNS_Inquirer`, `16: GalSpan_Orion`, `17: Hyper_Gate` |
| Scripts | `CANST.SCR`, `PLAYER.SCR`, `TNSA.SCR` |
| Scenes | None |
| Labels | `BFGE_02`, `BFBE_07`, `TNSA`, `BFBE_09`, `adder1`, `BFBF_07`, `ROSS`, `SPIKE`, `atkin`, `cruiser1` |
| Aliases | `fake_2`, `BC10_Waraxe`, `Coward`, `spy_1`, `fake_1`, `tnsa`, `BC10_Claymore4`, `BC10_Claymore3`, `BC10_Claymore2`, `BC10_Claymore1`, `BC10_Warhammer4`, `BC10_Warhammer3`, `BC10_Warhammer2`, `BC10_Warhammer1`, `BC10_Mace3`, `BC10_Mace4`, `BC10_Mace1`, `BC10_Mace2`, `Galileo`, `SPIKE`, `zeus`, `Stocks01` |
| Groups | `FG_MUSCA`, `TNS_INQUIRER`, `CONT_005`, `FG_ANVIL`, `FG_NOBLE`, `FG_AGENOR`, `FG_AFFAIRE`, `FG_AEGIPAN`, `FG_ADDER`, `FG_CAELUM`, `FG_CALLISTO`, `FG_DEATH`, `FG_DESPOT`, `FG_ELITE`, `FG_FAITH`, `FG_HAMMER`, `FG_DEGAS`, `FG_DELSEMME`, `FG_ACE`, `ZEUS`, `ACHILLES` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Group/spawn-list action: spawn list/group 275, subtype 3, param 2

### Event 1

**Trigger**

- Object event: subject GalSpan_Orion (object 1, id 10188), op 7, value 0
- Object event: subject GalSpan_Orion (object 2, id 10189), op 7, value 0
- Object event: subject GalSpan_Orion (object 3, id 10190), op 7, value 0
- Object event: subject GalSpan_Orion (object 4, id 10191), op 7, value 0

**Action**

- Set/add variable: variable group 21, variable 24, subtype 1, value 1

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Object spawn/action: Zeus_GalSpan_Carrier (object 76, id 10899), subtype 3
- Object spawn/action: TNS_Inquirer (object 5, id 10232), subtype 1, param 2
- Play dialog: CANST.SCR, line/variant 8

### Event 3

**Trigger**

- Object event: subject TNS_Inquirer (object 5, id 10232), op 15, value 0

**Action**

- Object spawn/action: TNS_Inquirer (object 5, id 10232), subtype 2, param 1

### Event 4

**Trigger**

- Object arrival: Zeus_GalSpan_Carrier (object 76, id 10899) reached Waypoint 16 (tag 351), point 0 (raw value 23003136)

**Action**

- Object spawn/action: Zeus_GalSpan_Carrier (object 76, id 10899), subtype 6

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 8, variable 3, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 262, subtype 0
- Group/spawn-list action: spawn list/group 190, subtype 0
- Show/update HUD contact: contact/list 0, subtype 9, param 28
- Object spawn/action: Zeus_GalSpan_Carrier (object 76, id 10899), subtype 14
- Play dialog: PLAYER.SCR, line/variant 161
- Object spawn/action: TNS_Inquirer (object 14, id 11009), subtype 1, param 1

### Event 6

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 161
- Variable comparison: subject variable group 20, variable 9, op 3, value 1

**Action**

- Group/spawn-list action: spawn list/group 15, subtype 1, param 6591
- Play dialog: TNSA.SCR, line/variant 8

### Event 7

**Trigger**

- Group/spawn-list event: subject 15, op 0, value 0

**Action**

- Group/spawn-list action: spawn list/group 42, subtype 0
- Play dialog: PLAYER.SCR, line/variant 172

### Event 8

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 10899; flags 2)

**Action**

- Play scene: unknown index 0, param 1
- Group/spawn-list action: spawn list/group 216, subtype 0
- Group/spawn-list action: spawn list/group 224, subtype 0
- Set runtime trigger variable: variable group 20, variable 9, subtype 0, value 0
- Set/add variable: variable group 18, variable 410, subtype 0, value 1
- Set/add variable: variable group 18, variable 411, subtype 0, value 2

### Event 9

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 15, subtype 3, param 6591
- Group/spawn-list action: spawn list/group 262, subtype 3, param 6591
- Group/spawn-list action: spawn list/group 42, subtype 3, param 6591
- Group/spawn-list action: spawn list/group 190, subtype 3, param 6591

### Event 10

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 54

**Action**

- Object spawn/action: GalSpan_Cruiser (object 77, id 11086), subtype 0
- Object spawn/action: Bflat04_GC10_Only (object 78, id 11365), subtype 0

### Event 11

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 55

**Action**

- Group/spawn-list action: spawn list/group 243, subtype 0
- Group/spawn-list action: spawn list/group 95, subtype 0

### Event 12

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 56

**Action**

- Group/spawn-list action: spawn list/group 270, subtype 0
- Group/spawn-list action: spawn list/group 67, subtype 0
- Group/spawn-list action: spawn list/group 148, subtype 0

### Event 13

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 74

**Action**

- Object spawn/action: Bflat03_GC10_Only (object 79, id 11366), subtype 0
- Object spawn/action: Bflat03_GC10_Only (object 79, id 11366), subtype 21, param 11

### Event 14

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 85

**Action**

- Group/spawn-list action: spawn list/group 61, subtype 0
- Group/spawn-list action: spawn list/group 220, subtype 0
- Group/spawn-list action: spawn list/group 31, subtype 0
- Group/spawn-list action: spawn list/group 86, subtype 0

### Event 15

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 87

**Action**

- Group/spawn-list action: spawn list/group 271, subtype 0

### Event 16

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 144

**Action**

- Object spawn/action: Mars_Billboard_GC10_Cinematic (object 51, id 11266), subtype 0

### Event 17

**Trigger**

- Object arrival: GalSpan_Cruiser (object 77, id 11086) reached Waypoint 9 (tag 358), point 1 (raw value 23461889)

**Action**

- Object spawn/action: GalSpan_Cruiser (object 77, id 11086), subtype 19

## Waypoints

### Waypoint 0

- Tag: `396`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (28405.65, 0.00, -232.51) | None |

### Waypoint 1

- Tag: `397`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (28373.43, 0.00, -187.59) | None |

### Waypoint 2

- Tag: `398`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (28299.77, 0.00, -95.24) | None |

### Waypoint 3

- Tag: `399`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (28246.82, 0.00, -25.36) | None |

### Waypoint 4

- Tag: `400`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (28204.91, 0.00, 19.84) | None |

### Waypoint 5

- Tag: `367`
- Members: `Bora_Shuttle_Medium (object 46, id 11231, starts at point 0)`, `Bora_Shuttle_Medium (object 47, id 11232, starts at point 0)`, `Bora_Shuttle_Medium (object 48, id 11233, starts at point 0)`, `Bora_Shuttle_Medium (object 49, id 11234, starts at point 0)`, `Bora_Shuttle_Medium (object 50, id 11235, starts at point 0)`, `Bora_Shuttle_Medium (object 61, id 11226, starts at point 0)`, `Bora_Shuttle_Medium (object 62, id 11229, starts at point 0)`, `Bora_Shuttle_Medium (object 63, id 11225, starts at point 0)`, `Bora_Shuttle_Medium (object 64, id 11230, starts at point 0)`, `Bora_Shuttle_Medium (object 65, id 11227, starts at point 0)`, `Bora_Shuttle_Medium (object 66, id 11228, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-256.88, 387.35, 1726.17) | None |
| 1 | (-1126.76, 378.56, 1885.82) | None |
| 2 | (-1853.70, 0.00, 2749.42) | on arrival play dialog/script or enter gate, param 1 |

### Waypoint 6

- Tag: `366`
- Members: `Bora_Shuttle_Medium (object 42, id 11215, starts at point 0)`, `Bora_Shuttle_Medium (object 43, id 11216, starts at point 0)`, `Bora_Shuttle_Medium (object 44, id 11217, starts at point 0)`, `Bora_Shuttle_Medium (object 45, id 11218, starts at point 0)`, `Bora_Shuttle_Medium (object 67, id 11219, starts at point 0)`, `Bora_Shuttle_Medium (object 68, id 11223, starts at point 0)`, `Bora_Shuttle_Medium (object 69, id 11221, starts at point 0)`, `Bora_Shuttle_Medium (object 70, id 11224, starts at point 0)`, `Bora_Shuttle_Medium (object 71, id 11220, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (157.56, 795.23, 1537.71) | None |
| 1 | (-772.90, 45.34, 2355.10) | None |
| 2 | (-1743.63, 0.00, 2998.70) | on arrival play dialog/script or enter gate, param 1 |

### Waypoint 7

- Tag: `365`
- Members: `GalSpan_Pegasus (object 40, id 11201, starts at point 0)`, `GalSpan_Pegasus (object 41, id 11202, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-3572.14, 1.54, 152.97) | None |
| 1 | (-1917.68, 0.02, 472.51) | None |
| 2 | (-1204.77, 210.25, 972.08) | None |
| 3 | (-1755.26, 211.57, 2381.30) | on arrival play dialog/script or enter gate, param 1 |

### Waypoint 8

- Tag: `364`
- Members: `GalSpan_Orion (object 38, id 11199, starts at point 0)`, `GalSpan_Orion (object 39, id 11200, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-4028.54, 36.87, -240.37) | None |
| 1 | (-3541.87, -20.37, 19.68) | None |
| 2 | (-2091.81, 17.58, 145.17) | None |
| 3 | (-1398.89, 17.91, 334.70) | None |
| 4 | (-1210.19, 6.94, 80.39) | None |
| 5 | (-1077.25, 1.01, -195.82) | on arrival play dialog/script or enter gate, param 6591 |

### Waypoint 9

- Tag: `358`
- Members: `GalSpan_Cruiser (object 77, id 11086, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (25651.93, 111.34, -2992.06) | None |
| 1 | (27620.56, 42.90, -822.27) | on arrival activate current object (raw param -1 ignored); listened by Event 17 for GalSpan_Cruiser (object 77, id 11086) |

### Waypoint 10

- Tag: `357`
- Members: `GalSpan_Pegasus (object 30, id 11105, starts at point 0)`, `GalSpan_Pegasus (object 31, id 11106, starts at point 0)`, `GalSpan_Pegasus (object 32, id 11107, starts at point 0)`, `GalSpan_Pegasus (object 33, id 11108, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (24326.81, -148.81, -4212.25) | None |
| 1 | (27376.06, 189.77, -1319.34) | on arrival redirect to Waypoint 0 (tag 396), point 0 |

### Waypoint 11

- Tag: `356`
- Members: `GalSpan_Archangel (object 72, id 11387, starts at point 0)`, `GalSpan_Archangel (object 73, id 11385, starts at point 0)`, `GalSpan_Archangel (object 74, id 11386, starts at point 0)`, `GalSpan_Archangel (object 75, id 11388, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (24638.16, -31.04, -4185.76) | None |
| 1 | (27416.70, 232.67, -1349.13) | on arrival redirect to Waypoint 1 (tag 397), point 0 |

### Waypoint 12

- Tag: `355`
- Members: `GalSpan_Poseidon (object 26, id 11101, starts at point 0)`, `GalSpan_Poseidon (object 27, id 11102, starts at point 0)`, `GalSpan_Poseidon (object 28, id 11103, starts at point 0)`, `GalSpan_Poseidon (object 29, id 11104, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (24939.85, 99.25, -2979.08) | None |
| 1 | (27587.38, 45.97, -790.63) | on arrival redirect to Waypoint 2 (tag 398), point 0 |

### Waypoint 13

- Tag: `354`
- Members: `GalSpan_Orion (object 34, id 11113, starts at point 0)`, `GalSpan_Orion (object 35, id 11114, starts at point 0)`, `GalSpan_Orion (object 36, id 11115, starts at point 0)`, `GalSpan_Orion (object 37, id 11116, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (24736.66, -47.68, -3926.78) | None |
| 1 | (27415.25, 189.77, -1335.43) | on arrival redirect to Waypoint 3 (tag 399), point 0 |

### Waypoint 14

- Tag: `353`
- Members: `GalSpan_Archangel (object 22, id 11097, starts at point 0)`, `GalSpan_Archangel (object 23, id 11098, starts at point 0)`, `GalSpan_Archangel (object 24, id 11099, starts at point 0)`, `GalSpan_Archangel (object 25, id 11100, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (24884.03, 0.00, -3205.71) | None |
| 1 | (27590.29, 0.00, -796.33) | on arrival redirect to Waypoint 4 (tag 400), point 0 |

### Waypoint 15

- Tag: `352`
- Members: `TNS_Inquirer (object 14, id 11009, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1005.44, 0.00, 1945.74) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 16

- Tag: `351`
- Members: `Zeus_GalSpan_Carrier (object 76, id 10899, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2790.76, 207.42, 65.01) | on arrival activate current object (raw param -1 ignored); listened by Event 4 for Zeus_GalSpan_Carrier (object 76, id 10899) |

## Spawn Lists

### Spawn List 0

- ID: `15`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | Zeus_GalSpan_Carrier (object 76, id 10899) | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 2 | Gate | 1153.62,0.00,2154.24 | 274,0,0 | Gate SPX: [disp07.spx](DISP07.md) |
| 1 | `GalSpan_Orion` | 10188 | Interactive | 782.26,0.00,-2.46 | 0,0,0 | group/role: FG_MUSCA / 1 |
| 2 | `GalSpan_Orion` | 10189 | Interactive | 738.02,0.00,-54.79 | 0,0,0 | group/role: FG_MUSCA / 2 |
| 3 | `GalSpan_Orion` | 10190 | Interactive | 806.39,0.00,-54.79 | 0,0,0 | group/role: FG_MUSCA / 3 |
| 4 | `GalSpan_Orion` | 10191 | Interactive | 830.52,0.00,-94.04 | 0,0,0 | group/role: FG_MUSCA / 4 |
| 5 | `TNS_Inquirer` | 10232 | Interactive | 1076.20,0.00,1957.55 | 427,0,0 | label: TNSA; alias: tnsa; secondary groups: CONT_005, TNS_INQUIRER |
| 6 | `Bora_Battleaxe` | 10936 | Interactive | -867.51,0.00,-671.14 | 0,0,0 | group/role: FG_ANVIL / 1 |
| 7 | `Bora_Battleaxe` | 10937 | Interactive | -810.94,0.00,-671.14 | 0,0,0 | group/role: FG_ANVIL / 2 |
| 8 | `Bora_Battleaxe` | 10938 | Interactive | -734.56,0.00,-674.21 | 0,0,0 | group/role: FG_ANVIL / 3 |
| 9 | `Bora_Battleaxe` | 10939 | Interactive | -676.05,0.00,-677.80 | 0,0,0 | group/role: FG_ANVIL / 4 |
| 10 | `Bora_Warhammer` | 10940 | Interactive | -2369.88,0.00,1302.94 | 0,0,0 | group/role: FG_NOBLE / 1 |
| 11 | `Bora_Warhammer` | 10941 | Interactive | -2299.61,0.00,1300.70 | 0,0,0 | group/role: FG_NOBLE / 2 |
| 12 | `Bora_Warhammer` | 10942 | Interactive | -2243.81,0.00,1300.70 | 0,0,0 | group/role: FG_NOBLE / 3 |
| 13 | `Bora_Warhammer` | 10943 | Interactive | -2182.06,0.00,1302.35 | 0,0,0 | group/role: FG_NOBLE / 4 |
| 14 | `TNS_Inquirer` | 11009 | Interactive | -2281.02,0.00,3297.58 | 0,0,0 | label: TNSA; alias: tnsa; secondary groups: CONT_005, TNS_INQUIRER; waypoint: Waypoint 15 (tag 352, 1 point(s)), starting point 0, arrival event value 23068672 |
| 15 | `Roid_Sm_Brown` | 11012 | Object | -680.60,309.54,932.20 | 326,403,89 | Scale/Radius: 3.00 |
| 16 | `Roid_Sm_Brown` | 11016 | Object | -765.44,277.21,914.65 | 482,199,471 | Scale/Radius: 2.00 |
| 17 | `Roid_Sm_Brown` | 11018 | Object | -702.54,294.45,838.58 | 493,34,70 | Scale/Radius: 4.00 |
| 18 | `Roid_Sm_Brown` | 11020 | Object | -667.08,280.44,898.92 | 202,207,76 | Scale/Radius: 2.00 |
| 19 | `Roid_Sm_Brown` | 11013 | Object | -733.26,360.20,850.28 | 281,108,148 | Scale/Radius: 1.00 |
| 20 | `Roid_Sm_Brown2` | 11017 | Object | -658.66,351.58,929.27 | 72,61,268 | Scale/Radius: 1.00 |
| 21 | `Roid_Sm_Brown` | 11014 | Object | -655.73,325.71,842.97 | 218,208,416 | Scale/Radius: 1.00 |
| 22 | `GalSpan_Archangel` | 11097 | Interactive | 24871.57,0.00,-3216.53 | 64,0,0 | group/role: FG_AGENOR / 1; waypoint: Waypoint 14 (tag 353, 2 point(s)), starting point 0, arrival event value 23134208 |
| 23 | `GalSpan_Archangel` | 11098 | Interactive | 24873.79,0.00,-3259.46 | 64,0,0 | group/role: FG_AGENOR / 2; waypoint: Waypoint 14 (tag 353, 2 point(s)), starting point 0, arrival event value 23134208 |
| 24 | `GalSpan_Archangel` | 11099 | Interactive | 24872.92,0.00,-3301.00 | 64,0,0 | group/role: FG_AGENOR / 3; waypoint: Waypoint 14 (tag 353, 2 point(s)), starting point 0, arrival event value 23134208 |
| 25 | `GalSpan_Archangel` | 11100 | Interactive | 24826.18,0.00,-3226.50 | 64,0,0 | group/role: FG_AGENOR / 4; waypoint: Waypoint 14 (tag 353, 2 point(s)), starting point 0, arrival event value 23134208 |
| 26 | `GalSpan_Poseidon` | 11101 | Interactive | 24923.70,100.99,-2996.08 | 64,0,0 | group/role: FG_AFFAIRE / 1; waypoint: Waypoint 12 (tag 355, 2 point(s)), starting point 0, arrival event value 23265280 |
| 27 | `GalSpan_Poseidon` | 11102 | Interactive | 24892.59,100.99,-3003.34 | 64,0,0 | group/role: FG_AFFAIRE / 4; waypoint: Waypoint 12 (tag 355, 2 point(s)), starting point 0, arrival event value 23265280 |
| 28 | `GalSpan_Poseidon` | 11103 | Interactive | 24921.87,100.99,-3028.80 | 64,0,0 | group/role: FG_AFFAIRE / 2; waypoint: Waypoint 12 (tag 355, 2 point(s)), starting point 0, arrival event value 23265280 |
| 29 | `GalSpan_Poseidon` | 11104 | Interactive | 24921.26,100.99,-3058.88 | 64,0,0 | group/role: FG_AFFAIRE / 3; waypoint: Waypoint 12 (tag 355, 2 point(s)), starting point 0, arrival event value 23265280 |
| 30 | `GalSpan_Pegasus` | 11105 | Interactive | 24222.62,-147.77,-4341.62 | 64,0,0 | group/role: FG_AEGIPAN / 1; waypoint: Waypoint 10 (tag 357, 2 point(s)), starting point 0, arrival event value 23396352 |
| 31 | `GalSpan_Pegasus` | 11106 | Interactive | 24216.70,-100.99,-4370.84 | 64,0,0 | group/role: FG_AEGIPAN / 2; waypoint: Waypoint 10 (tag 357, 2 point(s)), starting point 0, arrival event value 23396352 |
| 32 | `GalSpan_Pegasus` | 11107 | Interactive | 24216.44,-100.99,-4393.32 | 64,0,0 | group/role: FG_AEGIPAN / 3; waypoint: Waypoint 10 (tag 357, 2 point(s)), starting point 0, arrival event value 23396352 |
| 33 | `GalSpan_Pegasus` | 11108 | Interactive | 24190.10,-100.99,-4356.43 | 64,0,0 | group/role: FG_AEGIPAN / 4; waypoint: Waypoint 10 (tag 357, 2 point(s)), starting point 0, arrival event value 23396352 |
| 34 | `GalSpan_Orion` | 11113 | Interactive | 24629.42,-46.78,-4059.85 | 64,0,0 | label: adder1; group/role: FG_ADDER / 1; waypoint: Waypoint 13 (tag 354, 2 point(s)), starting point 0, arrival event value 23199744 |
| 35 | `GalSpan_Orion` | 11114 | Interactive | 24622.83,0.00,-4096.72 | 64,0,0 | group/role: FG_ADDER / 2; waypoint: Waypoint 13 (tag 354, 2 point(s)), starting point 0, arrival event value 23199744 |
| 36 | `GalSpan_Orion` | 11115 | Interactive | 24619.90,0.00,-4127.65 | 64,0,0 | group/role: FG_ADDER / 3; waypoint: Waypoint 13 (tag 354, 2 point(s)), starting point 0, arrival event value 23199744 |
| 37 | `GalSpan_Orion` | 11116 | Interactive | 24590.28,0.00,-4071.33 | 64,0,0 | group/role: FG_ADDER / 4; waypoint: Waypoint 13 (tag 354, 2 point(s)), starting point 0, arrival event value 23199744 |
| 38 | `GalSpan_Orion` | 11199 | Interactive | -4080.00,36.87,-263.51 | 85,0,0 | group/role: FG_CAELUM / 1; waypoint: Waypoint 8 (tag 364, 6 point(s)), starting point 0, arrival event value 23855104 |
| 39 | `GalSpan_Orion` | 11200 | Interactive | -4068.49,36.87,-295.12 | 71,0,0 | group/role: FG_CAELUM / 2; waypoint: Waypoint 8 (tag 364, 6 point(s)), starting point 0, arrival event value 23855104 |
| 40 | `GalSpan_Pegasus` | 11201 | Interactive | -3615.83,1.54,155.87 | 100,0,0 | group/role: FG_CALLISTO / 1; waypoint: Waypoint 7 (tag 365, 4 point(s)), starting point 0, arrival event value 23920640 |
| 41 | `GalSpan_Pegasus` | 11202 | Interactive | -3612.96,1.54,132.45 | 100,0,0 | group/role: FG_CALLISTO / 2; waypoint: Waypoint 7 (tag 365, 4 point(s)), starting point 0, arrival event value 23920640 |
| 42 | `Bora_Shuttle_Medium` | 11215 | Interactive | -143.35,147.50,1154.79 | 43,0,0 | group/role: FG_DEATH / 0; waypoint: Waypoint 6 (tag 366, 3 point(s)), starting point 0, arrival event value 23986176 |
| 43 | `Bora_Shuttle_Medium` | 11216 | Interactive | -96.48,147.50,1154.38 | 43,0,0 | group/role: FG_DEATH / 0; waypoint: Waypoint 6 (tag 366, 3 point(s)), starting point 0, arrival event value 23986176 |
| 44 | `Bora_Shuttle_Medium` | 11217 | Interactive | -15.91,147.50,1090.16 | 0,0,0 | group/role: FG_DESPOT / 0; waypoint: Waypoint 6 (tag 366, 3 point(s)), starting point 0, arrival event value 23986176 |
| 45 | `Bora_Shuttle_Medium` | 11218 | Interactive | -87.48,146.55,1012.40 | 0,0,0 | group/role: FG_DESPOT / 0; waypoint: Waypoint 6 (tag 366, 3 point(s)), starting point 0, arrival event value 23986176 |
| 46 | `Bora_Shuttle_Medium` | 11231 | Interactive | 322.03,392.24,1667.34 | 384,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 5 (tag 367, 3 point(s)), starting point 0, arrival event value 24051712 |
| 47 | `Bora_Shuttle_Medium` | 11232 | Interactive | 149.89,417.37,1569.17 | 412,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 5 (tag 367, 3 point(s)), starting point 0, arrival event value 24051712 |
| 48 | `Bora_Shuttle_Medium` | 11233 | Interactive | 380.26,409.43,1545.34 | 405,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 5 (tag 367, 3 point(s)), starting point 0, arrival event value 24051712 |
| 49 | `Bora_Shuttle_Medium` | 11234 | Interactive | 62.89,388.27,1642.25 | 384,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 5 (tag 367, 3 point(s)), starting point 0, arrival event value 24051712 |
| 50 | `Bora_Shuttle_Medium` | 11235 | Interactive | 233.02,400.17,1625.49 | 398,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 5 (tag 367, 3 point(s)), starting point 0, arrival event value 24051712 |
| 51 | `Mars_Billboard_GC10_Cinematic` | 11266 | Interactive | -16011.64,0.00,285.28 | 128,0,0 | None |
| 52 | `Bora_Mace` | 10911 | Interactive | -2192.60,0.00,2572.36 | 0,0,0 | group/role: FG_FAITH / 1 |
| 53 | `Bora_Mace` | 10912 | Interactive | -2231.72,0.00,2528.15 | 0,0,0 | group/role: FG_FAITH / 2 |
| 54 | `Bora_Mace` | 10913 | Interactive | -2153.38,0.00,2529.40 | 0,0,0 | group/role: FG_FAITH / 3 |
| 55 | `Bora_Mace` | 10924 | Interactive | -780.13,320.62,890.75 | 0,0,0 | group/role: FG_HAMMER / 1 |
| 56 | `Bora_Mace` | 10925 | Interactive | -724.79,320.62,890.75 | 0,0,0 | group/role: FG_HAMMER / 2 |
| 57 | `Bora_Mace` | 10926 | Interactive | -666.94,320.62,890.75 | 0,0,0 | group/role: FG_HAMMER / 3 |
| 58 | `Roid_Med_Brown` | 11021 | Object | -767.22,347.59,883.09 | 368,389,4 | Scale/Radius: 1.00 |
| 59 | `Roid_Med_Brown` | 11019 | Object | -702.54,318.16,949.75 | 3,501,500 | Scale/Radius: 1.00 |
| 60 | `Roid_Med_Brown` | 11015 | Object | -720.09,306.31,905.87 | 437,161,173 | Scale/Radius: 1.00 |
| 61 | `Bora_Shuttle_Medium` | 11226 | Interactive | 144.30,409.43,1708.05 | 384,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 5 (tag 367, 3 point(s)), starting point 0, arrival event value 24051712 |
| 62 | `Bora_Shuttle_Medium` | 11229 | Interactive | 37.31,409.43,1712.51 | 381,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 5 (tag 367, 3 point(s)), starting point 0, arrival event value 24051712 |
| 63 | `Bora_Shuttle_Medium` | 11225 | Interactive | -25.70,409.43,1669.51 | 384,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 5 (tag 367, 3 point(s)), starting point 0, arrival event value 24051712 |
| 64 | `Bora_Shuttle_Medium` | 11230 | Interactive | -50.63,423.98,1617.11 | 411,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 5 (tag 367, 3 point(s)), starting point 0, arrival event value 24051712 |
| 65 | `Bora_Shuttle_Medium` | 11227 | Interactive | -171.46,397.81,1676.53 | 412,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 5 (tag 367, 3 point(s)), starting point 0, arrival event value 24051712 |
| 66 | `Bora_Shuttle_Medium` | 11228 | Interactive | -112.39,414.72,1697.46 | 384,0,0 | group/role: FG_ELITE / 0; waypoint: Waypoint 5 (tag 367, 3 point(s)), starting point 0, arrival event value 24051712 |
| 67 | `Bora_Shuttle_Medium` | 11219 | Interactive | -51.70,146.55,1131.79 | 0,0,0 | group/role: FG_DEGAS / 0; waypoint: Waypoint 6 (tag 366, 3 point(s)), starting point 0, arrival event value 23986176 |
| 68 | `Bora_Shuttle_Medium` | 11223 | Interactive | -47.39,147.50,1060.66 | 0,0,0 | group/role: FG_DEGAS / 0; waypoint: Waypoint 6 (tag 366, 3 point(s)), starting point 0, arrival event value 23986176 |
| 69 | `Bora_Shuttle_Medium` | 11221 | Interactive | -105.09,146.55,1085.30 | 100,0,0 | label: ROSS; group/role: FG_DELSEMME / 0; waypoint: Waypoint 6 (tag 366, 3 point(s)), starting point 0, arrival event value 23986176 |
| 70 | `Bora_Shuttle_Medium` | 11224 | Interactive | -142.97,146.55,1028.02 | 71,0,0 | group/role: FG_DESPOT / 0; waypoint: Waypoint 6 (tag 366, 3 point(s)), starting point 0, arrival event value 23986176 |
| 71 | `Bora_Shuttle_Medium` | 11220 | Interactive | -158.98,146.55,1075.46 | 0,0,0 | group/role: FG_DEGAS / 0; waypoint: Waypoint 6 (tag 366, 3 point(s)), starting point 0, arrival event value 23986176 |
| 72 | `GalSpan_Archangel` | 11387 | Interactive | 24484.81,0.00,-4334.10 | 50,0,0 | group/role: FG_ACE / 3; waypoint: Waypoint 11 (tag 356, 2 point(s)), starting point 0, arrival event value 23330816 |
| 73 | `GalSpan_Archangel` | 11385 | Interactive | 24530.31,-29.71,-4325.34 | 50,0,0 | group/role: FG_ACE / 1; waypoint: Waypoint 11 (tag 356, 2 point(s)), starting point 0, arrival event value 23330816 |
| 74 | `GalSpan_Archangel` | 11386 | Interactive | 24533.29,0.00,-4372.20 | 50,0,0 | group/role: FG_ACE / 2; waypoint: Waypoint 11 (tag 356, 2 point(s)), starting point 0, arrival event value 23330816 |
| 75 | `GalSpan_Archangel` | 11388 | Interactive | 24476.03,0.00,-4393.02 | 50,0,0 | group/role: FG_ACE / 4; waypoint: Waypoint 11 (tag 356, 2 point(s)), starting point 0, arrival event value 23330816 |
| 76 | `Zeus_GalSpan_Carrier` | 10899 | Interactive | 2572.36,207.42,52.62 | 384,0,0 | label: atkin; alias: zeus; secondary groups: none, ZEUS; waypoint: Waypoint 16 (tag 351, 1 point(s)), starting point 0, arrival event value 23003136 |
| 77 | `GalSpan_Cruiser` | 11086 | Interactive | 25185.17,128.70,-3465.67 | 64,0,0 | label: cruiser1; secondary groups: none, ACHILLES; waypoint: Waypoint 9 (tag 358, 2 point(s)), starting point 0, arrival event value 23461888 |
| 78 | `Bflat04_GC10_Only` | 11365 | Interactive | 28669.09,0.00,126.34 | 327,0,0 | None |
| 79 | `Bflat03_GC10_Only` | 11366 | Interactive | 23086.55,0.00,-5611.36 | 71,0,0 | None |
