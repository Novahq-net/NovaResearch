# Tachyon: The Fringe NEUT07D.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT07D.SPX` |
| Sector | `QUAD_07` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 6 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 1 |
| Events | 4 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Light_Freighter` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | `g01bsa`, `g01bfa`, `g01bfb`, `g01bfc`, `G01bra`, `integ` |
| Aliases | `Todd08`, `Todd09`, `Todd10`, `Todd14`, `Todd15`, `Todd16`, `Todd12`, `Todd13`, `Todd18`, `Todd03`, `Todd04`, `Todd02`, `Todd05`, `Todd06`, `Todd07`, `Todd21`, `Todd22`, `Todd23`, `will_01`, `SHIP1_HYPER`, `SHIP2_HYPER`, `SHIP3_HYPER`, `ohshit` |
| Groups | `VENETIAN`, `CONT_022` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 21, variable 3, op 1, value 1

**Action**

- Object spawn/action: Generic_Light_Freighter (object 0, id 1753), subtype 3
- Show/update HUD contact: contact/list 0, subtype 6, param 1753
- Object spawn/action: Generic_Light_Freighter (object 0, id 1753), subtype 14

### Event 1

**Trigger**

- Object arrival: Generic_Light_Freighter (object 0, id 1753) reached Waypoint 0 (tag 251), point 2 (raw value 16449538)

**Action**

- Object spawn/action: Generic_Light_Freighter (object 0, id 1753), subtype 6
- Play dialog: PLAYER.SCR, line/variant 174
- Set/add variable: variable group 21, variable 21, subtype 0, value 1
- Object spawn/action: Generic_Light_Freighter (object 0, id 1753), subtype 15
- Hide/remove HUD contact: contact/list 0, subtype 6, param 1753

### Event 2

**Trigger**

- Variable comparison: subject variable group 21, variable 21, op 1, value 1

**Action**

- Set/add variable: variable group 13, variable 408, subtype 0, value 1
- Set/add variable: variable group 13, variable 409, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 12, param 33
- Show/update HUD contact: contact/list 0, subtype 8, param 0

### Event 3

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 174

**Action**

- Play dialog: PLAYER.SCR, line/variant 176

## Waypoints

### Waypoint 0

- Tag: `251`
- Members: `Generic_Light_Freighter (object 0, id 1753, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (153.94, -2087.50, -1289.20) | None |
| 1 | (149.43, -2081.74, -931.34) | None |
| 2 | (152.45, -2083.66, -752.47) | None; listened by Event 1 for Generic_Light_Freighter (object 0, id 1753) |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Generic_Light_Freighter` | 1753 | Interactive | 158.10,-2094.33,-1610.40 | 0,0,0 | alias: will_01; secondary groups: CONT_022, VENETIAN; waypoint: Waypoint 0 (tag 251, 3 point(s)), starting point 0, arrival event value 16449536 |
