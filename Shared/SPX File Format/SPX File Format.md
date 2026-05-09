# NovaLogic SPX File Format (Tachyon: The Fringe Mission File)

Visit [https://novahq.net](https://novahq.net) for more information on NovaLogic file formats and tools to work with these files.

## SPX Mission Index

[SPX Mission Index](SPX%20Mission%20Index.md) links to each SPX file's individual page, which includes a summary of the file's properties and resources, as well as lists of objects, waypoints, events and other data parsed from the file. 

## File Overview

`.SPX` files are mission files used by Tachyon: The Fringe. They contain placed objects, waypoints, events, scripts, references to child sectors and other mission-related data. They are used for both single-player and multi-player game modes. Single-player missions are attached to JOB files, while multi-player maps are attached to MPC files.

SPX files have a somewhat convoluted loading process that seems to chain multiple SPX files together. I believe they are used to create "Sector" or "Warp/Gate" zones. It was nearly impossible to map out the exact relationship with a debugger so most of the analysis was done by statically parsing the files and making assumptions based on links between files and the types of objects/events found in each related file.

Field descriptions in this document may be incomplete or inaccurate. Some of this information was assumed based on mission types from other NovaLogic games. If you have information to contribute, please submit a pull request or open an issue.

## File Layout

```
  Header
    CoreHeader
    SectorName
    ScriptList
    SenList
    LabelList
    BdfFilename
    WaypointList
    SpawnList                     optional
    AliasNameList                 optional
    RegionId / SectorId
    Groups                        optional
  ObjectTypes[]                     36-byte object records
  ChildSpxRefs[]                    44-byte child .spx reference records; may be empty
  ScriptNames[]                     fixed-width .SCR script names; may be empty
  SenNames[]                        fixed-width .SEN scene/conversation names; may be empty
  Labels[]                          fixed-width mission/script labels; may be empty
  Events[]                          20-byte event list headers
    ConditionRecords[]              40-byte condition records
    ActionRecords[]                 16-byte action records
  ObjectRecords[]                   variable-size object records
  Waypoints[]                       optional waypoints headers
    Points[]                        32-byte waypoints point records
  SpawnLists[]                      optional variable-size spawn-list/group seed records
    SpawnListEntries[]              optional 28-byte spawn rule records
  AliasNames[]                      optional 32-byte AI alias names
  Groups[]                          optional 32-byte group/contact/base names
```

## Header

Headers are variable in size. `DataStartOffset` at `0x00` gives the start of the first payload array.

| Offset | Field | Type | Description |
| ---: | --- | --- | --- |
| `0x00` | `DataStartOffset` | uint32 | Offset to `ObjectTypes` |
| `0x04` | `Magic` | char[4] | File magic `SPD\x01` |
| `0x08` | `HeaderDescriptorSize` | uint32 | Always `0x24` |
| `0x0C` | `ObjectTypeCount` | uint32 | Number of `ObjectTypes` |
| `0x10` | `ObjectTypeOffset` | uint32 | Offset to `ObjectTypes` |
| `0x14` | `ObjectCount` | uint32 | Number of `ObjectRecords` |
| `0x18` | `ObjectOffset` | uint32 | Offset to `ObjectRecords` |
| `0x1C` | `ObjectHeaderSize` | uint32 | Always `20` |
| `0x20` | `EventCount` | uint32 | Number of `Events` |
| `0x24` | `EventOffset` | uint32 | Offset to `Events` |
| `0x28` | `ChildSpxRefSize` | uint32 | Always `44` |
| `0x2C` | `ChildSpxCount` | uint32 | Number of `ChildSpxRefs` |
| `0x30` | `ChildSpxOffset` | uint32 | Offset to `ChildSpxRefs` |
| `0x34` | `SectorName` | char[32] | Sector/quad tag, ie `QUAD_01` |
| `0x54` | `ScriptNames` | ListItem<char[16]> | `.SCR` script list |
| `0x60` | `SenNames` | ListItem<char[16]> | `.SEN` scene list |
| `0x6C` | `Labels` | ListItem<char[32]> | 32-byte label list |
| `0x78` | `BdfFilename` | char[16] | `.BDF` file name |
| `0x88` | `SectorHazardFlags` | uint32 | `0x00` = None, `0x01` = Rad, `0x02` = Fog, `0x03` = Rad+Fog |
| `0x8C` | `WaypointCount` | uint32 | Number of `Waypoints` |
| `0x90` | `WaypointOffset` | uint32 | Offset to `Waypoints` |
| `0x94..0x9C` | `Padding` | uint32[3] | Unused/Reserved |
| `0xA0` | `Type2ObjectCount` | uint32 | Number of `ObjectRecords` where `ObjectType == 2` |
| `0xA4` | `Unknown` | uint32 | Unknown |
| `0xA8..0xE4` | `Padding` | uint32[16] | Unused/Reserved |
| `0xE8` | `SpawnListCount` | uint32 | Number of `SpawnLists` |
| `0xEC` | `SpawnListOffset` | uint32 | Offset to `SpawnLists` |
| `0xF0` | `AliasNameEntrySize` | uint32 | Always `32` |
| `0xF4` | `AliasNameCount` | uint32 | Number of `AliasNames` |
| `0xF8` | `AliasNameOffset` | uint32 | Offset to `AliasNames` |
| `0xFC` | `RegionId` | uint32 | Sector registry region id |
| `0x100` | `SectorId` | uint32 | Sector registry sector id |
| `0x104` | `GroupEntrySize` | uint32 | `32` when group table is present |
| `0x108` | `GroupCount` | uint32 | Number of `Groups` |
| `0x10C` | `GroupOffset` | uint32 | Offset to `Groups` |
| `0x110` | `ReservedMinusOne` | uint32 | Always `0xFFFFFFFF` when present |
| `0x114` | `Padding` | uint32 | Unused/Reserved |
| `0x118` | `BWBaseSector` | uint32 | `0` = None, `1` = Bora, `2` = GalSpan |
| `0x11C` | `BWBaseSectorRace` | uint32 | `0` = AGT/None, `1` = Bora, `2` = GalSpan |
| `0x120..0x19C` | `Padding` | uint32[32] | Unused/Reserved |
| `0x1A0` | `Unknown` | uint32 | Runtime Use |

## ListItem

| Offset | Field | Type | Description |
| :---: | --- | --- | --- |
| `0x00` | `EntrySize` | uint32 | List entry size |
| `0x04` | `Count` | uint32 | Number of list entries |
| `0x08` | `Offset` | uint32 | Offset to list entries |

## Object Types

Object type records name the object used by `ObjectRecords`

| Offset | Size | Field | Type | Description |
| :---: | :---: | --- | --- | --- |
| `0x00` | `32` | `Name` | char[32] | Null-terminated object name |
| `0x20` | `4` | `Reserved` | uint32 | Reserved |

## Child SPX References

| Offset | Size | Field | Type | Description |
| :---: | :---: | --- | --- | --- |
| `0x00` | `32` | `Filename` | char[32] | Child `.spx` file name |
| `0x20` | `4` | `Unknown0` | uint32 | Unknown |
| `0x24` | `4` | `Unknown1` | uint32 | Unknown |
| `0x28` | `4` | `Unknown2` | uint32 | Unknown |

### Events

| Offset | Size | Field | Type | Description |
| :---: | :---: | --- | --- | --- |
| `0x00` | `4` | `ConditionCount` | uint32 | Number of conditions |
| `0x04` | `4` | `ActionCount` | uint32 | Number of actions |
| `0x08` | `4` | `StateOrCache` | uint32 | Runtime state |
| `0x0C` | `4` | `ConditionArrayOffset` | uint32 | Offset to conditions |
| `0x10` | `4` | `ActionArrayOffset` | uint32 | Offset to actions |

### Event Conditions

| Offset | Size | Field | Type | Description |
| :---: | :---: | --- | --- | --- |
| `0x00` | `4` | `ConditionType` | int32 | Condition Type |
| `0x04` | `4` | `ConditionSubject` | int32 | Object id, variable id, group id, or condition-specific subject |
| `0x08` | `4` | `ConditionFlags` | int32 | Condition-specific flags |
| `0x0C` | `4` | `Param0` | int32 | Param0 |
| `0x10` | `4` | `Param1` | int32 | Param1 |
| `0x14` | `4` | `Param2` | int32 | Param2 |
| `0x18` | `4` | `BooleanJoin` | int32 | Condition join value |
| `0x1C` | `4` | `Flags` | int32 | Runtime Flags |
| `0x20` | `4` | `CachedResult` | int32 | Runtime cache field |
| `0x24` | `4` | `LastTriggerTick` | int32 | Runtime cache field |

### Event Actions

| Offset | Size | Field | Type | Description |
| :---: | :---: | --- | --- | --- |
| `0x00` | `4` | `ActionType` | int32 | Action Type |
| `0x04` | `4` | `Param0` | int32 | Object id, variable id, script index, group id, or type-specific value |
| `0x08` | `4` | `ActionSubtype` | int32 | Type-specific subtype |
| `0x0C` | `4` | `Param1` | int32 | Type-specific value |

## Object Record

Every object starts with a 20-byte common header. The high 16 bits of `PackedSizeType` store the full record size, the low 16 bits store the object type.

| Offset | Size | Field | Type | Description |
| :---: | :---: | --- | --- | --- |
| `0x00` | `4` | `PackedSizeType` | uint32 | `(RecordSize << 16) \| ObjectType` |
| `0x04` | `4` | `ObjectTypeIndex` | int32 | Index into `ObjectTypes`. Can be `-1` |
| `0x08` | `4` | `X` | int32 | 16.16 fixed-point X coordinate |
| `0x0C` | `4` | `Y` | int32 | 16.16 fixed-point Y coordinate |
| `0x10` | `4` | `Z` | int32 | 16.16 fixed-point Z coordinate |
| `0x14` | `RecordSize - 20` | `Payload` | byte[] | Type-specific object data |

## Object Types

| Value | Name | Notes |
| :---: | --- | --- |
| `0` | Special marker | Special object |
| `1` | Sector gate | SPX name |
| `2` | Placed object | Common static object |
| `3` | Interactive object | Larger object record with ids, flags, labels, waypoints, etc. |
| `4` | Variant placed object | Variant object |

## Spawn Flags

| Bit | Name |
| :---: | --- |
| `0x0001` | `PlayerStartShip` |
| `0x0002` | `UsePrimaryObjectSet` |
| `0x0004` | `UseSecondaryObjectSet` |
| `0x0008` | `StartUnspawned/deferred` |
| `0x0010` | `StartInactive/no normal AI` |
| `0x0020` | `SilentWaypointAttach/no initial event` |
| `0x0040` | `CopyRuntimeFlag40` |
| `0x0080` | `HasContents/cargo` |
| `0x0200` | `DistanceEventEmitter` |
| `0x0400` | `CopyRuntimeStateFlag20?` |
| `0x0800` | `GateObjectIdLookup` |
| `0x1000` | `WingmanStartMarker` |

### Waypoint

| Offset | Size | Field | Type | Description |
| :---: | :---: | --- | --- | --- |
| `0x00` | `4` | `PointCount` | uint32 | Number of waypoints |
| `0x04` | `4` | `PointOffset` | uint32 | Offset to entries |
| `0x08` | `4` | `WaypointTag` | int32 | Tag used by waypoint event values |
| `0x0C` | `4` | `Reserved0` | uint32 | Always `0` |
| `0x10` | `4` | `Reserved1` | uint32 | Always `0` |

### Waypoint Point

Waypoint coordinates are stored as 16.16 fixed-point values.

| Offset | Size | Field | Type | Description |
| :---: | :---: | --- | --- | --- |
| `0x00` | `4` | `X` | int32 | X coordinate |
| `0x04` | `4` | `Y` | int32 | Y coordinate |
| `0x08` | `4` | `Z` | int32 | Z coordinate |
| `0x0C` | `4` | `OnArrivalAction` | int32 | Action ID when point reached. `-1` = none |
| `0x10` | `4` | `OnArrivalParam` | int32 | Action param |
| `0x14` | `4` | `Unknown0` | int32 | Unknown |
| `0x18` | `4` | `Unknown1` | int32 | Unknown |
| `0x1C` | `4` | `Unknown2` | int32 | Unknown |

## Spawn Lists

Spawn-list records are variable-size group seed/action tables used by mission events.

| Offset | Size | Field | Type | Description |
| :---: | :---: | --- | --- | --- |
| `0x00` | `4` | `EntrySize` | uint32 | Size of spawn-list record |
| `0x04` | `4` | `SubEntrySize` | uint32 | Size of each entry, always `28` |
| `0x08` | `4` | `SpawnListId` | int32 | Spawn-list/group id used by events |
| `0x0C` | `4` | `SubEntryCount` | uint32 | Number of entries |
| `0x10` | `4` | `SubEntryOffset` | uint32 | Offset to entries |
