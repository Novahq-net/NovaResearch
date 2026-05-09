# Tachyon: The Fringe NEUT04C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT04C.SPX` |
| Sector | `QUAD_04` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 3 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 19 |
| Entities | 60 |
| Events | 33 |
| Waypoints | 9 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Light_Freighter`, `1: GalSpan_Frigate`, `2: Luxury_Liner`, `3: Bora_Carrier`, `4: Crate_5_Special_Placehold`, `5: GalSpan_Pegasus`, `6: Star_Patrol_Enforcer`, `7: Independent_Merc_Dart`, `8: GalSpan_Shuttle_Medium`, `9: GalSpan_Poseidon`, `10: Drone_Multipurpose`, `11: Junk_10`, `12: Junk_08`, `13: Junk_07`, `14: Junk_06`, `15: Junk_05`, `16: Junk_04`, `17: Junk_03`, `18: Shuttle_Medium` |
| Scripts | `PLAYER.SCR`, `LAREF.SCR`, `COURG.SCR` |
| Scenes | None |
| Labels | `bfne_06`, `BFBE_03`, `MISHK`, `HESPE`, `Merch` |
| Aliases | `Courage`, `kwI03_02`, `kwI03_03`, `kwi03_7`, `Jerome24`, `Jerome25`, `Jerome26`, `Jerome22`, `Jerome21`, `Jerome20`, `Intrepid`, `Artemis`, `KWi03_10`, `Hermes` |
| Groups | `COURAGE`, `CONT_025`, `FG_HELIOS`, `FG_NERGAL`, `FG_CRONUS`, `FG_WYRM`, `FG_NOVA`, `FG_CETUS`, `FG_CALLISTO`, `INTREPID`, `CONT_034`, `STAR_PRINCESS`, `ARTEMIS`, `CONT_028` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Object event: subject Shuttle_Medium (object 0, id 1290), op 15, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 16, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 6, param 1290
- Object spawn/action: id 1270, subtype 8, param 2
- Object spawn/action: Shuttle_Medium (object 0, id 1290), subtype 8, param 1
- Set/add variable: variable group 21, variable 24, subtype 0, value 0
- Object spawn/action: Bora_Carrier (object 56, id 1286), subtype 14

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 16, op 1, value 5
- Object event: subject Shuttle_Medium (object 0, id 1290), op 15, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 99
- Object spawn/action: Shuttle_Medium (object 0, id 1290), subtype 14

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 16, op 1, value 60
- Sector/startup condition family: subject 0, op 0, value 99 (join 1)
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Play dialog: LAREF.SCR, line/variant 2

### Event 3

**Trigger**

- Object arrival: Shuttle_Medium (object 0, id 1290) reached Waypoint 8 (tag 202), point 2 (raw value 13238274)

**Action**

- Object spawn/action: Shuttle_Medium (object 0, id 1290), subtype 11, param 1286

### Event 4

**Trigger**

- Object event: subject Shuttle_Medium (object 0, id 1290), op 13, value 0 (extra 1, 1286; flags 2)
- Sector/startup condition family: subject 0, op 0, value 99

**Action**

- Set/add variable: variable group 21, variable 26, subtype 0, value 1
- Set runtime trigger variable: variable group 20, variable 13, subtype 0, value 0
- Hide/remove HUD contact: contact/list 0, subtype 6, param 1290
- Show/update HUD contact: contact/list 0, subtype 9, param 41

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 13, op 1, value 3 (join 1)
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Play dialog: COURG.SCR, line/variant 1

### Event 6

**Trigger**

- Sector/startup condition family: subject 2, op 0, value 1 (join 1)
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Play dialog: LAREF.SCR, line/variant 3

### Event 7

**Trigger**

- Variable comparison: subject variable group 20, variable 13, op 1, value 30
- Sector/startup condition family: subject 1, op 0, value 3 (join 1)
- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Play dialog: COURG.SCR, line/variant 2
- Show/update HUD contact: contact/list 0, subtype 9, param 28
- Object spawn/action: Crate_5_Special_Placehold (object 55, id 2038), subtype 14
- Object spawn/action: Bora_Carrier (object 56, id 1286), subtype 15

### Event 8

**Trigger**

- Sector/startup condition family: subject 2, op 0, value 2

**Action**

- Play dialog: LAREF.SCR, line/variant 5
- Group/spawn-list action: spawn list/group 222, subtype 7

### Event 9

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 5

**Action**

- Play dialog: LAREF.SCR, line/variant 4
- Group/spawn-list action: spawn list/group 251, subtype 4, param 2

### Event 10

**Trigger**

- Variable comparison: subject variable group 20, variable 13, op 1, value 200 (join 1)
- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Play dialog: COURG.SCR, line/variant 4

### Event 11

**Trigger**

- Sector/startup condition family: subject 2, op 0, value 4
- Variable comparison: subject variable group 20, variable 13, op 1, value 260 (join 1)
- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Play dialog: COURG.SCR, line/variant 5

### Event 12

**Trigger**

- Object event: subject GalSpan_Shuttle_Medium (object 31, id 1529), op 13, value 0 (extra 1, 1286; join 1; flags 2)
- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Play dialog: COURG.SCR, line/variant 3

### Event 13

**Trigger**

- Object event: subject 1270, op 0, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 222, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 221, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 251, op 4, value 0 (join 2; flags 2)
- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Play dialog: LAREF.SCR, line/variant 6
- Group/spawn-list action: spawn list/group 251, subtype 4, param 2
- Set/add variable: variable group 21, variable 22, subtype 0, value 1

### Event 14

**Trigger**

- Object event: subject 1270, op 14, value 42
- Variable comparison: subject variable group 21, variable 26, op 1, value 1

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Play dialog: PLAYER.SCR, line/variant 203
- Show/update HUD contact: contact/list 0, subtype 2, param 1286
- Set runtime trigger variable: variable group 20, variable 15, subtype 0, value 0
- Set/add variable: variable group 21, variable 21, subtype 0, value 1
- Object spawn/action: Crate_5_Special_Placehold (object 55, id 2038), subtype 7
- Object spawn/action: Bora_Carrier (object 56, id 1286), subtype 14
- Object spawn/action: Bora_Carrier (object 56, id 1286), subtype 18

### Event 15

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 203

**Action**

- Play dialog: COURG.SCR, line/variant 8
- Object spawn/action: Bora_Carrier (object 56, id 1286), subtype 8, param 1

### Event 16

**Trigger**

- Variable comparison: subject variable group 20, variable 15, op 1, value 15
- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Object spawn/action: Bora_Carrier (object 56, id 1286), subtype 5
- Object spawn/action: Bora_Carrier (object 56, id 1286), subtype 13, param 13369344

### Event 17

**Trigger**

- Variable comparison: subject variable group 20, variable 13, op 1, value 315
- Sector/startup condition family: subject 2, op 0, value 5 (join 1)
- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Play dialog: COURG.SCR, line/variant 6

### Event 18

**Trigger**

- Variable comparison: subject variable group 20, variable 13, op 1, value 330
- Sector/startup condition family: subject 2, op 0, value 6 (join 1)
- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Play dialog: COURG.SCR, line/variant 7
- Object spawn/action: Shuttle_Medium (object 41, id 1896), subtype 1, param 1286
- Object spawn/action: Shuttle_Medium (object 41, id 1896), subtype 8, param 1
- Object spawn/action: Shuttle_Medium (object 41, id 1896), subtype 13, param 13959168

### Event 19

**Trigger**

- Variable comparison: subject variable group 20, variable 15, op 1, value 45 (join 2)
- Variable comparison: subject variable group 20, variable 13, op 1, value 275

**Action**

- Object spawn/action: GalSpan_Frigate (object 58, id 1477), subtype 3

### Event 20

**Trigger**

- Variable comparison: subject variable group 20, variable 15, op 1, value 30 (join 2)
- Variable comparison: subject variable group 20, variable 13, op 1, value 275 (join 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 134
- Group/spawn-list action: spawn list/group 227, subtype 1, param 7

### Event 21

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 134

**Action**

- Play dialog: PLAYER.SCR, line/variant 205

### Event 22

**Trigger**

- Object arrival: GalSpan_Shuttle_Medium (object 31, id 1529) reached Waypoint 3 (tag 212), point 0 (raw value 13893632)

**Action**

- Object spawn/action: GalSpan_Shuttle_Medium (object 31, id 1529), subtype 11, param 1286

### Event 23

**Trigger**

- Variable comparison: subject variable group 21, variable 24, op 3, value 1
- Object arrival: Bora_Carrier (object 56, id 1286) reached Waypoint 2 (tag 204), point 0 (raw value 13369344)

**Action**

- Object spawn/action: GalSpan_Shuttle_Medium (object 40, id 1895), subtype 1, param 1286
- Object spawn/action: GalSpan_Shuttle_Medium (object 40, id 1895), subtype 13, param 13893632
- Object spawn/action: GalSpan_Shuttle_Medium (object 40, id 1895), subtype 5

### Event 24

**Trigger**

- Variable comparison: subject variable group 20, variable 15, op 1, value 150

**Action**

- Play dialog: COURG.SCR, line/variant 9
- Set/add variable: variable group 21, variable 2, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Mission objective/state: param 65536, subtype 0, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 33
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 25

**Trigger**

- Variable comparison: subject variable group 20, variable 15, op 1, value 215

**Action**

- Group/spawn-list action: spawn list/group 120, subtype 1, param 8
- Group/spawn-list action: spawn list/group 224, subtype 1, param 7
- Group/spawn-list action: spawn list/group 120, subtype 4, param 2

### Event 26

**Trigger**

- Group/spawn-list event: subject 222, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 227, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 221, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 251, op 4, value 0 (join 2; flags 2)

**Action**

- Group/spawn-list action: spawn list/group 251, subtype 4, param 2

### Event 27

**Trigger**

- Object event: subject Shuttle_Medium (object 0, id 1290), op 2, value 0 (join 2)
- Object event: subject Shuttle_Medium (object 41, id 1896), op 2, value 0 (join 2)
- Object event: subject Shuttle_Medium (object 41, id 1896), op 7, value 0 (join 2)
- Variable comparison: subject variable group 21, variable 25, op 1, value 1

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Mission objective/state: param 65536, subtype 0, param 0
- Set/add variable: variable group 13, variable 418, subtype 0, value 1
- Set/add variable: variable group 13, variable 419, subtype 0, value 1
- Show/update HUD contact: contact/list 0, subtype 11, param 34
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 21, variable 22, subtype 0, value 1

### Event 28

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 90

**Action**

- Play dialog: PLAYER.SCR, line/variant 191

### Event 29

**Trigger**

- Group/spawn-list event: subject 227, op 1, value 30

**Action**

- Play dialog: PLAYER.SCR, line/variant 135

### Event 30

**Trigger**

- Group/spawn-list event: subject 251, op 0, value 0 (join 1)
- Group/spawn-list event: subject 227, op 3, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 144

### Event 31

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 0, value 10 (join 1)

**Action**

- Play dialog: PLAYER.SCR, line/variant 154

### Event 32

**Trigger**

- Group/spawn-list event: subject 222, op 0, value 0
- Sector/startup condition family: subject 1, op 0, value 6

**Action**

- Play dialog: PLAYER.SCR, line/variant 137
- Set/add variable: variable group 21, variable 24, subtype 0, value 1

## Waypoints

### Waypoint 0

- Tag: `214`
- Members: `GalSpan_Poseidon (object 28, id 1501, starts at point 0)`, `GalSpan_Poseidon (object 29, id 1503, starts at point 0)`, `GalSpan_Poseidon (object 30, id 1504, starts at point 0)`, `GalSpan_Poseidon (object 46, id 1996, starts at point 0)`, `GalSpan_Pegasus (object 47, id 1852, starts at point 0)`, `GalSpan_Pegasus (object 48, id 1853, starts at point 0)`, `GalSpan_Pegasus (object 49, id 1854, starts at point 0)`, `GalSpan_Poseidon (object 50, id 2015, starts at point 0)`, `GalSpan_Poseidon (object 51, id 2016, starts at point 0)`, `GalSpan_Poseidon (object 52, id 2017, starts at point 0)`, `GalSpan_Poseidon (object 53, id 2018, starts at point 0)`, `GalSpan_Pegasus (object 54, id 2019, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1427.56, 0.00, 545.03) | None |
| 1 | (1096.01, 0.00, -1192.14) | None |

### Waypoint 1

- Tag: `213`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1397.78, -892.15, -121.76) | None |
| 1 | (521.93, 0.00, -2259.37) | on arrival play dialog/script or enter gate, param 8 |

### Waypoint 2

- Tag: `204`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2010.44, -1128.10, -835.01) | None; listened by Event 23 for Bora_Carrier (object 56, id 1286) |
| 1 | (2005.87, -1128.10, -4682.28) | on arrival action 1, param -1 |

### Waypoint 3

- Tag: `212`
- Members: `GalSpan_Shuttle_Medium (object 31, id 1529, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (812.97, 652.23, -134.17) | None; listened by Event 22 for GalSpan_Shuttle_Medium (object 31, id 1529) |
| 1 | (1200.39, -895.64, 62.07) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 4

- Tag: `211`
- Members: `GalSpan_Frigate (object 58, id 1477, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1759.27, -559.34, 1157.29) | None |
| 1 | (1740.11, -559.34, 321.75) | None |
| 2 | (693.77, -559.34, -2431.73) | None |

### Waypoint 5

- Tag: `210`
- Members: `Independent_Merc_Dart (object 32, id 1726, starts at point -1)`, `Independent_Merc_Dart (object 33, id 1728, starts at point -1)`, `Star_Patrol_Enforcer (object 34, id 1809, starts at point -1)`, `Star_Patrol_Enforcer (object 35, id 1810, starts at point -1)`, `Star_Patrol_Enforcer (object 36, id 1811, starts at point -1)`, `Star_Patrol_Enforcer (object 37, id 1812, starts at point -1)`, `Independent_Merc_Dart (object 38, id 1832, starts at point -1)`, `Independent_Merc_Dart (object 39, id 1833, starts at point -1)`, `GalSpan_Shuttle_Medium (object 40, id 1895, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1009.08, -145.45, -752.60) | None |
| 1 | (1236.61, -145.45, -1188.02) | None |
| 2 | (2051.61, -145.45, -1168.68) | None |
| 3 | (2057.55, -145.45, -408.82) | None |
| 4 | (1275.77, -145.45, -412.40) | None |

### Waypoint 6

- Tag: `208`
- Members: `Drone_Multipurpose (object 24, id 1371, starts at point -1)`, `Drone_Multipurpose (object 25, id 1372, starts at point -1)`, `Drone_Multipurpose (object 26, id 1373, starts at point -1)`, `Drone_Multipurpose (object 27, id 1374, starts at point -1)`, `Drone_Multipurpose (object 42, id 1341, starts at point 0)`, `Drone_Multipurpose (object 43, id 1343, starts at point 0)`, `Drone_Multipurpose (object 44, id 1340, starts at point 0)`, `Drone_Multipurpose (object 45, id 1342, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2195.98, -609.87, 1607.86) | None |
| 1 | (1320.98, -609.87, 1254.97) | None |
| 2 | (1326.31, -609.87, -294.72) | None |
| 3 | (1614.42, -609.87, -919.52) | None |
| 4 | (2900.24, -609.87, -867.45) | None |
| 5 | (2894.91, -609.87, 1122.63) | on arrival redirect to Waypoint 6 (tag 208), point 0 |

### Waypoint 7

- Tag: `206`
- Members: `Generic_Light_Freighter (object 59, id 1364, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2540.83, 0.00, 207.48) | None |
| 1 | (-543.50, 0.00, 1013.01) | None |
| 2 | (-543.50, 0.00, 1524.75) | on arrival action 1, param -1 |

### Waypoint 8

- Tag: `202`
- Members: `Shuttle_Medium (object 0, id 1290, starts at point 0)`, `Shuttle_Medium (object 41, id 1896, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (126.77, 0.00, -2523.16) | None |
| 1 | (844.24, -854.96, -1697.06) | None |
| 2 | (1252.87, -961.24, -86.51) | on arrival activate current object (raw param -1 ignored); listened by Event 3 for Shuttle_Medium (object 0, id 1290) |

## Spawn Lists

### Spawn List 0

- ID: `227`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | Bora_Carrier (object 56, id 1286) | None |

### Spawn List 1

- ID: `251`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Shuttle_Medium` | 1290 | Interactive | -62.90,0.00,-3084.00 | 0,0,0 | alias: Courage; secondary groups: CONT_025, COURAGE; waypoint: Waypoint 8 (tag 202, 3 point(s)), starting point 0, arrival event value 13238272 |
| 1 | `Junk_03` | 1314 | Object | 1584.16,-1060.17,625.37 | 0,0,0 | Scale/Radius: 1.00 |
| 2 | `Junk_03` | 1315 | Object | 1652.88,-1025.45,90.84 | 0,20,0 | Scale/Radius: 1.00 |
| 3 | `Junk_03` | 1317 | Object | 1830.67,-1156.74,-18.03 | 0,0,0 | Scale/Radius: 1.00 |
| 4 | `Junk_04` | 1318 | Object | 2088.93,-1012.89,845.15 | 0,435,0 | Scale/Radius: 1.00 |
| 5 | `Junk_04` | 1319 | Object | 1620.01,-1060.17,719.32 | 0,130,0 | Scale/Radius: 1.00 |
| 6 | `Junk_05` | 1320 | Object | 2039.05,-1001.98,982.38 | 0,20,0 | Scale/Radius: 1.00 |
| 7 | `Junk_05` | 1321 | Object | 1826.77,-1191.42,-16.39 | 0,351,0 | Scale/Radius: 1.00 |
| 8 | `Junk_05` | 1322 | Object | 2023.20,-1099.75,283.22 | 0,0,0 | Scale/Radius: 1.00 |
| 9 | `Junk_06` | 1323 | Object | 1596.11,-1060.17,554.10 | 0,130,0 | Scale/Radius: 1.00 |
| 10 | `Junk_06` | 1324 | Object | 1995.49,-1023.70,443.25 | 124,0,0 | Scale/Radius: 1.00 |
| 11 | `Junk_06` | 1325 | Object | 2042.59,-1031.36,216.81 | 124,0,0 | Scale/Radius: 1.00 |
| 12 | `Junk_06` | 1326 | Object | 1685.75,-1060.17,661.01 | 0,0,0 | Scale/Radius: 1.00 |
| 13 | `Junk_07` | 1327 | Object | 1783.70,-1053.09,526.20 | 124,0,0 | Scale/Radius: 1.00 |
| 14 | `Junk_07` | 1328 | Object | 1802.21,-1050.94,573.53 | 0,0,0 | Scale/Radius: 1.00 |
| 15 | `Junk_07` | 1329 | Object | 1632.51,-1060.17,671.98 | 124,0,0 | Scale/Radius: 1.00 |
| 16 | `Junk_07` | 1330 | Object | 1617.06,-1033.39,753.73 | 0,0,0 | Scale/Radius: 1.00 |
| 17 | `Junk_08` | 1331 | Object | 1676.48,-1060.17,497.37 | 0,435,0 | Scale/Radius: 1.00 |
| 18 | `Junk_08` | 1332 | Object | 1661.84,-1060.17,742.00 | 0,435,0 | Scale/Radius: 1.00 |
| 19 | `Junk_08` | 1333 | Object | 2028.62,-1016.20,970.70 | 0,130,0 | Scale/Radius: 1.00 |
| 20 | `Junk_10` | 1336 | Object | 1824.68,-1039.34,638.33 | 0,130,0 | Scale/Radius: 1.00 |
| 21 | `Junk_10` | 1337 | Object | 1876.33,-1041.65,567.05 | 0,0,0 | Scale/Radius: 1.00 |
| 22 | `Junk_10` | 1338 | Object | 2153.35,-1034.79,1056.48 | 0,435,0 | Scale/Radius: 1.00 |
| 23 | `Junk_10` | 1339 | Object | 1613.28,-1025.45,458.43 | 0,20,0 | Scale/Radius: 1.00 |
| 24 | `Drone_Multipurpose` | 1371 | Interactive | 2543.28,-987.52,1368.13 | 0,0,0 | group/role: FG_HELIOS / 0; waypoint: Waypoint 6 (tag 208, 6 point(s)), starting point -1 |
| 25 | `Drone_Multipurpose` | 1372 | Interactive | 2575.60,-1028.59,1404.73 | 0,0,0 | group/role: FG_HELIOS / 0; waypoint: Waypoint 6 (tag 208, 6 point(s)), starting point -1 |
| 26 | `Drone_Multipurpose` | 1373 | Interactive | 2520.80,-1023.55,1410.09 | 0,0,0 | group/role: FG_HELIOS / 0; waypoint: Waypoint 6 (tag 208, 6 point(s)), starting point -1 |
| 27 | `Drone_Multipurpose` | 1374 | Interactive | 2563.25,-1013.47,1449.03 | 0,0,0 | group/role: FG_HELIOS / 0; waypoint: Waypoint 6 (tag 208, 6 point(s)), starting point -1 |
| 28 | `GalSpan_Poseidon` | 1501 | Interactive | 108.43,0.00,1710.22 | 0,0,0 | group/role: FG_NERGAL / 0; waypoint: Waypoint 0 (tag 214, 2 point(s)), starting point 0, arrival event value 14024704 |
| 29 | `GalSpan_Poseidon` | 1503 | Interactive | 151.29,0.00,1694.73 | 0,0,0 | group/role: FG_NERGAL / 0; waypoint: Waypoint 0 (tag 214, 2 point(s)), starting point 0, arrival event value 14024704 |
| 30 | `GalSpan_Poseidon` | 1504 | Interactive | 179.87,0.00,1725.72 | 0,0,0 | label: BFBE_03; group/role: FG_NERGAL / 0; waypoint: Waypoint 0 (tag 214, 2 point(s)), starting point 0, arrival event value 14024704 |
| 31 | `GalSpan_Shuttle_Medium` | 1529 | Interactive | 535.61,567.27,-95.58 | 0,0,0 | label: BFBE_03; group/role: FG_CRONUS / 0; secondary groups: CONT_025, none; waypoint: Waypoint 3 (tag 212, 2 point(s)), starting point -1 |
| 32 | `Independent_Merc_Dart` | 1726 | Interactive | 1033.37,0.00,-2082.89 | 0,0,0 | label: BFBE_03; group/role: FG_WYRM / 0; waypoint: Waypoint 5 (tag 210, 5 point(s)), starting point -1 |
| 33 | `Independent_Merc_Dart` | 1728 | Interactive | 1084.14,0.00,-2081.41 | 0,0,0 | group/role: FG_WYRM / 0; waypoint: Waypoint 5 (tag 210, 5 point(s)), starting point -1 |
| 34 | `Star_Patrol_Enforcer` | 1809 | Interactive | 199.63,0.00,-3043.66 | 0,0,0 | group/role: FG_NOVA / 0; waypoint: Waypoint 5 (tag 210, 5 point(s)), starting point -1 |
| 35 | `Star_Patrol_Enforcer` | 1810 | Interactive | 156.03,0.00,-3083.66 | 0,0,0 | group/role: FG_NOVA / 0; waypoint: Waypoint 5 (tag 210, 5 point(s)), starting point -1 |
| 36 | `Star_Patrol_Enforcer` | 1811 | Interactive | 259.99,0.00,-3090.93 | 0,0,0 | group/role: FG_NOVA / 0; waypoint: Waypoint 5 (tag 210, 5 point(s)), starting point -1 |
| 37 | `Star_Patrol_Enforcer` | 1812 | Interactive | 201.30,0.00,-3132.75 | 0,0,0 | group/role: FG_NOVA / 0; waypoint: Waypoint 5 (tag 210, 5 point(s)), starting point -1 |
| 38 | `Independent_Merc_Dart` | 1832 | Interactive | 1050.93,0.00,-2066.18 | 0,0,0 | label: BFBE_03; group/role: FG_WYRM / 0; waypoint: Waypoint 5 (tag 210, 5 point(s)), starting point -1 |
| 39 | `Independent_Merc_Dart` | 1833 | Interactive | 1061.97,0.00,-2086.65 | 0,0,0 | group/role: FG_WYRM / 0; waypoint: Waypoint 5 (tag 210, 5 point(s)), starting point -1 |
| 40 | `GalSpan_Shuttle_Medium` | 1895 | Interactive | 85.43,567.27,-3036.46 | 0,0,0 | label: BFBE_03; group/role: FG_CRONUS / 0; waypoint: Waypoint 5 (tag 210, 5 point(s)), starting point -1 |
| 41 | `Shuttle_Medium` | 1896 | Interactive | -19.07,0.00,-3057.61 | 0,0,0 | alias: Courage; secondary groups: CONT_025, COURAGE; waypoint: Waypoint 8 (tag 202, 3 point(s)), starting point 0, arrival event value 13238272 |
| 42 | `Drone_Multipurpose` | 1341 | Interactive | 20.17,0.00,-1772.78 | 128,0,0 | group/role: FG_CETUS / 0; waypoint: Waypoint 6 (tag 208, 6 point(s)), starting point 0, arrival event value 13631488 |
| 43 | `Drone_Multipurpose` | 1343 | Interactive | 1851.69,0.00,-1933.14 | 0,0,0 | group/role: FG_CETUS / 0; waypoint: Waypoint 6 (tag 208, 6 point(s)), starting point 0, arrival event value 13631488 |
| 44 | `Drone_Multipurpose` | 1340 | Interactive | 5499.42,0.00,-256.46 | 0,0,0 | group/role: FG_CETUS / 0; waypoint: Waypoint 6 (tag 208, 6 point(s)), starting point 0, arrival event value 13631488 |
| 45 | `Drone_Multipurpose` | 1342 | Interactive | 6168.68,0.00,-337.45 | 0,0,0 | group/role: FG_CETUS / 0; waypoint: Waypoint 6 (tag 208, 6 point(s)), starting point 0, arrival event value 13631488 |
| 46 | `GalSpan_Poseidon` | 1996 | Interactive | 142.29,0.00,1758.60 | 0,0,0 | label: BFBE_03; group/role: FG_NERGAL / 0; waypoint: Waypoint 0 (tag 214, 2 point(s)), starting point 0, arrival event value 14024704 |
| 47 | `GalSpan_Pegasus` | 1852 | Interactive | 284.59,0.00,2020.33 | 0,0,0 | group/role: FG_CALLISTO / 0; waypoint: Waypoint 0 (tag 214, 2 point(s)), starting point 0, arrival event value 14024704 |
| 48 | `GalSpan_Pegasus` | 1853 | Interactive | 248.10,0.00,2096.63 | 0,0,0 | group/role: FG_CALLISTO / 0; waypoint: Waypoint 0 (tag 214, 2 point(s)), starting point 0, arrival event value 14024704 |
| 49 | `GalSpan_Pegasus` | 1854 | Interactive | 241.58,0.00,2006.20 | 0,0,0 | label: BFBE_03; group/role: FG_CALLISTO / 0; waypoint: Waypoint 0 (tag 214, 2 point(s)), starting point 0, arrival event value 14024704 |
| 50 | `GalSpan_Poseidon` | 2015 | Interactive | 338.33,0.00,1780.86 | 0,0,0 | group/role: FG_NERGAL / 0; waypoint: Waypoint 0 (tag 214, 2 point(s)), starting point 0, arrival event value 14024704 |
| 51 | `GalSpan_Poseidon` | 2016 | Interactive | 298.09,0.00,1766.32 | 0,0,0 | group/role: FG_NERGAL / 0; waypoint: Waypoint 0 (tag 214, 2 point(s)), starting point 0, arrival event value 14024704 |
| 52 | `GalSpan_Poseidon` | 2017 | Interactive | 267.90,0.00,1795.41 | 0,0,0 | label: BFBE_03; group/role: FG_NERGAL / 0; waypoint: Waypoint 0 (tag 214, 2 point(s)), starting point 0, arrival event value 14024704 |
| 53 | `GalSpan_Poseidon` | 2018 | Interactive | 308.15,0.00,1828.14 | 0,0,0 | label: BFBE_03; group/role: FG_NERGAL / 0; waypoint: Waypoint 0 (tag 214, 2 point(s)), starting point 0, arrival event value 14024704 |
| 54 | `GalSpan_Pegasus` | 2019 | Interactive | 294.73,0.00,2133.59 | 0,0,0 | group/role: FG_CALLISTO / 0; waypoint: Waypoint 0 (tag 214, 2 point(s)), starting point 0, arrival event value 14024704 |
| 55 | `Crate_5_Special_Placehold` | 2038 | Interactive | 272.55,665.32,-363.04 | 0,0,0 | None |
| 56 | `Bora_Carrier` | 1286 | Interactive | 2016.41,-1140.83,533.92 | 256,0,0 | alias: Intrepid; secondary groups: CONT_034, INTREPID |
| 57 | `Luxury_Liner` | 1288 | Interactive | 1467.71,-217.52,-2019.27 | 384,0,0 | secondary groups: none, STAR_PRINCESS |
| 58 | `GalSpan_Frigate` | 1477 | Interactive | 1324.44,-511.74,4029.40 | 256,0,0 | label: BFBE_03; alias: Artemis; secondary groups: CONT_025, ARTEMIS; waypoint: Waypoint 4 (tag 211, 3 point(s)), starting point -1 |
| 59 | `Generic_Light_Freighter` | 1364 | Interactive | -2508.88,0.00,-1318.56 | 0,0,0 | alias: Hermes; secondary groups: CONT_028, none; waypoint: Waypoint 7 (tag 206, 3 point(s)), starting point -1 |
