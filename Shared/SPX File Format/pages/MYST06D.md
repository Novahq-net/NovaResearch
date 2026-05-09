# Tachyon: The Fringe MYST06D.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST06D.SPX` |
| Sector | `QUAD_06` |
| Backdrop | `(none)` |
| Region | 5 |
| Sector ID | 5 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 2 |
| Events | 15 |
| Waypoints | 0 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Luxury_Liner` |
| Scripts | `SIGHT.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `PISCE`, `RALPH` |
| Aliases | `PISCES1`, `PISCES2`, `pisces3`, `pisces4`, `stocks02` |
| Groups | `THE_SIGHTSEER` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 19, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 2
- Variable comparison: subject variable group 21, variable 20, op 1, value 0

**Action**

- Object spawn/action: Luxury_Liner (object 0, id 12), subtype 3
- Show/update HUD contact: contact/list 0, subtype 6, param 12
- Set runtime trigger variable: variable group 20, variable 20, subtype 0, value 0
- Object spawn/action: Luxury_Liner (object 0, id 12), subtype 14

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 20, op 1, value 2

**Action**

- Play dialog: SIGHT.SCR, line/variant 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 20, op 1, value 15

**Action**

- Play dialog: SIGHT.SCR, line/variant 1

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 20, op 1, value 20

**Action**

- Object spawn/action: Luxury_Liner (object 0, id 12), subtype 4
- Set/add variable: variable group 21, variable 20, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 6, param 12
- Hide/remove HUD contact: contact/list 0, subtype 11, param 0

### Event 5

**Trigger**

- Object event: subject Luxury_Liner (object 0, id 12), op 8, value 0

**Action**

- Mission objective/state: param 327686, subtype 0, param 0

### Event 6

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 4

**Action**

- Object spawn/action: Luxury_Liner (object 1, id 39), subtype 3
- Set runtime trigger variable: variable group 20, variable 25, subtype 1, value 0
- Set/add variable: variable group 20, variable 25, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 6, param 39
- Object spawn/action: Luxury_Liner (object 1, id 39), subtype 14

### Event 7

**Trigger**

- Object event: subject Luxury_Liner (object 1, id 39), op 9, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 4

**Action**

- Play dialog: SIGHT.SCR, line/variant 7

### Event 8

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 7

**Action**

- Object spawn/action: Luxury_Liner (object 1, id 39), subtype 4
- Hide/remove HUD contact: contact/list 0, subtype 6, param 39
- Play dialog: PLAYER.SCR, line/variant 168

### Event 9

**Trigger**

- Variable comparison: subject variable group 21, variable 20, op 1, value 4
- Object event: subject Luxury_Liner (object 1, id 39), op 8, value 0

**Action**

- Set/add variable: variable group 21, variable 28, subtype 0, value 1

### Event 10

**Trigger**

- Object event: subject Luxury_Liner (object 0, id 12), op 16, value 0 (join 2)
- Object event: subject Luxury_Liner (object 1, id 39), op 16, value 0 (join 2)
- Object event: subject Luxury_Liner (object 1, id 39), op 6, value 0 (join 2)
- Object event: subject Luxury_Liner (object 0, id 12), op 6, value 0 (join 2)

**Action**

- Set/add variable: variable group 17, variable 408, subtype 0, value 1
- Set/add variable: variable group 17, variable 409, subtype 0, value 1
- Mark/flash contact: contact/list 0, subtype 6, param 39
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 11, param 29

### Event 11

**Trigger**

- Variable comparison: subject variable group 21, variable 28, op 1, value 1
- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Set/add variable: variable group 17, variable 408, subtype 0, value 1
- Set/add variable: variable group 17, variable 409, subtype 0, value 3
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 28

### Event 12

**Trigger**

- Variable comparison: subject variable group 21, variable 28, op 1, value 1
- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Set/add variable: variable group 17, variable 408, subtype 0, value 1
- Set/add variable: variable group 17, variable 409, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 28

### Event 13

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 167

### Event 14

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 1

**Action**

- Play dialog: PLAYER.SCR, line/variant 102

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Luxury_Liner` | 12 | Interactive | 819.29,52.00,578.24 | 220,0,0 | alias: stocks02; secondary groups: none, THE_SIGHTSEER |
| 1 | `Luxury_Liner` | 39 | Interactive | -99.91,0.00,680.48 | 489,0,0 | alias: stocks02; secondary groups: none, THE_SIGHTSEER |
