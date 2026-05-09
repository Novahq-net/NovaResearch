# Tachyon: The Fringe FRON10A.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON10A.SPX` |
| Sector | `QUAD_10` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 9 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 2 |
| Entities | 9 |
| Events | 9 |
| Waypoints | 2 |
| Child Sectors | 0 |
| Scripts | 3 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Malkar_Treg`, `1: Susan_Bradley_Waraxe` |
| Scripts | `PLAYER.SCR`, `SUSAN.SCR`, `MALKR.SCR` |
| Scenes | None |
| Labels | `Susan`, `BFGE_01`, `BFGE_1`, `Malkar1` |
| Aliases | `BC05_sistine_chapel`, `Susan Bradley` |
| Groups | `SUSAN_BRADLEY`, `FG_CHARES` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Object spawn/action: id 1076, subtype 8, param 4
- Set runtime trigger variable: variable group 20, variable 0, subtype 0, value 0
- Group/spawn-list action: spawn list/group 116, subtype 4, param 4
- Play scene: unknown index 0, param 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 4

**Action**

- Play dialog: PLAYER.SCR, line/variant 16

### Event 2

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 16

**Action**

- Play dialog: PLAYER.SCR, line/variant 17

### Event 3

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 17

**Action**

- Play dialog: SUSAN.SCR, line/variant 2

### Event 4

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 2

**Action**

- Play dialog: SUSAN.SCR, line/variant 4
- Group/spawn-list action: spawn list/group 116, subtype 7

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 0, op 1, value 110

**Action**

- Group/spawn-list action: spawn list/group 116, subtype 4, param 1

### Event 6

**Trigger**

- Runtime condition family: subject 0, op 0, value 0

**Action**

- Object spawn/action: id 1076, subtype 8, param 1
- Set/add variable: variable group 21, variable 23, subtype 0, value 1
- Hide/remove HUD contact: contact/list 0, subtype 10, param 0
- Show/update HUD contact: contact/list 0, subtype 12, param 37
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Object spawn/action: Susan_Bradley_Waraxe (object 0, id 1111), subtype 19
- Mission objective/state: param 262144, subtype 0, param 0

### Event 7

**Trigger**

- Group/spawn-list event: subject 116, op 4, value 0 (flags 2)

**Action**

- Play dialog: MALKR.SCR, line/variant 4

### Event 8

**Trigger**

- Variable comparison: subject variable group 21, variable 23, op 1, value 1

**Action**

- Broadcast hide/remove contact: contact/list 0, subtype 0, param 29
- Broadcast hide/remove contact: contact/list 0, subtype 0, param 47

## Waypoints

### Waypoint 0

- Tag: `2`
- Members: `Malkar_Treg (object 1, id 1117, starts at point 0)`, `Malkar_Treg (object 2, id 1116, starts at point 0)`, `Malkar_Treg (object 3, id 1118, starts at point 0)`, `Malkar_Treg (object 4, id 1119, starts at point 0)`, `Malkar_Treg (object 5, id 1178, starts at point 0)`, `Malkar_Treg (object 6, id 1179, starts at point 0)`, `Malkar_Treg (object 7, id 1180, starts at point 0)`, `Malkar_Treg (object 8, id 1181, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (915.72, -70.66, -1269.79) | None |
| 1 | (-165.18, -70.66, -428.44) | None |
| 2 | (733.92, -70.66, 771.98) | None |
| 3 | (1868.72, -70.66, -112.73) | on arrival redirect to Waypoint 0 (tag 2), point 1 |

### Waypoint 1

- Tag: `1`
- Members: `Susan_Bradley_Waraxe (object 0, id 1111, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (916.40, -371.63, -1655.43) | None |
| 1 | (916.40, -372.78, -1920.12) | on arrival action 1, param -1 |
| 2 | (919.01, -373.06, -2940.81) | on arrival action 1, param -1 |

## Spawn Lists

### Spawn List 0

- ID: `116`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Susan_Bradley_Waraxe` | 1111 | Interactive | 916.40,-461.47,-1515.00 | 256,0,0 | label: Susan; alias: Susan Bradley; secondary groups: none, SUSAN_BRADLEY; waypoint: Waypoint 1 (tag 1, 3 point(s)), starting point 0, arrival event value 65536 |
| 1 | `Malkar_Treg` | 1117 | Interactive | 836.49,-457.07,-1431.91 | 256,128,0 | label: BFGE_01; group/role: FG_CHARES / 1; waypoint: Waypoint 0 (tag 2, 4 point(s)), starting point 0, arrival event value 131072 |
| 2 | `Malkar_Treg` | 1116 | Interactive | 881.49,-457.07,-1431.91 | 256,128,0 | label: BFGE_1; group/role: FG_CHARES / 2; waypoint: Waypoint 0 (tag 2, 4 point(s)), starting point 0, arrival event value 131072 |
| 3 | `Malkar_Treg` | 1118 | Interactive | 956.49,-457.07,-1431.90 | 256,128,0 | group/role: FG_CHARES / 3; waypoint: Waypoint 0 (tag 2, 4 point(s)), starting point 0, arrival event value 131072 |
| 4 | `Malkar_Treg` | 1119 | Interactive | 1002.49,-457.07,-1431.91 | 256,128,0 | group/role: FG_CHARES / 4; waypoint: Waypoint 0 (tag 2, 4 point(s)), starting point 0, arrival event value 131072 |
| 5 | `Malkar_Treg` | 1178 | Interactive | 1001.91,-457.07,-1483.60 | 256,128,0 | group/role: FG_CHARES / 8; waypoint: Waypoint 0 (tag 2, 4 point(s)), starting point 0, arrival event value 131072 |
| 6 | `Malkar_Treg` | 1179 | Interactive | 956.56,-457.07,-1483.60 | 256,128,0 | group/role: FG_CHARES / 7; waypoint: Waypoint 0 (tag 2, 4 point(s)), starting point 0, arrival event value 131072 |
| 7 | `Malkar_Treg` | 1180 | Interactive | 881.87,-457.07,-1483.60 | 256,128,0 | label: Malkar1; group/role: FG_CHARES / 6; waypoint: Waypoint 0 (tag 2, 4 point(s)), starting point 0, arrival event value 131072 |
| 8 | `Malkar_Treg` | 1181 | Interactive | 835.98,-457.07,-1483.60 | 256,128,0 | label: BFGE_01; group/role: FG_CHARES / 5; waypoint: Waypoint 0 (tag 2, 4 point(s)), starting point 0, arrival event value 131072 |
