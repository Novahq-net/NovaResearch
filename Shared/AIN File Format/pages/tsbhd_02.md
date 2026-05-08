# tsbhd_02.bms - Jungle Airfield Takedown

Back to [AIN Mission Index](../AIN%20Mission%20Index.md)

![AIN/MIS overlay](overlays/tsbhd_02_xy.png)

[Open full-size overlay image](overlays/tsbhd_02_xy.png)

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

- Terrain: `ts_02`
- AIN nodes: `3251`
- AIN areas: `256`
- MIS items/events/waypoint defs: `1589` / `102` / `38`
- MIS AI-positioned items: `89`
- MIS items with `waypoint_id`: `164`
- AINODEPATH events: `5`

## AIN Plot Maps

| Field | Description | XY | XZ | YZ |
| --- | --- | --- | --- | --- |
| Area ID | Node area/sector grouping. | [XY](plots/tsbhd_02_area_id_xy.png) | [XZ](plots/tsbhd_02_area_id_xz.png) | [YZ](plots/tsbhd_02_area_id_yz.png) |
| Node Class | `NodeClass` values, including special classes `6`-`9`. | [XY](plots/tsbhd_02_node_class_xy.png) | [XZ](plots/tsbhd_02_node_class_xz.png) | [YZ](plots/tsbhd_02_node_class_yz.png) |
| Node Flags | `NodeFlags` byte values and flag clusters. | [XY](plots/tsbhd_02_node_flags_xy.png) | [XZ](plots/tsbhd_02_node_flags_xz.png) | [YZ](plots/tsbhd_02_node_flags_yz.png) |
| Radius | Node `Radius` byte values. | [XY](plots/tsbhd_02_radius_xy.png) | [XZ](plots/tsbhd_02_radius_xz.png) | [YZ](plots/tsbhd_02_radius_yz.png) |
| Edge Flags | Combined outgoing `EdgeFlags`. | [XY](plots/tsbhd_02_edge_flags_xy.png) | [XZ](plots/tsbhd_02_edge_flags_xz.png) | [YZ](plots/tsbhd_02_edge_flags_yz.png) |

## AINODEPATH Events

### Event 0 - AINODEPATH_OFF

- Event block line: `642`
- AINODEPATH action line(s): `646`

**Trigger Items**

_None found._

**Referenced Items**

| Ref | Candidates |
| ---: | --- |
| `4` | item `4` / id `2357` / type `1286` / ai `gu_s` / group `50`; node `1731`, area `0`, dist `460.6`<br>item `211` / id `4` / type `4209` Small steel hangar with rounded roof (`104209`); node `1210`, area `0`, dist `1.6` |
| `5` | item `5` / id `2358` / type `1286` / ai `gu_s` / group `51`; node `1731`, area `0`, dist `470.2`<br>item `212` / id `5` / type `4209` Small steel hangar with rounded roof (`104209`); node `2522`, area `0`, dist `2.6` |
| `11` | item `11` / id `4679` / type `1881` 50cal on 360 tripod (`101881`); node `1879`, area `0`, dist `680.1` |
| `13` | item `13` / id `3715` / type `1902` 50cal on 180 tripod (`101902`); node `3192`, area `0`, dist `5.6` |
| `15` | item `15` / id `4430` / type `1902` 50cal on 180 tripod (`101902`); node `94`, area `0`, dist `9.9` |
| `200` | item `200` / id `3440` / type `2098` Med Wall Foliage, for placement right next to walls (`102098`); node `3190`, area `0`, dist `3.4` |

**Trigger Waypoints**

_None found._

### Event 14 - AINODEPATH_ON

- Event block line: `827`
- AINODEPATH action line(s): `841`

**Trigger Items**

| Ref | Candidates |
| ---: | --- |
| `8` | item `8` / id `4681` / type `1493` Small fishing boat type #2 (`101493`) / ai `wu`; node `1874`, area `0`, dist `862.8` |
| `10` | item `10` / id `4202` / type `1869` Mounted Grenade Launcher on Tripod (`101869`); node `719`, area `0`, dist `8.9` |
| `12` | item `12` / id `4097` / type `1881` 50cal on 360 tripod (`101881`); node `1879`, area `0`, dist `606.8` |
| `13` | item `13` / id `3715` / type `1902` 50cal on 180 tripod (`101902`); node `3192`, area `0`, dist `5.6` |
| `63` | item `63` / id `2808` / type `1632` Single placeable radio alternative (`101632`) / group `20`; node `3192`, area `0`, dist `3.8` |

**Referenced Items**

| Ref | Candidates |
| ---: | --- |
| `2` | item `2` / id `1310` / type `1272` Blackhawk, miniguns, both doors open (`101272`) / ai `h_bhawk` / team `1` / group `63`; node `1876`, area `0`, dist `1102.8`<br>item `209` / id `2` / type `4204` Three layer wooden guard tower (`104204`); node `1270`, area `0`, dist `6.0` |
| `4` | item `4` / id `2357` / type `1286` / ai `gu_s` / group `50`; node `1731`, area `0`, dist `460.6`<br>item `211` / id `4` / type `4209` Small steel hangar with rounded roof (`104209`); node `1210`, area `0`, dist `1.6` |
| `8` | item `8` / id `4681` / type `1493` Small fishing boat type #2 (`101493`) / ai `wu`; node `1874`, area `0`, dist `862.8` |
| `10` | item `10` / id `4202` / type `1869` Mounted Grenade Launcher on Tripod (`101869`); node `719`, area `0`, dist `8.9` |
| `12` | item `12` / id `4097` / type `1881` 50cal on 360 tripod (`101881`); node `1879`, area `0`, dist `606.8` |
| `13` | item `13` / id `3715` / type `1902` 50cal on 180 tripod (`101902`); node `3192`, area `0`, dist `5.6` |

**Trigger Waypoints**

| Ref | Candidates |
| ---: | --- |
| `8` | item `1212` / wp `8` / id `1917` / type `6005` waypoint (`106005`)<br>item `1234` / wp `8` / id `1918` / type `6005` waypoint (`106005`)<br>item `1256` / wp `8` / id `1919` / type `6005` waypoint (`106005`)<br>item `1280` / wp `8` / id `1920` / type `6005` waypoint (`106005`)<br>+2 more |
| `10` | item `1214` / wp `10` / id `3162` / type `6005` waypoint (`106005`)<br>item `1252` / wp `10` / id `3163` / type `6005` waypoint (`106005`)<br>item `1268` / wp `10` / id `3164` / type `6005` waypoint (`106005`)<br>item `1275` / wp `10` / id `3165` / type `6005` waypoint (`106005`)<br>+1 more |
| `12` | item `1215` / wp `12` / id `1930` / type `6005` waypoint (`106005`) / ai `null`<br>item `1242` / wp `12` / id `1945` / type `6005` waypoint (`106005`) |
| `13` | item `1216` / wp `13` / id `1931` / type `6005` waypoint (`106005`)<br>item `1244` / wp `13` / id `1946` / type `6005` waypoint (`106005`) |

### Event 22 - AINODEPATH_OFF

- Event block line: `935`
- AINODEPATH action line(s): `951`

**Trigger Items**

| Ref | Candidates |
| ---: | --- |
| `200` | item `200` / id `3440` / type `2098` Med Wall Foliage, for placement right next to walls (`102098`); node `3190`, area `0`, dist `3.4` |
| `201` | item `201` / id `3441` / type `2098` Med Wall Foliage, for placement right next to walls (`102098`); node `2004`, area `0`, dist `3.6` |

**Referenced Items**

| Ref | Candidates |
| ---: | --- |
| `5` | item `5` / id `2358` / type `1286` / ai `gu_s` / group `51`; node `1731`, area `0`, dist `470.2`<br>item `212` / id `5` / type `4209` Small steel hangar with rounded roof (`104209`); node `2522`, area `0`, dist `2.6` |
| `15` | item `15` / id `4430` / type `1902` 50cal on 180 tripod (`101902`); node `94`, area `0`, dist `9.9` |
| `20` | item `20` / id `4487` / type `2044` Power Up Med Pack Infinite (`102044`); node `1731`, area `0`, dist `449.7` |
| `28` | item `28` / id `4762` / type `1111` Mogadishu Slum, Small Wooden structure (`101111`) / ai `null`; node `934`, area `0`, dist `4.2` |
| `29` | item `29` / id `1899` / type `1111` Mogadishu Slum, Small Wooden structure (`101111`) / ai `null`; node `1162`, area `0`, dist `4.4` |
| `30` | item `30` / id `2672` / type `1111` Mogadishu Slum, Small Wooden structure (`101111`) / ai `null`; node `1731`, area `0`, dist `453.0` |

**Trigger Waypoints**

_None found._

### Event 26 - AINODEPATH_ON

- Event block line: `992`
- AINODEPATH action line(s): `1002`

**Trigger Items**

| Ref | Candidates |
| ---: | --- |
| `7` | item `7` / id `4441` / type `1288` Technical enemy vehicle #6 (`101288`) / ai `G_Jeep`; node `1846`, area `0`, dist `3.5`<br>item `206` / id `7` / type `4204` Three layer wooden guard tower (`104204`); node `93`, area `0`, dist `5.8` |
| `20` | item `20` / id `4487` / type `2044` Power Up Med Pack Infinite (`102044`); node `1731`, area `0`, dist `449.7` |
| `63` | item `63` / id `2808` / type `1632` Single placeable radio alternative (`101632`) / group `20`; node `3192`, area `0`, dist `3.8` |

**Referenced Items**

| Ref | Candidates |
| ---: | --- |
| `2` | item `2` / id `1310` / type `1272` Blackhawk, miniguns, both doors open (`101272`) / ai `h_bhawk` / team `1` / group `63`; node `1876`, area `0`, dist `1102.8`<br>item `209` / id `2` / type `4204` Three layer wooden guard tower (`104204`); node `1270`, area `0`, dist `6.0` |
| `4` | item `4` / id `2357` / type `1286` / ai `gu_s` / group `50`; node `1731`, area `0`, dist `460.6`<br>item `211` / id `4` / type `4209` Small steel hangar with rounded roof (`104209`); node `1210`, area `0`, dist `1.6` |
| `5` | item `5` / id `2358` / type `1286` / ai `gu_s` / group `51`; node `1731`, area `0`, dist `470.2`<br>item `212` / id `5` / type `4209` Small steel hangar with rounded roof (`104209`); node `2522`, area `0`, dist `2.6` |
| `7` | item `7` / id `4441` / type `1288` Technical enemy vehicle #6 (`101288`) / ai `G_Jeep`; node `1846`, area `0`, dist `3.5`<br>item `206` / id `7` / type `4204` Three layer wooden guard tower (`104204`); node `93`, area `0`, dist `5.8` |
| `15` | item `15` / id `4430` / type `1902` 50cal on 180 tripod (`101902`); node `94`, area `0`, dist `9.9` |
| `20` | item `20` / id `4487` / type `2044` Power Up Med Pack Infinite (`102044`); node `1731`, area `0`, dist `449.7` |

**Trigger Waypoints**

| Ref | Candidates |
| ---: | --- |
| `7` | item `1217` / wp `7` / id `4521` / type `6005` waypoint (`106005`)<br>item `1241` / wp `7` / id `4520` / type `6005` waypoint (`106005`)<br>item `1259` / wp `7` / id `4519` / type `6005` waypoint (`106005`)<br>item `1286` / wp `7` / id `4518` / type `6005` waypoint (`106005`)<br>+4 more |
| `20` | item `1213` / wp `20` / id `2936` / type `6005` waypoint (`106005`)<br>item `1248` / wp `20` / id `2937` / type `6005` waypoint (`106005`)<br>item `1261` / wp `20` / id `2938` / type `6005` waypoint (`106005`)<br>item `1277` / wp `20` / id `2939` / type `6005` waypoint (`106005`)<br>+4 more |

### Event 42 - AINODEPATH_ON

- Event block line: `1203`
- AINODEPATH action line(s): `1210`

**Trigger Items**

| Ref | Candidates |
| ---: | --- |
| `7` | item `7` / id `4441` / type `1288` Technical enemy vehicle #6 (`101288`) / ai `G_Jeep`; node `1846`, area `0`, dist `3.5`<br>item `206` / id `7` / type `4204` Three layer wooden guard tower (`104204`); node `93`, area `0`, dist `5.8` |
| `8` | item `8` / id `4681` / type `1493` Small fishing boat type #2 (`101493`) / ai `wu`; node `1874`, area `0`, dist `862.8` |
| `14` | item `14` / id `2810` / type `1902` 50cal on 180 tripod (`101902`); node `3193`, area `0`, dist `2.6` |
| `50` | item `50` / id `2917` / type `1435` Metal 50gal Drum (`101435`); node `1163`, area `0`, dist `2.9` |

**Referenced Items**

| Ref | Candidates |
| ---: | --- |
| `5` | item `5` / id `2358` / type `1286` / ai `gu_s` / group `51`; node `1731`, area `0`, dist `470.2`<br>item `212` / id `5` / type `4209` Small steel hangar with rounded roof (`104209`); node `2522`, area `0`, dist `2.6` |
| `6` | item `6` / id `4440` / type `1288` Technical enemy vehicle #6 (`101288`) / ai `G_Jeep`; node `1265`, area `0`, dist `4.1` |
| `7` | item `7` / id `4441` / type `1288` Technical enemy vehicle #6 (`101288`) / ai `G_Jeep`; node `1846`, area `0`, dist `3.5`<br>item `206` / id `7` / type `4204` Three layer wooden guard tower (`104204`); node `93`, area `0`, dist `5.8` |
| `8` | item `8` / id `4681` / type `1493` Small fishing boat type #2 (`101493`) / ai `wu`; node `1874`, area `0`, dist `862.8` |
| `14` | item `14` / id `2810` / type `1902` 50cal on 180 tripod (`101902`); node `3193`, area `0`, dist `2.6` |
| `15` | item `15` / id `4430` / type `1902` 50cal on 180 tripod (`101902`); node `94`, area `0`, dist `9.9` |

**Trigger Waypoints**

| Ref | Candidates |
| ---: | --- |
| `7` | item `1217` / wp `7` / id `4521` / type `6005` waypoint (`106005`)<br>item `1241` / wp `7` / id `4520` / type `6005` waypoint (`106005`)<br>item `1259` / wp `7` / id `4519` / type `6005` waypoint (`106005`)<br>item `1286` / wp `7` / id `4518` / type `6005` waypoint (`106005`)<br>+4 more |
| `8` | item `1212` / wp `8` / id `1917` / type `6005` waypoint (`106005`)<br>item `1234` / wp `8` / id `1918` / type `6005` waypoint (`106005`)<br>item `1256` / wp `8` / id `1919` / type `6005` waypoint (`106005`)<br>item `1280` / wp `8` / id `1920` / type `6005` waypoint (`106005`)<br>+2 more |
| `14` | item `1219` / wp `14` / id `1934` / type `6005` waypoint (`106005`)<br>item `1250` / wp `14` / id `1935` / type `6005` waypoint (`106005`)<br>item `1269` / wp `14` / id `1936` / type `6005` waypoint (`106005`)<br>item `1282` / wp `14` / id `1937` / type `6005` waypoint (`106005`)<br>+4 more |


## Spatial Notes

| Check | Result |
| --- | --- |
| AI item coverage | `61 / 89` AI-positioned items are inside the AIN XY bounds. |
| Positioned item coverage | `571 / 1589` positioned MIS items are inside the AIN XY bounds. |
| AI nearest-node distance | min `1.4`, median `8.9`, max `1102.8`. |
| Area coverage | `1` `AreaId` values used; dominant areas: `[(0, 3251)]`. |
| Special node classes | `{}`. |
| Nonzero edge flags | `{'0x00': 21289}`. |

### Outside AIN Bounds

| Item |
| --- |
| item `1` / id `4597` / type `1239` Technical enemy vehicle with mounted 50cal (`101239`) / ai `G_Jeep` / team `2` / group `28` |
| item `2` / id `1310` / type `1272` Blackhawk, miniguns, both doors open (`101272`) / ai `h_bhawk` / team `1` / group `63` |
| item `3` / id `1912` / type `1272` Blackhawk, miniguns, both doors open (`101272`) / ai `H_BHawk` / team `1` / group `62` |
| item `4` / id `2357` / type `1286` / ai `gu_s` / group `50` |
| item `5` / id `2358` / type `1286` / ai `gu_s` / group `51` |
| item `8` / id `4681` / type `1493` Small fishing boat type #2 (`101493`) / ai `wu` |
| item `9` / id `4680` / type `1494` Small fishing boat type #3 (`101494`) / ai `wu` |
| item `11` / id `4679` / type `1881` 50cal on 360 tripod (`101881`) |

### Farthest AI Items From AIN Nodes

| Item | Nearest Node | Area | Distance |
| --- | ---: | ---: | ---: |
| item `2` / id `1310` / type `1272` Blackhawk, miniguns, both doors open (`101272`) / ai `h_bhawk` / team `1` / group `63` | `1876` | `0` | `1102.8` |
| item `869` / id `4515` / type `6197` Tropical Tree Grouping 03 No ferns (`106197`) / ai `null` | `1951` | `0` | `1101.1` |
| item `1104` / id `4656` / type `6198` Tropical Tree Grouping 04 No ferns (`106198`) / ai `null` | `1951` | `0` | `1091.6` |
| item `3` / id `1912` / type `1272` Blackhawk, miniguns, both doors open (`101272`) / ai `H_BHawk` / team `1` / group `62` | `1876` | `0` | `1089.0` |
| item `1103` / id `4655` / type `6198` Tropical Tree Grouping 04 No ferns (`106198`) / ai `null` | `1951` | `0` | `1060.8` |

### Special Class Nodes

| Node | Class | Area | Flags | Nearest MIS Item | Distance |
| ---: | ---: | ---: | --- | --- | ---: |
| | | | | | |

### Nonzero Edge Flags

| Flag | Source | Target | Areas | Classes | Reverse | Distance |
| --- | ---: | ---: | --- | --- | --- | ---: |
| | | | | | | |
