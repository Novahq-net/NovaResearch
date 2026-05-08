# SPBHD_16.bms - Lost Convoy

Back to [AIN Mission Index](../AIN%20Mission%20Index.md)

![AIN/MIS overlay](overlays/spbhd_16_xy.png)

[Open full-size overlay image](overlays/spbhd_16_xy.png)

## Overlay Legend

| Marker | Meaning |
| --- | --- |
| Gray dots | Normal AIN navigation nodes. |
| Green dots | AIN nodes with `NodeFlags & 0x1C`. |
| Gold dots | AIN `NodeClass 6`. |
| Cyan-blue dots | AIN `NodeClass 7`. |
| Pink dots | AIN `NodeClass 8`. |
| Purple dots | AIN `NodeClass 9`. |
| Cyan circles | MIS items with `ai_textfile`. |
| Yellow circles | MIS items with `waypoint_id`. |
| White circles | Other MIS items with positions. |
| Red squares on frame | MIS items outside the AIN graph bounds. |

## Mission File Info

- Terrain: `mis16`
- AIN nodes: `5125`
- AIN areas: `256`
- MIS items/events/waypoint defs: `2150` / `138` / `88`
- MIS AI-positioned items: `15`
- MIS items with `waypoint_id`: `590`
- AINODEPATH events: `2`

## AIN Plot Maps

| Field | Description | XY | XZ | YZ |
| --- | --- | --- | --- | --- |
| Area ID | Node area/sector grouping. | [XY](plots/SPBHD_16_area_id_xy.png) | [XZ](plots/SPBHD_16_area_id_xz.png) | [YZ](plots/SPBHD_16_area_id_yz.png) |
| Node Class | `NodeClass` values, including special classes `6`-`9`. | [XY](plots/SPBHD_16_node_class_xy.png) | [XZ](plots/SPBHD_16_node_class_xz.png) | [YZ](plots/SPBHD_16_node_class_yz.png) |
| Node Flags | `NodeFlags` byte values and flag clusters. | [XY](plots/SPBHD_16_node_flags_xy.png) | [XZ](plots/SPBHD_16_node_flags_xz.png) | [YZ](plots/SPBHD_16_node_flags_yz.png) |
| Radius | Node `Radius` byte values. | [XY](plots/SPBHD_16_radius_xy.png) | [XZ](plots/SPBHD_16_radius_xz.png) | [YZ](plots/SPBHD_16_radius_yz.png) |
| Edge Flags | Combined outgoing `EdgeFlags`. | [XY](plots/SPBHD_16_edge_flags_xy.png) | [XZ](plots/SPBHD_16_edge_flags_xz.png) | [YZ](plots/SPBHD_16_edge_flags_yz.png) |

## AINODEPATH Events

### Event 0 - AINODEPATH_OFF

- Event block line: `831`
- AINODEPATH action line(s): `851`

**Trigger Items**

_None found._

**Referenced Items**

| Ref | Candidates |
| ---: | --- |
| `2` | item `2` / id `172` / type `1236` Friendly Light Helicopter LITTLE BIRD with benches (`101236`) / ai `h_ah6b_z` / wp `19` / group `19`; node `4191`, area `0`, dist `14.8`<br>item `2044` / id `2` / type `1745` Delta Force Teammate 3 (`101745`) / team `1`; node `4182`, area `0`, dist `24.9` |
| `3` | item `3` / id `176` / type `1239` Technical enemy vehicle with mounted 50cal (`101239`) / ai `g_jeep` / team `2` / group `6`; node `4875`, area `0`, dist `91.9`<br>item `2037` / id `3` / type `1745` Delta Force Teammate 3 (`101745`) / team `1`; node `5015`, area `0`, dist `5467.3` |
| `4` | item `4` / id `177` / type `1239` Technical enemy vehicle with mounted 50cal (`101239`) / ai `g_jeep` / team `2` / group `17`; node `5044`, area `0`, dist `3.0`<br>item `9` / id `4` / type `1276` Hummer with NON-Armored 50cal (`101276`) / ai `G_Jeep` / group `13`; node `4182`, area `0`, dist `10.7` |
| `5` | item `5` / id `178` / type `1239` Technical enemy vehicle with mounted 50cal (`101239`) / ai `g_jeep` / team `2` / group `7`; node `4762`, area `0`, dist `34.8`<br>item `10` / id `5` / type `1276` Hummer with NON-Armored 50cal (`101276`) / ai `G_Jeep` / group `14`; node `4182`, area `0`, dist `23.7` |
| `6` | item `6` / id `179` / type `1239` Technical enemy vehicle with mounted 50cal (`101239`) / ai `g_jeep` / team `2` / group `4`; node `4770`, area `0`, dist `26.4`<br>item `2036` / id `6` / type `1744` Delta Force Teammate 2 (`101744`) / team `1` / group `10`; node `2600`, area `0`, dist `578.9` |
| `7` | item `7` / id `175` / type `1239` Technical enemy vehicle with mounted 50cal (`101239`) / ai `g_jeep` / team `2` / group `5`; node `4875`, area `0`, dist `76.9` |

**Trigger Waypoints**

_None found._

### Event 60 - AINODEPATH_ON

- Event block line: `1670`
- AINODEPATH action line(s): `1681`

**Trigger Items**

| Ref | Candidates |
| ---: | --- |
| `3` | item `3` / id `176` / type `1239` Technical enemy vehicle with mounted 50cal (`101239`) / ai `g_jeep` / team `2` / group `6`; node `4875`, area `0`, dist `91.9`<br>item `2037` / id `3` / type `1745` Delta Force Teammate 3 (`101745`) / team `1`; node `5015`, area `0`, dist `5467.3` |
| `5` | item `5` / id `178` / type `1239` Technical enemy vehicle with mounted 50cal (`101239`) / ai `g_jeep` / team `2` / group `7`; node `4762`, area `0`, dist `34.8`<br>item `10` / id `5` / type `1276` Hummer with NON-Armored 50cal (`101276`) / ai `G_Jeep` / group `14`; node `4182`, area `0`, dist `23.7` |
| `7` | item `7` / id `175` / type `1239` Technical enemy vehicle with mounted 50cal (`101239`) / ai `g_jeep` / team `2` / group `5`; node `4875`, area `0`, dist `76.9` |
| `20` | item `20` / id `189` / type `1038` Desert Adobe hut 3 (`101038`); node `1726`, area `0`, dist `2.3`<br>item `1949` / id `20` / type `1697` Enemy Somalian Soldier with AK47 (`101697`) / team `2` / group `25`; node `3159`, area `0`, dist `1.6` |

**Referenced Items**

| Ref | Candidates |
| ---: | --- |
| `2` | item `2` / id `172` / type `1236` Friendly Light Helicopter LITTLE BIRD with benches (`101236`) / ai `h_ah6b_z` / wp `19` / group `19`; node `4191`, area `0`, dist `14.8`<br>item `2044` / id `2` / type `1745` Delta Force Teammate 3 (`101745`) / team `1`; node `4182`, area `0`, dist `24.9` |
| `3` | item `3` / id `176` / type `1239` Technical enemy vehicle with mounted 50cal (`101239`) / ai `g_jeep` / team `2` / group `6`; node `4875`, area `0`, dist `91.9`<br>item `2037` / id `3` / type `1745` Delta Force Teammate 3 (`101745`) / team `1`; node `5015`, area `0`, dist `5467.3` |
| `5` | item `5` / id `178` / type `1239` Technical enemy vehicle with mounted 50cal (`101239`) / ai `g_jeep` / team `2` / group `7`; node `4762`, area `0`, dist `34.8`<br>item `10` / id `5` / type `1276` Hummer with NON-Armored 50cal (`101276`) / ai `G_Jeep` / group `14`; node `4182`, area `0`, dist `23.7` |
| `7` | item `7` / id `175` / type `1239` Technical enemy vehicle with mounted 50cal (`101239`) / ai `g_jeep` / team `2` / group `5`; node `4875`, area `0`, dist `76.9` |
| `17` | item `17` / id `186` / type `1032` Desert Adobe hut 1 (`101032`); node `1979`, area `0`, dist `0.5`<br>item `1946` / id `17` / type `1697` Enemy Somalian Soldier with AK47 (`101697`) / team `2` / group `25`; node `2442`, area `0`, dist `1.5` |
| `20` | item `20` / id `189` / type `1038` Desert Adobe hut 3 (`101038`); node `1726`, area `0`, dist `2.3`<br>item `1949` / id `20` / type `1697` Enemy Somalian Soldier with AK47 (`101697`) / team `2` / group `25`; node `3159`, area `0`, dist `1.6` |

**Trigger Waypoints**

| Ref | Candidates |
| ---: | --- |
| `3` | item `1217` / wp `3` / id `3042` / type `6005` waypoint (`106005`)<br>item `1313` / wp `3` / id `3052` / type `6005` waypoint (`106005`)<br>item `1400` / wp `3` / id `3069` / type `6005` waypoint (`106005`) |
| `5` | item `1250` / wp `5` / id `3031` / type `6005` waypoint (`106005`)<br>item `1306` / wp `5` / id `3067` / type `6005` waypoint (`106005`)<br>item `1431` / wp `5` / id `3075` / type `6005` waypoint (`106005`)<br>item `1489` / wp `5` / id `3091` / type `6005` waypoint (`106005`)<br>+4 more |
| `7` | item `1288` / wp `7` / id `3040` / type `6005` waypoint (`106005`)<br>item `1325` / wp `7` / id `3055` / type `6005` waypoint (`106005`)<br>item `1395` / wp `7` / id `3084` / type `6005` waypoint (`106005`)<br>item `1445` / wp `7` / id `3094` / type `6005` waypoint (`106005`)<br>+4 more |
| `20` | item `1253` / wp `20` / id `3034` / type `6005` waypoint (`106005`)<br>item `1355` / wp `20` / id `3061` / type `6005` waypoint (`106005`)<br>item `1384` / wp `20` / id `3080` / type `6005` waypoint (`106005`)<br>item `1449` / wp `20` / id `3096` / type `6005` waypoint (`106005`)<br>+4 more |


## Spatial Notes

| Check | Result |
| --- | --- |
| AI item coverage | `14 / 15` AI-positioned items are inside the AIN XY bounds. |
| Positioned item coverage | `2095 / 2150` positioned MIS items are inside the AIN XY bounds. |
| AI nearest-node distance | min `3.0`, median `23.7`, max `577.9`. |
| Area coverage | `1` `AreaId` values used; dominant areas: `[(0, 5125)]`. |
| Special node classes | `{}`. |
| Nonzero edge flags | `{'0x00': 25878, '0x08': 2}`. |

### Outside AIN Bounds

| Item |
| --- |
| item `8` / id `180` / type `1243` Blackhawk used for fast roping (`101243`) / ai `h_bhawkf` / team `1` / group `39` |
| item `23` / id `4364` / type `1086` Mogadishu City Block2 Moderately Generic 64x64 (`101086`) |
| item `24` / id `4365` / type `1086` Mogadishu City Block2 Moderately Generic 64x64 (`101086`) |
| item `25` / id `4366` / type `1086` Mogadishu City Block2 Moderately Generic 64x64 (`101086`) |
| item `27` / id `4370` / type `1086` Mogadishu City Block2 Moderately Generic 64x64 (`101086`) |
| item `43` / id `204` / type `1088` Mogadishu City Block4 Moderately Generic 64x64 (`101088`) / group `23` |
| item `52` / id `4554` / type `1090` Mogadishu City Block6 Highly Generic 64x64 (`101090`) |
| item `54` / id `214` / type `1090` Mogadishu City Block6 Highly Generic 64x64 (`101090`) |

### Farthest AI Items From AIN Nodes

| Item | Nearest Node | Area | Distance |
| --- | ---: | ---: | ---: |
| item `8` / id `180` / type `1243` Blackhawk used for fast roping (`101243`) / ai `h_bhawkf` / team `1` / group `39` | `2600` | `0` | `577.9` |
| item `3` / id `176` / type `1239` Technical enemy vehicle with mounted 50cal (`101239`) / ai `g_jeep` / team `2` / group `6` | `4875` | `0` | `91.9` |
| item `1` / id `174` / type `1236` Friendly Light Helicopter LITTLE BIRD with benches (`101236`) / ai `h_ah6b_z` / group `8` | `4281` | `0` | `89.8` |
| item `7` / id `175` / type `1239` Technical enemy vehicle with mounted 50cal (`101239`) / ai `g_jeep` / team `2` / group `5` | `4875` | `0` | `76.9` |
| item `12` / id `182` / type `1276` Hummer with NON-Armored 50cal (`101276`) / ai `G_Jeep` / group `15` | `4182` | `0` | `36.2` |

### Special Class Nodes

| Node | Class | Area | Flags | Nearest MIS Item | Distance |
| ---: | ---: | ---: | --- | --- | ---: |
| | | | | | |

### Nonzero Edge Flags

| Flag | Source | Target | Areas | Classes | Reverse | Distance |
| --- | ---: | ---: | --- | --- | --- | ---: |
| `0x08` | `1987` | `2024` | `0` -> `0` | `0` -> `0` | `0x08` | `4.4` |
| `0x08` | `2024` | `1987` | `0` -> `0` | `0` -> `0` | `0x08` | `4.4` |
