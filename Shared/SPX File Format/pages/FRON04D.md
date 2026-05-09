# Tachyon: The Fringe FRON04D.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON04D.SPX` |
| Sector | `QUAD_04` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 3 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 7 |
| Events | 5 |
| Waypoints | 3 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Skav_Pirate_Manta` |
| Scripts | `PLAYER.SCR`, `SKAVP.SCR` |
| Scenes | None |
| Labels | `BFGF_05`, `bfne_01`, `BFGE_01`, `BFNE_06`, `BFGE_05` |
| Aliases | `Jerome13`, `Kimodo 2`, `Kimodo 1`, `Kimodo 3`, `Kimodo 4`, `Python 1`, `Python 2`, `Python 3`, `Python 4`, `Aphid2`, `Aphid1`, `Mantis1`, `Mantis2`, `Cephius` |
| Groups | `FG_ROACH`, `FG_BEETLE` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Mission objective/state: param 262148, subtype 0, param 0
- Play dialog: PLAYER.SCR, line/variant 108

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Group/spawn-list action: spawn list/group 183, subtype 2

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 16, variable 802, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 182, subtype 1, param 1
- Group/spawn-list action: spawn list/group 183, subtype 4, param 9

### Event 3

**Trigger**

- Group/spawn-list event: subject 182, op 5, value 0 (join 2)
- Group/spawn-list event: subject 183, op 5, value 0

**Action**

- Play dialog: SKAVP.SCR, line/variant 1

### Event 4

**Trigger**

- Group/spawn-list event: subject 183, op 1, value 50 (join 2)
- Group/spawn-list event: subject 183, op 1, value 50

**Action**

- Play dialog: PLAYER.SCR, line/variant 185

## Waypoints

### Waypoint 0

- Tag: `253`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1995.67, 0.00, -788.75) | None |
| 1 | (961.52, 0.00, -2084.50) | None |
| 2 | (-1122.90, 0.00, -537.48) | None |
| 3 | (-1940.93, 0.00, 488.99) | None |
| 4 | (-886.56, 0.00, 55.46) | None |
| 5 | (-1942.85, 0.00, 150.35) | None |

### Waypoint 1

- Tag: `252`
- Members: `Skav_Pirate_Manta (object 4, id 885, starts at point 0)`, `Skav_Pirate_Manta (object 5, id 886, starts at point 0)`, `Skav_Pirate_Manta (object 6, id 887, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1623.25, 0.00, 57.70) | None |
| 1 | (-1583.54, 0.00, -925.64) | None |
| 2 | (-2220.82, 0.00, -487.97) | None |
| 3 | (-2464.43, 0.00, -157.74) | None |
| 4 | (-441.80, 0.00, -539.72) | None |
| 5 | (-2036.23, 0.00, 307.85) | None |

### Waypoint 2

- Tag: `251`
- Members: `Skav_Pirate_Manta (object 0, id 879, starts at point 0)`, `Skav_Pirate_Manta (object 1, id 880, starts at point 0)`, `Skav_Pirate_Manta (object 2, id 881, starts at point 0)`, `Skav_Pirate_Manta (object 3, id 882, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-1007.86, 0.00, 335.25) | None |
| 1 | (569.48, 0.00, -637.07) | None |
| 2 | (1361.41, 0.00, -2325.63) | None |
| 3 | (-1144.73, 0.00, -1628.32) | None |
| 4 | (-971.44, 0.00, -867.35) | None |
| 5 | (-2861.37, 0.00, -97.44) | None |
| 6 | (-2337.23, 0.00, 141.70) | None |
| 7 | (-1858.15, 0.00, -376.22) | None |

## Spawn Lists

### Spawn List 0

- ID: `182`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 1

- ID: `183`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Skav_Pirate_Manta` | 879 | Interactive | 602.99,0.00,6590.26 | 0,0,0 | label: BFNE_06; group/role: FG_ROACH / 0; waypoint: Waypoint 2 (tag 251, 8 point(s)), starting point 0, arrival event value 16449536 |
| 1 | `Skav_Pirate_Manta` | 880 | Interactive | 1005.22,0.00,6502.89 | 0,0,0 | group/role: FG_ROACH / 0; waypoint: Waypoint 2 (tag 251, 8 point(s)), starting point 0, arrival event value 16449536 |
| 2 | `Skav_Pirate_Manta` | 881 | Interactive | 1219.74,0.00,6561.13 | 0,0,0 | label: BFNE_06; group/role: FG_ROACH / 0; waypoint: Waypoint 2 (tag 251, 8 point(s)), starting point 0, arrival event value 16449536 |
| 3 | `Skav_Pirate_Manta` | 882 | Interactive | 1568.34,0.00,6619.38 | 0,0,0 | group/role: FG_ROACH / 0; waypoint: Waypoint 2 (tag 251, 8 point(s)), starting point 0, arrival event value 16449536 |
| 4 | `Skav_Pirate_Manta` | 885 | Interactive | -1654.32,0.00,72.09 | 0,0,0 | label: BFNE_06; group/role: FG_BEETLE / 0; waypoint: Waypoint 1 (tag 252, 6 point(s)), starting point 0, arrival event value 16515072 |
| 5 | `Skav_Pirate_Manta` | 886 | Interactive | -1625.72,0.00,126.46 | 0,0,0 | group/role: FG_BEETLE / 0; waypoint: Waypoint 1 (tag 252, 6 point(s)), starting point 0, arrival event value 16515072 |
| 6 | `Skav_Pirate_Manta` | 887 | Interactive | -1568.51,0.00,211.89 | 0,0,0 | label: BFNE_06; group/role: FG_BEETLE / 0; waypoint: Waypoint 1 (tag 252, 6 point(s)), starting point 0, arrival event value 16515072 |
