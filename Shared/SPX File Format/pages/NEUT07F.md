# Tachyon: The Fringe NEUT07F.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT07F.SPX` |
| Sector | `QUAD_07` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 6 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 1 |
| Events | 3 |
| Waypoints | 1 |
| Child Sectors | 0 |
| Scripts | 0 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Light_Freighter` |
| Scripts | None |
| Scenes | None |
| Labels | `g01bsa`, `g01bfc`, `g01gfc`, `g01gfa`, `g01bfa`, `g01bfb`, `g01gfd`, `G01bra`, `Integ` |
| Aliases | `Todd03`, `Todd04`, `Todd02`, `Todd05`, `Todd06`, `Todd07`, `Todd08`, `Todd09`, `Todd10`, `Todd11`, `Todd12`, `Todd13`, `Todd14`, `Todd15`, `Todd16`, `Todd17`, `Todd18`, `Todd19`, `Todd20`, `Todd21`, `Todd22`, `Todd23`, `SHIP1_HYPER`, `SHIP3_HYPER`, `SHIP2_HYPER`, `will_01`, `kevin02` |
| Groups | `CAYUGAN_HAULER`, `CONT_041` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 19, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 7

**Action**

- Object spawn/action: Generic_Light_Freighter (object 0, id 1778), subtype 3
- Show/update HUD contact: contact/list 0, subtype 6, param 1778

### Event 2

**Trigger**

- Object arrival: Generic_Light_Freighter (object 0, id 1778) reached Waypoint 0 (tag 351), point 1 (raw value 23003137)

**Action**

- Set/add variable: variable group 13, variable 412, subtype 0, value 1
- Set/add variable: variable group 13, variable 413, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 21, variable 20, subtype 1, value 1
- Hide/remove HUD contact: contact/list 0, subtype 6, param 1778

## Waypoints

### Waypoint 0

- Tag: `351`
- Members: `Generic_Light_Freighter (object 0, id 1778, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-367.84, -2506.97, 1415.99) | None |
| 1 | (-210.82, -1715.04, 1099.52) | on arrival activate current object (raw param -1 ignored); listened by Event 2 for Generic_Light_Freighter (object 0, id 1778) |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Generic_Light_Freighter` | 1778 | Interactive | -624.02,-3291.98,1761.18 | 175,91,91 | alias: kevin02; secondary groups: CONT_041, CAYUGAN_HAULER; waypoint: Waypoint 0 (tag 351, 2 point(s)), starting point 0, arrival event value 23003136 |
