# Tachyon: The Fringe EARTH02D.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH02D.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `(none)` |
| Region | 0 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 3 |
| Entities | 6 |
| Events | 7 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Science_Vessel`, `1: Generic_Light_Freighter`, `2: Independent_Merc_Mako` |
| Scripts | `TINS.SCR` |
| Scenes | None |
| Labels | `bfnf_03`, `ariv`, `AGT FIGHTER`, `CAPB`, `CAPA`, `ofrt` |
| Aliases | `danc_blowfish1`, `danc_blowfish2`, `danc_blowfish5`, `danc_blowfish3`, `danc_blowfish4`, `Jerome50` |
| Groups | `FG_BORA3`, `ARGOSO 914`, `CONT_027`, `FG_BORA2`, `CONT_040`, `EXPLORATION`, `CONT_005` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 31, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 31, op 1, value 2

**Action**

- Play dialog: TINS.SCR, line/variant 5

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 31, op 1, value 5

**Action**

- Object spawn/action: Science_Vessel (object 5, id 1457), subtype 12
- Show/update HUD contact: contact/list 0, subtype 9, param 21

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 31, op 1, value 15

**Action**

- Set runtime trigger variable: variable group 20, variable 31, subtype 1, value 0

### Event 4

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 5

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 21

### Event 5

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 20, op 1, value 1

**Action**

- Set runtime trigger variable: variable group 20, variable 30, subtype 0, value 0

### Event 6

**Trigger**

- Variable comparison: subject variable group 20, variable 30, op 1, value 3

**Action**

- Play dialog: TINS.SCR, line/variant 20
- Set runtime trigger variable: variable group 20, variable 30, subtype 1, value 0

## Waypoints

### Waypoint 0

- Tag: `21`
- Members: `Independent_Merc_Mako (object 0, id 1399, starts at point 1)`, `Independent_Merc_Mako (object 1, id 1398, starts at point 1)`, `Independent_Merc_Mako (object 2, id 1400, starts at point 1)`, `Generic_Light_Freighter (object 3, id 1388, starts at point 0)`, `Generic_Light_Freighter (object 4, id 1389, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (290.40, 0.00, 324.30) | None |
| 1 | (165.64, 0.00, 185.02) | None |
| 2 | (-664.33, 200.00, 164.64) | None |
| 3 | (-2081.55, 800.00, -2695.18) | None |
| 4 | (-2017.89, 1000.00, -6162.56) | None |
| 5 | (913.08, -300.00, -8070.42) | None |
| 6 | (2881.36, -800.00, -2431.36) | None |
| 7 | (2225.26, 0.00, 504.68) | None |

### Waypoint 1

- Tag: `20`
- Members: `Science_Vessel (object 5, id 1457, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-2753.20, 155.70, -1669.57) | None |
| 1 | (-2749.80, 0.00, -1196.32) | on arrival action 1, param -1 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Independent_Merc_Mako` | 1399 | Interactive | 398.69,0.00,408.60 | 320,0,0 | group/role: FG_BORA3 / 2; waypoint: Waypoint 0 (tag 21, 8 point(s)), starting point 1, arrival event value 1376257 |
| 1 | `Independent_Merc_Mako` | 1398 | Interactive | 391.50,0.00,371.94 | 320,0,0 | group/role: FG_BORA3 / 1; secondary groups: none, ARGOSO 914; waypoint: Waypoint 0 (tag 21, 8 point(s)), starting point 1, arrival event value 1376257 |
| 2 | `Independent_Merc_Mako` | 1400 | Interactive | 422.25,0.00,386.72 | 320,0,0 | group/role: FG_BORA3 / 3; waypoint: Waypoint 0 (tag 21, 8 point(s)), starting point 1, arrival event value 1376257 |
| 3 | `Generic_Light_Freighter` | 1388 | Interactive | 430.85,0.00,534.28 | 320,0,0 | group/role: none / 1; secondary groups: CONT_027, none; waypoint: Waypoint 0 (tag 21, 8 point(s)), starting point 0, arrival event value 1376256 |
| 4 | `Generic_Light_Freighter` | 1389 | Interactive | 555.50,0.00,550.66 | 320,0,0 | group/role: FG_BORA2 / 2; secondary groups: CONT_040, none; waypoint: Waypoint 0 (tag 21, 8 point(s)), starting point 0, arrival event value 1376256 |
| 5 | `Science_Vessel` | 1457 | Interactive | -2748.80,155.70,-2060.85 | 0,0,0 | group/role: none / 1; secondary groups: CONT_005, EXPLORATION; waypoint: Waypoint 1 (tag 20, 2 point(s)), starting point 0, arrival event value 1310720 |
