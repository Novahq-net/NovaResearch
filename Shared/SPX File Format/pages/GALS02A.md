# Tachyon: The Fringe GALS02A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `GALS02A.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `(none)` |
| Region | 2 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 4 |
| Entities | 18 |
| Events | 8 |
| Waypoints | 0 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Satellite`, `1: Crate_7`, `2: Crate_6`, `3: Crate_5` |
| Scripts | `PLAYER.SCR`, `PROME.SCR` |
| Scenes | None |
| Labels | `bfge_02`, `BFGF_03`, `BFGE_03` |
| Aliases | `stocks04`, `Jerome07`, `Jerome08`, `Jerome09`, `Jerome10`, `Jerome11`, `Jerome12`, `stocks03`, `stocks02`, `stocks01` |
| Groups | `CONT_037`, `CONT_038`, `CONT_UNKNOWN`, `CONT_040`, `CONT_053` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Gate state/action: param 3, subtype 3, param 0

### Event 1

**Trigger**

- Object event: subject Crate_5 (object 0, id 387), op 10, value 0 (join 2)
- Object event: subject Crate_5 (object 1, id 388), op 10, value 0 (join 2)
- Object event: subject Crate_5 (object 2, id 389), op 10, value 0 (join 2)
- Object event: subject Crate_5 (object 3, id 390), op 10, value 0 (join 2)
- Object event: subject Crate_5 (object 4, id 391), op 10, value 0 (join 2)
- Object event: subject Crate_5 (object 5, id 392), op 10, value 0 (join 2)
- Object event: subject Crate_5 (object 6, id 393), op 10, value 0 (join 1)
- Variable comparison: subject variable group 21, variable 22, op 1, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 8

### Event 2

**Trigger**

- Object event: subject Crate_6 (object 7, id 394), op 10, value 0 (join 2)
- Object event: subject Crate_6 (object 8, id 395), op 10, value 0 (join 2)
- Object event: subject Crate_6 (object 9, id 396), op 10, value 0 (join 2)
- Object event: subject Crate_6 (object 10, id 397), op 10, value 0 (join 2)
- Object event: subject Crate_7 (object 11, id 398), op 10, value 0 (join 2)
- Object event: subject Crate_7 (object 12, id 399), op 10, value 0 (join 2)
- Object event: subject Crate_7 (object 13, id 400), op 10, value 0 (join 1)
- Variable comparison: subject variable group 21, variable 22, op 1, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 8

### Event 3

**Trigger**

- Object event: subject Satellite (object 14, id 436), op 2, value 0
- Object event: subject Satellite (object 15, id 437), op 2, value 0
- Object event: subject Satellite (object 16, id 438), op 2, value 0
- Object event: subject Satellite (object 17, id 439), op 2, value 0

**Action**

- Broadcast HUD contact action: contact/list 0, subtype 0, param 15
- Set/add variable: variable group 21, variable 21, subtype 0, value 1
- Play dialog: PLAYER.SCR, line/variant 10
- Broadcast hide/remove contact: contact/list 0, subtype 0, param 12
- Mission objective/state: param 131074, subtype 0, param 0

### Event 4

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 10

**Action**

- Play dialog: PROME.SCR, line/variant 7

### Event 5

**Trigger**

- Object event: subject Satellite (object 14, id 436), op 10, value 0 (join 2)
- Object event: subject Satellite (object 14, id 436), op 2, value 0 (join 2)

**Action**

- Object spawn/action: Satellite (object 14, id 436), subtype 8, param 1
- Object spawn/action: Satellite (object 15, id 437), subtype 0
- Object spawn/action: Satellite (object 16, id 438), subtype 0
- Object spawn/action: Satellite (object 17, id 439), subtype 0

### Event 6

**Trigger**

- Object event: subject Satellite (object 14, id 436), op 0, value 0 (flags 2)

**Action**

- Object spawn/action: Satellite (object 14, id 436), subtype 7

### Event 7

**Trigger**

- Variable comparison: subject variable group 21, variable 22, op 1, value 1

**Action**

- Object spawn/action: Satellite (object 14, id 436), subtype 0

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Crate_5` | 387 | Interactive | 82.47,-43.33,4223.55 | 0,0,0 | secondary groups: CONT_037, none |
| 1 | `Crate_5` | 388 | Interactive | 211.41,86.65,3947.76 | 0,0,0 | secondary groups: CONT_037, none |
| 2 | `Crate_5` | 389 | Interactive | 527.90,-46.94,3950.98 | 0,0,0 | secondary groups: CONT_038, none |
| 3 | `Crate_5` | 390 | Interactive | 703.73,-43.33,3501.25 | 0,0,0 | secondary groups: CONT_037, none |
| 4 | `Crate_5` | 391 | Interactive | 949.90,0.00,3425.67 | 0,0,0 | secondary groups: CONT_038, none |
| 5 | `Crate_5` | 392 | Interactive | 1067.12,124.20,2938.88 | 0,0,0 | secondary groups: CONT_037, none |
| 6 | `Crate_5` | 393 | Interactive | 1336.72,86.65,3081.00 | 0,0,0 | secondary groups: CONT_UNKNOWN, none |
| 7 | `Crate_6` | 394 | Interactive | 668.57,0.00,3845.92 | 0,0,0 | secondary groups: CONT_038, none |
| 8 | `Crate_6` | 395 | Interactive | -187.14,124.20,4296.33 | 0,0,0 | secondary groups: CONT_040, none |
| 9 | `Crate_6` | 396 | Interactive | 828.68,-62.03,2772.26 | 0,0,0 | secondary groups: CONT_040, none |
| 10 | `Crate_6` | 397 | Interactive | 1278.11,-104.70,3228.68 | 0,0,0 | secondary groups: CONT_UNKNOWN, none |
| 11 | `Crate_7` | 398 | Interactive | 0.00,58.96,3976.96 | 0,0,0 | secondary groups: CONT_040, none |
| 12 | `Crate_7` | 399 | Interactive | 861.28,0.00,3063.54 | 0,0,0 | secondary groups: CONT_040, none |
| 13 | `Crate_7` | 400 | Interactive | 744.06,61.06,3693.91 | 0,0,0 | secondary groups: CONT_038, none |
| 14 | `Satellite` | 436 | Interactive | 535.84,0.00,3887.71 | 0,0,0 | secondary groups: CONT_053, none |
| 15 | `Satellite` | 437 | Interactive | 15.31,0.00,4263.99 | 0,0,0 | secondary groups: CONT_053, none |
| 16 | `Satellite` | 438 | Interactive | 1330.14,0.00,3264.76 | 0,0,0 | secondary groups: CONT_053, none |
| 17 | `Satellite` | 439 | Interactive | 1245.32,0.00,2859.22 | 0,0,0 | secondary groups: CONT_053, none |
