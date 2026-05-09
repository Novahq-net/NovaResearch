# Tachyon: The Fringe NEUT07A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT07A.SPX` |
| Sector | `QUAD_07` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 6 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 11 |
| Entities | 58 |
| Events | 74 |
| Waypoints | 13 |
| Child Sectors | 0 |
| Scripts | 10 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: GalSpan_Destroyer`, `1: Bora_Carrier`, `2: Bora_Light_Freighter`, `3: Bora_Mace`, `4: GalSpan_Archangel`, `5: GalSpan_Pegasus`, `6: Bora_Battleaxe`, `7: Bora_Mine`, `8: GalSpan_Poseidon`, `9: Bora_Cutlass`, `10: Bora_Shuttle_Medium` |
| Scripts | `BFIGH.SCR`, `G01BSA.SCR`, `G01BFC.SCR`, `PLAYER.SCR`, `INDEP.SCR`, `G01BRA.SCR`, `INTEG.SCR`, `G01GFA.SCR`, `G10GPB.SCR`, `G01GFD.SCR` |
| Scenes | None |
| Labels | `g01bsa`, `g01bfa`, `g01bfb`, `g01bfc`, `G01bra`, `integ` |
| Aliases | `Todd08`, `Todd09`, `Todd10`, `Todd14`, `Todd15`, `Todd16`, `Todd12`, `Todd13`, `Todd18`, `Todd03`, `Todd04`, `Todd02`, `Todd05`, `Todd06`, `Todd07`, `Todd21`, `Todd22`, `Todd23`, `will_01`, `SHIP1_HYPER`, `SHIP2_HYPER`, `SHIP3_HYPER`, `ohshit` |
| Groups | `FG_ROVER`, `CONT_033`, `FG_HAMMER`, `FG_GEMINI`, `FG_CANCER`, `FG_ANVIL`, `FG_SWORD`, `FG_MORNING_STAR`, `FG_SCORPIUS`, `FG_PEGASI`, `FG_MAUL`, `FG_ATLAS`, `FG_CAELUM`, `FG_CATAPULT`, `FG_RIGHTEOUS`, `FG_SERPENS`, `PILGRIM`, `EXEMPTION`, `INTEGRITY`, `CONT_025`, `PAN` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 29
- Set/add variable: variable group 21, variable 33, subtype 0, value 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 1, param 46
- Show/update HUD contact: contact/list 0, subtype 1, param 42
- Mission objective/state: param 65542, subtype 0, param 0
- Set/add variable: variable group 21, variable 33, subtype 0, value 0
- Set/add variable: variable group 21, variable 10, subtype 0, value 1

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 1, subtype 0, value 0
- Set/add variable: variable group 21, variable 24, subtype 0, value 0
- Set/add variable: variable group 21, variable 35, subtype 0, value 1
- Group/spawn-list action: spawn list/group 42, subtype 0
- Group/spawn-list action: spawn list/group 46, subtype 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 4, op 1, value 15

**Action**

- Group/spawn-list action: spawn list/group 51, subtype 0
- Object spawn/action: Bora_Light_Freighter (object 54, id 951), subtype 0
- Object spawn/action: Bora_Light_Freighter (object 55, id 969), subtype 0

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 4, op 1, value 15
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Show/update HUD contact: contact/list 0, subtype 3, param 51
- Hide/remove HUD contact: contact/list 0, subtype 9, param 29
- Object spawn/action: Bora_Shuttle_Medium (object 0, id 841), subtype 14
- Object spawn/action: Bora_Shuttle_Medium (object 1, id 842), subtype 14
- Object spawn/action: Bora_Shuttle_Medium (object 2, id 843), subtype 14

### Event 5

**Trigger**

- Group/spawn-list event: subject 51, op 2, value 65540 (Waypoint 11 (tag 1), point 4)

**Action**

- Object spawn/action: Bora_Carrier (object 56, id 937), subtype 3
- Set/add variable: variable group 21, variable 32, subtype 0, value 1

### Event 6

**Trigger**

- Object arrival: Bora_Carrier (object 56, id 937) reached Waypoint 7 (tag 6), point 0 (raw value 393216)

**Action**

- Set runtime trigger variable: variable group 20, variable 22, subtype 0, value 0

### Event 7

**Trigger**

- Variable comparison: subject variable group 20, variable 22, op 1, value 5

**Action**

- Object spawn/action: Bora_Shuttle_Medium (object 0, id 841), subtype 5
- Object spawn/action: Bora_Shuttle_Medium (object 1, id 842), subtype 5
- Object spawn/action: Bora_Shuttle_Medium (object 2, id 843), subtype 5
- Object spawn/action: Bora_Shuttle_Medium (object 0, id 841), subtype 11, param 937
- Object spawn/action: Bora_Shuttle_Medium (object 1, id 842), subtype 11, param 937
- Object spawn/action: Bora_Shuttle_Medium (object 2, id 843), subtype 11, param 937

### Event 8

**Trigger**

- Object event: subject Bora_Shuttle_Medium (object 0, id 841), op 2, value 0 (join 2)
- Object event: subject Bora_Shuttle_Medium (object 0, id 841), op 13, value 0 (extra 1, 937; flags 2)

**Action**

- Set/add variable: variable group 21, variable 24, subtype 1, value 1
- Object spawn/action: Bora_Shuttle_Medium (object 0, id 841), subtype 15

### Event 9

**Trigger**

- Object event: subject Bora_Shuttle_Medium (object 1, id 842), op 2, value 0 (join 2)
- Object event: subject Bora_Shuttle_Medium (object 1, id 842), op 13, value 0 (extra 1, 937; flags 2)

**Action**

- Set/add variable: variable group 21, variable 24, subtype 1, value 1
- Object spawn/action: Bora_Shuttle_Medium (object 1, id 842), subtype 15

### Event 10

**Trigger**

- Object event: subject Bora_Shuttle_Medium (object 2, id 843), op 2, value 0 (join 2)
- Object event: subject Bora_Shuttle_Medium (object 2, id 843), op 13, value 0 (extra 1, 937; flags 2)

**Action**

- Set/add variable: variable group 21, variable 24, subtype 1, value 1
- Object spawn/action: Bora_Shuttle_Medium (object 2, id 843), subtype 15

### Event 11

**Trigger**

- Variable comparison: subject variable group 21, variable 24, op 1, value 3 (join 2)

**Action**

- Set runtime trigger variable: variable group 20, variable 9, subtype 0, value 0
- Hide/remove HUD contact: contact/list 0, subtype 1, param 51
- Hide/remove HUD contact: contact/list 0, subtype 3, param 51

### Event 12

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 5

**Action**

- Object spawn/action: Bora_Carrier (object 56, id 937), subtype 5
- Object spawn/action: Bora_Carrier (object 56, id 937), subtype 13, param 393218

### Event 13

**Trigger**

- Object event: subject Bora_Carrier (object 56, id 937), op 8, value 0

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 2, param 937
- Set/add variable: variable group 21, variable 23, subtype 0, value 1

### Event 14

**Trigger**

- Variable comparison: subject variable group 21, variable 24, op 1, value 3
- Variable comparison: subject variable group 21, variable 33, op 1, value 0
- Object event: subject Bora_Carrier (object 56, id 937), op 8, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Set/add variable: variable group 13, variable 400, subtype 0, value 1
- Set/add variable: variable group 13, variable 401, subtype 0, value 3
- Show/update HUD contact: contact/list 0, subtype 12, param 33
- Hide/remove HUD contact: contact/list 0, subtype 3, param 51

### Event 15

**Trigger**

- Variable comparison: subject variable group 0, variable 0, op 1, value 2
- Group/spawn-list event: subject 51, op 0, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 11, param 34
- Set/add variable: variable group 13, variable 400, subtype 0, value 0
- Set/add variable: variable group 13, variable 401, subtype 0, value 1
- Play dialog: BFIGH.SCR, line/variant 1

### Event 16

**Trigger**

- Variable comparison: subject variable group 0, variable 0, op 1, value 1
- Group/spawn-list event: subject 51, op 0, value 0
- Group/spawn-list event: subject 42, op 0, value 0
- Group/spawn-list event: subject 46, op 0, value 0
- Variable comparison: subject variable group 21, variable 6, op 1, value 1

**Action**

- Set/add variable: variable group 13, variable 404, subtype 0, value 1
- Set/add variable: variable group 13, variable 405, subtype 0, value 3
- Hide/remove HUD contact: contact/list 0, subtype 10, param 0

### Event 17

**Trigger**

- Variable comparison: subject variable group 21, variable 24, op 1, value 3
- Variable comparison: subject variable group 21, variable 33, op 1, value 0
- Variable comparison: subject variable group 21, variable 23, op 1, value 1
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Set/add variable: variable group 13, variable 404, subtype 0, value 0
- Set/add variable: variable group 13, variable 405, subtype 0, value 1
- Mark/flash contact: contact/list 0, subtype 1, param 51
- Show/update HUD contact: contact/list 0, subtype 11, param 34
- Hide/remove HUD contact: contact/list 0, subtype 1, param 46
- Hide/remove HUD contact: contact/list 0, subtype 1, param 42
- Hide/remove HUD contact: contact/list 0, subtype 1, param 47
- Hide/remove HUD contact: contact/list 0, subtype 1, param 56

### Event 18

**Trigger**

- Group/spawn-list event: subject 281, op 3, value 0 (join 2; flags 1)
- Group/spawn-list event: subject 18, op 3, value 0 (join 2; flags 1)
- Group/spawn-list event: subject 41, op 3, value 0 (join 2; flags 1)
- Group/spawn-list event: subject 27, op 3, value 0 (join 2)
- Group/spawn-list event: subject 52, op 3, value 0 (join 2)
- Group/spawn-list event: subject 55, op 3, value 0 (join 2)

**Action**

- Set/add variable: variable group 21, variable 28, subtype 0, value 1

### Event 19

**Trigger**

- Object event: subject Bora_Shuttle_Medium (object 0, id 841), op 4, value 10

**Action**

- Play dialog: G01BSA.SCR, line/variant 6

### Event 20

**Trigger**

- Object event: subject Bora_Shuttle_Medium (object 1, id 842), op 4, value 10

**Action**

- Play dialog: G01BSA.SCR, line/variant 7

### Event 21

**Trigger**

- Object event: subject Bora_Shuttle_Medium (object 2, id 843), op 4, value 10

**Action**

- Play dialog: G01BFC.SCR, line/variant 14

### Event 22

**Trigger**

- Object arrival: Bora_Light_Freighter (object 54, id 951) reached Waypoint 8 (tag 4), point 4 (raw value 262148)
- Variable comparison: subject variable group 20, variable 4, op 1, value 75

**Action**

- Object spawn/action: Bora_Light_Freighter (object 54, id 951), subtype 4

### Event 23

**Trigger**

- Object arrival: Bora_Light_Freighter (object 55, id 969) reached Waypoint 1 (tag 120), point 4 (raw value 7864324)
- Variable comparison: subject variable group 20, variable 4, op 1, value 75

**Action**

- Object spawn/action: Bora_Light_Freighter (object 55, id 969), subtype 4

### Event 24

**Trigger**

- Variable comparison: subject variable group 20, variable 4, op 1, value 325
- Variable comparison: subject variable group 0, variable 0, op 0, value 2

**Action**

- Play dialog: BFIGH.SCR, line/variant 2
- Object spawn/action: id 1986, subtype 8, param 2

### Event 25

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 2
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Play dialog: PLAYER.SCR, line/variant 4
- Set runtime trigger variable: variable group 20, variable 1, subtype 1, value 0
- Group/spawn-list action: spawn list/group 133, subtype 0
- Group/spawn-list action: spawn list/group 28, subtype 0
- Group/spawn-list action: spawn list/group 47, subtype 0

### Event 26

**Trigger**

- Sector/startup condition family: subject 3, op 0, value 4
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Group/spawn-list action: spawn list/group 27, subtype 1, param 936

### Event 27

**Trigger**

- Group/spawn-list event: subject 27, op 3, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Play dialog: PLAYER.SCR, line/variant 6
- Set runtime trigger variable: variable group 20, variable 4, subtype 0, value 0

### Event 28

**Trigger**

- Sector/startup condition family: subject 3, op 0, value 6

**Action**

- Set runtime trigger variable: variable group 20, variable 1, subtype 0, value 0

### Event 29

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 4
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Play dialog: INDEP.SCR, line/variant 3
- Set runtime trigger variable: variable group 20, variable 1, subtype 1, value 0

### Event 30

**Trigger**

- Sector/startup condition family: subject 4, op 0, value 3

**Action**

- Set runtime trigger variable: variable group 20, variable 1, subtype 0, value 0

### Event 31

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 6
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Play dialog: G01BRA.SCR, line/variant 0
- Set runtime trigger variable: variable group 20, variable 1, subtype 1, value 0

### Event 32

**Trigger**

- Variable comparison: subject variable group 20, variable 4, op 1, value 300
- Variable comparison: subject variable group 0, variable 0, op 1, value 2 (join 2)
- Variable comparison: subject variable group 0, variable 0, op 1, value 2
- Variable comparison: subject variable group 13, variable 401, op 1, value 3

**Action**

- Group/spawn-list action: spawn list/group 52, subtype 1, param 936
- Play dialog: PLAYER.SCR, line/variant 17

### Event 33

**Trigger**

- Variable comparison: subject variable group 0, variable 0, op 1, value 2
- Variable comparison: subject variable group 21, variable 32, op 1, value 1

**Action**

- Set runtime trigger variable: variable group 20, variable 1, subtype 0, value 0
- Play dialog: G01BSA.SCR, line/variant 1
- Object spawn/action: id 723, subtype 8, param 4
- Object spawn/action: id 739, subtype 8, param 4
- Object spawn/action: id 1986, subtype 8, param 4

### Event 34

**Trigger**

- Variable comparison: subject variable group 0, variable 0, op 1, value 2
- Sector/startup condition family: subject 1, op 0, value 1 (join 2)
- Variable comparison: subject variable group 0, variable 0, op 1, value 2
- Variable comparison: subject variable group 20, variable 1, op 1, value 3
- Object event: subject Bora_Shuttle_Medium (object 0, id 841), op 2, value 0

**Action**

- Play dialog: INTEG.SCR, line/variant 0
- Set runtime trigger variable: variable group 20, variable 1, subtype 1, value 0

### Event 35

**Trigger**

- Variable comparison: subject variable group 0, variable 0, op 1, value 2
- Variable comparison: subject variable group 21, variable 34, op 1, value 1
- Variable comparison: subject variable group 21, variable 33, op 1, value 0
- Variable comparison: subject variable group 21, variable 24, op 1, value 3

**Action**

- Play dialog: INTEG.SCR, line/variant 1
- Show/update HUD contact: contact/list 0, subtype 2, param 937

### Event 36

**Trigger**

- Variable comparison: subject variable group 21, variable 23, op 1, value 1
- Variable comparison: subject variable group 21, variable 33, op 1, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Play dialog: BFIGH.SCR, line/variant 3
- Hide/remove HUD contact: contact/list 0, subtype 2, param 937

### Event 37

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 3
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Play dialog: G01GFA.SCR, line/variant 5

### Event 38

**Trigger**

- Variable comparison: subject variable group 0, variable 0, op 1, value 2
- Object event: subject Bora_Light_Freighter (object 54, id 951), op 4, value 20 (join 2)
- Variable comparison: subject variable group 0, variable 0, op 1, value 2
- Object event: subject Bora_Light_Freighter (object 55, id 969), op 4, value 20

**Action**

- Play dialog: G01BRA.SCR, line/variant 1

### Event 39

**Trigger**

- Variable comparison: subject variable group 0, variable 0, op 1, value 2
- Group/spawn-list event: subject 51, op 1, value 30

**Action**

- Play dialog: G01GFA.SCR, line/variant 10

### Event 40

**Trigger**

- Variable comparison: subject variable group 0, variable 0, op 1, value 2
- Group/spawn-list event: subject 51, op 1, value 60

**Action**

- Play dialog: PLAYER.SCR, line/variant 18

### Event 41

**Trigger**

- Group/spawn-list event: subject 56, op 1, value 50
- Variable comparison: subject variable group 0, variable 0, op 1, value 2
- Variable comparison: subject variable group 21, variable 23, op 1, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 7

### Event 42

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 2
- Variable comparison: subject variable group 0, variable 0, op 1, value 1
- Variable comparison: subject variable group 21, variable 28, op 1, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 40
- Set runtime trigger variable: variable group 20, variable 1, subtype 1, value 0

### Event 43

**Trigger**

- Sector/startup condition family: subject 3, op 0, value 40

**Action**

- Set runtime trigger variable: variable group 20, variable 1, subtype 0, value 0

### Event 44

**Trigger**

- Variable comparison: subject variable group 20, variable 1, op 1, value 4
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Play dialog: G01GFA.SCR, line/variant 17
- Set runtime trigger variable: variable group 20, variable 4, subtype 0, value 0
- Set runtime trigger variable: variable group 20, variable 1, subtype 1, value 0
- Group/spawn-list action: spawn list/group 27, subtype 1, param 936
- Group/spawn-list action: spawn list/group 55, subtype 1, param 936

### Event 45

**Trigger**

- Sector/startup condition family: subject 7, op 0, value 17
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Play dialog: INDEP.SCR, line/variant 5

### Event 46

**Trigger**

- Variable comparison: subject variable group 21, variable 32, op 1, value 1
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Play dialog: G10GPB.SCR, line/variant 0
- Object spawn/action: id 723, subtype 8, param 4
- Object spawn/action: id 739, subtype 8, param 4
- Object spawn/action: id 1986, subtype 8, param 4

### Event 47

**Trigger**

- Sector/startup condition family: subject 8, op 0, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Play dialog: G01GFD.SCR, line/variant 0

### Event 48

**Trigger**

- Group/spawn-list event: subject 51, op 1, value 30
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 43

### Event 49

**Trigger**

- Group/spawn-list event: subject 51, op 1, value 60
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Play dialog: G01BFC.SCR, line/variant 13

### Event 50

**Trigger**

- Group/spawn-list event: subject 51, op 0, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 44
- Hide/remove HUD contact: contact/list 0, subtype 1, param 51

### Event 51

**Trigger**

- Variable comparison: subject variable group 0, variable 0, op 1, value 1
- Variable comparison: subject variable group 21, variable 33, op 1, value 0
- Variable comparison: subject variable group 21, variable 24, op 1, value 3
- Variable comparison: subject variable group 21, variable 32, op 1, value 1

**Action**

- Play dialog: INTEG.SCR, line/variant 5

### Event 52

**Trigger**

- Object event: subject Bora_Light_Freighter (object 54, id 951), op 0, value 0 (flags 2)
- Variable comparison: subject variable group 21, variable 33, op 1, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 1 (join 2)
- Object event: subject Bora_Light_Freighter (object 55, id 969), op 0, value 0 (flags 2)
- Variable comparison: subject variable group 0, variable 0, op 1, value 1
- Variable comparison: subject variable group 21, variable 33, op 1, value 0

**Action**

- Play dialog: G01GFA.SCR, line/variant 24

### Event 53

**Trigger**

- Variable comparison: subject variable group 13, variable 401, op 1, value 1 (join 2)
- Variable comparison: subject variable group 13, variable 401, op 1, value 3 (join 2)
- Variable comparison: subject variable group 13, variable 405, op 1, value 1 (join 2)
- Variable comparison: subject variable group 13, variable 405, op 1, value 3 (join 2)

**Action**

- Set runtime trigger variable: variable group 20, variable 26, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 54

**Trigger**

- Variable comparison: subject variable group 20, variable 26, op 1, value 120
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Object spawn/action: GalSpan_Destroyer (object 57, id 1857), subtype 3
- Play dialog: PLAYER.SCR, line/variant 123
- Group/spawn-list action: spawn list/group 216, subtype 1, param 936
- Group/spawn-list action: spawn list/group 55, subtype 1, param 936
- Group/spawn-list action: spawn list/group 52, subtype 1, param 936

### Event 55

**Trigger**

- Variable comparison: subject variable group 13, variable 405, op 1, value 3
- Variable comparison: subject variable group 20, variable 26, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 176
- Show/update HUD contact: contact/list 0, subtype 12, param 33
- Object spawn/action: GalSpan_Destroyer (object 57, id 1857), subtype 3
- Object spawn/action: id 1986, subtype 8, param 2

### Event 56

**Trigger**

- Object event: subject Bora_Carrier (object 56, id 937), op 9, value 0
- Variable comparison: subject variable group 0, variable 0, op 0, value 1

**Action**

- Object spawn/action: Bora_Carrier (object 56, id 937), subtype 18

### Event 57

**Trigger**

- Variable comparison: subject variable group 20, variable 4, op 1, value 5
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Play dialog: G01GFD.SCR, line/variant 0
- Group/spawn-list action: spawn list/group 52, subtype 1, param 936
- Group/spawn-list action: spawn list/group 216, subtype 1, param 936

### Event 58

**Trigger**

- Group/spawn-list event: subject 51, op 0, value 0

**Action**

- Set/add variable: variable group 21, variable 33, subtype 0, value 1

### Event 59

**Trigger**

- Object event: subject Bora_Shuttle_Medium (object 0, id 841), op 13, value 0 (extra 1, 937; join 2; flags 2)
- Object event: subject Bora_Shuttle_Medium (object 1, id 842), op 13, value 0 (extra 1, 937; join 2; flags 2)
- Object event: subject Bora_Shuttle_Medium (object 2, id 843), op 13, value 0 (extra 1, 937; join 2; flags 2)

**Action**

- Set/add variable: variable group 21, variable 34, subtype 0, value 1

### Event 60

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Group/spawn-list event: subject 56, op 3, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 1
- Variable comparison: subject variable group 21, variable 11, op 1, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 1, param 56

### Event 61

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Group/spawn-list event: subject 56, op 3, value 0
- Group/spawn-list event: subject 51, op 0, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 1
- Variable comparison: subject variable group 21, variable 6, op 1, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 1, param 56

### Event 62

**Trigger**

- Group/spawn-list event: subject 51, op 3, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 1, param 51
- Hide/remove HUD contact: contact/list 0, subtype 1, param 47
- Hide/remove HUD contact: contact/list 0, subtype 1, param 46
- Hide/remove HUD contact: contact/list 0, subtype 1, param 56
- Hide/remove HUD contact: contact/list 0, subtype 1, param 42
- Set/add variable: variable group 21, variable 11, subtype 0, value 1

### Event 63

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Object spawn/action: id 723, subtype 8, param 1
- Object spawn/action: id 739, subtype 8, param 1

### Event 64

**Trigger**

- Variable comparison: subject variable group 21, variable 24, op 1, value 1

**Action**

- Set runtime trigger variable: variable group 20, variable 31, subtype 0, value 0

### Event 65

**Trigger**

- Variable comparison: subject variable group 20, variable 31, op 1, value 50 (join 1)
- Variable comparison: subject variable group 21, variable 24, op 1, value 3

**Action**

- Group/spawn-list action: spawn list/group 51, subtype 8, param 8519680 (Waypoint 0 (tag 130), point 0)
- Group/spawn-list action: spawn list/group 51, subtype 2
- Set runtime trigger variable: variable group 20, variable 31, subtype 1, value 0

### Event 66

**Trigger**

- Group/spawn-list event: subject 51, op 2, value 8519681 (Waypoint 0 (tag 130), point 1)

**Action**

- Group/spawn-list action: spawn list/group 51, subtype 2
- Group/spawn-list action: spawn list/group 51, subtype 5, param 937

### Event 67

**Trigger**

- Group/spawn-list event: subject 56, op 3, value 0 (join 2)
- Area/player/sector/dock/time event: subject 0, op 2, value 0 (join 2)
- Group/spawn-list event: subject 281, op 3, value 0 (join 2)
- Group/spawn-list event: subject 18, op 3, value 0 (join 2)
- Group/spawn-list event: subject 27, op 3, value 0 (join 2)
- Group/spawn-list event: subject 41, op 3, value 0 (join 2)

**Action**

- Object spawn/action: id 723, subtype 6
- Object spawn/action: id 739, subtype 6
- Object spawn/action: id 1986, subtype 8, param 1

### Event 68

**Trigger**

- Group/spawn-list event: subject 56, op 0, value 0 (join 2)
- Group/spawn-list event: subject 56, op 6, value 0 (join 2)

**Action**

- Set/add variable: variable group 21, variable 6, subtype 0, value 1

### Event 69

**Trigger**

- Group/spawn-list event: subject 51, op 0, value 0
- Variable comparison: subject variable group 21, variable 12, op 1, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 1, param 42

### Event 70

**Trigger**

- Group/spawn-list event: subject 51, op 0, value 0
- Variable comparison: subject variable group 21, variable 13, op 1, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 1, param 46

### Event 71

**Trigger**

- Group/spawn-list event: subject 51, op 2, value 65542 (Waypoint 11 (tag 1), point 6) (flags 4)

**Action**

- Object spawn/action: Bora_Shuttle_Medium (object 0, id 841), subtype 11, param 937
- Object spawn/action: Bora_Shuttle_Medium (object 1, id 842), subtype 11, param 937
- Object spawn/action: Bora_Shuttle_Medium (object 2, id 843), subtype 11, param 937

### Event 72

**Trigger**

- Group/spawn-list event: subject 42, op 0, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Set/add variable: variable group 21, variable 12, subtype 0, value 1

### Event 73

**Trigger**

- Group/spawn-list event: subject 46, op 0, value 0
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Set/add variable: variable group 21, variable 13, subtype 0, value 1

## Waypoints

### Waypoint 0

- Tag: `130`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-559.86, -3387.11, -1570.82) | None |
| 1 | (-639.25, -3388.16, -1570.82) | on arrival activate current object (raw param -1 ignored) |
| 2 | (-807.70, -3388.16, -1570.82) | None |

### Waypoint 1

- Tag: `120`
- Members: `Bora_Light_Freighter (object 55, id 969, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (210.42, -2117.28, 1110.87) | None |
| 1 | (208.08, -2108.77, 1678.31) | None |
| 2 | (207.99, -2196.14, 1983.04) | None |
| 3 | (207.99, -2658.54, 2257.34) | None |
| 4 | (207.68, -3540.61, 2253.14) | on arrival action 1, param -1; listened by Event 23 for Bora_Light_Freighter (object 55, id 969) |

### Waypoint 2

- Tag: `101`
- Members: `GalSpan_Destroyer (object 57, id 1857, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (1391.83, -3454.09, 0.00) | None |
| 1 | (450.98, -3454.09, 0.00) | None |
| 2 | (-13.17, -3461.36, 0.00) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 3

- Tag: `10`
- Members: `Bora_Battleaxe (object 14, id 1181, starts at point 0)`, `Bora_Battleaxe (object 15, id 1182, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (9.21, -3931.17, 125.00) | None |
| 1 | (128.11, -3685.25, 245.36) | None |
| 2 | (-232.33, -3610.91, 245.37) | None |
| 3 | (-379.85, -3406.43, 3.86) | on arrival redirect to Waypoint 3 (tag 10), point 0 |

### Waypoint 4

- Tag: `9`
- Members: `GalSpan_Poseidon (object 6, id 1124, starts at point 0)`, `GalSpan_Poseidon (object 7, id 1125, starts at point 0)`, `GalSpan_Poseidon (object 8, id 1126, starts at point 0)`, `GalSpan_Pegasus (object 50, id 1196, starts at point 0)`, `GalSpan_Pegasus (object 51, id 1197, starts at point 0)`, `GalSpan_Pegasus (object 52, id 1198, starts at point 0)`, `GalSpan_Pegasus (object 53, id 1989, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-11.59, -3962.40, 170.12) | None |
| 1 | (-11.00, -3760.07, 697.24) | None |
| 2 | (230.00, -3316.75, 988.56) | None |
| 3 | (-328.83, -3313.46, 778.14) | None |
| 4 | (27.31, -3273.88, -693.89) | on arrival redirect to Waypoint 4 (tag 9), point 3 |

### Waypoint 5

- Tag: `8`
- Members: `GalSpan_Poseidon (object 23, id 1193, starts at point 0)`, `GalSpan_Poseidon (object 24, id 1805, starts at point 0)`, `GalSpan_Poseidon (object 25, id 1806, starts at point 0)`, `GalSpan_Poseidon (object 37, id 983, starts at point 0)`, `GalSpan_Poseidon (object 38, id 984, starts at point 0)`, `GalSpan_Poseidon (object 39, id 985, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-11.59, -3958.83, 78.00) | None |
| 1 | (-155.93, -3880.35, -405.30) | None |
| 2 | (-206.96, -3700.99, -1499.75) | None |
| 3 | (250.00, -3205.59, -342.13) | on arrival redirect to Waypoint 5 (tag 8), point 2 |

### Waypoint 6

- Tag: `7`
- Members: `GalSpan_Poseidon (object 9, id 1189, starts at point 0)`, `GalSpan_Poseidon (object 10, id 1190, starts at point 0)`, `GalSpan_Poseidon (object 11, id 1191, starts at point 0)`, `GalSpan_Pegasus (object 26, id 950, starts at point 0)`, `GalSpan_Pegasus (object 27, id 978, starts at point 0)`, `GalSpan_Pegasus (object 28, id 980, starts at point 0)`, `GalSpan_Archangel (object 40, id 1888, starts at point 0)`, `GalSpan_Archangel (object 41, id 1889, starts at point 0)`, `GalSpan_Archangel (object 42, id 1890, starts at point 0)`, `GalSpan_Archangel (object 43, id 1988, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-11.59, -3955.69, 113.45) | None |
| 1 | (53.74, -3213.48, 78.97) | None |
| 2 | (137.27, -3264.60, -878.13) | None |
| 3 | (5.07, -3787.77, 87.58) | None |
| 4 | (59.00, -3810.86, 621.67) | on arrival redirect to Waypoint 6 (tag 7), point 3 |

### Waypoint 7

- Tag: `6`
- Members: `Bora_Carrier (object 56, id 937, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1533.65, -3488.23, -1843.76) | on arrival activate current object (raw param -1 ignored); listened by Event 6 for Bora_Carrier (object 56, id 937) |
| 1 | (-1531.20, -3488.23, -1508.96) | on arrival activate current object (raw param -1 ignored) |
| 2 | (-1531.59, -3490.66, -1187.21) | on arrival action 1, param -1 |

### Waypoint 8

- Tag: `4`
- Members: `Bora_Light_Freighter (object 54, id 951, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (121.70, -2110.00, 1108.93) | None |
| 1 | (118.11, -2246.37, 1515.95) | None |
| 2 | (118.11, -2402.45, 1722.06) | None |
| 3 | (118.11, -2910.47, 1998.93) | None |
| 4 | (118.11, -3606.33, 1995.60) | on arrival action 1, param -1; listened by Event 22 for Bora_Light_Freighter (object 54, id 951) |

### Waypoint 9

- Tag: `5`
- Members: `Bora_Battleaxe (object 44, id 893, starts at point 0)`, `Bora_Battleaxe (object 45, id 894, starts at point 0)`, `Bora_Battleaxe (object 46, id 2008, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (147.78, -2110.00, 1175.52) | None |
| 1 | (170.08, -2143.12, 1582.98) | None |
| 2 | (245.32, -3679.55, 585.86) | on arrival redirect to Waypoint 10 (tag 3), point 2 |

### Waypoint 10

- Tag: `3`
- Members: `Bora_Cutlass (object 29, id 890, starts at point 0)`, `Bora_Cutlass (object 30, id 891, starts at point 0)`, `Bora_Cutlass (object 31, id 892, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (129.10, -2130.00, 1022.11) | None |
| 1 | (98.00, -2110.00, 1171.66) | None |
| 2 | (-40.00, -3324.38, 1105.74) | None |
| 3 | (-40.00, -3746.84, -89.19) | on arrival redirect to Waypoint 10 (tag 3), point 2 |

### Waypoint 11

- Tag: `1`
- Members: `Bora_Shuttle_Medium (object 0, id 841, starts at point 0)`, `Bora_Shuttle_Medium (object 1, id 842, starts at point 0)`, `Bora_Shuttle_Medium (object 2, id 843, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (166.57, -2121.79, -812.17) | None |
| 1 | (3.32, -2117.82, -976.67) | None |
| 2 | (-409.95, -2695.89, -1621.10) | None |
| 3 | (-400.50, -3387.13, -1584.91) | None |
| 4 | (-559.97, -3387.20, -1583.32) | None |
| 5 | (-636.02, -3387.72, -1583.04) | on arrival activate current object (raw param -1 ignored) |
| 6 | (-804.64, -3387.83, -1582.87) | on arrival redirect to Waypoint 11 (tag 1), point 6 |

### Waypoint 12

- Tag: `2`
- Members: `Bora_Cutlass (object 3, id 844, starts at point 0)`, `Bora_Cutlass (object 4, id 845, starts at point 0)`, `Bora_Cutlass (object 5, id 846, starts at point 0)`, `Bora_Cutlass (object 17, id 838, starts at point 1)`, `Bora_Cutlass (object 18, id 839, starts at point 1)`, `Bora_Cutlass (object 19, id 840, starts at point 1)`, `Bora_Mace (object 47, id 1941, starts at point 0)`, `Bora_Mace (object 48, id 1942, starts at point 0)`, `Bora_Mace (object 49, id 1943, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (151.45, -2121.79, -792.03) | None |
| 1 | (73.15, -2110.41, -1112.96) | None |
| 2 | (-593.01, -3222.42, -983.33) | None |
| 3 | (-355.91, -3239.68, -672.06) | None |
| 4 | (-247.22, -3219.97, 513.95) | on arrival redirect to Waypoint 12 (tag 2), point 2 |

## Spawn Lists

### Spawn List 0

- ID: `281`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 9 | none | None |
| 1 | 6 | id 1986 | None |
| 2 | 6 | id 723 | None |
| 3 | 6 | id 739 | None |
| 4 | 5 | id 51 | None |
| 5 | 5 | spawn list 15 | None |
| 6 | 2 | Bora_Light_Freighter (object 55, id 969) | None |
| 7 | 2 | Bora_Light_Freighter (object 54, id 951) | None |
| 8 | 6 | Bora_Carrier (object 56, id 937) | None |
| 9 | 0 | none | None |

### Spawn List 1

- ID: `41`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 5 | spawn list 15 | None |
| 1 | 1 | id 51 | None |
| 2 | 6 | id 723 | None |
| 3 | 6 | id 739 | None |
| 4 | 6 | id 1986 | None |
| 5 | 9 | none | None |
| 6 | 0 | none | None |
| 7 | 6 | Bora_Carrier (object 56, id 937) | None |

### Spawn List 2

- ID: `216`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 5 | id 51 | None |
| 1 | 6 | id 1986 | None |
| 2 | 5 | spawn list 15 | None |
| 3 | 6 | id 739 | None |
| 4 | 6 | id 723 | None |
| 5 | 6 | Bora_Carrier (object 56, id 937) | None |
| 6 | 0 | none | None |

### Spawn List 3

- ID: `133`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 9 | none | None |
| 1 | 6 | id 723 | None |
| 2 | 6 | id 739 | None |
| 3 | 6 | id 1986 | None |
| 4 | 0 | none | None |
| 5 | 8 | id 51 | None |

### Spawn List 4

- ID: `27`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |
| 1 | 6 | id 723 | None |
| 2 | 6 | id 739 | None |
| 3 | 5 | id 51 | None |
| 4 | 6 | id 1986 | None |
| 5 | 5 | spawn list 15 | None |
| 6 | 6 | Bora_Carrier (object 56, id 937) | None |

### Spawn List 5

- ID: `55`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 5 | id 51 | None |
| 1 | 0 | none | None |
| 2 | 6 | id 739 | None |
| 3 | 6 | id 723 | None |
| 4 | 6 | id 1986 | None |
| 5 | 6 | Bora_Carrier (object 56, id 937) | None |
| 6 | 5 | spawn list 15 | None |

### Spawn List 6

- ID: `18`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 9 | none | None |
| 1 | 6 | id 723 | None |
| 2 | 6 | id 739 | None |
| 3 | 5 | spawn list 15 | None |
| 4 | 6 | id 1986 | None |
| 5 | 5 | id 51 | None |
| 6 | 0 | none | None |

### Spawn List 7

- ID: `15`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 8

- ID: `56`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 9 | none | None |
| 1 | 8 | id 51 | None |
| 2 | 6 | id 1986 | None |
| 3 | 6 | id 723 | None |
| 4 | 6 | id 739 | None |
| 5 | 0 | none | None |

### Spawn List 9

- ID: `47`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 6 | Bora_Battleaxe (object 14, id 1181) | None |
| 1 | 8 | id 51 | None |
| 2 | 6 | id 1986 | None |
| 3 | 6 | id 723 | None |
| 4 | 6 | id 739 | None |
| 5 | 0 | none | None |

### Spawn List 10

- ID: `42`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 8 | id 51 | None |
| 1 | 6 | id 1986 | None |
| 2 | 6 | id 723 | None |
| 3 | 6 | id 739 | None |
| 4 | 0 | none | None |

### Spawn List 11

- ID: `28`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 8 | id 51 | None |
| 1 | 0 | none | None |
| 2 | 6 | id 1986 | None |
| 3 | 6 | id 739 | None |
| 4 | 6 | id 723 | None |

### Spawn List 12

- ID: `46`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 9 | none | None |
| 1 | 8 | id 51 | None |
| 2 | 0 | none | None |
| 3 | 6 | id 1986 | None |
| 4 | 6 | id 723 | None |
| 5 | 6 | id 739 | None |

### Spawn List 13

- ID: `52`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 5 | id 51 | None |
| 1 | 0 | none | None |
| 2 | 6 | id 739 | None |
| 3 | 6 | id 723 | None |
| 4 | 6 | id 1986 | None |
| 5 | 6 | Bora_Carrier (object 56, id 937) | None |
| 6 | 9 | none | None |
| 7 | 5 | spawn list 15 | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Bora_Shuttle_Medium` | 841 | Interactive | 108.81,-2133.97,-435.32 | 256,0,0 | label: g01bsa; group/role: FG_ROVER / 0; secondary groups: CONT_033, none; waypoint: Waypoint 11 (tag 1, 7 point(s)), starting point 0, arrival event value 65536 |
| 1 | `Bora_Shuttle_Medium` | 842 | Interactive | 143.74,-2134.80,-435.86 | 256,0,0 | group/role: FG_ROVER / 0; secondary groups: CONT_033, none; waypoint: Waypoint 11 (tag 1, 7 point(s)), starting point 0, arrival event value 65536 |
| 2 | `Bora_Shuttle_Medium` | 843 | Interactive | 179.90,-2134.80,-437.60 | 256,0,0 | group/role: FG_ROVER / 0; secondary groups: CONT_033, none; waypoint: Waypoint 11 (tag 1, 7 point(s)), starting point 0, arrival event value 65536 |
| 3 | `Bora_Cutlass` | 844 | Interactive | 182.00,-2137.35,-600.30 | 256,0,0 | group/role: FG_HAMMER / 1; waypoint: Waypoint 12 (tag 2, 5 point(s)), starting point 0, arrival event value 131072 |
| 4 | `Bora_Cutlass` | 845 | Interactive | 161.42,-2137.35,-600.59 | 256,0,0 | group/role: FG_HAMMER / 2; waypoint: Waypoint 12 (tag 2, 5 point(s)), starting point 0, arrival event value 131072 |
| 5 | `Bora_Cutlass` | 846 | Interactive | 144.20,-2137.35,-599.49 | 256,0,0 | group/role: FG_HAMMER / 3; waypoint: Waypoint 12 (tag 2, 5 point(s)), starting point 0, arrival event value 131072 |
| 6 | `GalSpan_Poseidon` | 1124 | Interactive | 0.00,-4889.27,210.26 | 128,128,0 | group/role: FG_GEMINI / 1; alias: Todd08; waypoint: Waypoint 4 (tag 9, 5 point(s)), starting point 0, arrival event value 589824 |
| 7 | `GalSpan_Poseidon` | 1125 | Interactive | 0.00,-4889.38,177.03 | 128,128,0 | group/role: FG_GEMINI / 2; alias: Todd09; waypoint: Waypoint 4 (tag 9, 5 point(s)), starting point 0, arrival event value 589824 |
| 8 | `GalSpan_Poseidon` | 1126 | Interactive | 0.00,-4888.96,144.40 | 128,128,0 | group/role: FG_GEMINI / 3; alias: Todd10; waypoint: Waypoint 4 (tag 9, 5 point(s)), starting point 0, arrival event value 589824 |
| 9 | `GalSpan_Poseidon` | 1189 | Interactive | 0.00,-4888.03,38.74 | 128,128,0 | group/role: FG_CANCER / 1; alias: Todd14; waypoint: Waypoint 6 (tag 7, 5 point(s)), starting point 0, arrival event value 458752 |
| 10 | `GalSpan_Poseidon` | 1190 | Interactive | 0.00,-4888.94,10.32 | 128,128,0 | group/role: FG_CANCER / 2; alias: Todd15; waypoint: Waypoint 6 (tag 7, 5 point(s)), starting point 0, arrival event value 458752 |
| 11 | `GalSpan_Poseidon` | 1191 | Interactive | 0.00,-4887.21,-20.64 | 128,128,0 | group/role: FG_CANCER / 3; alias: Todd16; waypoint: Waypoint 6 (tag 7, 5 point(s)), starting point 0, arrival event value 458752 |
| 12 | `Bora_Mine` | 1231 | Interactive | 325.48,-4141.01,-133.55 | 184,156,113 | group/role: FG_ANVIL / 0 |
| 13 | `Bora_Mine` | 1246 | Interactive | -372.83,-4024.84,304.04 | 188,269,347 | group/role: FG_ANVIL / 0 |
| 14 | `Bora_Battleaxe` | 1181 | Interactive | 0.00,-4704.04,107.56 | 128,128,0 | label: g01bfa; group/role: FG_SWORD / 1; alias: Todd12; waypoint: Waypoint 3 (tag 10, 4 point(s)), starting point 0, arrival event value 655360 |
| 15 | `Bora_Battleaxe` | 1182 | Interactive | 0.00,-4704.04,82.72 | 128,128,0 | label: g01bfb; group/role: FG_SWORD / 2; alias: Todd13; waypoint: Waypoint 3 (tag 10, 4 point(s)), starting point 0, arrival event value 655360 |
| 16 | `Bora_Mine` | 1783 | Interactive | 199.46,-4022.11,142.68 | 229,47,281 | group/role: FG_ANVIL / 0 |
| 17 | `Bora_Cutlass` | 838 | Interactive | 153.00,-2138.80,-529.64 | 256,0,0 | group/role: FG_MORNING_STAR / 1; waypoint: Waypoint 12 (tag 2, 5 point(s)), starting point 1, arrival event value 131073 |
| 18 | `Bora_Cutlass` | 839 | Interactive | 172.18,-2138.80,-496.15 | 256,0,0 | group/role: FG_MORNING_STAR / 2; waypoint: Waypoint 12 (tag 2, 5 point(s)), starting point 1, arrival event value 131073 |
| 19 | `Bora_Cutlass` | 840 | Interactive | 130.34,-2138.80,-496.72 | 256,0,0 | group/role: FG_MORNING_STAR / 3; waypoint: Waypoint 12 (tag 2, 5 point(s)), starting point 1, arrival event value 131073 |
| 20 | `Bora_Mine` | 1845 | Interactive | -127.60,-4111.22,6.39 | 229,47,281 | group/role: FG_ANVIL / 0 |
| 21 | `Bora_Mine` | 1922 | Interactive | 114.52,-4252.85,453.41 | 229,47,281 | group/role: FG_ANVIL / 0 |
| 22 | `Bora_Mine` | 1923 | Interactive | -184.01,-4040.97,-316.28 | 229,47,281 | group/role: FG_ANVIL / 0 |
| 23 | `GalSpan_Poseidon` | 1193 | Interactive | 0.00,-4958.03,64.01 | 128,128,0 | group/role: FG_SCORPIUS / 1; alias: Todd18; waypoint: Waypoint 5 (tag 8, 4 point(s)), starting point 0, arrival event value 524288 |
| 24 | `GalSpan_Poseidon` | 1805 | Interactive | 0.00,-4959.32,98.61 | 128,128,0 | group/role: FG_SCORPIUS / 1; alias: Todd18; waypoint: Waypoint 5 (tag 8, 4 point(s)), starting point 0, arrival event value 524288 |
| 25 | `GalSpan_Poseidon` | 1806 | Interactive | 0.00,-4958.46,130.28 | 128,128,0 | group/role: FG_SCORPIUS / 1; alias: Todd18; waypoint: Waypoint 5 (tag 8, 4 point(s)), starting point 0, arrival event value 524288 |
| 26 | `GalSpan_Pegasus` | 950 | Interactive | 0.00,-4820.92,177.16 | 128,128,0 | group/role: FG_PEGASI / 2; alias: Todd03; waypoint: Waypoint 6 (tag 7, 5 point(s)), starting point 0, arrival event value 458752 |
| 27 | `GalSpan_Pegasus` | 978 | Interactive | 0.00,-4820.46,145.27 | 128,128,0 | group/role: FG_PEGASI / 3; alias: Todd04; waypoint: Waypoint 6 (tag 7, 5 point(s)), starting point 0, arrival event value 458752 |
| 28 | `GalSpan_Pegasus` | 980 | Interactive | 0.00,-4821.46,208.65 | 128,128,0 | group/role: FG_PEGASI / 1; alias: Todd02; waypoint: Waypoint 6 (tag 7, 5 point(s)), starting point 0, arrival event value 458752 |
| 29 | `Bora_Cutlass` | 890 | Interactive | 145.79,-2136.00,893.83 | 0,0,0 | group/role: FG_MAUL / 1; waypoint: Waypoint 10 (tag 3, 4 point(s)), starting point 0, arrival event value 196608 |
| 30 | `Bora_Cutlass` | 891 | Interactive | 162.86,-2136.00,894.28 | 0,0,0 | group/role: FG_MAUL / 2; waypoint: Waypoint 10 (tag 3, 4 point(s)), starting point 0, arrival event value 196608 |
| 31 | `Bora_Cutlass` | 892 | Interactive | 178.70,-2136.00,895.75 | 0,0,0 | group/role: FG_MAUL / 3; waypoint: Waypoint 10 (tag 3, 4 point(s)), starting point 0, arrival event value 196608 |
| 32 | `Bora_Mine` | 1955 | Interactive | -279.92,-4170.47,290.45 | 229,47,281 | group/role: FG_ANVIL / 0 |
| 33 | `Bora_Mine` | 1956 | Interactive | 34.67,-4266.24,40.55 | 229,47,281 | group/role: FG_ANVIL / 0 |
| 34 | `Bora_Mine` | 1968 | Interactive | -372.83,-4024.92,491.68 | 188,269,347 | group/role: FG_ANVIL / 0 |
| 35 | `Bora_Mine` | 1971 | Interactive | -485.13,-4277.27,-195.62 | 188,269,347 | group/role: FG_ANVIL / 0 |
| 36 | `Bora_Mine` | 1972 | Interactive | 473.02,-4302.24,-360.77 | 188,269,347 | group/role: FG_ANVIL / 0 |
| 37 | `GalSpan_Poseidon` | 983 | Interactive | 0.00,-4814.46,41.78 | 128,128,0 | group/role: FG_ATLAS / 1; alias: Todd05; waypoint: Waypoint 5 (tag 8, 4 point(s)), starting point 0, arrival event value 524288 |
| 38 | `GalSpan_Poseidon` | 984 | Interactive | 0.00,-4813.77,12.37 | 128,128,0 | group/role: FG_ATLAS / 2; alias: Todd06; waypoint: Waypoint 5 (tag 8, 4 point(s)), starting point 0, arrival event value 524288 |
| 39 | `GalSpan_Poseidon` | 985 | Interactive | 0.00,-4815.13,-17.34 | 128,128,0 | group/role: FG_ATLAS / 3; alias: Todd07; waypoint: Waypoint 5 (tag 8, 4 point(s)), starting point 0, arrival event value 524288 |
| 40 | `GalSpan_Archangel` | 1888 | Interactive | 0.00,-5114.54,53.22 | 128,128,0 | group/role: FG_CAELUM / 0; waypoint: Waypoint 6 (tag 7, 5 point(s)), starting point 0, arrival event value 458752 |
| 41 | `GalSpan_Archangel` | 1889 | Interactive | 0.00,-5113.18,25.72 | 128,128,0 | group/role: FG_CAELUM / 1; waypoint: Waypoint 6 (tag 7, 5 point(s)), starting point 0, arrival event value 458752 |
| 42 | `GalSpan_Archangel` | 1890 | Interactive | 0.00,-5115.22,-0.53 | 128,128,0 | group/role: FG_CAELUM / 2; waypoint: Waypoint 6 (tag 7, 5 point(s)), starting point 0, arrival event value 458752 |
| 43 | `GalSpan_Archangel` | 1988 | Interactive | 0.00,-5114.62,-26.33 | 128,128,0 | group/role: FG_CAELUM / 3; waypoint: Waypoint 6 (tag 7, 5 point(s)), starting point 0, arrival event value 458752 |
| 44 | `Bora_Battleaxe` | 893 | Interactive | 148.40,-2136.00,704.75 | 0,0,0 | label: g01bfc; group/role: FG_CATAPULT / 1; waypoint: Waypoint 9 (tag 5, 3 point(s)), starting point 0, arrival event value 327680 |
| 45 | `Bora_Battleaxe` | 894 | Interactive | 173.56,-2136.00,704.41 | 0,0,0 | group/role: FG_CATAPULT / 2; waypoint: Waypoint 9 (tag 5, 3 point(s)), starting point 0, arrival event value 327680 |
| 46 | `Bora_Battleaxe` | 2008 | Interactive | 124.07,-2136.00,704.77 | 0,0,0 | group/role: FG_CATAPULT / 2; waypoint: Waypoint 9 (tag 5, 3 point(s)), starting point 0, arrival event value 327680 |
| 47 | `Bora_Mace` | 1941 | Interactive | 162.80,-2136.00,-347.36 | 257,0,0 | group/role: FG_RIGHTEOUS / 0; waypoint: Waypoint 12 (tag 2, 5 point(s)), starting point 0, arrival event value 131072 |
| 48 | `Bora_Mace` | 1942 | Interactive | 146.34,-2136.00,-347.36 | 257,0,0 | group/role: FG_RIGHTEOUS / 0; waypoint: Waypoint 12 (tag 2, 5 point(s)), starting point 0, arrival event value 131072 |
| 49 | `Bora_Mace` | 1943 | Interactive | 131.71,-2136.00,-346.36 | 257,0,0 | group/role: FG_RIGHTEOUS / 0; waypoint: Waypoint 12 (tag 2, 5 point(s)), starting point 0, arrival event value 131072 |
| 50 | `GalSpan_Pegasus` | 1196 | Interactive | 0.00,-5109.50,216.11 | 128,128,0 | group/role: FG_SERPENS / 1; alias: Todd21; waypoint: Waypoint 4 (tag 9, 5 point(s)), starting point 0, arrival event value 589824 |
| 51 | `GalSpan_Pegasus` | 1197 | Interactive | 0.00,-5110.31,187.24 | 128,128,0 | group/role: FG_SERPENS / 2; alias: Todd22; waypoint: Waypoint 4 (tag 9, 5 point(s)), starting point 0, arrival event value 589824 |
| 52 | `GalSpan_Pegasus` | 1198 | Interactive | 0.00,-5110.75,157.33 | 128,128,0 | group/role: FG_SERPENS / 3; alias: Todd23; waypoint: Waypoint 4 (tag 9, 5 point(s)), starting point 0, arrival event value 589824 |
| 53 | `GalSpan_Pegasus` | 1989 | Interactive | 0.00,-5110.32,130.01 | 128,128,0 | group/role: FG_SERPENS / 3; alias: Todd23; waypoint: Waypoint 4 (tag 9, 5 point(s)), starting point 0, arrival event value 589824 |
| 54 | `Bora_Light_Freighter` | 951 | Interactive | 126.81,-2123.19,805.27 | 0,0,0 | label: G01bra; group/role: none / 1; secondary groups: CONT_033, PILGRIM; waypoint: Waypoint 8 (tag 4, 5 point(s)), starting point 0, arrival event value 262144 |
| 55 | `Bora_Light_Freighter` | 969 | Interactive | 203.03,-2123.09,808.22 | 0,0,0 | group/role: none / 1; secondary groups: CONT_033, EXEMPTION; waypoint: Waypoint 1 (tag 120, 5 point(s)), starting point 0, arrival event value 7864320 |
| 56 | `Bora_Carrier` | 937 | Interactive | -1536.24,-3488.24,-2313.90 | 0,0,0 | label: integ; group/role: none / 1; secondary groups: CONT_025, INTEGRITY; waypoint: Waypoint 7 (tag 6, 3 point(s)), starting point 0, arrival event value 393216 |
| 57 | `GalSpan_Destroyer` | 1857 | Interactive | 2307.02,-3459.17,7.53 | 384,0,0 | secondary groups: CONT_025, PAN; waypoint: Waypoint 2 (tag 101, 3 point(s)), starting point 0, arrival event value 6619136 |
