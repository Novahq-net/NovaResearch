# Tachyon: The Fringe NEUT01B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `NEUT01B.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 1 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 6 |
| Events | 3 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Generic_Light_Freighter` |
| Scripts | `ALPHA.SCR` |
| Scenes | None |
| Labels | `MISHK`, `FakeJake`, `Daymir` |
| Aliases | `Courage`, `kwi03_7`, `Jerome26`, `Jerome25`, `Jerome24`, `Jerome22`, `Jerome21`, `Jerome20`, `kevin01`, `Intrepid`, `kwI03_10`, `SHIP1_HYPER`, `ohshit`, `SHIP2_HYPER`, `SHIP3_HYPER` |
| Groups | `FG_MAGELLAN` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 21, variable 20, op 3, value 1

**Action**

- Object spawn/action: Generic_Light_Freighter (object 2, id 188), subtype 14
- Show/update HUD contact: contact/list 0, subtype 7, param 181

### Event 1

**Trigger**

- Object event: subject Generic_Light_Freighter (object 0, id 186), op 8, value 0 (join 2)
- Object event: subject Generic_Light_Freighter (object 1, id 187), op 8, value 0 (join 2)
- Object event: subject Generic_Light_Freighter (object 2, id 188), op 8, value 0 (join 2)
- Object event: subject Generic_Light_Freighter (object 3, id 190), op 8, value 0 (join 2)
- Object event: subject Generic_Light_Freighter (object 4, id 191), op 8, value 0 (join 2)
- Object event: subject Generic_Light_Freighter (object 5, id 192), op 8, value 0 (join 2)

**Action**

- Set/add variable: variable group 21, variable 20, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 7, param 181
- Mission objective/state: param 65539, subtype 0, param 0
- Object spawn/action: Generic_Light_Freighter (object 2, id 188), subtype 15

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 9, value 0

**Action**

- Play dialog: ALPHA.SCR, line/variant 1

## Waypoints

### Waypoint 0

- Tag: `152`
- Members: `Generic_Light_Freighter (object 0, id 186, starts at point 1)`, `Generic_Light_Freighter (object 1, id 187, starts at point 2)`, `Generic_Light_Freighter (object 2, id 188, starts at point 3)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (4556.57, 119.33, -8187.97) | None |
| 1 | (4696.69, 116.35, -8348.75) | None |
| 2 | (4874.32, 111.79, -8516.88) | None |
| 3 | (5057.26, 112.80, -8704.23) | None |
| 4 | (5416.64, 118.40, -8979.37) | None |
| 5 | (6386.68, 131.91, -9534.23) | on arrival action 1, param -1 |

### Waypoint 1

- Tag: `151`
- Members: `Generic_Light_Freighter (object 3, id 190, starts at point 1)`, `Generic_Light_Freighter (object 4, id 191, starts at point 2)`, `Generic_Light_Freighter (object 5, id 192, starts at point 3)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (4669.19, 119.32, -7989.38) | None |
| 1 | (4812.71, 109.48, -8149.24) | None |
| 2 | (4981.27, 113.17, -8339.60) | None |
| 3 | (5172.60, 110.75, -8535.34) | None |
| 4 | (5505.29, 118.40, -8832.56) | None |
| 5 | (6396.80, 131.91, -9415.86) | on arrival action 1, param -1 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Generic_Light_Freighter` | 186 | Interactive | 4249.30,128.05,-7727.37 | 217,0,0 | group/role: FG_MAGELLAN / 0; alias: Jerome26; waypoint: Waypoint 0 (tag 152, 6 point(s)), starting point 1, arrival event value 9961473 |
| 1 | `Generic_Light_Freighter` | 187 | Interactive | 4322.17,128.05,-7866.35 | 217,0,0 | group/role: FG_MAGELLAN / 0; alias: Jerome25; waypoint: Waypoint 0 (tag 152, 6 point(s)), starting point 2, arrival event value 9961474 |
| 2 | `Generic_Light_Freighter` | 188 | Interactive | 4395.78,128.04,-8009.61 | 217,0,0 | group/role: FG_MAGELLAN / 0; alias: Jerome24; waypoint: Waypoint 0 (tag 152, 6 point(s)), starting point 3, arrival event value 9961475 |
| 3 | `Generic_Light_Freighter` | 190 | Interactive | 4402.19,128.05,-7494.46 | 217,0,0 | group/role: FG_MAGELLAN / 0; alias: Jerome22; waypoint: Waypoint 1 (tag 151, 6 point(s)), starting point 1, arrival event value 9895937 |
| 4 | `Generic_Light_Freighter` | 191 | Interactive | 4473.48,128.05,-7629.52 | 217,0,0 | group/role: FG_MAGELLAN / 0; alias: Jerome21; waypoint: Waypoint 1 (tag 151, 6 point(s)), starting point 2, arrival event value 9895938 |
| 5 | `Generic_Light_Freighter` | 192 | Interactive | 4548.83,128.05,-7771.36 | 217,0,0 | group/role: FG_MAGELLAN / 0; alias: Jerome20; waypoint: Waypoint 1 (tag 151, 6 point(s)), starting point 3, arrival event value 9895939 |
