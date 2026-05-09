# Tachyon: The Fringe EARTH01.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH01.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `EARTH01.BDF` |
| Region | 0 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 7 |
| Entities | 40 |
| Events | 5 |
| Waypoints | 3 |
| Child Sectors | 1 |
| Scripts | 1 |
| Scenes | 1 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Independent_Shipyard`, `1: Generic_Light_Freighter`, `2: Ganymede_Station`, `3: AGT_Mako`, `4: Star_Patrol_Enforcer`, `5: Shuttle_Medium`, `6: Hyper_Gate` |
| Scripts | `NZST.SCR` |
| Scenes | `EARTH01.SEN` |
| Labels | `argo`, `bfnf_04`, `bfnf_05`, `bfnf_06`, `bfnf_03`, `bfnf_09`, `bfnf_01`, `bfdnf_05`, `bfnf_02`, `bfnf_08` |
| Aliases | `Todd01` |
| Groups | `FG_AGT4`, `CONT_033`, `FG_GALSPAN2`, `FG_GALSPAN1`, `FG_AGT5`, `FG_AGT10`, `NEW_ZURICH_ORBITAL`, `CONT_006`, `FG_GALSPAN8`, `CONT_015`, `FG_GALSPAN7`, `CONT_011` |
| Child Sectors | [earth01A.spx](EARTH01A.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 147; flags 6)
- Variable comparison: subject variable group 8, variable 21, op 1, value 1 (flags 4)

**Action**

- Play dialog: NZST.SCR, line/variant 1
- Set/add variable: variable group 0, variable 2, subtype 1, value 200
- Show/update HUD contact: contact/list 0, subtype 9, param 33
- Set/add variable: variable group 8, variable 21, subtype 0, value 0
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 147; flags 6)
- Variable comparison: subject variable group 8, variable 21, op 1, value 2 (flags 4)

**Action**

- Play dialog: NZST.SCR, line/variant 1
- Set/add variable: variable group 0, variable 2, subtype 1, value 400
- Show/update HUD contact: contact/list 0, subtype 9, param 33
- Set/add variable: variable group 8, variable 21, subtype 0, value 0
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 4, value 0 (extra 1, 147; flags 6)
- Variable comparison: subject variable group 8, variable 21, op 2, value 2 (flags 4)

**Action**

- Play dialog: NZST.SCR, line/variant 1
- Set/add variable: variable group 0, variable 2, subtype 1, value 600
- Show/update HUD contact: contact/list 0, subtype 9, param 33
- Set/add variable: variable group 8, variable 21, subtype 0, value 0
- Set runtime trigger variable: variable group 20, variable 32, subtype 0, value 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 20, variable 32, op 2, value 10

**Action**

- Hide/remove HUD contact: contact/list 0, subtype 9, param 33
- Set/add variable: variable group 20, variable 32, subtype 0, value 0

### Event 4

**Trigger**

- Group/spawn-list event: subject 1, op 4, value 0 (flags 2)
- Variable comparison: subject variable group 0, variable 4, op 1, value 1002

**Action**

- Group/spawn-list action: spawn list/group 1, subtype 7
- Group/spawn-list action: spawn list/group 1, subtype 4, param 5
- Group/spawn-list action: spawn list/group 1, subtype 2

## Waypoints

### Waypoint 0

- Tag: `4`
- Members: `AGT_Mako (object 8, id 253, starts at point 2)`, `AGT_Mako (object 9, id 252, starts at point 2)`, `AGT_Mako (object 10, id 254, starts at point 2)`, `Generic_Light_Freighter (object 37, id 245, starts at point 0)`, `Generic_Light_Freighter (object 38, id 228, starts at point 1)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (343.79, 420.91, 4378.50) | None |
| 1 | (334.67, 420.91, 2098.21) | None |
| 2 | (2087.07, 420.91, -869.92) | None |
| 3 | (7814.45, 420.91, -900.82) | None |
| 4 | (4381.42, 420.91, 10307.36) | None |
| 5 | (-50.80, 420.91, 10255.40) | None |

### Waypoint 1

- Tag: `2`
- Members: `Star_Patrol_Enforcer (object 4, id 205, starts at point 4)`, `Star_Patrol_Enforcer (object 5, id 206, starts at point 4)`, `Star_Patrol_Enforcer (object 6, id 195, starts at point 0)`, `Star_Patrol_Enforcer (object 7, id 196, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (2108.69, 0.00, 771.43) | None |
| 1 | (973.33, 182.00, 8603.73) | None |
| 2 | (3210.99, 289.98, 10110.97) | None |
| 3 | (5305.98, -163.99, 7539.31) | None |
| 4 | (4702.69, -262.98, 5235.38) | None |
| 5 | (-1323.60, 0.00, 2110.64) | None |
| 6 | (-1549.52, 402.98, -695.10) | None |
| 7 | (801.66, 0.00, -1081.44) | None |

### Waypoint 2

- Tag: `1`
- Members: `Shuttle_Medium (object 2, id 293, starts at point 0)`, `Shuttle_Medium (object 3, id 148, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (434.97, -524.99, 1394.92) | None |
| 1 | (3474.24, -191.00, 5100.31) | None |
| 2 | (4399.64, 220.00, 6113.36) | None |
| 3 | (4509.43, 238.00, 7864.20) | None |
| 4 | (3640.94, 168.93, 8523.55) | None |
| 5 | (2138.79, 498.90, 8288.10) | None |
| 6 | (2932.46, 0.00, 7334.21) | None |
| 7 | (3423.85, 165.63, 7314.39) | on arrival redirect to Waypoint 2 (tag 1), point 2 |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | -10.72,838.00,2589.92 | 284,471,0 | Gate SPX: [Earth02.spx](EARTH02.md) |
| 1 | `Hyper_Gate` | 2 | Gate | -2044.14,-288.00,10.37 | 384,256,0 | Gate SPX: [Earth05.spx](EARTH05.md) |
| 2 | `Shuttle_Medium` | 293 | Interactive | 70.85,-653.19,868.07 | 64,0,0 | label: bfnf_04; group/role: FG_AGT4 / 0; secondary groups: CONT_033, none; waypoint: Waypoint 2 (tag 1, 8 point(s)), starting point 0, arrival event value 65536 |
| 3 | `Shuttle_Medium` | 148 | Interactive | 111.75,-653.19,831.05 | 64,0,0 | label: bfnf_05; group/role: FG_AGT4 / 0; secondary groups: CONT_033, none; waypoint: Waypoint 2 (tag 1, 8 point(s)), starting point 0, arrival event value 65536 |
| 4 | `Star_Patrol_Enforcer` | 205 | Interactive | 5175.49,0.00,6291.78 | 320,0,0 | group/role: FG_GALSPAN2 / 1; waypoint: Waypoint 1 (tag 2, 8 point(s)), starting point 4, arrival event value 131076 |
| 5 | `Star_Patrol_Enforcer` | 206 | Interactive | 5361.45,0.00,6327.16 | 320,0,0 | group/role: FG_GALSPAN2 / 2; waypoint: Waypoint 1 (tag 2, 8 point(s)), starting point 4, arrival event value 131076 |
| 6 | `Star_Patrol_Enforcer` | 195 | Interactive | 1023.10,-294.00,122.08 | 64,0,0 | group/role: FG_GALSPAN1 / 1; waypoint: Waypoint 1 (tag 2, 8 point(s)), starting point 0, arrival event value 131072 |
| 7 | `Star_Patrol_Enforcer` | 196 | Interactive | 1035.71,-294.00,-45.40 | 64,0,0 | group/role: FG_GALSPAN1 / 2; waypoint: Waypoint 1 (tag 2, 8 point(s)), starting point 0, arrival event value 131072 |
| 8 | `AGT_Mako` | 253 | Interactive | 343.68,420.91,4968.94 | 256,0,0 | label: bfnf_06; group/role: FG_AGT5 / 0; waypoint: Waypoint 0 (tag 4, 6 point(s)), starting point 2, arrival event value 262146 |
| 9 | `AGT_Mako` | 252 | Interactive | 328.68,420.91,4988.86 | 256,0,0 | group/role: FG_AGT5 / 0; waypoint: Waypoint 0 (tag 4, 6 point(s)), starting point 2, arrival event value 262146 |
| 10 | `AGT_Mako` | 254 | Interactive | 313.68,420.91,5016.03 | 256,0,0 | group/role: FG_AGT5 / 0; waypoint: Waypoint 0 (tag 4, 6 point(s)), starting point 2, arrival event value 262146 |
| 11 | `AGT_Mako` | 266 | Interactive | -14.23,-693.19,594.30 | 448,0,0 | label: bfnf_03; group/role: FG_AGT10 / 0 |
| 12 | `AGT_Mako` | 262 | Interactive | 3.00,-693.19,575.55 | 448,0,0 | group/role: FG_AGT10 / 0 |
| 13 | `AGT_Mako` | 263 | Interactive | -6.00,-693.19,565.34 | 448,0,0 | label: bfnf_06; group/role: FG_AGT10 / 0 |
| 14 | `AGT_Mako` | 267 | Interactive | -23.30,-693.19,581.44 | 448,0,0 | group/role: FG_AGT10 / 0 |
| 15 | `AGT_Mako` | 268 | Interactive | -33.55,-693.19,570.02 | 448,0,0 | group/role: FG_AGT10 / 0 |
| 16 | `AGT_Mako` | 265 | Interactive | -18.00,-693.19,554.74 | 448,0,0 | group/role: FG_AGT10 / 0 |
| 17 | `AGT_Mako` | 264 | Interactive | -28.00,-693.19,544.84 | 448,0,0 | label: bfnf_09; group/role: FG_AGT10 / 0 |
| 18 | `AGT_Mako` | 269 | Interactive | -44.20,-693.19,559.06 | 448,0,0 | label: bfnf_01; group/role: FG_AGT10 / 0 |
| 19 | `AGT_Mako` | 270 | Interactive | -52.87,-693.19,549.54 | 448,0,0 | group/role: FG_AGT10 / 0 |
| 20 | `AGT_Mako` | 261 | Interactive | -37.00,-693.19,535.44 | 448,0,0 | group/role: FG_AGT10 / 0 |
| 21 | `AGT_Mako` | 260 | Interactive | -47.00,-693.19,524.98 | 448,0,0 | group/role: FG_AGT10 / 0 |
| 22 | `AGT_Mako` | 271 | Interactive | -61.15,-693.19,539.07 | 448,0,0 | group/role: FG_AGT10 / 0 |
| 23 | `AGT_Mako` | 272 | Interactive | -172.49,-693.19,754.50 | 192,0,0 | label: bfdnf_05; group/role: FG_AGT10 / 0 |
| 24 | `AGT_Mako` | 278 | Interactive | -156.20,-693.19,738.26 | 192,0,0 | label: bfnf_06; group/role: FG_AGT10 / 0 |
| 25 | `AGT_Mako` | 279 | Interactive | -164.28,-693.19,727.80 | 192,0,0 | group/role: FG_AGT10 / 0 |
| 26 | `AGT_Mako` | 273 | Interactive | -181.30,-693.19,744.08 | 192,0,0 | group/role: FG_AGT10 / 0 |
| 27 | `AGT_Mako` | 274 | Interactive | -189.93,-693.19,732.70 | 192,0,0 | group/role: FG_AGT10 / 0 |
| 28 | `AGT_Mako` | 280 | Interactive | -173.36,-693.19,713.46 | 192,0,0 | group/role: FG_AGT10 / 0 |
| 29 | `AGT_Mako` | 275 | Interactive | -200.15,-693.19,721.32 | 192,0,0 | label: bfnf_02; group/role: FG_AGT10 / 0 |
| 30 | `AGT_Mako` | 281 | Interactive | -182.58,-693.19,702.21 | 192,0,0 | label: bfnf_04; group/role: FG_AGT10 / 0 |
| 31 | `AGT_Mako` | 282 | Interactive | -191.08,-693.19,690.79 | 192,0,0 | group/role: FG_AGT10 / 0 |
| 32 | `AGT_Mako` | 276 | Interactive | -208.47,-693.19,709.46 | 192,0,0 | group/role: FG_AGT10 / 0 |
| 33 | `AGT_Mako` | 277 | Interactive | -217.97,-693.19,698.00 | 192,0,0 | label: bfnf_08; group/role: FG_AGT10 / 0 |
| 34 | `AGT_Mako` | 283 | Interactive | -202.43,-693.19,678.32 | 192,0,0 | group/role: FG_AGT10 / 0 |
| 35 | `Ganymede_Station` | 147 | Interactive | -146.87,667.00,577.36 | 64,0,0 | secondary groups: none, NEW_ZURICH_ORBITAL |
| 36 | `Generic_Light_Freighter` | 284 | Interactive | -72.66,-675.19,658.40 | 64,0,0 | label: bfnf_03; secondary groups: CONT_006, none |
| 37 | `Generic_Light_Freighter` | 245 | Interactive | 413.19,410.91,5561.00 | 256,0,0 | label: bfnf_05; group/role: FG_GALSPAN8 / 0; secondary groups: CONT_015, none; waypoint: Waypoint 0 (tag 4, 6 point(s)), starting point 0, arrival event value 262144 |
| 38 | `Generic_Light_Freighter` | 228 | Interactive | 433.98,420.00,4886.33 | 256,0,0 | label: bfnf_06; group/role: FG_GALSPAN7 / 0; secondary groups: CONT_011, none; waypoint: Waypoint 0 (tag 4, 6 point(s)), starting point 1, arrival event value 262145 |
| 39 | `Independent_Shipyard` | 303 | Interactive | 3519.22,0.00,7887.86 | 448,0,64 | None |
