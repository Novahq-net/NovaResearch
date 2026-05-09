# Tachyon: The Fringe FRON01D.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `FRON01D.SPX` |
| Sector | `QUAD_01` |
| Backdrop | `(none)` |
| Region | 4 |
| Sector ID | 0 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 0 |
| Entities | 0 |
| Events | 4 |
| Waypoints | 0 |
| Child Sectors | 0 |
| Scripts | 1 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | None |
| Scripts | `ARMAN.SCR` |
| Scenes | None |
| Labels | `BFGF_05`, `BFNE_03`, `BFNF_03`, `BFGE_01`, `BFGF_01`, `bfne_05` |
| Aliases | `Python 4`, `Python 3`, `Python 1`, `Python 2`, `Kimodo 1`, `Jerome02`, `Jerome03`, `Jerome04`, `Jerome05`, `Jerome06`, `Jerome01`, `BC05_sistine_chapel`, `bc05_1`, `bc05_2`, `bc05_4`, `bc05_5`, `Mantis1`, `Mantis2`, `Mantis3`, `Mantis4`, `Aphid1`, `Aphid2`, `Aphid3`, `Aphid4`, `Python1`, `Python2`, `Python3`, `Python4`, `Komodo1`, `Komodo2`, `Komodo3`, `Komodo4`, `Kimodo 2`, `Kimodo 3`, `Kimodo 4`, `Cephius`, `Stocks01` |
| Groups | None |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Mission objective/state: param 262148, subtype 0, param 0
- Set runtime trigger variable: variable group 20, variable 13, subtype 0, value 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 13, op 1, value 20

**Action**

- Play dialog: ARMAN.SCR, line/variant 5

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0 (flags 1)
- Variable comparison: subject variable group 16, variable 802, op 1, value 1

**Action**

- Play dialog: ARMAN.SCR, line/variant 6

### Event 3

**Trigger**

- Sector/startup condition family: subject 0, op 0, value 6

**Action**

- Play dialog: ARMAN.SCR, line/variant 7

## Waypoints

None
## Spawn Lists

None

## Objects

None
