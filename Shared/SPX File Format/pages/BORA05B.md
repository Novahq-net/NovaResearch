# Tachyon: The Fringe BORA05B.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `BORA05B.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `(none)` |
| Region | 3 |
| Sector ID | 4 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 12 |
| Entities | 324 |
| Events | 13 |
| Waypoints | 7 |
| Child Sectors | 0 |
| Scripts | 2 |
| Scenes | 0 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Bora_Carrier`, `1: GalSpan_Frigate`, `2: Bora_Claymore`, `3: Bora_Leviathan`, `4: Navigational_Bouy`, `5: Bora_Mace`, `6: Roid_Lrg_Grey`, `7: Asteroid_2`, `8: Bora_Mine`, `9: Roid_SM_Grey_Points`, `10: Roid_Sm_Grey`, `11: GalSpan_Orion` |
| Scripts | `PLAYER.SCR`, `BFORT.SCR` |
| Scenes | None |
| Labels | `bfbe_08`, `bfbf_08` |
| Aliases | None |
| Groups | `FG_ATHENE`, `FG_HONOR`, `FG_FORNAX`, `APUS`, `APHRODITE`, `FORTRESS` |
| Child Sectors | None |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 2, value 0

**Action**

- Object spawn/action: Navigational_Bouy (object 313, id 2139), subtype 14
- Show/update HUD contact: contact/list 0, subtype 9, param 14
- Play dialog: PLAYER.SCR, line/variant 31

### Event 1

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 1, value 3500 (extra 1, 1068; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 3500 (extra 1, 1069; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 3500 (extra 1, 1070; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 3500 (extra 1, 1071; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 3500 (extra 1, 1066; join 2; flags 2)
- Area/player/sector/dock/time event: subject 0, op 1, value 3500 (extra 1, 1067; join 2; flags 2)

**Action**

- Group/spawn-list action: spawn list/group 231, subtype 2
- Show/update HUD contact: contact/list 0, subtype 1, param 231
- Object spawn/action: Navigational_Bouy (object 313, id 2139), subtype 15
- Hide/remove HUD contact: contact/list 0, subtype 9, param 14
- Play dialog: PLAYER.SCR, line/variant 33

### Event 2

**Trigger**

- Group/spawn-list event: subject 231, op 0, value 0

**Action**

- Object spawn/action: Bora_Carrier (object 323, id 1864), subtype 3
- Set/add variable: variable group 15, variable 406, subtype 0, value 1
- Object spawn/action: GalSpan_Frigate (object 321, id 1066), subtype 5
- Object spawn/action: GalSpan_Frigate (object 322, id 1067), subtype 5
- Set/add variable: variable group 15, variable 407, subtype 0, value 2
- Show/update HUD contact: contact/list 0, subtype 8, param 0
- Play dialog: BFORT.SCR, line/variant 0
- Show/update HUD contact: contact/list 0, subtype 12, param 19

### Event 3

**Trigger**

- Object arrival: Bora_Carrier (object 323, id 1864) reached Waypoint 3 (tag 154), point 0 (raw value 10092544)

**Action**

- Group/spawn-list action: spawn list/group 106, subtype 1, param 1864
- Group/spawn-list action: spawn list/group 178, subtype 1, param 1864

### Event 4

**Trigger**

- Object event: subject GalSpan_Frigate (object 321, id 1066), op 2, value 0 (join 2)
- Object event: subject GalSpan_Frigate (object 321, id 1066), op 8, value 0

**Action**

- Set/add variable: variable group 21, variable 19, subtype 1, value 1

### Event 5

**Trigger**

- Object event: subject GalSpan_Frigate (object 322, id 1067), op 2, value 0 (join 2)
- Object event: subject GalSpan_Frigate (object 322, id 1067), op 8, value 0

**Action**

- Set/add variable: variable group 21, variable 19, subtype 1, value 1

### Event 6

**Trigger**

- Variable comparison: subject variable group 21, variable 19, op 1, value 2

**Action**

- Object spawn/action: Bora_Carrier (object 323, id 1864), subtype 5
- Object spawn/action: Bora_Carrier (object 323, id 1864), subtype 13, param 10223616
- Group/spawn-list action: spawn list/group 178, subtype 8, param 10289152 (Waypoint 0 (tag 157), point 0)
- Group/spawn-list action: spawn list/group 106, subtype 8, param 10289152 (Waypoint 0 (tag 157), point 0)

### Event 7

**Trigger**

- Object arrival: Bora_Carrier (object 323, id 1864) reached Waypoint 2 (tag 156), point 0 (raw value 10223616)

**Action**

- Set runtime trigger variable: variable group 20, variable 19, subtype 0, value 0

### Event 8

**Trigger**

- Variable comparison: subject variable group 20, variable 19, op 1, value 35

**Action**

- Object spawn/action: Bora_Carrier (object 323, id 1864), subtype 4

### Event 9

**Trigger**

- Object event: subject GalSpan_Frigate (object 321, id 1066), op 2, value 0
- Object event: subject GalSpan_Frigate (object 322, id 1067), op 2, value 0

**Action**

- Play dialog: PLAYER.SCR, line/variant 35

### Event 10

**Trigger**

- Object event: subject GalSpan_Frigate (object 321, id 1066), op 14, value 21
- Object event: subject GalSpan_Frigate (object 322, id 1067), op 14, value 21

**Action**

- Set/add variable: variable group 0, variable 2, subtype 1, value 5000

### Event 11

**Trigger**

- Group/spawn-list event: subject 178, op 2, value 10289153 (Waypoint 0 (tag 157), point 1)

**Action**

- Group/spawn-list action: spawn list/group 178, subtype 5, param 1864

### Event 12

**Trigger**

- Group/spawn-list event: subject 106, op 2, value 65536

**Action**

- Group/spawn-list action: spawn list/group 106, subtype 5, param 1864

## Waypoints

### Waypoint 0

- Tag: `157`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-9330.14, 617.84, -8296.10) | None |
| 1 | (-8960.55, 267.98, -5830.55) | None |

### Waypoint 1

- Tag: `155`
- Members: `GalSpan_Orion (object 0, id 1068, starts at point 0)`, `GalSpan_Orion (object 1, id 1069, starts at point 0)`, `GalSpan_Orion (object 2, id 1070, starts at point 0)`, `GalSpan_Orion (object 3, id 1071, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-6150.58, 0.00, -3063.59) | None |

### Waypoint 2

- Tag: `156`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-10941.79, 345.91, -3467.60) | on arrival activate current object (raw param -1 ignored); listened by Event 7 for Bora_Carrier (object 323, id 1864) |

### Waypoint 3

- Tag: `154`
- Members: `Bora_Carrier (object 323, id 1864, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-10046.60, 187.81, -8412.54) | None; listened by Event 3 for Bora_Carrier (object 323, id 1864) |
| 1 | (-9346.24, 261.59, -5687.10) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 4

- Tag: `153`
- Members: `Bora_Mace (object 156, id 1865, starts at point 0)`, `Bora_Mace (object 314, id 2146, starts at point 0)`, `Bora_Leviathan (object 315, id 2145, starts at point 0)`, `Bora_Leviathan (object 316, id 2148, starts at point 0)`, `Bora_Mace (object 317, id 2144, starts at point 0)`, `Bora_Mace (object 318, id 2147, starts at point 0)`, `Bora_Claymore (object 319, id 1866, starts at point 0)`, `Bora_Claymore (object 320, id 1868, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-10770.21, 187.81, -8987.52) | None |
| 1 | (-9785.48, 187.81, -7049.80) | None |

### Waypoint 5

- Tag: `152`
- Members: `GalSpan_Frigate (object 321, id 1066, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-9648.35, 178.25, -4585.54) | None |
| 1 | (-10136.49, 179.19, -5556.49) | None |
| 2 | (-10723.23, 326.75, -7482.31) | on arrival action 1, param -1 |

### Waypoint 6

- Tag: `151`
- Members: `GalSpan_Frigate (object 322, id 1067, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (-8185.52, 178.25, -5255.98) | None |
| 1 | (-8734.74, 179.19, -6124.59) | None |
| 2 | (-9123.97, 326.75, -7842.86) | on arrival action 1, param -1 |

## Spawn Lists

### Spawn List 0

- ID: `178`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | GalSpan_Frigate (object 322, id 1067) | None |
| 1 | 2 | GalSpan_Frigate (object 321, id 1066) | None |

### Spawn List 1

- ID: `231`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 0 | none | None |

### Spawn List 2

- ID: `106`
| Rule | Op | Target | Params |
| ---: | ---: | --- | --- |
| 0 | 2 | GalSpan_Frigate (object 321, id 1066) | None |
| 1 | 2 | GalSpan_Frigate (object 322, id 1067) | None |


## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `GalSpan_Orion` | 1068 | Interactive | -8211.59,178.25,-3868.78 | 90,0,0 | label: bfbe_08; group/role: FG_ATHENE / 2; waypoint: Waypoint 1 (tag 155, 1 point(s)), starting point 0, arrival event value 10158080 |
| 1 | `GalSpan_Orion` | 1069 | Interactive | -7346.92,178.25,-4345.42 | 71,0,0 | label: bfbe_08; group/role: FG_ATHENE / 3; waypoint: Waypoint 1 (tag 155, 1 point(s)), starting point 0, arrival event value 10158080 |
| 2 | `GalSpan_Orion` | 1070 | Interactive | -8099.49,178.25,-3861.16 | 90,0,0 | group/role: FG_ATHENE / 1; waypoint: Waypoint 1 (tag 155, 1 point(s)), starting point 0, arrival event value 10158080 |
| 3 | `GalSpan_Orion` | 1071 | Interactive | -7175.93,178.25,-4374.70 | 71,0,0 | group/role: FG_ATHENE / 4; waypoint: Waypoint 1 (tag 155, 1 point(s)), starting point 0, arrival event value 10158080 |
| 4 | `Roid_Sm_Grey` | 1657 | Object | -8656.03,-392.63,-5170.88 | 298,418,419 | Scale/Radius: 7.00 |
| 5 | `Roid_SM_Grey_Points` | 1658 | Object | -8591.82,-103.93,-3058.41 | 177,173,136 | Scale/Radius: 6.00 |
| 6 | `Bora_Mine` | 1659 | Interactive | -7888.08,-230.96,-3867.76 | 311,199,61 | None |
| 7 | `Asteroid_2` | 1660 | Object | -8128.30,-207.86,-4718.20 | 172,459,408 | Scale/Radius: 4.00 |
| 8 | `Roid_Lrg_Grey` | 1661 | Object | -6629.54,427.27,-3670.51 | 341,421,502 | Scale/Radius: 2.00 |
| 9 | `Roid_Sm_Grey` | 1662 | Object | -8009.25,254.05,-3207.29 | 284,482,366 | Scale/Radius: 7.00 |
| 10 | `Bora_Mine` | 1664 | Interactive | -8406.28,588.94,-5057.49 | 113,187,207 | None |
| 11 | `Asteroid_2` | 1665 | Object | -9032.35,-92.38,-3697.43 | 223,188,82 | Scale/Radius: 8.00 |
| 12 | `Bora_Mine` | 1669 | Interactive | -6622.32,0.00,-5553.24 | 123,445,159 | None |
| 13 | `Asteroid_2` | 1670 | Object | -7110.46,-254.05,-4089.37 | 29,369,285 | Scale/Radius: 7.00 |
| 14 | `Roid_Sm_Grey` | 1672 | Object | -6742.02,254.05,-5354.78 | 419,230,247 | Scale/Radius: 5.00 |
| 15 | `Bora_Mine` | 1674 | Interactive | -7484.34,-565.85,-5641.98 | 317,401,331 | None |
| 16 | `Asteroid_2` | 1675 | Object | -8746.99,-115.48,-5307.87 | 338,247,340 | Scale/Radius: 3.00 |
| 17 | `Roid_Lrg_Grey` | 1676 | Object | -6028.43,369.53,-4732.14 | 229,92,49 | Scale/Radius: 7.00 |
| 18 | `Roid_Sm_Grey` | 1677 | Object | -7707.51,150.12,-5839.10 | 235,224,77 | Scale/Radius: 4.00 |
| 19 | `Roid_SM_Grey_Points` | 1678 | Object | -8634.03,-346.44,-4905.62 | 264,6,441 | Scale/Radius: 3.00 |
| 20 | `Bora_Mine` | 1679 | Interactive | -6160.29,600.49,-4272.92 | 496,242,477 | None |
| 21 | `Asteroid_2` | 1680 | Object | -7597.13,300.25,-3087.51 | 75,356,160 | Scale/Radius: 9.00 |
| 22 | `Roid_Sm_Grey` | 1682 | Object | -8124.36,-334.89,-4822.21 | 134,38,284 | Scale/Radius: 9.00 |
| 23 | `Roid_Lrg_Grey` | 1686 | Object | -6818.67,404.18,-3284.48 | 171,108,371 | Scale/Radius: 1.00 |
| 24 | `Bora_Mine` | 1689 | Interactive | -6981.41,207.86,-4957.87 | 387,12,63 | None |
| 25 | `Roid_Lrg_Grey` | 1691 | Object | -9067.49,161.67,-3615.96 | 470,426,152 | Scale/Radius: 1.00 |
| 26 | `Roid_SM_Grey_Points` | 1693 | Object | -7563.81,-508.11,-5236.34 | 304,50,511 | Scale/Radius: 2.00 |
| 27 | `Bora_Mine` | 1694 | Interactive | -8380.67,288.70,-4401.90 | 461,413,256 | None |
| 28 | `Asteroid_2` | 1695 | Object | -7571.02,80.84,-3353.61 | 506,75,183 | Scale/Radius: 2.00 |
| 29 | `Roid_Lrg_Grey` | 1696 | Object | -7175.16,346.44,-4919.80 | 300,32,400 | Scale/Radius: 7.00 |
| 30 | `Roid_Sm_Grey` | 1697 | Object | -7993.82,-461.92,-2768.67 | 181,497,132 | Scale/Radius: 7.00 |
| 31 | `Roid_SM_Grey_Points` | 1698 | Object | -7382.69,-11.55,-2825.65 | 270,166,469 | Scale/Radius: 6.00 |
| 32 | `Roid_Sm_Grey` | 1702 | Object | -7731.27,-392.63,-2507.66 | 360,388,299 | Scale/Radius: 1.00 |
| 33 | `Asteroid_2` | 1705 | Object | -9424.94,11.55,-3909.95 | 187,279,147 | Scale/Radius: 7.00 |
| 34 | `Roid_Lrg_Grey` | 1706 | Object | -6332.68,-415.72,-4738.32 | 15,383,282 | Scale/Radius: 7.00 |
| 35 | `Roid_Sm_Grey` | 1707 | Object | -8748.13,-542.75,-2316.48 | 31,156,244 | Scale/Radius: 9.00 |
| 36 | `Roid_SM_Grey_Points` | 1708 | Object | -8063.77,508.11,-3460.42 | 103,143,172 | Scale/Radius: 8.00 |
| 37 | `Bora_Mine` | 1709 | Interactive | -6559.10,-485.01,-4260.79 | 178,422,38 | None |
| 38 | `Roid_Sm_Grey` | 1712 | Object | -7371.37,-265.60,-5239.73 | 376,51,414 | Scale/Radius: 1.00 |
| 39 | `Bora_Mine` | 1714 | Interactive | -7351.17,-230.96,-3657.78 | 263,394,79 | None |
| 40 | `Asteroid_2` | 1715 | Object | -7881.17,161.67,-1511.74 | 11,144,73 | Scale/Radius: 9.00 |
| 41 | `Roid_Lrg_Grey` | 1716 | Object | -6518.55,-80.84,-4908.29 | 255,252,251 | Scale/Radius: 3.00 |
| 42 | `Roid_SM_Grey_Points` | 1718 | Object | -6570.60,-103.93,-4803.42 | 464,64,452 | Scale/Radius: 7.00 |
| 43 | `Bora_Mine` | 1719 | Interactive | -6497.53,-288.70,-5463.04 | 153,365,4 | None |
| 44 | `Roid_Sm_Grey` | 1722 | Object | -7170.23,-184.77,-4203.81 | 335,124,395 | Scale/Radius: 1.00 |
| 45 | `Roid_SM_Grey_Points` | 1723 | Object | -8786.72,-450.37,-3413.02 | 138,212,107 | Scale/Radius: 6.00 |
| 46 | `Roid_Sm_Grey` | 1727 | Object | -6725.27,46.19,-4950.84 | 239,374,305 | Scale/Radius: 5.00 |
| 47 | `Roid_SM_Grey_Points` | 1728 | Object | -7614.87,92.38,-4311.46 | 490,239,156 | Scale/Radius: 7.00 |
| 48 | `Bora_Mine` | 1729 | Interactive | -10263.81,-519.66,-3340.76 | 457,62,2 | None |
| 49 | `Roid_Sm_Grey` | 1732 | Object | -7190.25,184.77,-2829.04 | 216,506,16 | Scale/Radius: 9.00 |
| 50 | `Roid_SM_Grey_Points` | 1733 | Object | -7593.69,-57.74,-5293.56 | 333,67,175 | Scale/Radius: 9.00 |
| 51 | `Bora_Mine` | 1734 | Interactive | -9110.35,11.55,-3753.80 | 505,409,68 | None |
| 52 | `Roid_Sm_Grey` | 1737 | Object | -8759.46,-450.37,-3286.45 | 452,112,384 | Scale/Radius: 8.00 |
| 53 | `Roid_SM_Grey_Points` | 1738 | Object | -6325.45,184.77,-3236.99 | 371,412,67 | Scale/Radius: 2.00 |
| 54 | `Bora_Mine` | 1739 | Interactive | -9106.73,-196.31,-3003.13 | 480,237,444 | None |
| 55 | `Asteroid_2` | 1740 | Object | -7875.11,404.18,-3787.14 | 356,84,182 | Scale/Radius: 1.00 |
| 56 | `Roid_Lrg_Grey` | 1741 | Object | -6853.64,-11.55,-3483.33 | 503,194,211 | Scale/Radius: 3.00 |
| 57 | `Roid_Sm_Grey` | 1742 | Object | -8345.54,46.19,-4483.37 | 47,231,102 | Scale/Radius: 7.00 |
| 58 | `Roid_SM_Grey_Points` | 1743 | Object | -7633.09,34.64,-4253.39 | 89,226,36 | Scale/Radius: 9.00 |
| 59 | `Bora_Mine` | 1744 | Interactive | -6764.00,-311.79,-3458.69 | 254,414,406 | None |
| 60 | `Asteroid_2` | 1745 | Object | -9043.35,-612.04,-2138.02 | 256,18,91 | Scale/Radius: 6.00 |
| 61 | `Roid_Lrg_Grey` | 1746 | Object | -8216.64,-311.79,-4924.53 | 428,122,480 | Scale/Radius: 7.00 |
| 62 | `Roid_Sm_Grey` | 1747 | Object | -8572.44,-69.29,-2723.81 | 487,176,69 | Scale/Radius: 2.00 |
| 63 | `Bora_Mine` | 1749 | Interactive | -8256.21,219.41,-3457.02 | 466,353,156 | None |
| 64 | `Roid_Lrg_Grey` | 1751 | Object | -7456.26,588.94,-4268.06 | 492,367,402 | Scale/Radius: 1.00 |
| 65 | `Roid_SM_Grey_Points` | 1753 | Object | -8303.99,381.08,-4310.86 | 170,176,76 | Scale/Radius: 9.00 |
| 66 | `Bora_Mine` | 1754 | Interactive | -7569.87,-242.51,-2960.94 | 174,320,473 | None |
| 67 | `Asteroid_2` | 1755 | Object | -8833.84,-69.29,-2592.16 | 38,331,419 | Scale/Radius: 6.00 |
| 68 | `Roid_Sm_Grey` | 1757 | Object | -7901.86,-357.99,-1811.66 | 97,407,406 | Scale/Radius: 1.00 |
| 69 | `Roid_SM_Grey_Points` | 1758 | Object | -8022.55,427.27,-2433.22 | 423,292,63 | Scale/Radius: 3.00 |
| 70 | `Bora_Mine` | 1759 | Interactive | -8182.31,-57.74,-2869.29 | 330,317,354 | None |
| 71 | `Asteroid_2` | 1760 | Object | -7500.10,-381.08,-5225.91 | 440,406,151 | Scale/Radius: 4.00 |
| 72 | `Roid_Lrg_Grey` | 1761 | Object | -6711.47,-23.10,-3622.87 | 465,197,261 | Scale/Radius: 9.00 |
| 73 | `Roid_Sm_Grey` | 1762 | Object | -7987.92,311.79,-4616.72 | 242,14,391 | Scale/Radius: 2.00 |
| 74 | `Roid_SM_Grey_Points` | 1763 | Object | -7428.63,127.03,-2500.54 | 408,284,182 | Scale/Radius: 6.00 |
| 75 | `Bora_Mine` | 1764 | Interactive | -7355.61,-80.84,-5655.80 | 448,365,51 | None |
| 76 | `Asteroid_2` | 1765 | Object | -7933.89,161.67,-3081.57 | 119,482,312 | Scale/Radius: 2.00 |
| 77 | `Roid_Lrg_Grey` | 1766 | Object | -9096.22,-184.77,-3280.51 | 334,44,140 | Scale/Radius: 9.00 |
| 78 | `Roid_Sm_Grey` | 1767 | Object | -7739.66,-92.38,-4401.66 | 0,407,69 | Scale/Radius: 6.00 |
| 79 | `Roid_SM_Grey_Points` | 1768 | Object | -7011.62,-23.10,-4160.41 | 165,453,470 | Scale/Radius: 6.00 |
| 80 | `Bora_Mine` | 1769 | Interactive | -7749.33,542.75,-2876.93 | 304,404,471 | None |
| 81 | `Roid_Lrg_Grey` | 1771 | Object | -7802.53,161.67,-3164.73 | 39,397,192 | Scale/Radius: 9.00 |
| 82 | `Roid_SM_Grey_Points` | 1773 | Object | -6377.33,138.57,-3559.46 | 329,364,408 | Scale/Radius: 2.00 |
| 83 | `Bora_Mine` | 1774 | Interactive | -6314.45,508.11,-4796.39 | 106,345,36 | None |
| 84 | `Asteroid_2` | 1775 | Object | -7903.84,-115.48,-3451.69 | 150,192,434 | Scale/Radius: 2.00 |
| 85 | `Roid_Lrg_Grey` | 1776 | Object | -9709.98,127.03,-3154.19 | 251,16,503 | Scale/Radius: 3.00 |
| 86 | `Roid_Sm_Grey` | 1777 | Object | -7271.86,-196.31,-3636.08 | 41,339,469 | Scale/Radius: 8.00 |
| 87 | `Roid_SM_Grey_Points` | 1778 | Object | -7812.72,450.37,-3742.04 | 104,457,393 | Scale/Radius: 6.00 |
| 88 | `Bora_Mine` | 1779 | Interactive | -8157.04,-57.74,-4382.75 | 98,392,66 | None |
| 89 | `Asteroid_2` | 1780 | Object | -7154.79,-115.48,-3765.19 | 476,31,332 | Scale/Radius: 5.00 |
| 90 | `Roid_Lrg_Grey` | 1781 | Object | -7353.31,-184.77,-4870.46 | 98,29,250 | Scale/Radius: 2.00 |
| 91 | `Roid_Sm_Grey` | 1782 | Object | -6998.16,-184.77,-5361.82 | 314,430,393 | Scale/Radius: 7.00 |
| 92 | `Roid_SM_Grey_Points` | 1783 | Object | -7383.68,-80.84,-3645.66 | 444,115,74 | Scale/Radius: 2.00 |
| 93 | `Bora_Mine` | 1784 | Interactive | -6520.83,-461.92,-3532.27 | 299,300,380 | None |
| 94 | `Asteroid_2` | 1785 | Object | -8380.51,-207.86,-4829.24 | 324,472,79 | Scale/Radius: 2.00 |
| 95 | `Roid_Lrg_Grey` | 1786 | Object | -7190.76,69.29,-4931.08 | 219,408,398 | Scale/Radius: 3.00 |
| 96 | `Roid_Sm_Grey` | 1787 | Object | -8894.92,242.51,-2671.93 | 39,229,129 | Scale/Radius: 8.00 |
| 97 | `Roid_SM_Grey_Points` | 1788 | Object | -7224.58,-92.38,-4884.28 | 213,343,18 | Scale/Radius: 1.00 |
| 98 | `Asteroid_2` | 1790 | Object | -8310.40,161.67,-4564.84 | 326,107,142 | Scale/Radius: 7.00 |
| 99 | `Roid_Lrg_Grey` | 1791 | Object | -7903.52,23.10,-4306.37 | 416,366,113 | Scale/Radius: 1.00 |
| 100 | `Roid_Sm_Grey` | 1792 | Object | -6734.11,-404.18,-3401.46 | 413,77,65 | Scale/Radius: 9.00 |
| 101 | `Roid_SM_Grey_Points` | 1793 | Object | -7583.83,357.99,-3861.57 | 474,380,507 | Scale/Radius: 5.00 |
| 102 | `Bora_Mine` | 1794 | Interactive | -8391.02,-115.48,-4551.87 | 496,262,139 | None |
| 103 | `Roid_Lrg_Grey` | 1796 | Object | -7733.57,531.20,-3293.00 | 115,317,356 | Scale/Radius: 2.00 |
| 104 | `Roid_Sm_Grey` | 1797 | Object | -8611.84,-196.31,-1683.64 | 446,43,383 | Scale/Radius: 7.00 |
| 105 | `Roid_SM_Grey_Points` | 1798 | Object | -9754.15,-404.18,-3257.36 | 418,71,473 | Scale/Radius: 8.00 |
| 106 | `Bora_Mine` | 1799 | Interactive | -7201.59,-242.51,-3799.02 | 223,272,172 | None |
| 107 | `Asteroid_2` | 1800 | Object | -9327.00,427.27,-3546.05 | 345,74,97 | Scale/Radius: 3.00 |
| 108 | `Roid_Lrg_Grey` | 1801 | Object | -8507.26,230.96,-3175.40 | 240,503,44 | Scale/Radius: 3.00 |
| 109 | `Roid_Sm_Grey` | 1802 | Object | -7483.51,404.18,-4394.63 | 401,251,225 | Scale/Radius: 4.00 |
| 110 | `Roid_SM_Grey_Points` | 1803 | Object | -7187.60,531.20,-3462.23 | 34,445,451 | Scale/Radius: 3.00 |
| 111 | `Bora_Mine` | 1804 | Interactive | -7454.46,219.41,-5584.76 | 387,158,299 | None |
| 112 | `Asteroid_2` | 1805 | Object | -7047.08,-415.72,-3224.26 | 329,208,363 | Scale/Radius: 4.00 |
| 113 | `Roid_Lrg_Grey` | 1806 | Object | -7245.76,34.64,-3902.19 | 183,177,297 | Scale/Radius: 9.00 |
| 114 | `Roid_SM_Grey_Points` | 1808 | Object | -7506.99,46.19,-4197.87 | 241,331,163 | Scale/Radius: 1.00 |
| 115 | `Bora_Mine` | 1809 | Interactive | -7086.98,-485.01,-4286.13 | 289,61,250 | None |
| 116 | `Roid_Lrg_Grey` | 1811 | Object | -6756.95,-311.79,-3691.36 | 201,180,243 | Scale/Radius: 5.00 |
| 117 | `Roid_Sm_Grey` | 1812 | Object | -6272.57,-138.57,-3317.21 | 119,14,419 | Scale/Radius: 4.00 |
| 118 | `Roid_SM_Grey_Points` | 1813 | Object | -6544.49,80.84,-5069.52 | 351,469,392 | Scale/Radius: 7.00 |
| 119 | `Bora_Mine` | 1814 | Interactive | -6531.02,-277.15,-2886.87 | 9,62,398 | None |
| 120 | `Asteroid_2` | 1815 | Object | -8745.99,357.99,-1103.79 | 504,392,457 | Scale/Radius: 6.00 |
| 121 | `Roid_SM_Grey_Points` | 1818 | Object | -7510.45,-230.96,-5375.88 | 141,338,466 | Scale/Radius: 9.00 |
| 122 | `Bora_Mine` | 1819 | Interactive | -8301.02,-57.74,-1850.82 | 316,8,106 | None |
| 123 | `Asteroid_2` | 1820 | Object | -7620.44,265.60,-3318.09 | 382,348,370 | Scale/Radius: 2.00 |
| 124 | `Roid_Lrg_Grey` | 1821 | Object | -7003.90,-450.37,-3941.10 | 503,199,331 | Scale/Radius: 6.00 |
| 125 | `Roid_SM_Grey_Points` | 1823 | Object | -7422.43,138.57,-4314.86 | 259,298,99 | Scale/Radius: 5.00 |
| 126 | `Bora_Mine` | 1824 | Interactive | -7509.78,150.12,-3701.18 | 323,218,453 | None |
| 127 | `Asteroid_2` | 1825 | Object | -6278.17,-80.84,-4485.19 | 55,400,236 | Scale/Radius: 1.00 |
| 128 | `Roid_Lrg_Grey` | 1826 | Object | -6130.22,-254.05,-3737.07 | 308,434,380 | Scale/Radius: 8.00 |
| 129 | `Roid_Sm_Grey` | 1827 | Object | -6679.62,161.67,-5309.68 | 178,348,139 | Scale/Radius: 6.00 |
| 130 | `Roid_SM_Grey_Points` | 1828 | Object | -9197.69,311.79,-3140.12 | 304,248,417 | Scale/Radius: 2.00 |
| 131 | `Bora_Mine` | 1829 | Interactive | -8944.18,-207.86,-3063.75 | 230,380,148 | None |
| 132 | `Asteroid_2` | 1830 | Object | -7048.90,46.19,-5291.62 | 115,125,493 | Scale/Radius: 3.00 |
| 133 | `Roid_Lrg_Grey` | 1831 | Object | -6892.72,92.38,-3297.85 | 118,146,300 | Scale/Radius: 3.00 |
| 134 | `Roid_Sm_Grey` | 1832 | Object | -6398.29,150.12,-3930.77 | 445,408,484 | Scale/Radius: 7.00 |
| 135 | `Roid_SM_Grey_Points` | 1833 | Object | -9112.31,127.03,-2009.76 | 108,365,91 | Scale/Radius: 9.00 |
| 136 | `Roid_Lrg_Grey` | 1836 | Object | -7249.16,34.64,-2584.55 | 165,228,186 | Scale/Radius: 9.00 |
| 137 | `Roid_SM_Grey_Points` | 1838 | Object | -7732.30,34.64,-5607.67 | 116,37,275 | Scale/Radius: 1.00 |
| 138 | `Bora_Mine` | 1839 | Interactive | -8401.85,-508.11,-3419.81 | 253,15,417 | None |
| 139 | `Asteroid_2` | 1840 | Object | -8286.25,-173.22,-3086.90 | 430,330,212 | Scale/Radius: 2.00 |
| 140 | `Roid_Sm_Grey` | 1842 | Object | -8589.03,-161.67,-3555.10 | 183,473,443 | Scale/Radius: 1.00 |
| 141 | `Asteroid_2` | 1845 | Object | -9717.70,-11.55,-3373.50 | 283,454,387 | Scale/Radius: 8.00 |
| 142 | `Roid_Lrg_Grey` | 1846 | Object | -8415.81,-127.03,-4320.44 | 141,56,132 | Scale/Radius: 3.00 |
| 143 | `Roid_Sm_Grey` | 1847 | Object | -7188.92,-519.66,-3427.56 | 110,402,146 | Scale/Radius: 4.00 |
| 144 | `Roid_SM_Grey_Points` | 1848 | Object | -6274.87,34.64,-2879.84 | 341,472,45 | Scale/Radius: 4.00 |
| 145 | `Bora_Mine` | 1849 | Interactive | -6922.61,-300.25,-3502.09 | 102,505,62 | None |
| 146 | `Asteroid_2` | 1850 | Object | -9332.66,150.12,-3807.63 | 33,447,418 | Scale/Radius: 6.00 |
| 147 | `Roid_Sm_Grey` | 1852 | Object | -7590.56,-173.22,-3260.87 | 138,304,304 | Scale/Radius: 3.00 |
| 148 | `Roid_SM_Grey_Points` | 1853 | Object | -8548.31,138.57,-4629.94 | 1,127,91 | Scale/Radius: 7.00 |
| 149 | `Bora_Mine` | 1854 | Interactive | -6169.44,-46.19,-3375.81 | 53,127,216 | None |
| 150 | `Asteroid_2` | 1855 | Object | -8008.27,0.00,-2387.27 | 95,119,2 | Scale/Radius: 8.00 |
| 151 | `Roid_Lrg_Grey` | 1856 | Object | -7862.14,-103.93,-3706.52 | 226,382,345 | Scale/Radius: 7.00 |
| 152 | `Roid_Sm_Grey` | 1857 | Object | -8658.66,-311.79,-5101.53 | 344,378,299 | Scale/Radius: 5.00 |
| 153 | `Roid_SM_Grey_Points` | 1858 | Object | -8317.94,588.94,-1827.43 | 61,291,330 | Scale/Radius: 2.00 |
| 154 | `Bora_Mine` | 1859 | Interactive | -6684.05,196.31,-3923.64 | 153,284,415 | None |
| 155 | `Asteroid_2` | 1860 | Object | -7731.11,127.03,-2935.00 | 365,73,277 | Scale/Radius: 3.00 |
| 156 | `Bora_Mace` | 1865 | Interactive | -11154.26,187.81,-9596.04 | 14,0,0 | group/role: FG_HONOR / 0; waypoint: Waypoint 4 (tag 153, 2 point(s)), starting point 0, arrival event value 10027008 |
| 157 | `Roid_SM_Grey_Points` | 1884 | Object | -6526.72,-103.93,-2654.53 | 177,173,136 | Scale/Radius: 6.00 |
| 158 | `Roid_SM_Grey_Points` | 1889 | Object | -6330.84,-450.37,-3008.52 | 138,212,107 | Scale/Radius: 6.00 |
| 159 | `Roid_Sm_Grey` | 1891 | Object | -6358.82,-450.37,-2887.15 | 452,112,384 | Scale/Radius: 8.00 |
| 160 | `Bora_Mine` | 1892 | Interactive | -6013.69,-196.31,-2603.95 | 480,237,444 | None |
| 161 | `Roid_Sm_Grey` | 1893 | Object | -6545.38,-69.29,-2320.76 | 487,176,69 | Scale/Radius: 2.00 |
| 162 | `Bora_Mine` | 1894 | Interactive | -6862.53,219.41,-3059.10 | 466,353,156 | None |
| 163 | `Asteroid_2` | 1896 | Object | -6284.20,-69.29,-2189.27 | 38,331,419 | Scale/Radius: 6.00 |
| 164 | `Roid_Lrg_Grey` | 1897 | Object | -6023.01,-184.77,-2877.04 | 334,44,140 | Scale/Radius: 9.00 |
| 165 | `Roid_Sm_Grey` | 1898 | Object | -6218.90,242.51,-2270.18 | 39,229,129 | Scale/Radius: 8.00 |
| 166 | `Roid_Lrg_Grey` | 1899 | Object | -6610.67,230.96,-2775.90 | 240,503,44 | Scale/Radius: 3.00 |
| 167 | `Roid_SM_Grey_Points` | 1900 | Object | -5920.41,311.79,-2735.44 | 304,248,417 | Scale/Radius: 2.00 |
| 168 | `Bora_Mine` | 1901 | Interactive | -6172.26,-207.86,-2664.64 | 230,380,148 | None |
| 169 | `Bora_Mine` | 1902 | Interactive | -6713.28,-508.11,-3018.64 | 253,15,417 | None |
| 170 | `Asteroid_2` | 1903 | Object | -6825.22,-173.22,-2684.87 | 430,330,212 | Scale/Radius: 2.00 |
| 171 | `Roid_SM_Grey_Points` | 1904 | Object | -7011.77,-103.93,-2887.15 | 177,173,136 | Scale/Radius: 6.00 |
| 172 | `Roid_SM_Grey_Points` | 1909 | Object | -6815.89,-450.37,-3241.15 | 138,212,107 | Scale/Radius: 6.00 |
| 173 | `Roid_Sm_Grey` | 1911 | Object | -6843.87,-450.37,-3119.78 | 452,112,384 | Scale/Radius: 8.00 |
| 174 | `Bora_Mine` | 1912 | Interactive | -6498.74,-196.31,-2836.58 | 480,237,444 | None |
| 175 | `Roid_Sm_Grey` | 1913 | Object | -7030.43,-69.29,-2553.38 | 487,176,69 | Scale/Radius: 2.00 |
| 176 | `Bora_Mine` | 1914 | Interactive | -7347.58,219.41,-3291.72 | 466,353,156 | None |
| 177 | `Asteroid_2` | 1916 | Object | -6769.25,-69.29,-2421.90 | 38,331,419 | Scale/Radius: 6.00 |
| 178 | `Roid_Lrg_Grey` | 1917 | Object | -6508.07,-184.77,-3109.67 | 334,44,140 | Scale/Radius: 9.00 |
| 179 | `Roid_Sm_Grey` | 1918 | Object | -6703.95,242.51,-2502.81 | 39,229,129 | Scale/Radius: 8.00 |
| 180 | `Roid_Lrg_Grey` | 1919 | Object | -7095.73,230.96,-3008.52 | 240,503,44 | Scale/Radius: 3.00 |
| 181 | `Roid_SM_Grey_Points` | 1920 | Object | -6405.46,311.79,-2968.07 | 304,248,417 | Scale/Radius: 2.00 |
| 182 | `Bora_Mine` | 1921 | Interactive | -6657.31,-207.86,-2897.27 | 230,380,148 | None |
| 183 | `Bora_Mine` | 1922 | Interactive | -7198.33,-508.11,-3251.27 | 253,15,417 | None |
| 184 | `Asteroid_2` | 1923 | Object | -7310.27,-173.22,-2917.50 | 430,330,212 | Scale/Radius: 2.00 |
| 185 | `Asteroid_2` | 1924 | Object | -6097.64,-92.38,-3848.01 | 223,188,82 | Scale/Radius: 8.00 |
| 186 | `Roid_Lrg_Grey` | 1927 | Object | -6060.33,161.67,-3767.09 | 470,426,152 | Scale/Radius: 1.00 |
| 187 | `Asteroid_2` | 1928 | Object | -5705.87,11.55,-4060.41 | 187,279,147 | Scale/Radius: 7.00 |
| 188 | `Roid_SM_Grey_Points` | 1929 | Object | -6340.16,-450.37,-3564.81 | 138,212,107 | Scale/Radius: 6.00 |
| 189 | `Bora_Mine` | 1930 | Interactive | -6013.69,11.55,-3908.69 | 505,409,68 | None |
| 190 | `Roid_Sm_Grey` | 1931 | Object | -6368.15,-450.37,-3433.32 | 452,112,384 | Scale/Radius: 8.00 |
| 191 | `Roid_Lrg_Grey` | 1933 | Object | -6032.34,-184.77,-3433.32 | 334,44,140 | Scale/Radius: 9.00 |
| 192 | `Roid_Lrg_Grey` | 1934 | Object | -5416.70,127.03,-3301.84 | 251,16,503 | Scale/Radius: 3.00 |
| 193 | `Roid_SM_Grey_Points` | 1935 | Object | -5370.06,-404.18,-3413.09 | 418,71,473 | Scale/Radius: 8.00 |
| 194 | `Asteroid_2` | 1936 | Object | -5864.44,427.27,-4222.23 | 345,74,97 | Scale/Radius: 3.00 |
| 195 | `Roid_SM_Grey_Points` | 1937 | Object | -5929.74,311.79,-3291.72 | 304,248,417 | Scale/Radius: 2.00 |
| 196 | `Asteroid_2` | 1938 | Object | -5407.37,-11.55,-3524.35 | 283,454,387 | Scale/Radius: 8.00 |
| 197 | `Asteroid_2` | 1939 | Object | -5789.82,150.12,-3959.26 | 33,447,418 | Scale/Radius: 6.00 |
| 198 | `Asteroid_2` | 1940 | Object | -7832.63,-92.38,-2057.78 | 223,188,82 | Scale/Radius: 8.00 |
| 199 | `Roid_Lrg_Grey` | 1943 | Object | -7795.32,161.67,-1976.87 | 470,426,152 | Scale/Radius: 1.00 |
| 200 | `Asteroid_2` | 1944 | Object | -7440.86,11.55,-2270.18 | 187,279,147 | Scale/Radius: 7.00 |
| 201 | `Roid_SM_Grey_Points` | 1945 | Object | -8075.16,-450.37,-1774.59 | 138,212,107 | Scale/Radius: 6.00 |
| 202 | `Bora_Mine` | 1946 | Interactive | -7748.68,11.55,-2118.47 | 505,409,68 | None |
| 203 | `Roid_Sm_Grey` | 1947 | Object | -8103.14,-450.37,-1643.10 | 452,112,384 | Scale/Radius: 8.00 |
| 204 | `Roid_Lrg_Grey` | 1949 | Object | -7767.34,-184.77,-1643.10 | 334,44,140 | Scale/Radius: 9.00 |
| 205 | `Roid_Lrg_Grey` | 1950 | Object | -7151.69,127.03,-1511.62 | 251,16,503 | Scale/Radius: 3.00 |
| 206 | `Roid_SM_Grey_Points` | 1951 | Object | -7105.05,-404.18,-1622.87 | 418,71,473 | Scale/Radius: 8.00 |
| 207 | `Asteroid_2` | 1952 | Object | -7599.43,427.27,-2432.01 | 345,74,97 | Scale/Radius: 3.00 |
| 208 | `Roid_SM_Grey_Points` | 1953 | Object | -7664.73,311.79,-1501.50 | 304,248,417 | Scale/Radius: 2.00 |
| 209 | `Asteroid_2` | 1954 | Object | -7142.37,-11.55,-1734.13 | 283,454,387 | Scale/Radius: 8.00 |
| 210 | `Asteroid_2` | 1955 | Object | -7524.81,150.12,-2169.04 | 33,447,418 | Scale/Radius: 6.00 |
| 211 | `Asteroid_2` | 1956 | Object | -6797.23,-92.38,-3504.12 | 223,188,82 | Scale/Radius: 8.00 |
| 212 | `Roid_Lrg_Grey` | 1959 | Object | -6759.92,161.67,-3423.21 | 470,426,152 | Scale/Radius: 1.00 |
| 213 | `Asteroid_2` | 1960 | Object | -6405.46,11.55,-3716.52 | 187,279,147 | Scale/Radius: 7.00 |
| 214 | `Roid_SM_Grey_Points` | 1961 | Object | -7039.76,-450.37,-3220.92 | 138,212,107 | Scale/Radius: 6.00 |
| 215 | `Bora_Mine` | 1962 | Interactive | -6713.28,11.55,-3564.81 | 505,409,68 | None |
| 216 | `Roid_Sm_Grey` | 1963 | Object | -7067.74,-450.37,-3089.44 | 452,112,384 | Scale/Radius: 8.00 |
| 217 | `Roid_Lrg_Grey` | 1965 | Object | -6731.94,-184.77,-3089.44 | 334,44,140 | Scale/Radius: 9.00 |
| 218 | `Roid_Lrg_Grey` | 1966 | Object | -6116.29,127.03,-2957.95 | 251,16,503 | Scale/Radius: 3.00 |
| 219 | `Roid_SM_Grey_Points` | 1967 | Object | -6069.65,-404.18,-3069.21 | 418,71,473 | Scale/Radius: 8.00 |
| 220 | `Asteroid_2` | 1968 | Object | -6564.03,427.27,-3878.35 | 345,74,97 | Scale/Radius: 3.00 |
| 221 | `Roid_SM_Grey_Points` | 1969 | Object | -6629.33,311.79,-2947.84 | 304,248,417 | Scale/Radius: 2.00 |
| 222 | `Asteroid_2` | 1970 | Object | -6106.97,-11.55,-3180.47 | 283,454,387 | Scale/Radius: 8.00 |
| 223 | `Asteroid_2` | 1971 | Object | -6489.41,150.12,-3615.38 | 33,447,418 | Scale/Radius: 6.00 |
| 224 | `Asteroid_2` | 1972 | Object | -8709.46,-92.38,-2148.81 | 223,188,82 | Scale/Radius: 8.00 |
| 225 | `Roid_Lrg_Grey` | 1975 | Object | -8672.15,161.67,-2067.90 | 470,426,152 | Scale/Radius: 1.00 |
| 226 | `Asteroid_2` | 1976 | Object | -8317.69,11.55,-2361.21 | 187,279,147 | Scale/Radius: 7.00 |
| 227 | `Roid_SM_Grey_Points` | 1977 | Object | -8951.99,-450.37,-1865.61 | 138,212,107 | Scale/Radius: 6.00 |
| 228 | `Bora_Mine` | 1978 | Interactive | -8625.51,11.55,-2209.50 | 505,409,68 | None |
| 229 | `Roid_Sm_Grey` | 1979 | Object | -8979.97,-450.37,-1734.13 | 452,112,384 | Scale/Radius: 8.00 |
| 230 | `Roid_Lrg_Grey` | 1981 | Object | -8644.16,-184.77,-1734.13 | 334,44,140 | Scale/Radius: 9.00 |
| 231 | `Roid_Lrg_Grey` | 1982 | Object | -8028.52,127.03,-1602.64 | 251,16,503 | Scale/Radius: 3.00 |
| 232 | `Roid_SM_Grey_Points` | 1983 | Object | -7981.88,-404.18,-1713.90 | 418,71,473 | Scale/Radius: 8.00 |
| 233 | `Asteroid_2` | 1984 | Object | -8476.26,427.27,-2523.04 | 345,74,97 | Scale/Radius: 3.00 |
| 234 | `Roid_SM_Grey_Points` | 1985 | Object | -8541.56,311.79,-1592.53 | 304,248,417 | Scale/Radius: 2.00 |
| 235 | `Asteroid_2` | 1986 | Object | -8019.19,-11.55,-1825.16 | 283,454,387 | Scale/Radius: 8.00 |
| 236 | `Asteroid_2` | 1987 | Object | -8401.64,150.12,-2260.07 | 33,447,418 | Scale/Radius: 6.00 |
| 237 | `Asteroid_2` | 1988 | Object | -6981.78,-92.38,-5383.67 | 223,188,82 | Scale/Radius: 8.00 |
| 238 | `Roid_Lrg_Grey` | 1991 | Object | -7189.00,161.67,-5365.14 | 470,426,152 | Scale/Radius: 1.00 |
| 239 | `Asteroid_2` | 1992 | Object | -6834.54,11.55,-5658.45 | 187,279,147 | Scale/Radius: 7.00 |
| 240 | `Roid_SM_Grey_Points` | 1993 | Object | -7468.84,-450.37,-5162.86 | 138,212,107 | Scale/Radius: 6.00 |
| 241 | `Bora_Mine` | 1994 | Interactive | -7142.37,11.55,-5506.74 | 505,409,68 | None |
| 242 | `Roid_Sm_Grey` | 1995 | Object | -7496.83,-450.37,-5031.37 | 452,112,384 | Scale/Radius: 8.00 |
| 243 | `Roid_Lrg_Grey` | 1997 | Object | -7161.02,-184.77,-5031.37 | 334,44,140 | Scale/Radius: 9.00 |
| 244 | `Roid_Lrg_Grey` | 1998 | Object | -6545.38,127.03,-4899.89 | 251,16,503 | Scale/Radius: 3.00 |
| 245 | `Roid_SM_Grey_Points` | 1999 | Object | -6498.74,-404.18,-5011.14 | 418,71,473 | Scale/Radius: 8.00 |
| 246 | `Asteroid_2` | 2000 | Object | -6993.12,427.27,-5820.28 | 345,74,97 | Scale/Radius: 3.00 |
| 247 | `Roid_SM_Grey_Points` | 2001 | Object | -7058.41,311.79,-4889.77 | 304,248,417 | Scale/Radius: 2.00 |
| 248 | `Asteroid_2` | 2002 | Object | -6536.05,-11.55,-5122.40 | 283,454,387 | Scale/Radius: 8.00 |
| 249 | `Asteroid_2` | 2003 | Object | -6918.50,150.12,-5557.31 | 33,447,418 | Scale/Radius: 6.00 |
| 250 | `Asteroid_2` | 2008 | Object | -9278.46,11.55,-2957.95 | 187,279,147 | Scale/Radius: 7.00 |
| 251 | `Roid_Lrg_Grey` | 2014 | Object | -8989.30,127.03,-2199.38 | 251,16,503 | Scale/Radius: 3.00 |
| 252 | `Roid_SM_Grey_Points` | 2015 | Object | -8942.66,-404.18,-2310.64 | 418,71,473 | Scale/Radius: 8.00 |
| 253 | `Asteroid_2` | 2016 | Object | -9437.04,427.27,-3119.78 | 345,74,97 | Scale/Radius: 3.00 |
| 254 | `Asteroid_2` | 2018 | Object | -8979.97,-11.55,-2421.90 | 283,454,387 | Scale/Radius: 8.00 |
| 255 | `Asteroid_2` | 2019 | Object | -9362.41,150.12,-2856.81 | 33,447,418 | Scale/Radius: 6.00 |
| 256 | `Asteroid_2` | 2020 | Object | -5611.74,-92.38,-2871.50 | 223,188,82 | Scale/Radius: 8.00 |
| 257 | `Roid_Lrg_Grey` | 2023 | Object | -5577.90,161.67,-2798.12 | 470,426,152 | Scale/Radius: 1.00 |
| 258 | `Asteroid_2` | 2024 | Object | -5222.59,11.55,-3091.65 | 187,279,147 | Scale/Radius: 7.00 |
| 259 | `Roid_SM_Grey_Points` | 2025 | Object | -5865.53,-450.37,-2596.31 | 138,212,107 | Scale/Radius: 6.00 |
| 260 | `Bora_Mine` | 2026 | Interactive | -5544.06,11.55,-2926.54 | 505,409,68 | None |
| 261 | `Roid_Sm_Grey` | 2027 | Object | -5882.45,-450.37,-2467.89 | 452,112,384 | Scale/Radius: 8.00 |
| 262 | `Roid_Lrg_Grey` | 2029 | Object | -5544.06,-184.77,-2449.55 | 334,44,140 | Scale/Radius: 9.00 |
| 263 | `Asteroid_2` | 2032 | Object | -5391.79,427.27,-3238.41 | 345,74,97 | Scale/Radius: 3.00 |
| 264 | `Roid_SM_Grey_Points` | 2033 | Object | -5442.55,311.79,-2321.13 | 304,248,417 | Scale/Radius: 2.00 |
| 265 | `Asteroid_2` | 2035 | Object | -5307.19,150.12,-2981.57 | 33,447,418 | Scale/Radius: 6.00 |
| 266 | `Asteroid_2` | 2036 | Object | -5950.13,-92.38,-3183.38 | 223,188,82 | Scale/Radius: 8.00 |
| 267 | `Roid_Lrg_Grey` | 2039 | Object | -5916.29,161.67,-3109.99 | 470,426,152 | Scale/Radius: 1.00 |
| 268 | `Asteroid_2` | 2040 | Object | -5560.98,11.55,-3403.52 | 187,279,147 | Scale/Radius: 7.00 |
| 269 | `Roid_SM_Grey_Points` | 2041 | Object | -6203.92,-450.37,-2908.19 | 138,212,107 | Scale/Radius: 6.00 |
| 270 | `Bora_Mine` | 2042 | Interactive | -5882.45,11.55,-3238.41 | 505,409,68 | None |
| 271 | `Roid_Sm_Grey` | 2043 | Object | -6220.84,-450.37,-2779.77 | 452,112,384 | Scale/Radius: 8.00 |
| 272 | `Roid_Lrg_Grey` | 2045 | Object | -5882.45,-184.77,-2761.43 | 334,44,140 | Scale/Radius: 9.00 |
| 273 | `Roid_Lrg_Grey` | 2046 | Object | -5273.35,127.03,-2633.01 | 251,16,503 | Scale/Radius: 3.00 |
| 274 | `Roid_SM_Grey_Points` | 2047 | Object | -5239.51,-404.18,-2743.08 | 418,71,473 | Scale/Radius: 8.00 |
| 275 | `Asteroid_2` | 2048 | Object | -5730.18,427.27,-3550.29 | 345,74,97 | Scale/Radius: 3.00 |
| 276 | `Roid_SM_Grey_Points` | 2049 | Object | -5780.93,311.79,-2633.01 | 304,248,417 | Scale/Radius: 2.00 |
| 277 | `Asteroid_2` | 2050 | Object | -5273.35,-11.55,-2853.15 | 283,454,387 | Scale/Radius: 8.00 |
| 278 | `Asteroid_2` | 2051 | Object | -5645.58,150.12,-3293.45 | 33,447,418 | Scale/Radius: 6.00 |
| 279 | `Asteroid_2` | 2052 | Object | -7168.32,-92.38,-1055.28 | 223,188,82 | Scale/Radius: 8.00 |
| 280 | `Roid_Lrg_Grey` | 2055 | Object | -7134.49,161.67,-981.90 | 470,426,152 | Scale/Radius: 1.00 |
| 281 | `Asteroid_2` | 2056 | Object | -6779.18,11.55,-1275.43 | 187,279,147 | Scale/Radius: 7.00 |
| 282 | `Roid_SM_Grey_Points` | 2057 | Object | -7422.12,-450.37,-780.09 | 138,212,107 | Scale/Radius: 6.00 |
| 283 | `Bora_Mine` | 2058 | Interactive | -7100.65,11.55,-1110.32 | 505,409,68 | None |
| 284 | `Roid_Sm_Grey` | 2059 | Object | -7439.03,-450.37,-651.68 | 452,112,384 | Scale/Radius: 8.00 |
| 285 | `Asteroid_2` | 2064 | Object | -6948.37,427.27,-1422.19 | 345,74,97 | Scale/Radius: 3.00 |
| 286 | `Asteroid_2` | 2067 | Object | -6863.78,150.12,-1165.35 | 33,447,418 | Scale/Radius: 6.00 |
| 287 | `Asteroid_2` | 2068 | Object | -6728.42,-92.38,-1477.23 | 223,188,82 | Scale/Radius: 8.00 |
| 288 | `Roid_Lrg_Grey` | 2071 | Object | -6694.58,161.67,-1403.85 | 470,426,152 | Scale/Radius: 1.00 |
| 289 | `Asteroid_2` | 2072 | Object | -6339.27,11.55,-1697.38 | 187,279,147 | Scale/Radius: 7.00 |
| 290 | `Roid_SM_Grey_Points` | 2073 | Object | -6982.21,-450.37,-1202.04 | 138,212,107 | Scale/Radius: 6.00 |
| 291 | `Bora_Mine` | 2074 | Interactive | -6660.74,11.55,-1532.27 | 505,409,68 | None |
| 292 | `Roid_Sm_Grey` | 2075 | Object | -6999.13,-450.37,-1073.63 | 452,112,384 | Scale/Radius: 8.00 |
| 293 | `Roid_Lrg_Grey` | 2077 | Object | -6660.74,-184.77,-1055.28 | 334,44,140 | Scale/Radius: 9.00 |
| 294 | `Asteroid_2` | 2080 | Object | -6508.47,427.27,-1844.14 | 345,74,97 | Scale/Radius: 3.00 |
| 295 | `Roid_SM_Grey_Points` | 2081 | Object | -6559.23,311.79,-926.86 | 304,248,417 | Scale/Radius: 2.00 |
| 296 | `Asteroid_2` | 2083 | Object | -6423.87,150.12,-1587.30 | 33,447,418 | Scale/Radius: 6.00 |
| 297 | `Asteroid_2` | 2084 | Object | -7303.68,-92.38,-1789.11 | 223,188,82 | Scale/Radius: 8.00 |
| 298 | `Roid_Lrg_Grey` | 2087 | Object | -7269.84,161.67,-1715.72 | 470,426,152 | Scale/Radius: 1.00 |
| 299 | `Asteroid_2` | 2088 | Object | -6914.53,11.55,-2009.25 | 187,279,147 | Scale/Radius: 7.00 |
| 300 | `Roid_SM_Grey_Points` | 2089 | Object | -7557.47,-450.37,-1513.92 | 138,212,107 | Scale/Radius: 6.00 |
| 301 | `Bora_Mine` | 2090 | Interactive | -7236.00,11.55,-1844.14 | 505,409,68 | None |
| 302 | `Roid_Sm_Grey` | 2091 | Object | -7574.39,-450.37,-1385.50 | 452,112,384 | Scale/Radius: 8.00 |
| 303 | `Roid_Lrg_Grey` | 2093 | Object | -7236.00,-184.77,-1367.16 | 334,44,140 | Scale/Radius: 9.00 |
| 304 | `Roid_Lrg_Grey` | 2094 | Object | -6626.90,127.03,-1238.74 | 251,16,503 | Scale/Radius: 3.00 |
| 305 | `Roid_SM_Grey_Points` | 2095 | Object | -6593.06,-404.18,-1348.81 | 418,71,473 | Scale/Radius: 8.00 |
| 306 | `Asteroid_2` | 2096 | Object | -7083.73,427.27,-2156.02 | 345,74,97 | Scale/Radius: 3.00 |
| 307 | `Roid_SM_Grey_Points` | 2097 | Object | -7134.49,311.79,-1238.74 | 304,248,417 | Scale/Radius: 2.00 |
| 308 | `Asteroid_2` | 2098 | Object | -6626.90,-11.55,-1458.88 | 283,454,387 | Scale/Radius: 8.00 |
| 309 | `Asteroid_2` | 2099 | Object | -6999.13,150.12,-1899.18 | 33,447,418 | Scale/Radius: 6.00 |
| 310 | `Roid_Sm_Grey` | 2107 | Object | -6016.33,-450.37,-4964.87 | 452,112,384 | Scale/Radius: 8.00 |
| 311 | `Roid_SM_Grey_Points` | 2121 | Object | -6457.71,-450.37,-5421.54 | 138,212,107 | Scale/Radius: 6.00 |
| 312 | `Roid_Sm_Grey` | 2123 | Object | -6474.63,-450.37,-5293.12 | 452,112,384 | Scale/Radius: 8.00 |
| 313 | `Navigational_Bouy` | 2139 | Interactive | -7327.05,0.00,-3070.98 | 87,0,0 | None |
| 314 | `Bora_Mace` | 2146 | Interactive | -11027.82,187.81,-9626.60 | 14,0,0 | group/role: FG_HONOR / 0; waypoint: Waypoint 4 (tag 153, 2 point(s)), starting point 0, arrival event value 10027008 |
| 315 | `Bora_Leviathan` | 2145 | Interactive | -10805.59,187.81,-9614.76 | 14,0,0 | label: bfbf_08; group/role: FG_FORNAX / 0; waypoint: Waypoint 4 (tag 153, 2 point(s)), starting point 0, arrival event value 10027008 |
| 316 | `Bora_Leviathan` | 2148 | Interactive | -10872.62,187.81,-9503.65 | 14,0,0 | group/role: FG_FORNAX / 0; waypoint: Waypoint 4 (tag 153, 2 point(s)), starting point 0, arrival event value 10027008 |
| 317 | `Bora_Mace` | 2144 | Interactive | -10746.67,187.81,-9470.32 | 14,0,0 | group/role: FG_FORNAX / 0; waypoint: Waypoint 4 (tag 153, 2 point(s)), starting point 0, arrival event value 10027008 |
| 318 | `Bora_Mace` | 2147 | Interactive | -10813.70,187.81,-9359.20 | 14,0,0 | label: bfbf_08; group/role: FG_FORNAX / 0; waypoint: Waypoint 4 (tag 153, 2 point(s)), starting point 0, arrival event value 10027008 |
| 319 | `Bora_Claymore` | 1866 | Interactive | -11094.93,187.81,-9740.79 | 14,0,0 | label: bfbf_08; group/role: FG_HONOR / 0; waypoint: Waypoint 4 (tag 153, 2 point(s)), starting point 0, arrival event value 10027008 |
| 320 | `Bora_Claymore` | 1868 | Interactive | -10916.94,187.81,-9740.78 | 14,0,0 | group/role: FG_HONOR / 0; waypoint: Waypoint 4 (tag 153, 2 point(s)), starting point 0, arrival event value 10027008 |
| 321 | `GalSpan_Frigate` | 1066 | Interactive | -9174.44,178.25,-4102.16 | 321,0,0 | secondary groups: none, APUS; waypoint: Waypoint 5 (tag 152, 3 point(s)), starting point 0, arrival event value 9961472 |
| 322 | `GalSpan_Frigate` | 1067 | Interactive | -7699.63,178.25,-4875.14 | 333,0,0 | secondary groups: none, APHRODITE; waypoint: Waypoint 6 (tag 151, 3 point(s)), starting point 0, arrival event value 9895936 |
| 323 | `Bora_Carrier` | 1864 | Interactive | -10292.10,187.81,-9728.42 | 14,0,0 | secondary groups: none, FORTRESS; waypoint: Waypoint 3 (tag 154, 2 point(s)), starting point 0, arrival event value 10092544 |
