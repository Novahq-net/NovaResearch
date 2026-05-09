# Tachyon: The Fringe MYST03B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `MYST03B.SPX` |
| Sector | `QUAD_03` |
| Backdrop | `(none)` |
| Region | 5 |
| Sector ID | 2 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 1 |
| Entities | 11 |
| Events | 7 |
| Waypoints | 0 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Cassitor_Assault_Drone` |
| Scripts | `PLAYER.SCR`, `DRCAS.SCR` |
| Scenes | None |
| Labels | `BFNE_06` |
| Aliases | `Will_02` |
| Groups | `FG_STRAIN_PSI`, `FG_STRAIN_MU`, `FG_STRAIN_RHO` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Group/spawn-list action: spawn list/group 88, subtype 6
- Group/spawn-list action: spawn list/group 93, subtype 6
- Group/spawn-list action: spawn list/group 90, subtype 6
- Play dialog: PLAYER.SCR, line/variant 18

### Event 1

**Trigger**

- Group/spawn-list event: subject 88, op 1, value 10 (join 2)
- Group/spawn-list event: subject 93, op 1, value 10 (join 2)
- Group/spawn-list event: subject 90, op 1, value 10

**Action**

- Group/spawn-list action: spawn list/group 88, subtype 2
- Group/spawn-list action: spawn list/group 93, subtype 2
- Group/spawn-list action: spawn list/group 90, subtype 2

### Event 2

**Trigger**

- Group/spawn-list event: subject 88, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 93, op 4, value 0 (join 2; flags 2)
- Group/spawn-list event: subject 90, op 4, value 0 (flags 2)

**Action**

- Play dialog: DRCAS.SCR, line/variant 23

### Event 3

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 23

**Action**

- Play dialog: PLAYER.SCR, line/variant 67

### Event 4

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0
- Variable comparison: subject variable group 8, variable 7, op 1, value 1

**Action**

- Group/spawn-list action: spawn list/group 88, subtype 6
- Group/spawn-list action: spawn list/group 93, subtype 6
- Group/spawn-list action: spawn list/group 90, subtype 6

### Event 5

**Trigger**

- Variable comparison: subject variable group 8, variable 7, op 1, value 1
- Group/spawn-list event: subject 88, op 4, value 0 (join 2; flags 2)
- Variable comparison: subject variable group 8, variable 7, op 1, value 1
- Group/spawn-list event: subject 93, op 4, value 0 (join 2; flags 2)
- Variable comparison: subject variable group 8, variable 7, op 1, value 1
- Group/spawn-list event: subject 90, op 4, value 0 (flags 2)

**Action**

- Play dialog: DRCAS.SCR, line/variant 24

### Event 6

**Trigger**

- Sector/startup condition family: subject 1, op 0, value 24

**Action**

- Play dialog: PLAYER.SCR, line/variant 68

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Cassitor_Assault_Drone` | 31 | Interactive | 46.25,262.00,-853.84 | 457,0,0 | group/role: FG_STRAIN_PSI / 1 |
| 1 | `Cassitor_Assault_Drone` | 32 | Interactive | 41.63,262.00,-928.94 | 457,0,0 | group/role: FG_STRAIN_PSI / 2 |
| 2 | `Cassitor_Assault_Drone` | 33 | Interactive | 92.00,262.00,-851.06 | 442,0,0 | group/role: FG_STRAIN_PSI / 3 |
| 3 | `Cassitor_Assault_Drone` | 35 | Interactive | 718.52,0.00,463.40 | 316,0,0 | group/role: FG_STRAIN_MU / 1 |
| 4 | `Cassitor_Assault_Drone` | 36 | Interactive | 705.30,0.00,506.41 | 309,0,0 | group/role: FG_STRAIN_MU / 3 |
| 5 | `Cassitor_Assault_Drone` | 37 | Interactive | 761.50,0.00,456.23 | 316,0,0 | group/role: FG_STRAIN_MU / 2 |
| 6 | `Cassitor_Assault_Drone` | 38 | Interactive | 763.15,0.00,511.79 | 302,0,0 | group/role: FG_STRAIN_MU / 4 |
| 7 | `Cassitor_Assault_Drone` | 39 | Interactive | -315.25,0.00,387.32 | 385,0,0 | group/role: FG_STRAIN_RHO / 1 |
| 8 | `Cassitor_Assault_Drone` | 40 | Interactive | -257.74,0.00,449.14 | 385,0,0 | group/role: FG_STRAIN_RHO / 3 |
| 9 | `Cassitor_Assault_Drone` | 41 | Interactive | -257.74,0.00,320.03 | 385,0,0 | group/role: FG_STRAIN_RHO / 2 |
| 10 | `Cassitor_Assault_Drone` | 42 | Interactive | -192.79,0.00,507.82 | 385,0,0 | group/role: FG_STRAIN_RHO / 4 |
