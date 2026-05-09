# Tachyon: The Fringe EARTH05.SPX

Back to [SPX Mission Index](../SPX%20Mission%20Index.md)

## Summary

| Property | Value |
| --- | --- |
| SPX File | `EARTH05.SPX` |
| Sector | `QUAD_05` |
| Backdrop | `EARTH05.BDF` |
| Region | 0 |
| Sector ID | 4 |
| SectorHazardFlags | None (0x00000000) |
| BWBaseSector | None (0) |
| BWBaseSectorRace | AGT/None (0) |
| Object Types | 6 |
| Entities | 97 |
| Events | 1 |
| Waypoints | 2 |
| Child Sectors | 1 |
| Scripts | 0 |
| Scenes | 1 |

## Resources

| List | Values |
| --- | --- |
| Object Types | `0: Halley_Research_Base`, `1: Roid_XL_Green`, `2: Roid_Med_Green`, `3: Shuttle_Medium`, `4: Mega_Gate`, `5: Hyper_Gate` |
| Scripts | None |
| Scenes | `EARTH05.SEN` |
| Labels | `ESC1`, `ESC2`, `argo`, `Escort3`, `Escort2`, `Escort4`, `Escort1`, `SOLShuttle`, `Imposter`, `Sol1`, `Sol4`, `Sol7`, `BLFT`, `SOLCapShip` |
| Aliases | `Todd01` |
| Groups | `DELSEMME`, `CONT_033`, `SEKANINA`, `HALLEY_RESEARCH` |
| Child Sectors | [earth05A.spx](EARTH05A.md) |

## Events

### Event 0

**Trigger**

- Area/player/sector/dock/time event: subject 0, op 3, value 0

**Action**

- Object spawn/action: Shuttle_Medium (object 2, id 1064), subtype 8, param 4
- Object spawn/action: Shuttle_Medium (object 3, id 1065), subtype 8, param 4

## Waypoints

### Waypoint 0

- Tag: `4`
- Members: `Shuttle_Medium (object 2, id 1064, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (175.56, -1416.00, -9.20) | None |
| 1 | (460.00, -1426.00, 334.60) | None |
| 2 | (1020.00, -1773.32, 197.14) | None |
| 3 | (3454.29, -1776.79, 200.00) | None |
| 4 | (3450.00, -1223.05, 2873.88) | None |
| 5 | (2543.00, 36.81, 3592.67) | None |
| 6 | (2637.30, -144.07, 3621.02) | None |
| 7 | (2605.81, -146.07, 3657.09) | None |
| 8 | (1005.32, 615.14, 3729.17) | on arrival activate current object (raw param -1 ignored) |

### Waypoint 1

- Tag: `3`
- Members: `Shuttle_Medium (object 3, id 1065, starts at point 0)`
| Point | Position | On Arrival |
| ---: | --- | --- |
| 0 | (218.86, -1414.01, -54.97) | None |
| 1 | (716.46, -1585.70, -3.87) | None |
| 2 | (863.91, -1624.28, -29.00) | None |
| 3 | (1537.26, -1671.50, 790.01) | None |
| 4 | (2173.00, -1787.70, 2866.79) | None |
| 5 | (2630.00, 213.17, 3821.75) | None |
| 6 | (2864.01, -168.50, 2954.01) | on arrival activate current object (raw param -1 ignored) |

## Spawn Lists

None

## Objects

| # | Object | ID | Type | Pos (X,Y,Z) | Rot (A,B,C) | Details |
| ---: | --- | ---: | --- | --- | --- | --- |
| 0 | `Hyper_Gate` | 1 | Gate | -1710.55,632.04,-2764.46 | 64,466,0 | Gate SPX: [Earth01.spx](EARTH01.md) |
| 1 | `Mega_Gate` | 926 | Gate | 2077.08,-2518.73,681.40 | 320,55,0 | Gate SPX: `hub01.spx` |
| 2 | `Shuttle_Medium` | 1064 | Interactive | 81.81,-1416.00,-113.57 | 64,0,0 | label: ESC1; group/role: none / 1; secondary groups: CONT_033, DELSEMME; waypoint: Waypoint 0 (tag 4, 9 point(s)), starting point 0, arrival event value 262144 |
| 3 | `Shuttle_Medium` | 1065 | Interactive | 120.68,-1416.00,-157.06 | 64,0,0 | label: ESC2; group/role: none / 1; secondary groups: CONT_033, SEKANINA; waypoint: Waypoint 1 (tag 3, 7 point(s)), starting point 0, arrival event value 196608 |
| 4 | `Roid_Med_Green` | 876 | Object | 3353.48,884.61,3567.72 | 13,322,136 | Scale/Radius: 1.00 |
| 5 | `Roid_Med_Green` | 822 | Object | 2537.54,117.04,3749.80 | 393,222,384 | Scale/Radius: 1.00 |
| 6 | `Roid_Med_Green` | 824 | Object | 2511.05,32.21,3569.07 | 395,369,182 | Scale/Radius: 1.00 |
| 7 | `Roid_Med_Green` | 826 | Object | 2702.98,-11.79,3484.28 | 239,335,503 | Scale/Radius: 1.00 |
| 8 | `Roid_Med_Green` | 828 | Object | 2613.03,102.07,3612.08 | 481,375,266 | Scale/Radius: 1.00 |
| 9 | `Roid_Med_Green` | 830 | Object | 2618.39,133.83,3318.03 | 385,11,185 | Scale/Radius: 1.00 |
| 10 | `Roid_Med_Green` | 832 | Object | 2609.29,81.66,3458.64 | 354,463,85 | Scale/Radius: 1.00 |
| 11 | `Roid_Med_Green` | 834 | Object | 2658.33,-120.67,3580.26 | 268,431,303 | Scale/Radius: 1.00 |
| 12 | `Roid_Med_Green` | 836 | Object | 2712.05,55.80,3411.70 | 376,56,30 | Scale/Radius: 1.00 |
| 13 | `Roid_Med_Green` | 838 | Object | 2452.02,-117.04,3319.52 | 152,283,254 | Scale/Radius: 1.00 |
| 14 | `Roid_Med_Green` | 840 | Object | 2868.94,32.66,3627.55 | 207,175,44 | Scale/Radius: 1.00 |
| 15 | `Roid_Med_Green` | 842 | Object | 3371.21,56.25,3630.82 | 27,441,81 | Scale/Radius: 1.00 |
| 16 | `Roid_Med_Green` | 844 | Object | 2308.09,-452.74,3347.97 | 26,52,225 | Scale/Radius: 1.00 |
| 17 | `Roid_Med_Green` | 846 | Object | 2624.42,213.21,3655.23 | 65,460,129 | Scale/Radius: 1.00 |
| 18 | `Roid_Med_Green` | 848 | Object | 2749.56,22.68,3517.25 | 134,329,197 | Scale/Radius: 1.00 |
| 19 | `Roid_Med_Green` | 850 | Object | 2856.03,523.96,3247.19 | 105,161,107 | Scale/Radius: 1.00 |
| 20 | `Roid_Med_Green` | 852 | Object | 2822.45,-262.37,2909.99 | 267,496,231 | Scale/Radius: 1.00 |
| 21 | `Roid_Med_Green` | 854 | Object | 2871.00,-102.07,2962.76 | 450,183,244 | Scale/Radius: 1.00 |
| 22 | `Roid_Med_Green` | 856 | Object | 2717.34,-137.45,3897.84 | 406,343,14 | Scale/Radius: 1.00 |
| 23 | `Roid_Med_Green` | 858 | Object | 3435.13,-110.24,3295.53 | 197,155,501 | Scale/Radius: 1.00 |
| 24 | `Roid_Med_Green` | 860 | Object | 2517.84,90.73,3947.85 | 65,301,47 | Scale/Radius: 1.00 |
| 25 | `Roid_Med_Green` | 862 | Object | 2573.00,-65.32,3240.88 | 302,286,388 | Scale/Radius: 1.00 |
| 26 | `Roid_Med_Green` | 864 | Object | 2696.66,-223.19,4289.98 | 103,352,385 | Scale/Radius: 1.00 |
| 27 | `Roid_Med_Green` | 866 | Object | 2965.34,-841.96,3433.63 | 505,333,504 | Scale/Radius: 1.00 |
| 28 | `Roid_Med_Green` | 868 | Object | 3255.66,-145.17,3338.35 | 164,32,124 | Scale/Radius: 1.00 |
| 29 | `Roid_Med_Green` | 870 | Object | 1543.47,440.04,4030.47 | 351,121,487 | Scale/Radius: 1.00 |
| 30 | `Roid_Med_Green` | 872 | Object | 2451.69,-1016.16,3577.76 | 211,476,471 | Scale/Radius: 1.00 |
| 31 | `Roid_Med_Green` | 874 | Object | 2081.54,396.94,3457.11 | 220,48,42 | Scale/Radius: 1.00 |
| 32 | `Roid_Med_Green` | 878 | Object | 3278.81,117.04,2649.27 | 300,66,471 | Scale/Radius: 1.00 |
| 33 | `Roid_Med_Green` | 880 | Object | 1420.49,704.96,3676.14 | 176,322,454 | Scale/Radius: 1.00 |
| 34 | `Roid_Med_Green` | 882 | Object | 2907.22,381.06,2685.97 | 72,188,69 | Scale/Radius: 1.00 |
| 35 | `Roid_Med_Green` | 884 | Object | 2909.65,-1117.78,3545.78 | 85,267,265 | Scale/Radius: 1.00 |
| 36 | `Roid_Med_Green` | 886 | Object | 2928.24,-1317.38,3886.46 | 364,494,267 | Scale/Radius: 1.00 |
| 37 | `Roid_Med_Green` | 888 | Object | 1036.62,-1005.28,3591.67 | 471,11,8 | Scale/Radius: 1.00 |
| 38 | `Roid_Med_Green` | 890 | Object | 2815.40,-1420.82,3247.40 | 275,104,0 | Scale/Radius: 1.00 |
| 39 | `Roid_Med_Green` | 892 | Object | 3457.76,571.59,4175.55 | 102,0,208 | Scale/Radius: 1.00 |
| 40 | `Roid_Med_Green` | 894 | Object | 883.25,594.27,3574.39 | 403,156,90 | Scale/Radius: 1.00 |
| 41 | `Roid_Med_Green` | 896 | Object | 2197.71,308.48,3754.74 | 415,431,379 | Scale/Radius: 1.00 |
| 42 | `Roid_Med_Green` | 898 | Object | 1145.29,-234.53,2566.23 | 397,402,105 | Scale/Radius: 1.00 |
| 43 | `Roid_Med_Green` | 900 | Object | 1002.44,615.14,3720.80 | 168,214,31 | Scale/Radius: 1.00 |
| 44 | `Roid_Med_Green` | 902 | Object | 2083.54,-1480.24,3890.08 | 191,113,385 | Scale/Radius: 1.00 |
| 45 | `Roid_Med_Green` | 904 | Object | 3410.97,-816.56,1951.26 | 123,454,300 | Scale/Radius: 1.00 |
| 46 | `Roid_Med_Green` | 906 | Object | 3280.47,1164.51,3276.97 | 306,376,457 | Scale/Radius: 1.00 |
| 47 | `Roid_Med_Green` | 908 | Object | 2457.51,801.59,3638.01 | 53,103,162 | Scale/Radius: 1.00 |
| 48 | `Roid_Med_Green` | 910 | Object | 3976.85,190.53,4041.39 | 319,31,419 | Scale/Radius: 1.00 |
| 49 | `Roid_Med_Green` | 912 | Object | 3528.84,52.17,2677.02 | 57,65,455 | Scale/Radius: 1.00 |
| 50 | `Roid_XL_Green` | 849 | Object | 2990.49,449.11,4007.69 | 365,353,171 | Scale/Radius: 1.00 |
| 51 | `Roid_XL_Green` | 823 | Object | 2610.67,-60.79,3568.89 | 222,157,182 | Scale/Radius: 1.00 |
| 52 | `Roid_XL_Green` | 825 | Object | 2533.82,180.10,3401.31 | 408,412,15 | Scale/Radius: 1.00 |
| 53 | `Roid_XL_Green` | 827 | Object | 2539.65,198.24,3652.11 | 34,194,389 | Scale/Radius: 1.00 |
| 54 | `Roid_XL_Green` | 829 | Object | 2493.60,102.07,3705.86 | 93,487,416 | Scale/Radius: 1.00 |
| 55 | `Roid_XL_Green` | 831 | Object | 2470.22,231.81,3609.90 | 320,423,144 | Scale/Radius: 1.00 |
| 56 | `Roid_XL_Green` | 833 | Object | 2687.59,-125.21,3595.91 | 86,228,421 | Scale/Radius: 1.00 |
| 57 | `Roid_XL_Green` | 835 | Object | 2607.80,203.69,3370.96 | 317,66,214 | Scale/Radius: 1.00 |
| 58 | `Roid_XL_Green` | 837 | Object | 2476.68,-528.95,3543.78 | 295,427,61 | Scale/Radius: 1.00 |
| 59 | `Roid_XL_Green` | 839 | Object | 2965.30,449.11,3442.66 | 90,459,407 | Scale/Radius: 1.00 |
| 60 | `Roid_XL_Green` | 841 | Object | 2415.18,-94.36,3337.11 | 433,404,455 | Scale/Radius: 1.00 |
| 61 | `Roid_XL_Green` | 843 | Object | 2573.79,137.91,3722.54 | 13,488,416 | Scale/Radius: 1.00 |
| 62 | `Roid_XL_Green` | 845 | Object | 2575.61,-541.65,3488.47 | 339,91,360 | Scale/Radius: 1.00 |
| 63 | `Roid_XL_Green` | 847 | Object | 2219.02,-293.05,3621.81 | 281,10,337 | Scale/Radius: 1.00 |
| 64 | `Roid_XL_Green` | 851 | Object | 2146.07,136.09,3639.59 | 452,389,380 | Scale/Radius: 1.00 |
| 65 | `Roid_XL_Green` | 853 | Object | 3142.12,473.61,3859.91 | 102,283,42 | Scale/Radius: 1.00 |
| 66 | `Roid_XL_Green` | 855 | Object | 3389.69,-265.38,3290.92 | 495,464,257 | Scale/Radius: 1.00 |
| 67 | `Roid_XL_Green` | 857 | Object | 2205.73,-247.69,3699.25 | 208,465,434 | Scale/Radius: 1.00 |
| 68 | `Roid_XL_Green` | 859 | Object | 2235.46,3.63,3429.58 | 206,337,208 | Scale/Radius: 1.00 |
| 69 | `Roid_XL_Green` | 861 | Object | 3070.93,205.05,3720.67 | 128,8,340 | Scale/Radius: 1.00 |
| 70 | `Roid_XL_Green` | 863 | Object | 2265.70,480.86,3314.65 | 210,177,24 | Scale/Radius: 1.00 |
| 71 | `Roid_XL_Green` | 865 | Object | 2597.38,773.01,3519.31 | 134,137,349 | Scale/Radius: 1.00 |
| 72 | `Roid_XL_Green` | 867 | Object | 2232.26,-1023.42,3807.44 | 432,213,72 | Scale/Radius: 1.00 |
| 73 | `Roid_XL_Green` | 869 | Object | 3796.26,99.80,3221.17 | 311,90,94 | Scale/Radius: 1.00 |
| 74 | `Roid_XL_Green` | 871 | Object | 2039.14,673.66,2915.70 | 89,229,270 | Scale/Radius: 1.00 |
| 75 | `Roid_XL_Green` | 873 | Object | 2553.04,13.61,2340.86 | 38,195,293 | Scale/Radius: 1.00 |
| 76 | `Roid_XL_Green` | 875 | Object | 3876.02,-288.52,4280.80 | 258,71,89 | Scale/Radius: 1.00 |
| 77 | `Roid_XL_Green` | 877 | Object | 2841.13,1693.00,3899.15 | 37,329,193 | Scale/Radius: 1.00 |
| 78 | `Roid_XL_Green` | 879 | Object | 2917.98,-530.76,4003.22 | 285,164,90 | Scale/Radius: 1.00 |
| 79 | `Roid_XL_Green` | 881 | Object | 2615.83,-146.07,3633.02 | 328,437,130 | Scale/Radius: 1.00 |
| 80 | `Roid_XL_Green` | 883 | Object | 4172.35,663.68,3760.57 | 349,481,382 | Scale/Radius: 1.00 |
| 81 | `Roid_XL_Green` | 885 | Object | 2632.14,-1140.01,1744.03 | 226,14,501 | Scale/Radius: 1.00 |
| 82 | `Roid_XL_Green` | 887 | Object | 2127.96,-312.11,3521.68 | 437,38,116 | Scale/Radius: 1.00 |
| 83 | `Roid_XL_Green` | 889 | Object | 3664.90,780.27,3570.66 | 389,153,235 | Scale/Radius: 1.00 |
| 84 | `Roid_XL_Green` | 891 | Object | 3669.09,-102.07,2549.61 | 344,474,44 | Scale/Radius: 1.00 |
| 85 | `Roid_XL_Green` | 893 | Object | 1618.96,-881.89,2295.93 | 445,192,4 | Scale/Radius: 1.00 |
| 86 | `Roid_XL_Green` | 895 | Object | 1713.11,-308.48,3315.51 | 485,59,36 | Scale/Radius: 1.00 |
| 87 | `Roid_XL_Green` | 897 | Object | 2845.75,-173.59,2914.91 | 75,275,139 | Scale/Radius: 1.00 |
| 88 | `Roid_XL_Green` | 899 | Object | 4109.01,-337.51,2962.31 | 230,477,237 | Scale/Radius: 1.00 |
| 89 | `Roid_XL_Green` | 901 | Object | 1176.27,-1533.32,3454.59 | 193,340,245 | Scale/Radius: 1.00 |
| 90 | `Roid_XL_Green` | 903 | Object | 1319.76,165.13,3321.37 | 142,456,10 | Scale/Radius: 1.00 |
| 91 | `Roid_XL_Green` | 905 | Object | 1209.19,-515.34,4220.21 | 26,118,164 | Scale/Radius: 1.00 |
| 92 | `Roid_XL_Green` | 907 | Object | 1982.77,228.64,4302.08 | 5,138,326 | Scale/Radius: 1.00 |
| 93 | `Roid_XL_Green` | 909 | Object | 1652.85,1143.18,3119.15 | 333,504,9 | Scale/Radius: 1.00 |
| 94 | `Roid_XL_Green` | 911 | Object | 3682.23,-99.80,2308.72 | 511,51,129 | Scale/Radius: 1.00 |
| 95 | `Roid_XL_Green` | 913 | Object | 780.43,544.37,4134.06 | 258,25,49 | Scale/Radius: 1.00 |
| 96 | `Halley_Research_Base` | 928 | Interactive | 85.57,-1463.00,-212.54 | 320,0,0 | secondary groups: none, HALLEY_RESEARCH |
