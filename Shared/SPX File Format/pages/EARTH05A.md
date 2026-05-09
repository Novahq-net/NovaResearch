# Tachyon: The Fringe EARTH05A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH05A.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `(none)` |
| Region | 0 |
| Sector ID | 4 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 8 |
| Entities | 29 |
| Events | 55 |
| Waypoints | 11 |
| Child Sectors | 0 |
| Scripts | 4 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Exile_Star_Patrol_Capship`, `1: Biolith_Dart`, `2: Exile_Claw_Mace`, `3: Sol_Shuttle_Exile_Cinematic`, `4: Exile_Star_Patrol_Enforcer`, `5: Star_Patrol_Enforcer`, `6: Shuttle_Medium`, `7: Mega_Gate` |
| Scripts | `PLAYER.SCR`, `HAST.SCR`, `ARGO.SCR`, `DILL.SCR` |
| Scenes | None |
| Labels | `ESC1`, `ESC2`, `argo`, `Escort3`, `Escort2`, `Escort4`, `Escort1`, `SOLShuttle`, `Imposter`, `Sol1`, `Sol4`, `Sol7`, `BLFT`, `SOLCapShip` |
| Aliases | `Todd01` |
| Groups | `ARGOSO 914`, `CONT_UNKNOWN`, `FG_AGT1`, `FG_AGT2`, `FG_AGT3`, `FG_NEWBURN`, `CONT_023` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Gate state/action: param 799, subtype 3, param 0
- Gate state/action: param 926, subtype 3, param 0
- Set runtime trigger variable: variable group 20, variable 3, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 10

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 3, op 1, value 4
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 22
- Hide/remove HUD contact: contact/list 0, subtype 11, param 0

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 3, op 1, value 35
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 14

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 3, op 1, value 45
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Play dialog: HAST.SCR, line/variant 6
- Object spawn/action: id 1064, subtype 12
- Object spawn/action: id 1065, subtype 12

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 3, op 1, value 60

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 15
- Show/update HUD contact: contact/list 0, subtype 9, param 16

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 3, op 1, value 60

**Action**

- Gate state/action: param 1, subtype 3, param 0

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 3, op 1, value 70
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 21

### Event 7

**Trigger**

- Variable comparison: subject variable group 20, variable 3, op 1, value 127
- Variable comparison: subject variable group 21, variable 24, op 1, value 0
- Variable comparison: subject variable group 21, variable 20, op 1, value 0
- Variable comparison: subject variable group 21, variable 26, op 1, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 15

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 3, op 1, value 136

**Action**

- Object spawn/action: Biolith_Dart (object 25, id 1066), subtype 0
- Set runtime trigger variable: variable group 20, variable 4, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 9, param 51
- Show/update HUD contact: contact/list 0, subtype 2, param 717

### Event 9

**Trigger**

- Variable comparison: subject variable group 20, variable 3, op 1, value 138

**Action**

- Play dialog: HAST.SCR, line/variant 1

### Event 10

**Trigger**

- Variable comparison: subject variable group 20, variable 4, op 1, value 3

**Action**

- Object spawn/action: Biolith_Dart (object 26, id 1067), subtype 0

### Event 11

**Trigger**

- Variable comparison: subject variable group 20, variable 4, op 1, value 5

**Action**

- Object spawn/action: Biolith_Dart (object 27, id 1068), subtype 0

### Event 12

**Trigger**

- Object event: subject 1065, op 2, value 0 (join 2)
- Object event: subject 1065, op 6, value 0

**Action**

- Set/add variable: variable group 21, variable 20, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 16

### Event 13

**Trigger**

- Object event: subject 1064, op 2, value 0 (join 2)
- Object event: subject 1064, op 6, value 0

**Action**

- Set/add variable: variable group 21, variable 26, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 15

### Event 14

**Trigger**

- Object event: subject Biolith_Dart (object 25, id 1066), op 2, value 0 (join 2)
- Object event: subject Biolith_Dart (object 25, id 1066), op 6, value 0

**Action**

- Set/add variable: variable group 21, variable 23, subtype 0, value 1

### Event 15

**Trigger**

- Object event: subject Biolith_Dart (object 27, id 1068), op 2, value 0 (join 2)
- Object event: subject Biolith_Dart (object 27, id 1068), op 6, value 0

**Action**

- Set/add variable: variable group 21, variable 25, subtype 0, value 1

### Event 16

**Trigger**

- Object event: subject Biolith_Dart (object 26, id 1067), op 2, value 0 (join 2)
- Object event: subject Biolith_Dart (object 26, id 1067), op 6, value 0

**Action**

- Set/add variable: variable group 21, variable 27, subtype 0, value 1

### Event 17

**Trigger**

- Variable comparison: subject variable group 21, variable 23, op 1, value 1
- Variable comparison: subject variable group 21, variable 25, op 1, value 1
- Variable comparison: subject variable group 21, variable 27, op 1, value 1

**Action**

- Set/add variable: variable group 21, variable 21, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 2, param 717
- Hide/remove HUD contact: contact/list 0, subtype 9, param 51

### Event 18

**Trigger**

- Object event: subject Shuttle_Medium (object 1, id 717), op 11, value 0 (extra 1, 928; flags 2)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Variable comparison: subject variable group 21, variable 21, op 1, value 1
- Variable comparison: subject variable group 21, variable 26, op 1, value 1

**Action**

- Set/add variable: variable group 12, variable 2, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 9, param 10

### Event 19

**Trigger**

- Object event: subject Shuttle_Medium (object 1, id 717), op 2, value 0 (join 1)
- Variable comparison: subject variable group 21, variable 29, op 0, value 1

**Action**

- Set/add variable: variable group 12, variable 2, subtype 0, value 0
- Set/add variable: variable group 12, variable 6, subtype 0, value 1
- Set/add variable: variable group 21, variable 22, subtype 0, value 0
- Mark/flash contact: contact/list 0, subtype 8, param 10
- Mark/flash contact: contact/list 0, subtype 2, param 717
- Set runtime trigger variable: variable group 20, variable 3, subtype 1, value 0

### Event 20

**Trigger**

- Object event: subject Shuttle_Medium (object 1, id 717), op 2, value 0 (join 1)
- Variable comparison: subject variable group 21, variable 29, op 0, value 1

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 15
- Hide/remove HUD contact: contact/list 0, subtype 9, param 16
- Hide/remove HUD contact: contact/list 0, subtype 9, param 10
- Show/update HUD contact: contact/list 0, subtype 11, param 31

### Event 21

**Trigger**

- Object event: subject Shuttle_Medium (object 1, id 717), op 4, value 50

**Action**

- Play dialog: ARGO.SCR, line/variant 7

### Event 22

**Trigger**

- Sector/startup condition family: subject 2, op 0, value 7

**Action**

- Play dialog: DILL.SCR, line/variant 21

### Event 23

**Trigger**

- Object event: subject Shuttle_Medium (object 1, id 717), op 6, value 0 (join 1)
- Object event: subject Shuttle_Medium (object 1, id 717), op 11, value 0 (extra 1, 928; flags 2)

**Action**

- Play dialog: DILL.SCR, line/variant 34
- Mission objective/state: param 2, subtype 0, param 0
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Gate state/action: param 1, subtype 2, param 0
- Set runtime trigger variable: variable group 20, variable 3, subtype 1, value 0
- Mark/flash contact: contact/list 0, subtype 2, param 717
- Mark/flash contact: contact/list 0, subtype 8, param 10
- Show/update HUD contact: contact/list 0, subtype 11, param 31

### Event 24

**Trigger**

- Object event: subject 1065, op 2, value 0 (join 2)
- Object event: subject 1064, op 2, value 0
- Variable comparison: subject variable group 5, variable 11, op 1, value 1

**Action**

- Play dialog: DILL.SCR, line/variant 33
- Set runtime trigger variable: variable group 20, variable 3, subtype 1, value 0

### Event 25

**Trigger**

- Variable comparison: subject variable group 21, variable 22, op 1, value 1
- Object event: subject Shuttle_Medium (object 1, id 717), op 4, value 10

**Action**

- Play dialog: ARGO.SCR, line/variant 2

### Event 26

**Trigger**

- Object event: subject Shuttle_Medium (object 1, id 717), op 3, value 40

**Action**

- Play dialog: ARGO.SCR, line/variant 15

### Event 27

**Trigger**

- Group/spawn-list event: subject 48, op 1, value 40

**Action**

- Play dialog: PLAYER.SCR, line/variant 19

### Event 28

**Trigger**

- Group/spawn-list event: subject 48, op 1, value 70

**Action**

- Play dialog: PLAYER.SCR, line/variant 24

### Event 29

**Trigger**

- Object event: subject Biolith_Dart (object 25, id 1066), op 2, value 0
- Object event: subject Biolith_Dart (object 26, id 1067), op 2, value 0
- Object event: subject Biolith_Dart (object 27, id 1068), op 2, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 6

### Event 30

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 1 (join 1; flags 1)
- Variable comparison: subject variable group 21, variable 26, op 1, value 1 (join 2; flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1 (flags 1)

**Action**

- Play dialog: PLAYER.SCR, line/variant 7

### Event 31

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Variable comparison: subject variable group 21, variable 26, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 2

### Event 32

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Variable comparison: subject variable group 21, variable 21, op 1, value 1
- Variable comparison: subject variable group 21, variable 26, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 13

### Event 33

**Trigger**

- Object event: subject Shuttle_Medium (object 1, id 717), op 2, value 0
- Variable comparison: subject variable group 20, variable 5, op 1, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 6, subtype 0, value 0
- Play dialog: DILL.SCR, line/variant 20
- Set runtime trigger variable: variable group 20, variable 4, subtype 1, value 0

### Event 34

**Trigger**

- Variable comparison: subject variable group 20, variable 6, op 1, value 19
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 36

### Event 35

**Trigger**

- Variable comparison: subject variable group 20, variable 6, op 1, value 27

**Action**

- Play dialog: DILL.SCR, line/variant 21
- Gate state/action: param 1, subtype 2, param 0
- Set/add variable: variable group 12, variable 6, subtype 0, value 0
- Mission objective/state: param 2, subtype 0, param 0
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 36

**Trigger**

- Variable comparison: subject variable group 12, variable 6, op 1, value 2
- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Play dialog: ARGO.SCR, line/variant 12

### Event 37

**Trigger**

- Object arrival: Shuttle_Medium (object 1, id 717) reached Waypoint 10 (tag 1), point 3 (raw value 65539)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Variable comparison: subject variable group 21, variable 21, op 1, value 1
- Variable comparison: subject variable group 21, variable 26, op 1, value 1

**Action**

- Set runtime trigger variable: variable group 20, variable 5, subtype 0, value 0
- Object spawn/action: Shuttle_Medium (object 1, id 717), subtype 5
- Object spawn/action: Shuttle_Medium (object 1, id 717), subtype 9, param 928

### Event 38

**Trigger**

- Object event: subject Shuttle_Medium (object 1, id 717), op 11, value 0 (extra 1, 928; join 2; flags 2)
- Variable comparison: subject variable group 20, variable 5, op 1, value 35

**Action**

- Object spawn/action: Shuttle_Medium (object 1, id 717), subtype 6
- Hide/remove HUD contact: contact/list 0, subtype 9, param 10
- Play scene: unknown index 0, param 0
- Set/add variable: variable group 21, variable 29, subtype 0, value 1
- Set runtime trigger variable: variable group 20, variable 9, subtype 0, value 0
- Set runtime trigger variable: variable group 20, variable 5, subtype 1, value 0

### Event 39

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 1

**Action**

- Object spawn/action: Exile_Claw_Mace (object 21, id 1060), subtype 0

### Event 40

**Trigger**

- Object arrival: Exile_Claw_Mace (object 21, id 1060) reached Waypoint 8 (tag 10), point 2 (raw value 655362)

**Action**

- Object spawn/action: Shuttle_Medium (object 1, id 717), subtype 7
- Set runtime trigger variable: variable group 20, variable 7, subtype 0, value 0
- Gate state/action: param 1, subtype 2, param 0

### Event 41

**Trigger**

- Variable comparison: subject variable group 20, variable 7, op 1, value 1

**Action**

- Object spawn/action: id 928, subtype 7

### Event 42

**Trigger**

- Object arrival: Exile_Claw_Mace (object 21, id 1060) reached Waypoint 8 (tag 10), point 4 (raw value 655364)

**Action**

- Group/spawn-list action: spawn list/group 0, subtype 1, param 1
- Set runtime trigger variable: variable group 20, variable 8, subtype 0, value 0

### Event 43

**Trigger**

- Variable comparison: subject variable group 20, variable 8, op 1, value 3

**Action**

- Group/spawn-list action: spawn list/group 2, subtype 1, param 1

### Event 44

**Trigger**

- Variable comparison: subject variable group 20, variable 8, op 1, value 6

**Action**

- Group/spawn-list action: spawn list/group 3, subtype 1, param 1

### Event 45

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 79

**Action**

- Object spawn/action: Exile_Star_Patrol_Capship (object 28, id 770), subtype 3
- Object spawn/action: Star_Patrol_Enforcer (object 3, id 800), subtype 0
- Object spawn/action: Star_Patrol_Enforcer (object 4, id 801), subtype 0
- Object spawn/action: Star_Patrol_Enforcer (object 5, id 802), subtype 0
- Object spawn/action: Star_Patrol_Enforcer (object 6, id 803), subtype 0
- Object spawn/action: Star_Patrol_Enforcer (object 7, id 804), subtype 0
- Object spawn/action: Star_Patrol_Enforcer (object 8, id 805), subtype 0
- Object spawn/action: Star_Patrol_Enforcer (object 2, id 806), subtype 0

### Event 46

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 85

**Action**

- Object spawn/action: Sol_Shuttle_Exile_Cinematic (object 20, id 796), subtype 0
- Object spawn/action: Star_Patrol_Enforcer (object 9, id 807), subtype 0
- Object spawn/action: Star_Patrol_Enforcer (object 10, id 808), subtype 0
- Object spawn/action: Star_Patrol_Enforcer (object 11, id 809), subtype 0
- Object spawn/action: Star_Patrol_Enforcer (object 12, id 810), subtype 0
- Object spawn/action: Star_Patrol_Enforcer (object 13, id 811), subtype 0
- Object spawn/action: Star_Patrol_Enforcer (object 14, id 812), subtype 0
- Object spawn/action: Star_Patrol_Enforcer (object 15, id 814), subtype 0

### Event 47

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 87

**Action**

- Object spawn/action: Exile_Star_Patrol_Enforcer (object 18, id 794), subtype 0

### Event 48

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 88

**Action**

- Object spawn/action: Exile_Star_Patrol_Enforcer (object 17, id 792), subtype 0
- Object spawn/action: Exile_Star_Patrol_Enforcer (object 16, id 793), subtype 0

### Event 49

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 89

**Action**

- Object spawn/action: Exile_Star_Patrol_Enforcer (object 19, id 791), subtype 0

### Event 50

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 112

**Action**

- Gate state/action: param 799, subtype 2, param 0

### Event 51

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 129

**Action**

- Gate state/action: param 799, subtype 3, param 0

### Event 52

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 1
- Variable comparison: subject variable group 21, variable 26, op 1, value 1

**Action**

- Set/add variable: variable group 21, variable 24, subtype 0, value 1

### Event 53

**Trigger**

- Variable comparison: subject variable group 20, variable 5, op 1, value 2

**Action**

- Set/add variable: variable group 0, variable 3, subtype 0, value 1
- Set/add variable: variable group 0, variable 12, subtype 0, value 1
- Set/add variable: variable group 22, variable 25, subtype 0, value 1
- Set/add variable: variable group 22, variable 10, subtype 0, value 1
- Set/add variable: variable group 22, variable 1, subtype 0, value 0
- Set/add variable: variable group 0, variable 1, subtype 0, value 10
- Set/add variable: variable group 12, variable 2, subtype 0, value 1
- Set/add variable: variable group 0, variable 4, subtype 0, value 0

### Event 54

**Trigger**

- Variable comparison: subject variable group 20, variable 5, op 1, value 2

**Action**

- Set/add variable: variable group 0, variable 2, subtype 0, value 6000
- Player inventory/default-state: param 0, subtype 0, param 0

## Waypoints

### Waypoint 0

- Tag: `24`
- Members: `Sol_Shuttle_Exile_Cinematic (object 20, id 796, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (27229.93, -43.00, -892.44) | None |
| 1 | (27324.01, -34.00, -766.33) | None |
| 2 | (27249.47, -15.00, -641.38) | None |
| 3 | (27101.24, -10.00, -483.73) | None |
| 4 | (27092.28, 0.00, 1038.92) | on arrival play dialog/script or enter gate, param 799 |

### Waypoint 1

- Tag: `23`
- Members: `Exile_Star_Patrol_Enforcer (object 18, id 794, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (27230.25, -43.00, -919.12) | None |
| 1 | (27364.30, -34.00, -763.24) | None |
| 2 | (27280.66, -15.00, -626.46) | None |
| 3 | (27144.59, 0.00, -481.71) | None |
| 4 | (27144.59, 0.00, 551.21) | None |
| 5 | (27282.25, 0.00, 596.60) | None |
| 6 | (27479.44, 0.00, 483.72) | None |

### Waypoint 2

- Tag: `20`
- Members: `Exile_Star_Patrol_Enforcer (object 19, id 791, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (27221.25, -43.00, -859.42) | None |
| 1 | (27280.14, -34.00, -757.48) | None |
| 2 | (27206.96, -15.00, -653.47) | None |
| 3 | (27055.39, 0.00, -481.71) | None |
| 4 | (27050.39, 0.00, 541.27) | None |
| 5 | (26902.54, 0.00, 599.03) | None |
| 6 | (26719.06, 0.00, 472.11) | None |

### Waypoint 3

- Tag: `21`
- Members: `Exile_Star_Patrol_Enforcer (object 17, id 792, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (27099.74, 20.00, -482.71) | None |
| 1 | (27091.49, 20.00, 545.74) | None |
| 2 | (27092.50, 110.00, 601.46) | None |
| 3 | (27091.82, 245.00, 475.54) | None |

### Waypoint 4

- Tag: `50`
- Members: `Exile_Star_Patrol_Enforcer (object 16, id 793, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (27099.95, -25.00, -483.49) | None |
| 1 | (27092.36, -20.00, 551.21) | None |
| 2 | (27092.29, -110.00, 603.46) | None |
| 3 | (27083.29, -245.00, 474.11) | None |

### Waypoint 5

- Tag: `13`
- Members: `Exile_Star_Patrol_Enforcer (object 24, id 754, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1517.09, -600.00, -2123.49) | on arrival activate current object (raw param -1 ignored) |
| 1 | (-1507.89, -600.00, -2101.75) | None |

### Waypoint 6

- Tag: `12`
- Members: `Exile_Star_Patrol_Enforcer (object 23, id 751, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1561.26, -600.00, -2107.04) | on arrival activate current object (raw param -1 ignored) |
| 1 | (-1541.55, -600.00, -2074.47) | None |

### Waypoint 7

- Tag: `11`
- Members: `Exile_Star_Patrol_Enforcer (object 22, id 742, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1469.22, -600.00, -2133.80) | on arrival activate current object (raw param -1 ignored) |
| 1 | (-1466.91, -600.00, -2104.29) | None |

### Waypoint 8

- Tag: `10`
- Members: `Exile_Claw_Mace (object 21, id 1060, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (8.82, -1350.00, -522.05) | None |
| 1 | (-73.30, -1330.00, -437.83) | None |
| 2 | (-505.30, -1330.00, -866.83) | None; listened by Event 40 for Exile_Claw_Mace (object 21, id 1060) |
| 3 | (-577.00, -1280.00, -950.89) | None |
| 4 | (-948.08, -1100.00, -1403.30) | None; listened by Event 42 for Exile_Claw_Mace (object 21, id 1060) |
| 5 | (-1279.78, -945.35, -1727.85) | on arrival activate current object (raw param -1 ignored) |
| 6 | (-1504.55, -764.34, -2054.50) | None |

### Waypoint 9

- Tag: `2`
- Members: `Biolith_Dart (object 25, id 1066, starts at point 0)`, `Biolith_Dart (object 26, id 1067, starts at point 0)`, `Biolith_Dart (object 27, id 1068, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (339.73, -1429.00, 97.62) | None |

### Waypoint 10

- Tag: `1`
- Members: `Shuttle_Medium (object 1, id 717, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1446.69, 568.51, -2449.74) | None |
| 1 | (-305.99, -733.83, -1364.01) | None |
| 2 | (659.08, -1233.00, -73.38) | None |
| 3 | (444.33, -1324.83, 146.86) | on arrival activate current object (raw param -1 ignored); listened by Event 37 for Shuttle_Medium (object 1, id 717) |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Mega_Gate` | 799 | Gate | 27095.41,0.00,1105.04 | 0,0,0 | None |
| 1 | `Shuttle_Medium` | 717 | Interactive | -1643.23,571.08,-2697.90 | 64,0,0 | label: argo; alias: Todd01; secondary groups: CONT_UNKNOWN, ARGOSO 914; waypoint: Waypoint 10 (tag 1, 4 point(s)), starting point 0, arrival event value 65536 |
| 2 | `Star_Patrol_Enforcer` | 806 | Interactive | 26957.65,0.00,449.95 | 128,0,0 | None |
| 3 | `Star_Patrol_Enforcer` | 800 | Interactive | 26966.91,0.00,-305.54 | 128,0,0 | None |
| 4 | `Star_Patrol_Enforcer` | 801 | Interactive | 26963.78,0.00,-177.97 | 128,0,0 | None |
| 5 | `Star_Patrol_Enforcer` | 802 | Interactive | 26966.84,0.00,-51.72 | 128,0,0 | None |
| 6 | `Star_Patrol_Enforcer` | 803 | Interactive | 26963.78,0.00,77.85 | 128,0,0 | None |
| 7 | `Star_Patrol_Enforcer` | 804 | Interactive | 26963.78,0.00,200.78 | 128,0,0 | None |
| 8 | `Star_Patrol_Enforcer` | 805 | Interactive | 26960.71,0.00,327.02 | 128,0,0 | None |
| 9 | `Star_Patrol_Enforcer` | 807 | Interactive | 27222.71,0.00,458.24 | 384,0,0 | None |
| 10 | `Star_Patrol_Enforcer` | 808 | Interactive | 27225.64,0.00,329.67 | 384,0,0 | None |
| 11 | `Star_Patrol_Enforcer` | 809 | Interactive | 27225.64,0.00,196.78 | 384,0,0 | None |
| 12 | `Star_Patrol_Enforcer` | 810 | Interactive | 27225.64,0.00,70.53 | 384,0,0 | None |
| 13 | `Star_Patrol_Enforcer` | 811 | Interactive | 27225.64,0.00,-55.72 | 385,0,0 | None |
| 14 | `Star_Patrol_Enforcer` | 812 | Interactive | 27228.71,0.00,-185.29 | 385,0,0 | None |
| 15 | `Star_Patrol_Enforcer` | 814 | Interactive | 27228.61,0.00,-309.12 | 385,0,0 | None |
| 16 | `Exile_Star_Patrol_Enforcer` | 793 | Interactive | 27328.50,-70.00,-1115.93 | 495,0,0 | label: Escort3; secondary groups: none, ARGOSO 914; waypoint: Waypoint 4 (tag 50, 4 point(s)), starting point 0, arrival event value 3276800 |
| 17 | `Exile_Star_Patrol_Enforcer` | 792 | Interactive | 27287.08,-34.00,-1123.93 | 495,0,0 | label: Escort2; waypoint: Waypoint 3 (tag 21, 4 point(s)), starting point 0, arrival event value 1376256 |
| 18 | `Exile_Star_Patrol_Enforcer` | 794 | Interactive | 27132.38,-43.00,-917.50 | 128,0,0 | label: Escort4; waypoint: Waypoint 1 (tag 23, 7 point(s)), starting point 0, arrival event value 1507328 |
| 19 | `Exile_Star_Patrol_Enforcer` | 791 | Interactive | 27131.87,-43.00,-874.93 | 128,0,0 | label: Escort1; waypoint: Waypoint 2 (tag 20, 7 point(s)), starting point 0, arrival event value 1310720 |
| 20 | `Sol_Shuttle_Exile_Cinematic` | 796 | Interactive | 27130.00,-43.00,-897.88 | 128,0,0 | label: SOLShuttle; waypoint: Waypoint 0 (tag 24, 5 point(s)), starting point 0, arrival event value 1572864 |
| 21 | `Exile_Claw_Mace` | 1060 | Interactive | 102.76,-1349.70,-586.26 | 444,0,0 | label: Imposter; waypoint: Waypoint 8 (tag 10, 7 point(s)), starting point 0, arrival event value 655360 |
| 22 | `Exile_Star_Patrol_Enforcer` | 742 | Interactive | -2226.65,0.00,-3192.07 | 0,0,0 | label: Sol1; group/role: FG_AGT1 / 0; waypoint: Waypoint 7 (tag 11, 2 point(s)), starting point 0, arrival event value 720896 |
| 23 | `Exile_Star_Patrol_Enforcer` | 751 | Interactive | -2333.65,0.00,-3303.99 | 0,0,0 | label: Sol4; group/role: FG_AGT2 / 0; secondary groups: none, ARGOSO 914; waypoint: Waypoint 6 (tag 12, 2 point(s)), starting point 0, arrival event value 786432 |
| 24 | `Exile_Star_Patrol_Enforcer` | 754 | Interactive | -2426.88,0.00,-3407.23 | 0,0,0 | label: Sol7; group/role: FG_AGT3 / 0; secondary groups: none, ARGOSO 914; waypoint: Waypoint 5 (tag 13, 2 point(s)), starting point 0, arrival event value 851968 |
| 25 | `Biolith_Dart` | 1066 | Interactive | 2202.79,-1429.00,1590.22 | 320,0,0 | label: BLFT; group/role: FG_NEWBURN / 1; secondary groups: CONT_023, none; waypoint: Waypoint 9 (tag 2, 1 point(s)), starting point 0, arrival event value 131072 |
| 26 | `Biolith_Dart` | 1067 | Interactive | 2221.40,-1429.00,1560.06 | 320,0,0 | group/role: FG_NEWBURN / 2; secondary groups: CONT_023, none; waypoint: Waypoint 9 (tag 2, 1 point(s)), starting point 0, arrival event value 131072 |
| 27 | `Biolith_Dart` | 1068 | Interactive | 2247.83,-1429.00,1536.37 | 320,0,0 | group/role: FG_NEWBURN / 3; secondary groups: CONT_023, none; waypoint: Waypoint 9 (tag 2, 1 point(s)), starting point 0, arrival event value 131072 |
| 28 | `Exile_Star_Patrol_Capship` | 770 | Interactive | 27082.26,34.00,-1261.13 | 0,0,0 | label: SOLCapShip; secondary groups: none, ARGOSO 914 |
