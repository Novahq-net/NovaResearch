# Tachyon: The Fringe EARTH10.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH10.SPX` |
| Sector | `QUAD_10` |
| Backdrop | `EARTH10.BDF` |
| Region | 0 |
| Sector ID | 9 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 2 |
| Events | 2 |
| Waypoints | 0 |
| Child Sectors | 1 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Spcargo_Credits`, `1: Hyper_Gate` |
| Scripts | `PLAYER.SCR` |
| Scenes | None |
| Labels | None |
| Aliases | None |
| Groups | `CONT_068` |
| Child Sectors | [earth10G.spx](EARTH10G.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 3; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 134
- Set/add variable: variable group 0, variable 2, subtype 1, value 500
- Show/update HUD contact: contact/list 0, subtype 9, param 34
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0
- Set/add variable: variable group 12, variable 304, subtype 0, value 1

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 32, op 2, value 10

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 34
- Set/add variable: variable group 20, variable 32, subtype 0, value 0

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | 878.30,0.00,1980.17 | 0,0,0 | Gate SPX: [earth03.spx](EARTH03.md) |
| 1 | `Spcargo_Credits` | 3 | Interactive | 917.33,0.00,1227.13 | 0,0,0 | secondary groups: CONT_068, none |
