# Tachyon: The Fringe FRON01.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON01.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `FRONTI1.BDF` |
| Region | 4 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 6 |
| Entities | 19 |
| Events | 25 |
| Waypoints | 0 |
| Child Sectors | 14 |
| Scripts | 2 |
| Scenes | 5 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Atlantic_Casino_Station`, `1: Frontier_StarBase`, `2: Spcargo_Credits`, `3: Navigational_Bouy`, `4: Mega_Gate`, `5: Hyper_Gate` |
| Scripts | `TRISH.SCR`, `PLAYER.SCR` |
| Scenes | `FRON2MYS.SEN`, `F1BC050A.SEN`, `FRON2HUB.SEN`, `FRON2GAL.SEN`, `FRON2BOR.SEN` |
| Labels | `BFGF_05`, `BFNE_03`, `BFNF_03`, `BFGE_01`, `BFGF_01`, `bfne_05` |
| Aliases | `Python 4`, `Python 3`, `Python 1`, `Python 2`, `Kimodo 1`, `Jerome02`, `Jerome03`, `Jerome04`, `Jerome05`, `Jerome06`, `Jerome01`, `BC05_sistine_chapel`, `bc05_1`, `bc05_2`, `bc05_4`, `bc05_5`, `Mantis1`, `Mantis2`, `Mantis3`, `Mantis4`, `Aphid1`, `Aphid2`, `Aphid3`, `Aphid4`, `Python1`, `Python2`, `Python3`, `Python4`, `Komodo1`, `Komodo2`, `Komodo3`, `Komodo4`, `Kimodo 2`, `Kimodo 3`, `Kimodo 4`, `Cephius`, `Stocks01` |
| Groups | `NEW_VEGAS_STARBASE`, `ATLANTIC_CASINO`, `ATLANTIC_BUOY1`, `ATLANTIC_BUOY2`, `ATLANTIC_BUOY3`, `CONT_069` |
| Child Sectors | [fron01A.spx](FRON01A.md), [fron01B.spx](FRON01B.md), [fron01D.spx](FRON01D.md), [fron01E.spx](FRON01E.md), [fron01F.spx](FRON01F.md), [fron01G.spx](FRON01G.md), [fron01H.spx](FRON01H.md), [fron01I.spx](FRON01I.md), [fron01J.spx](FRON01J.md), [fron01K.spx](FRON01K.md), [fron01L.spx](FRON01L.md), [fron01M.spx](FRON01M.md), [fron01N.spx](FRON01N.md), [fron01O.spx](FRON01O.md) |

## Events

### Event 0

**Trigger**

- Variable comparison: subject variable group 0, variable 4, op 1, value 3006

**Action**

- Mission objective/state: param 262154, subtype 0, param 0
- Gate state/action: param 7, subtype 3, param 0
- Gate state/action: param 8, subtype 3, param 0
- Gate state/action: param 9, subtype 3, param 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 9, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 3006

**Action**

- Play dialog: TRISH.SCR, line/variant 3

### Event 2

**Trigger**

- Variable comparison: subject variable group 0, variable 4, op 1, value 2003

**Action**

- Mission objective/state: param 262150, subtype 0, param 0
- Set runtime trigger variable: variable group 20, variable 2, subtype 0, value 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 2, op 1, value 21
- Variable comparison: subject variable group 0, variable 4, op 1, value 2003

**Action**

- Play dialog: PLAYER.SCR, line/variant 37
- Set runtime trigger variable: variable group 20, variable 2, subtype 1, value 0

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4012

**Action**

- Mission objective/state: param 262148, subtype 0, param 0

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 16, variable 417, op 0, value 2 (join 2)

**Action**

- Set/add variable: variable group 16, variable 416, subtype 0, value 1

### Event 6

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 16, variable 417, op 0, value 3

**Action**

- Set/add variable: variable group 16, variable 416, subtype 0, value 1

### Event 7

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 2004

**Action**

- Mission objective/state: param 262149, subtype 0, param 0

### Event 8

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4025

**Action**

- Mission objective/state: param 262155, subtype 0, param 0
- Gate state/action: param 7, subtype 3, param 0
- Gate state/action: param 8, subtype 3, param 0
- Gate state/action: param 9, subtype 3, param 0

### Event 9

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4020

**Action**

- Mission objective/state: param 262154, subtype 0, param 0

### Event 10

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4032

**Action**

- Mission objective/state: param 262154, subtype 0, param 0

### Event 11

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4033

**Action**

- Mission objective/state: param 262154, subtype 0, param 0

### Event 12

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4034

**Action**

- Mission objective/state: param 262154, subtype 0, param 0

### Event 13

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4035

**Action**

- Mission objective/state: param 262154, subtype 0, param 0

### Event 14

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4036

**Action**

- Mission objective/state: param 262154, subtype 0, param 0

### Event 15

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4037

**Action**

- Mission objective/state: param 262154, subtype 0, param 0

### Event 16

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4038

**Action**

- Mission objective/state: param 262154, subtype 0, param 0

### Event 17

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4039

**Action**

- Mission objective/state: param 262154, subtype 0, param 0

### Event 18

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4040

**Action**

- Mission objective/state: param 262154, subtype 0, param 0

### Event 19

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 4026

**Action**

- Mission objective/state: param 262151, subtype 0, param 0

### Event 20

**Trigger**

- Variable comparison: subject variable group 0, variable 4, op 0, value 4058
- Area/player/sector/dock/time event: subject 0, op 9, value 0

**Action**

- Play scene: FRON2MYS.SEN, param 0
- Set/add variable: variable group 0, variable 12, subtype 0, value 5
- Set/add variable: variable group 0, variable 3, subtype 0, value 5
- Set/add variable: variable group 0, variable 4, subtype 0, value 0

### Event 21

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 733; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 213
- Set/add variable: variable group 0, variable 2, subtype 1, value 777
- Show/update HUD contact: contact/list 0, subtype 9, param 41
- Set/add variable: variable group 16, variable 809, subtype 0, value 1
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 22

**Trigger**

- Variable comparison: subject variable group 20, variable 32, op 2, value 10

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 41
- Set/add variable: variable group 20, variable 32, subtype 0, value 0

### Event 23

**Trigger**

- Variable comparison: subject variable group 16, variable 409, op 0, value 2

**Action**

- Set/add variable: variable group 22, variable 15, subtype 0, value 1

### Event 24

**Trigger**

- Variable comparison: subject variable group 16, variable 401, op 0, value 2

**Action**

- Set/add variable: variable group 22, variable 20, subtype 0, value 1

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | -1476.74,0.00,3370.30 | 213,0,0 | Gate SPX: [fron02.spx](FRON02.md) |
| 1 | `Hyper_Gate` | 2 | Gate | 1402.08,0.00,3404.75 | 299,0,0 | Gate SPX: [fron03.spx](FRON03.md) |
| 2 | `Hyper_Gate` | 3 | Gate | 1648.84,0.00,2884.63 | 313,0,0 | Gate SPX: [fron04.spx](FRON04.md) |
| 3 | `Hyper_Gate` | 4 | Gate | 1679.53,0.00,2238.88 | 327,0,0 | Gate SPX: [fron06.spx](FRON06.md) |
| 4 | `Hyper_Gate` | 5 | Gate | -1730.47,0.00,2235.54 | 199,0,0 | Gate SPX: [fron11.spx](FRON11.md) |
| 5 | `Hyper_Gate` | 6 | Gate | -1719.20,0.00,2892.93 | 213,0,0 | Gate SPX: [fron08.spx](FRON08.md) |
| 6 | `Mega_Gate` | 7 | Gate | -81.30,0.00,4146.86 | 256,0,0 | Gate SPX: [neut06.spx](NEUT06.md) |
| 7 | `Mega_Gate` | 8 | Gate | 826.37,0.00,3951.87 | 284,0,0 | Gate SPX: [bora03.spx](BORA03.md) |
| 8 | `Mega_Gate` | 9 | Gate | -994.80,0.00,3903.07 | 228,0,0 | Gate SPX: [gals02.spx](GALS02.md) |
| 9 | `Navigational_Bouy` | 393 | Interactive | -54.15,0.00,-4840.91 | 0,0,0 | secondary groups: none, NEW_VEGAS_STARBASE |
| 10 | `Navigational_Bouy` | 397 | Interactive | -5347.17,0.00,-9052.13 | 0,0,0 | secondary groups: none, ATLANTIC_CASINO |
| 11 | `none` | 511 | Marker | 32.98,0.00,-102.39 | 0,0,0 | None |
| 12 | `Navigational_Bouy` | 549 | Interactive | -1576.09,0.00,-5913.05 | 0,0,0 | secondary groups: none, ATLANTIC_BUOY1 |
| 13 | `Navigational_Bouy` | 550 | Interactive | -2996.21,0.00,-7096.77 | 0,0,0 | secondary groups: none, ATLANTIC_BUOY2 |
| 14 | `Navigational_Bouy` | 551 | Interactive | -4255.50,0.00,-8119.49 | 0,0,0 | secondary groups: none, ATLANTIC_BUOY3 |
| 15 | `Navigational_Bouy` | 722 | Interactive | -70.22,-1113.79,-499.26 | 0,0,0 | None |
| 16 | `Spcargo_Credits` | 733 | Interactive | -7817.03,-1204.10,-10969.92 | 100,0,0 | secondary groups: CONT_069, none |
| 17 | `Frontier_StarBase` | 336 | Interactive | -74.38,-1438.54,-1202.44 | 0,0,0 | None |
| 18 | `Atlantic_Casino_Station` | 337 | Interactive | -6437.53,0.00,-10086.44 | 0,0,0 | None |
