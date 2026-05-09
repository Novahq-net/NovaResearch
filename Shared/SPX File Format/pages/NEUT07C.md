# Tachyon: The Fringe NEUT07C.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT07C.SPX` |
| Sector | `QUAD_07` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 6 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 4 |
| Events | 11 |
| Waypoints | 0 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Light_Freighter`, `1: Bora_Hvy_Freighter`, `2: Medical_Frigate` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `g01bsa`, `g01bfa`, `g01bfb`, `g01bfc`, `G01bra`, `integ` |
| Aliases | `Todd08`, `Todd09`, `Todd10`, `Todd14`, `Todd15`, `Todd16`, `Todd12`, `Todd13`, `Todd18`, `Todd03`, `Todd04`, `Todd02`, `Todd05`, `Todd06`, `Todd07`, `Todd21`, `Todd22`, `Todd23`, `will_01`, `SHIP1_HYPER`, `SHIP2_HYPER`, `SHIP3_HYPER`, `ohshit` |
| Groups | `DROMEDARY`, `CONT_002`, `BOLD`, `CONT_004`, `TRAVELER`, `CONT_028`, `FINDER`, `CONT_030` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 8, op 1, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 76
- Show/update HUD contact: contact/list 0, subtype 9, param 47
- Show/update HUD contact: contact/list 0, subtype 9, param 19

### Event 1

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 76

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 19
- Set/add variable: variable group 13, variable 410, subtype 0, value 1
- Set/add variable: variable group 13, variable 411, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 33
- Hide/remove HUD contact: contact/list 0, subtype 9, param 22
- Hide/remove HUD contact: contact/list 0, subtype 9, param 23
- Hide/remove HUD contact: contact/list 0, subtype 9, param 47

### Event 2

**Trigger**

- Variable comparison: subject variable group 21, variable 8, op 1, value 1

**Action**

- Object spawn/action: Medical_Frigate (object 0, id 1919), subtype 3

### Event 3

**Trigger**

- Variable comparison: subject variable group 21, variable 9, op 1, value 1

**Action**

- Object spawn/action: Bora_Hvy_Freighter (object 2, id 1153), subtype 3

### Event 4

**Trigger**

- Variable comparison: subject variable group 21, variable 10, op 1, value 1

**Action**

- Object spawn/action: Bora_Hvy_Freighter (object 1, id 1162), subtype 3

### Event 5

**Trigger**

- Variable comparison: subject variable group 21, variable 30, op 1, value 1

**Action**

- Object spawn/action: Generic_Light_Freighter (object 3, id 1987), subtype 3

### Event 6

**Trigger**

- Object event: subject Generic_Light_Freighter (object 3, id 1987), op 9, value 0

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 3000

### Event 7

**Trigger**

- Object event: subject Bora_Hvy_Freighter (object 2, id 1153), op 9, value 0
- Object event: subject Bora_Hvy_Freighter (object 1, id 1162), op 9, value 0
- Object event: subject Medical_Frigate (object 0, id 1919), op 9, value 0

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 5000

### Event 8

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Object spawn/action: id 723, subtype 18
- Object spawn/action: id 739, subtype 18

### Event 9

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 9, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 22

### Event 10

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 10, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 23

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Medical_Frigate` | 1919 | Interactive | 2064.34,-945.29,-989.53 | 0,0,0 | alias: SHIP1_HYPER; secondary groups: CONT_002, DROMEDARY |
| 1 | `Bora_Hvy_Freighter` | 1162 | Interactive | 1874.51,-947.70,-962.41 | 0,0,0 | alias: SHIP2_HYPER; secondary groups: CONT_004, BOLD |
| 2 | `Bora_Hvy_Freighter` | 1153 | Interactive | 2248.39,-947.70,-981.99 | 0,0,0 | alias: SHIP3_HYPER; secondary groups: CONT_028, TRAVELER |
| 3 | `Generic_Light_Freighter` | 1987 | Interactive | 2442.25,0.00,-990.38 | 0,0,0 | alias: ohshit; secondary groups: CONT_030, FINDER |
