# Tachyon: The Fringe DISP02.SPX - Weasel in the Coop; Crystal Hunt

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `DISP02.SPX` |
| Sector | `QUAD_02` |
| Backdrop | `DISPUT2.BDF` |
| Region | 6 |
| Sector ID | 1 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 5 |
| Entities | 56 |
| Events | 4 |
| Waypoints | 0 |
| Child Sectors | 6 |
| Scripts | 1 |
| Scenes | 2 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Roid_Sm_Brown2`, `1: Spcargo_Mining`, `2: Spcargo_Medical`, `3: Ripstar`, `4: Hyper_Gate` |
| Scripts | `PLAYER.SCR` |
| Scenes | `D2BC090A.SEN`, `D4BC080A.SEN` |
| Labels | `BFGE_03`, `BFGF_03`, `MERC_17`, `BFNE_01`, `CLEON`, `Patrol1`, `Patrol2`, `SPIKE`, `Redemption` |
| Aliases | `BC10_Claymore1`, `BC10_Claymore2`, `BC10_Claymore3`, `BC10_Claymore4`, `Coward`, `BC10_Waraxe`, `BC10_Mace1`, `BC10_Mace2`, `BC10_Mace3`, `BC10_Mace4`, `BC10_Warhammer1`, `BC10_Warhammer2`, `BC10_Warhammer3`, `BC10_Warhammer4`, `SPIKE`, `Stocks01` |
| Groups | `CONT_002`, `CONT_027` |
| Child Sectors | [disp02A.spx](DISP02A.md), [disp02B.spx](DISP02B.md), [disp02C.spx](DISP02C.md), [disp02D.spx](DISP02D.md), [disp02E.spx](DISP02E.md), [disp02F.spx](DISP02F.md) |

## Events

### Event 0

**Trigger**

- Variable comparison: subject variable group 0, variable 0, op 1, value 2

**Action**

- Object spawn/action: Spcargo_Medical (object 32, id 1920), subtype 0

### Event 1

**Trigger**

- Variable comparison: subject variable group 0, variable 0, op 1, value 1

**Action**

- Object spawn/action: Spcargo_Mining (object 33, id 1921), subtype 0

### Event 2

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 1920; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 185
- Set/add variable: variable group 18, variable 802, subtype 0, value 1

### Event 3

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 7, value 0 (extra 1, 1921; flags 2)

**Action**

- Play dialog: PLAYER.SCR, line/variant 185
- Set/add variable: variable group 18, variable 803, subtype 0, value 1

## Waypoints

None
## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | -1975.61,0.00,2490.06 | 215,0,0 | Gate SPX: [disp01.spx](DISP01.md) |
| 1 | `Hyper_Gate` | 2 | Gate | 2237.20,0.00,-4805.56 | 464,0,0 | Gate SPX: [disp03.spx](DISP03.md) |
| 2 | `Ripstar` | 1809 | Interactive | -2239.55,-105.00,1289.11 | 0,0,0 | None |
| 3 | `Ripstar` | 1810 | Interactive | -2250.62,105.00,727.97 | 0,0,0 | None |
| 4 | `Ripstar` | 1811 | Interactive | -2596.72,68.00,268.52 | 0,0,0 | None |
| 5 | `Ripstar` | 1812 | Interactive | -2943.57,0.00,-185.53 | 0,0,0 | None |
| 6 | `Ripstar` | 1813 | Interactive | -2372.94,46.00,-616.17 | 0,0,0 | None |
| 7 | `Ripstar` | 1814 | Interactive | 492.51,-123.00,1393.51 | 0,0,0 | None |
| 8 | `Ripstar` | 1815 | Interactive | 1192.59,171.00,845.41 | 0,0,0 | None |
| 9 | `Ripstar` | 1816 | Interactive | 1249.70,231.00,23.27 | 0,0,0 | None |
| 10 | `Ripstar` | 1817 | Interactive | 867.60,141.00,-342.13 | 0,0,0 | None |
| 11 | `Ripstar` | 1818 | Interactive | 1532.51,112.00,-1777.61 | 0,0,0 | None |
| 12 | `Ripstar` | 1819 | Interactive | -2255.91,62.00,-1986.41 | 0,0,0 | None |
| 13 | `Ripstar` | 1820 | Interactive | 2076.18,30.00,-5888.74 | 0,0,0 | None |
| 14 | `Ripstar` | 1821 | Interactive | 2002.82,21.00,-5934.49 | 0,0,0 | None |
| 15 | `Ripstar` | 1822 | Interactive | -1642.71,51.00,-1738.46 | 0,0,0 | None |
| 16 | `Ripstar` | 1823 | Interactive | -1442.26,111.00,1028.11 | 0,0,0 | None |
| 17 | `Ripstar` | 1824 | Interactive | 173.15,65.00,-447.20 | 0,0,0 | None |
| 18 | `Ripstar` | 1825 | Interactive | 126.52,-42.00,-2808.56 | 0,0,0 | None |
| 19 | `Ripstar` | 1826 | Interactive | -822.17,70.00,-2599.76 | 0,0,0 | None |
| 20 | `Ripstar` | 1827 | Interactive | -313.71,213.00,-2882.35 | 0,0,0 | None |
| 21 | `Ripstar` | 1828 | Interactive | -1842.58,-73.00,585.54 | 0,0,0 | None |
| 22 | `Ripstar` | 1829 | Interactive | 319.98,135.00,466.97 | 0,0,0 | None |
| 23 | `Ripstar` | 1830 | Interactive | -496.39,-116.00,1432.66 | 0,0,0 | None |
| 24 | `Ripstar` | 1831 | Interactive | -479.36,48.00,323.42 | 0,0,0 | None |
| 25 | `Ripstar` | 1832 | Interactive | -625.93,0.00,-2006.44 | 0,0,0 | None |
| 26 | `Ripstar` | 1833 | Interactive | -1473.26,168.00,-942.42 | 0,0,0 | None |
| 27 | `Ripstar` | 1834 | Interactive | 880.81,93.00,-1020.72 | 0,0,0 | None |
| 28 | `Ripstar` | 1835 | Interactive | -527.42,0.00,-280.87 | 0,0,0 | None |
| 29 | `Ripstar` | 1836 | Interactive | -3018.67,0.00,-1212.55 | 0,0,0 | None |
| 30 | `Ripstar` | 1837 | Interactive | 1687.12,86.00,-2713.29 | 0,0,0 | None |
| 31 | `Ripstar` | 1838 | Interactive | 2018.78,68.00,-5842.38 | 0,0,0 | None |
| 32 | `Spcargo_Medical` | 1920 | Interactive | -1836.74,58.38,-2568.68 | 0,0,0 | secondary groups: CONT_002, none |
| 33 | `Spcargo_Mining` | 1921 | Interactive | -2548.50,63.14,-1079.72 | 119,262,6 | secondary groups: CONT_027, none |
| 34 | `Roid_Sm_Brown2` | 1840 | Object | -399.96,68.00,1341.31 | 0,0,0 | Scale/Radius: 1.00 |
| 35 | `Roid_Sm_Brown2` | 1839 | Object | -2134.02,130.00,1263.01 | 0,0,0 | Scale/Radius: 1.00 |
| 36 | `Roid_Sm_Brown2` | 1841 | Object | -425.89,76.00,258.17 | 0,0,0 | Scale/Radius: 1.00 |
| 37 | `Roid_Sm_Brown2` | 1842 | Object | -1844.43,64.00,507.24 | 0,0,0 | Scale/Radius: 1.00 |
| 38 | `Roid_Sm_Brown2` | 1843 | Object | -1783.29,58.00,689.94 | 0,0,0 | Scale/Radius: 1.00 |
| 39 | `Roid_Sm_Brown2` | 1844 | Object | -2576.36,63.00,-1072.92 | 0,0,0 | Scale/Radius: 1.00 |
| 40 | `Roid_Sm_Brown2` | 1845 | Object | -2453.97,-56.00,-1164.27 | 0,0,0 | Scale/Radius: 1.00 |
| 41 | `Roid_Sm_Brown2` | 1846 | Object | -2337.79,68.00,-981.57 | 0,0,0 | Scale/Radius: 1.00 |
| 42 | `Roid_Sm_Brown2` | 1847 | Object | 643.11,70.00,-1242.57 | 0,0,0 | Scale/Radius: 1.00 |
| 43 | `Roid_Sm_Brown2` | 1848 | Object | 405.75,57.00,-515.83 | 0,0,0 | Scale/Radius: 1.00 |
| 44 | `Roid_Sm_Brown2` | 1849 | Object | 797.36,72.00,-1425.27 | 0,0,0 | Scale/Radius: 1.00 |
| 45 | `Roid_Sm_Brown2` | 1850 | Object | -1178.22,0.00,-1634.07 | 0,0,0 | Scale/Radius: 1.00 |
| 46 | `Roid_Sm_Brown2` | 1851 | Object | -1158.19,54.00,-1921.16 | 0,0,0 | Scale/Radius: 1.00 |
| 47 | `Roid_Sm_Brown2` | 1852 | Object | -973.62,0.00,-1764.56 | 0,0,0 | Scale/Radius: 1.00 |
| 48 | `Roid_Sm_Brown2` | 1853 | Object | -1908.38,43.00,-2547.56 | 0,0,0 | Scale/Radius: 1.00 |
| 49 | `Roid_Sm_Brown2` | 1854 | Object | -1749.92,90.00,-2547.56 | 0,0,0 | Scale/Radius: 1.00 |
| 50 | `Roid_Sm_Brown2` | 1855 | Object | -1864.20,-28.00,-2834.66 | 0,0,0 | Scale/Radius: 1.00 |
| 51 | `Roid_Sm_Brown2` | 1856 | Object | 207.25,0.00,-3515.51 | 0,0,0 | Scale/Radius: 1.00 |
| 52 | `Roid_Sm_Brown2` | 1857 | Object | 368.71,77.00,-3463.31 | 0,0,0 | Scale/Radius: 1.00 |
| 53 | `Roid_Sm_Brown2` | 1858 | Object | 415.07,-63.00,-3254.52 | 0,0,0 | Scale/Radius: 1.00 |
| 54 | `Roid_Sm_Brown2` | 1859 | Object | 219.29,0.00,-3228.42 | 0,0,0 | Scale/Radius: 1.00 |
| 55 | `Roid_Sm_Brown2` | 1860 | Object | -1346.72,76.00,649.67 | 0,0,0 | Scale/Radius: 1.00 |
