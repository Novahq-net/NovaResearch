# NovaLogic AIN File Format (BHD/TS)

Visit [https://novahq.net](https://novahq.net) for more information on NovaLogic file formats and tools to work with these files.

## Mission Index

[AIN Mission Index](AIN%20Mission%20Index.md) provides a detailed index of AIN node and area counts for each mission in Black Hawk Down and Team Sabre. 

## Overview

`.AIN` files store mission navigation graphs used by AI pathing. A file contains a short header, a fixed-size array of AI node records, and an area state table. All multi-byte integer fields are little-endian.

## File Layout

| Offset | Size | Field | Type | Description |
| ---: | ---: | --- | --- | --- |
| `0x00` | `4` | `Magic` | char[4] | File Magic `NAI2`. |
| `0x04` | `4` | `NodeCount` | uint32 | Number of AI node records. |
| `0x08` | `NodeCount * 52` | `Nodes` | AinNode[] | AI navigation node array. |
| `0x08 + NodeCount * 52` | `4` | `AreaCount` | uint32 | Always `256` area state records. |
| `0x0C + NodeCount * 52` | `AreaCount * 12` | `AreaStates` | AreaState[] | Area/room state table. |

## Header

| Offset | Field | Type | Description |
| ---: | --- | --- | --- |
| `0x00` | `Magic` | char[4] | `NAI2` |
| `0x04` | `NodeCount` | uint32 | Number of 52-byte records in the node table. |

## Node Table

Node offset: `0x08 + NodeIndex * 52`

| Offset | Size | Field | Type | Description |
| ---: | ---: | --- | --- | --- |
| `0x00` | `4` | `X` | int32 | World/navigation X coordinate. |
| `0x04` | `4` | `Y` | int32 | World/navigation Y coordinate. |
| `0x08` | `4` | `Z` | int32 | World/navigation Z coordinate. |
| `0x0C` | `1` | `NodeFlags` | uint8 | Node behavior flags. |
| `0x0D` | `1` | `NodeClass` | uint8 | Node class/type. |
| `0x0E` | `1` | `AreaId` | uint8 | Primary area/room/sector id. |
| `0x0F` | `1` | `Radius` | uint8 | Node acceptance/search radius. |
| `0x10` | `1` | `DirectionSectors` | uint8 | Packed directional gate. |
| `0x11` | `1` | `SecondaryAreaId` | uint8 | Secondary/linked area id. |
| `0x12` | `1` | `RuntimeOccupancy` | uint8 | Runtime occupancy/reservation byte. Always `0`. |
| `0x13` | `1` | `LinkCount` | uint8 | Number of active neighbor links, maximum `10`. |
| `0x14` | `20` | `NeighborIndex` | uint16[10] | Neighbor node indices. Only entries below `LinkCount` are active. |
| `0x28` | `10` | `EdgeFlags` | uint8[10] | Per-link edge flags aligned with `NeighborIndex`. |
| `0x32` | `2` | `Unknown` | uint16 | Preserved authoring value. No confirmed runtime consumer. |

## Node Flags

| Bit | Name | Description |
| ---: | --- | --- |
| `0x01` | `NoRouteShortcut` | Marks nodes that should not be bypassed by route shortcutting. |
| `0x02` | `ReverseDirectionAllowed` | Allows the opposite direction sector to pass directional checks. |
| `0x04` | `AreaList0Member` | Adds the node to an area-indexed runtime list family. |
| `0x08` | `AreaList1Member` | Adds the node to a second area-indexed runtime list family. |
| `0x10` | `AreaList2Member` | Adds the node to a third area-indexed runtime list family. |
| `0x40` | `Unknown40` | Unknown |
| `0x80` | `RuntimeTaskMark` | Runtime/task marker. |

## Node Class

| Value | Name | Description |
| ---: | --- | --- |
| `0` | `Default` | Standard navigation node. |
| `1` | `Unknown` | Unknown |
| `2` | `AreaTransition` | Uses `SecondaryAreaId` for linked area behavior. |
| `6` | `Class6AreaNode` | Special area-indexed node class. |
| `7` | `Class7AreaNode` | Special area-indexed node class. |
| `8` | `Class8AreaNode` | Special area-indexed node class. |
| `9` | `Class9AreaNode` | Special area-indexed node class. |

## DirectionSectors

`DirectionSectors` packs two 4-bit direction sector values into one byte.

| Bits | Field | Description |
| --- | --- | --- |
| `0xF0` | `DirectionSectorA` | High-nibble sector value. |
| `0x0F` | `DirectionSectorB` | Low-nibble sector value. |

Sector values range from `0` to `15` around the horizontal plane. A value of `0x00` means no directional gate is applied.

## Neighbor Links

Each node has space for ten neighbor links.

| Field | Description |
| --- | --- |
| `LinkCount` | Number of active link slots. Valid range is `0..10`. |
| `NeighborIndex[i]` | Target node index for link slot `i`. |
| `EdgeFlags[i]` | Edge behavior flags for link slot `i`. |

Only slots where `i < LinkCount` are active. Unused `NeighborIndex` and `EdgeFlags` slots can contain nonzero data and should be preserved.

## EdgeFlags

| Bit / Value | Name | Description |
| ---: | --- | --- |
| `0x00` | `Normal` | Standard link. |
| `0x01` | `SpecialTraversal` | Marks a link requiring special traversal behavior. |
| `0x08` | `NoShortcut` | Prevents shortcutting across the edge and marks special movement behavior. |
| `0x10` | `Unknown10` | Unknown |
| `0x20` | `Unknown20` | Unknown |
| `0x30` | `Unknown10_20` | Combined `Unknown10` / `Unknown20` flags. |

## Area State Table

The area state table follows the node records.

| Offset From Table | Size | Field | Type | Description |
| ---: | ---: | --- | --- | --- |
| `0x00` | `4` | `AreaCount` | uint32 | Number of area state records. Always `256`. |
| `0x04` | `AreaCount * 12` | `AreaStates` | AreaState[] | Area state records. |

## Area Entry

| Offset | Size | Field | Type | Description |
| ---: | ---: | --- | --- | --- |
| `0x00` | `4` | `AreaFlags` | int32 | Area/room state flags. |
| `0x04` | `4` | `Unknown4` | int32 | Always `0`. |
| `0x08` | `4` | `Unknown8` | int32 | Always `0`. |

## Area Flags

| Bit | Name | Description |
| ---: | --- | --- |
| `0x01` | `AreaBoundaryModifier` | Area movement/state modifier. |
| `0x02` | `SecondaryAreaTaskEligible` | Marks a secondary area as eligible for task behavior. |
| `0x04` | `SecondaryAreaTaskRequested` | Runtime/requested task state. |
| `0x08` | `SecondaryAreaTaskActive` | Runtime/active task state. |
| `0x10` | `AttackRoomTaskActive` | Runtime/attack-room task state. |
