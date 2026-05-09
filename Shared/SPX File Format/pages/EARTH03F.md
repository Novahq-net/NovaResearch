# Tachyon: The Fringe EARTH03F.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH03F.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `(none)` |
| Region | 0 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 1 |
| Events | 16 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Light_Freighter` |
| Scripts | `TINS.SCR`, `PLAYER.SCR` |
| Scenes | None |
| Labels | `SHUT`, `bfnf_03`, `PLAYER`, `ORION03`, `ORION02`, `ORION01`, `PEGASUS01`, `PEGASUS02`, `PEGASUS03`, `MAKO01`, `MAKO03`, `PIRANHA01`, `PIRANHA02`, `PIRANHA03`, `PIRANHA04`, `DART01`, `DART02`, `DART03`, `DART04`, `FRGT`, `CPSH`, `SAMA`, `FREIGHT01` |
| Aliases | `fred2`, `fred1`, `fred3` |
| Groups | `ONTARIO` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0
- Variable comparison: subject variable group 0, variable 4, op 1, value 1007

**Action**

- Set runtime trigger variable: variable group 20, variable 3, subtype 0, value 0
- Gate state/action: param 1, subtype 3, param 0
- Gate state/action: param 301, subtype 3, param 0
- Gate state/action: param 913, subtype 3, param 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 3, op 1, value 4

**Action**

- Play dialog: TINS.SCR, line/variant 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 9, value 0
- Sector/startup condition family: subject 0, op 0, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 110

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 3, op 1, value 20

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 17

### Event 4

**Trigger**

- Variable comparison: subject variable group 20, variable 3, op 1, value 35

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 17
- Show/update HUD contact: contact/list 0, subtype 9, param 18
- Show/update HUD contact: contact/list 0, subtype 9, param 19
- Show/update HUD contact: contact/list 0, subtype 9, param 20

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 3, op 1, value 48

**Action**

- Set runtime trigger variable: variable group 20, variable 3, subtype 1, value 0
- Play dialog: TINS.SCR, line/variant 2
- Show/update HUD contact: contact/list 0, subtype 9, param 35

### Event 6

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 2

**Action**

- Set runtime trigger variable: variable group 20, variable 3, subtype 0, value 0

### Event 7

**Trigger**

- Variable comparison: subject variable group 20, variable 3, op 1, value 50

**Action**

- Play dialog: TINS.SCR, line/variant 3

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 3, op 1, value 67

**Action**

- Gate state/action: param 301, subtype 0, param 0
- Set runtime trigger variable: variable group 20, variable 3, subtype 1, value 0

### Event 9

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 3

**Action**

- Set runtime trigger variable: variable group 20, variable 3, subtype 0, value 0

### Event 10

**Trigger**

- Variable comparison: subject variable group 20, variable 3, op 1, value 69

**Action**

- Mission objective/state: param 7, subtype 0, param 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 18
- Hide/remove HUD contact: contact/list 0, subtype 9, param 19
- Hide/remove HUD contact: contact/list 0, subtype 9, param 20
- Hide/remove HUD contact: contact/list 0, subtype 9, param 35

### Event 11

**Trigger**

- Variable comparison: subject variable group 20, variable 3, op 1, value 75

**Action**

- Play dialog: PLAYER.SCR, line/variant 166

### Event 12

**Trigger**

- Variable comparison: subject variable group 20, variable 3, op 1, value 76

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 36
- Set runtime trigger variable: variable group 20, variable 3, subtype 1, value 0

### Event 13

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 3, subtype 0, value 0
- Hide/remove HUD contact: contact/list 0, subtype 9, param 36
- Gate state/action: param 1, subtype 2, param 0
- Gate state/action: param 913, subtype 2, param 0

### Event 14

**Trigger**

- Variable comparison: subject variable group 20, variable 3, op 1, value 78

**Action**

- Play dialog: TINS.SCR, line/variant 21

### Event 15

**Trigger**

- Variable comparison: subject variable group 20, variable 3, op 1, value 89

**Action**

- Show/update HUD contact: contact/list 0, subtype 9, param 36
- Set runtime trigger variable: variable group 20, variable 3, subtype 1, value 0

## Waypoints

### Waypoint 0

- Tag: `12`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-702.57, 330.00, -689.74) | None |
| 1 | (-3708.89, 325.00, 1050.25) | None |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Generic_Light_Freighter` | 870 | Interactive | -535.10,330.00,-768.26 | 0,0,0 | group/role: none / 1; secondary groups: none, ONTARIO |
