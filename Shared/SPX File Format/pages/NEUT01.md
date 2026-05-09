# Tachyon: The Fringe NEUT01.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT01.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `NEUTRA1.BDF` |
| Region | 1 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 7 |
| Entities | 12 |
| Events | 25 |
| Waypoints | 2 |
| Child Sectors | 11 |
| Scripts | 3 |
| Scenes | 3 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Hub_StarBase`, `1: Independent_Merc_Dart`, `2: AGT_Mako`, `3: Spcargo_Food`, `4: Navigational_Bouy`, `5: Mega_Gate`, `6: Hyper_Gate` |
| Scripts | `ANNAH.SCR`, `TRISH.scr`, `PLAYER.SCR` |
| Scenes | `HUB2BORA.SEN`, `HUB2FRON.SEN`, `HUB2GAL.SEN` |
| Labels | `MISHK`, `FakeJake`, `Daymir` |
| Aliases | `Courage`, `kwi03_7`, `Jerome26`, `Jerome25`, `Jerome24`, `Jerome22`, `Jerome21`, `Jerome20`, `kevin01`, `Intrepid`, `kwI03_10`, `SHIP1_HYPER`, `ohshit`, `SHIP2_HYPER`, `SHIP3_HYPER` |
| Groups | `ALPHA_STARBASE`, `CONT_063` |
| Child Sectors | [neut01A.spx](NEUT01A.md), [neut01B.spx](NEUT01B.md), [neut01C.spx](NEUT01C.md), [neut01D.spx](NEUT01D.md), [neut01E.spx](NEUT01E.md), [neut01F.spx](NEUT01F.md), [neut01G.spx](NEUT01G.md), [neut01H.spx](NEUT01H.md), [neut01I.spx](NEUT01I.md), [neut01J.spx](NEUT01J.md), [neut01K.spx](NEUT01K.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 2000

**Action**

- Set/add variable: variable group 0, variable 0, subtype 0, value 2
- Mission objective/state: param 65542, subtype 0, param 0
- Gate state/action: param 67, subtype 3, param 0
- Set runtime trigger variable: variable group 20, variable 11, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 11, op 1, value 22
- Variable comparison: subject variable group 0, variable 4, op 1, value 2000

**Action**

- Play dialog: ANNAH.SCR, line/variant 0
- Object spawn/action: id 256, subtype 3

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 3000

**Action**

- Set/add variable: variable group 0, variable 0, subtype 0, value 1
- Mission objective/state: param 65541, subtype 0, param 0
- Gate state/action: param 67, subtype 3, param 0
- Set runtime trigger variable: variable group 20, variable 11, subtype 0, value 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 11, op 1, value 22
- Variable comparison: subject variable group 0, variable 4, op 1, value 3000

**Action**

- Play dialog: TRISH.scr, line/variant 0

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 3001

**Action**

- Mission objective/state: param 65537, subtype 0, param 0
- Set runtime trigger variable: variable group 20, variable 8, subtype 0, value 0
- Gate state/action: param 67, subtype 3, param 0

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 8, op 1, value 22
- Variable comparison: subject variable group 0, variable 4, op 1, value 3001

**Action**

- Play dialog: TRISH.scr, line/variant 3
- Gate state/action: param 64, subtype 2, param 0

### Event 6

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 2002

**Action**

- Mission objective/state: param 65539, subtype 0, param 0

### Event 7

**Trigger**

- Variable comparison: subject variable group 0, variable 4, op 1, value 4000
- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Mission objective/state: param 65540, subtype 0, param 0

### Event 8

**Trigger**

- Object event: subject 231, op 15, value 0
- Object event: subject 233, op 15, value 0

**Action**

- Object spawn/action: id 231, subtype 8, param 4
- Object spawn/action: id 233, subtype 8, param 4

### Event 9

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 11, variable 2, op 1, value 6

**Action**

- Object spawn/action: id 231, subtype 3
- Object spawn/action: id 233, subtype 3

### Event 10

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 9, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 2002

**Action**

- Play dialog: ANNAH.SCR, line/variant 2

### Event 11

**Trigger**

- Object arrival: 256 reached waypoint tag 96, point 3 (raw value 6291459)

**Action**

- Object spawn/action: id 256, subtype 6

### Event 12

**Trigger**

- Object event: subject 223, op 4, value 90 (join 2)
- Object event: subject 224, op 4, value 90 (join 2)
- Object event: subject 222, op 4, value 90 (join 2)
- Object event: subject 256, op 4, value 90 (join 2)
- Object event: subject 231, op 4, value 90 (join 2)
- Object event: subject 233, op 4, value 90 (join 2)

**Action**

- Object spawn/action: id 264, subtype 0
- Object spawn/action: id 265, subtype 0
- Object spawn/action: id 266, subtype 0
- Object spawn/action: id 267, subtype 0

### Event 13

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4002

**Action**

- Mission objective/state: param 65539, subtype 0, param 0

### Event 14

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4029

**Action**

- Mission objective/state: param 65541, subtype 0, param 0

### Event 15

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4009

**Action**

- Mission objective/state: param 65539, subtype 0, param 0

### Event 16

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4003

**Action**

- Mission objective/state: param 65541, subtype 0, param 0

### Event 17

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4046

**Action**

- Mission objective/state: param 65545, subtype 0, param 0

### Event 18

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4047

**Action**

- Mission objective/state: param 65545, subtype 0, param 0

### Event 19

**Trigger**

- Variable comparison: subject variable group 13, variable 401, op 0, value 3
- Variable comparison: subject variable group 3, variable 7, op 0, value 0

**Action**

- Set/add variable: variable group 22, variable 6, subtype 0, value 1
- Set/add variable: variable group 0, variable 1, subtype 0, value 6
- Set/add variable: variable group 22, variable 10, subtype 0, value 0
- Set/add variable: variable group 3, variable 7, subtype 0, value 1
- Set/add variable: variable group 22, variable 21, subtype 0, value 1

### Event 20

**Trigger**

- Variable comparison: subject variable group 13, variable 405, op 0, value 3
- Variable comparison: subject variable group 3, variable 2, op 0, value 0

**Action**

- Set/add variable: variable group 22, variable 4, subtype 0, value 1
- Set/add variable: variable group 0, variable 1, subtype 0, value 1
- Set/add variable: variable group 22, variable 10, subtype 0, value 0
- Set/add variable: variable group 3, variable 2, subtype 0, value 1
- Set/add variable: variable group 22, variable 19, subtype 0, value 1

### Event 21

**Trigger**

- Variable comparison: subject variable group 13, variable 407, op 0, value 2

**Action**

- Set/add variable: variable group 22, variable 16, subtype 0, value 1

### Event 22

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 697; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 125
- Set/add variable: variable group 13, variable 804, subtype 0, value 1

### Event 23

**Trigger**

- Variable comparison: subject variable group 0, variable 4, op 1, value 4045
- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 24

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4045

**Action**

- Mission objective/state: param 65544, subtype 0, param 0

## Waypoints

### Waypoint 0

- Tag: `52`
- Members: `Independent_Merc_Dart (object 10, id 770, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (5370.38, 292.56, -8006.08) | None |
| 1 | (5006.34, 292.56, -5829.63) | None |
| 2 | (4569.66, 292.56, -4386.91) | None |

### Waypoint 1

- Tag: `51`
- Members: `AGT_Mako (object 9, id 769, starts at point -1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (4668.36, 292.56, -7949.70) | None |
| 1 | (4980.37, 292.56, -5835.29) | None |
| 2 | (5230.33, 292.56, -4672.03) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 63 | Gate | 6927.86,1221.92,-1602.88 | 320,448,0 | Gate SPX: [neut09.spx](NEUT09.md) |
| 1 | `Hyper_Gate` | 64 | Gate | 8411.89,-459.92,-4620.28 | 320,0,0 | Gate SPX: [neut02.spx](NEUT02.md) |
| 2 | `Hyper_Gate` | 65 | Gate | 6427.15,88.00,-9678.14 | 449,0,0 | Gate SPX: [neut04.spx](NEUT04.md) |
| 3 | `Hyper_Gate` | 66 | Gate | 4343.25,453.27,-10750.44 | 454,0,0 | Gate SPX: [neut05.spx](NEUT05.md) |
| 4 | `Mega_Gate` | 67 | Gate | 7701.10,-1370.79,-7861.81 | 128,64,0 | Gate SPX: [earth05.spx](EARTH05.md) |
| 5 | `none` | 642 | Marker | 2418.62,0.00,-6354.73 | 0,0,0 | None |
| 6 | `Navigational_Bouy` | 671 | Interactive | 2147.32,309.26,-5933.05 | 0,0,0 | secondary groups: none, ALPHA_STARBASE |
| 7 | `Spcargo_Food` | 697 | Interactive | 2659.15,19.24,-1565.19 | 0,0,0 | secondary groups: CONT_063, none |
| 8 | `Hyper_Gate` | 745 | Gate | 6069.90,0.00,-5710.07 | 0,0,0 | Gate SPX: [neut10.spx](NEUT10.md) |
| 9 | `AGT_Mako` | 769 | Interactive | 4646.60,292.56,-8071.82 | 0,0,0 | label: FakeJake; waypoint: Waypoint 1 (tag 51, 3 point(s)), starting point -1 |
| 10 | `Independent_Merc_Dart` | 770 | Interactive | 5395.35,292.56,-8188.25 | 0,0,0 | label: Daymir; waypoint: Waypoint 0 (tag 52, 3 point(s)), starting point -1 |
| 11 | `Hub_StarBase` | 458 | Interactive | 1037.47,0.00,-5934.00 | 127,0,0 | None |
