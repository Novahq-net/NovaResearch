# Tachyon: The Fringe DISP07B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP07B.SPX` |
| Sector | `QUAD_07` |
| Backdrop | `(none)` |
| Region | 6 |
| Sector ID | 6 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 0 |
| Entities | 0 |
| Events | 10 |
| Waypoints | 0 |
| Child Sectors | 0 |
| Scripts | 0 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | None |
| Scripts | None |
| Scenes | None |
| Labels | `TNSA`, `CRGUS`, `INTEG`, `HEPHA` |
| Aliases | `tnsa` |
| Groups | None |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Set runtime trigger variable: variable group 20, variable 9, subtype 0, value 0
- Show/update HUD contact: contact/list 0, subtype 0, param 2

### Event 1

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 35

**Action**

- Object spawn/action: id 786, subtype 3
- Object spawn/action: id 815, subtype 3
- Object spawn/action: id 830, subtype 0
- Object spawn/action: id 831, subtype 0
- Object spawn/action: id 832, subtype 0
- Object spawn/action: id 833, subtype 0
- Object spawn/action: id 838, subtype 0
- Object spawn/action: id 839, subtype 0

### Event 2

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 35

**Action**

- Object spawn/action: id 840, subtype 0
- Object spawn/action: id 841, subtype 0
- Object spawn/action: id 834, subtype 0
- Object spawn/action: id 835, subtype 0
- Object spawn/action: id 836, subtype 0
- Object spawn/action: id 837, subtype 0

### Event 3

**Trigger**

- Variable comparison: subject variable group 21, variable 6, op 1, value 1
- Variable comparison: subject variable group 20, variable 9, op 1, value 35

**Action**

- Object spawn/action: id 815, subtype 3

### Event 4

**Trigger**

- Variable comparison: subject variable group 21, variable 7, op 1, value 1
- Variable comparison: subject variable group 20, variable 9, op 1, value 35

**Action**

- Object spawn/action: id 786, subtype 3

### Event 5

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 80

**Action**

- Object spawn/action: id 531, subtype 3

### Event 6

**Trigger**

- Object event: subject 815, op 0, value 0 (extra 1, 531; flags 2)

**Action**

- Object spawn/action: id 786, subtype 7

### Event 7

**Trigger**

- Object event: subject 786, op 0, value 0 (extra 1, 531; flags 2)

**Action**

- Object spawn/action: id 815, subtype 7

### Event 8

**Trigger**

- Object event: subject 1234, op 2, value 0

**Action**

- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Set/add variable: variable group 18, variable 404, subtype 0, value 1
- Set/add variable: variable group 18, variable 405, subtype 0, value 2
- Set/add variable: variable group 21, variable 20, subtype 0, value 0

### Event 9

**Trigger**

- Variable comparison: subject variable group 20, variable 9, op 1, value 85

**Action**

- Object spawn/action: id 1314, subtype 1, param 2

## Waypoints

None
## Spawn Lists

None

## Objects

None
