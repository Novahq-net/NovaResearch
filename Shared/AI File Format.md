# NovaLogic AI File Format
Visit [https://novahq.net](https://novahq.net) for more information on NovaLogic file formats and tools to work with these files.  

This information was gathered from reverse engineering the formats statically and while loaded in-game. Some of the entries are best guesses based on behaviour after loading into the engine or inferred from the data. While researching, some of the fields were renamed or re-identified and may be inconsistent across versions. If you have any corrections or insights, please create an issue or submit a pull request. 

## AI Information
The `.AI` file is the top-level composition manifest used by `Armored Fist 3` and `Comanche 3 Gold` to combine several `.3DO` models into one single model.

## AI Structure
```
File (ASCII text)
  HeaderLine                      type number + status comment
  >G | >D | >S | >N               one block per environment variant
  >R | >B                         red / blue team item
  >IDOV                           internal id	
  >DATA                           per-entity numeric parameters
  >LEAF                           optional, vegetation / debris piece count
```

## AI Structure

### [Header]

| Field | Type | Description |
| --- | --- | --- |
| Comment | string | Model Info |
| Type | int | Entity type id |

---

### [Environment Block]

**Block markers:**

| Marker | Meaning |
| --- | --- |
| `>G` | Green |
| `>D` | Desert |
| `>S` | Snow |
| `>N` | Night |
| `>R` | Red team |
| `>B` | Blue team |

**Block contents:**

```
><env-marker>
<part_1.3DO>
<part_2.3DO>
...
<part_N.3DO>
```

Each line is a `.3DO` filename, see [3DO File Format](./3DO%20File%20Format.md). 

---

### [IDOV] Block
Size: `1 line`  

```
>IDOV
D###
```

| Field | Type | Description |
| --- | --- | --- |
| Identifier | string | A capital `D` followed by exactly 3 digits (e.g. `D060`, `D240`, `D591`). 

---

### [DATA] Block
Size: `5 lines`  

```
>DATA
15      ;CUTOFF DISTANCE IN METERS FOR MEDIUM RES
30      ;CUTOFF DISTANCE IN METERS FOR LOW RES
1       ;COLLIDABLE
1       ;CRUSHABLE
1       ;RUN ON TOPOFABLE
```

| Index | Field | Type | Description |
| --- | --- | --- | --- |
| 0 | MediumLodCutoff | int | Distance in meters at which the engine swaps to medium-detail LOD |
| 1 | LowLodCutoff | int | Distance in meters at which the engine swaps to low-detail LOD |
| 2 | Collidable | int | `0` or `1` whether other entities collide with this one |
| 3 | Crushable | int | `0` or `1` whether the entity can be destroyed by being run over |
| 4 | RunOnTopOfable | int | `0` or `1` whether other entities can drive on top of this one |

---

### [LEAF] Block
Size: `1 line`  
*Notes: Optional. For trees the value is the number of sprite instances the engine scatters around the trunk; for vehicle debris it is the number of debris pieces to use.*

```
>LEAF
<count>
```

| Field | Type | Description |
| --- | --- | --- |
| Count | int | Leaf-sprite or debris-piece count |
