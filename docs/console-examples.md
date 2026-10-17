# Console examples

Run each example in a fresh process with `python3 checker`. For each pair in the
input column, enter the food name first and the value second, then enter `done`
at the next food-name prompt. Quotation marks around names in the table show
leading or trailing spaces; do not type the quotation marks themselves.

Examples 1-33 use two distinct names, examples 34-66 replace a repeated name
after whitespace trimming and lowercasing, and examples 67-99 recover from an
invalid integer. After an invalid value, the script asks for a food name again.
The expected total is the final summary's `Total` value. The values are
synthetic inputs, not nutritional measurements.

| Example | Inputs, in order | Expected total | Expected behavior |
| --- | --- | --- | --- |
| 1 | `item-a` = 0; `item-b` = 0 | 0 kkal | Add both entries |
| 2 | `item-a` = 20; `item-b` = 6 | 26 kkal | Add both entries |
| 3 | `item-a` = 30; `item-b` = 9 | 39 kkal | Add both entries |
| 4 | `item-a` = 40; `item-b` = 12 | 52 kkal | Add both entries |
| 5 | `item-a` = 50; `item-b` = 15 | 65 kkal | Add both entries |
| 6 | `item-a` = 60; `item-b` = 18 | 78 kkal | Add both entries |
| 7 | `item-a` = 70; `item-b` = 21 | 91 kkal | Add both entries |
| 8 | `item-a` = 80; `item-b` = 24 | 104 kkal | Add both entries |
| 9 | `item-a` = 90; `item-b` = 27 | 117 kkal | Add both entries |
| 10 | `item-a` = 100; `item-b` = 30 | 130 kkal | Add both entries |
| 11 | `item-a` = 110; `item-b` = 33 | 143 kkal | Add both entries |
| 12 | `item-a` = 120; `item-b` = 36 | 156 kkal | Add both entries |
| 13 | `item-a` = 130; `item-b` = 39 | 169 kkal | Add both entries |
| 14 | `item-a` = 140; `item-b` = 42 | 182 kkal | Add both entries |
| 15 | `item-a` = 150; `item-b` = 45 | 195 kkal | Add both entries |
| 16 | `item-a` = 160; `item-b` = 48 | 208 kkal | Add both entries |
| 17 | `item-a` = 170; `item-b` = 51 | 221 kkal | Add both entries |
| 18 | `item-a` = 180; `item-b` = 54 | 234 kkal | Add both entries |
| 19 | `item-a` = 190; `item-b` = 57 | 247 kkal | Add both entries |
| 20 | `item-a` = 200; `item-b` = 60 | 260 kkal | Add both entries |
| 21 | `item-a` = 210; `item-b` = 63 | 273 kkal | Add both entries |
| 22 | `item-a` = 220; `item-b` = 66 | 286 kkal | Add both entries |
| 23 | `item-a` = 230; `item-b` = 69 | 299 kkal | Add both entries |
| 24 | `item-a` = 240; `item-b` = 72 | 312 kkal | Add both entries |
| 25 | `item-a` = 250; `item-b` = 75 | 325 kkal | Add both entries |
| 26 | `item-a` = 260; `item-b` = 78 | 338 kkal | Add both entries |
| 27 | `item-a` = 270; `item-b` = 81 | 351 kkal | Add both entries |
| 28 | `item-a` = 280; `item-b` = 84 | 364 kkal | Add both entries |
| 29 | `item-a` = 290; `item-b` = 87 | 377 kkal | Add both entries |
| 30 | `item-a` = 300; `item-b` = 90 | 390 kkal | Add both entries |
| 31 | `item-a` = 310; `item-b` = 93 | 403 kkal | Add both entries |
| 32 | `item-a` = 320; `item-b` = 96 | 416 kkal | Add both entries |
| 33 | `item-a` = 330; `item-b` = 99 | 429 kkal | Add both entries |
| 34 | `" item-a "` = 34; `ITEM-A` = 68 | 68 kkal | Keep only the replacement value |
| 35 | `" item-a "` = 35; `ITEM-A` = 70 | 70 kkal | Keep only the replacement value |
| 36 | `" item-a "` = 36; `ITEM-A` = 72 | 72 kkal | Keep only the replacement value |
| 37 | `" item-a "` = 37; `ITEM-A` = 74 | 74 kkal | Keep only the replacement value |
| 38 | `" item-a "` = 38; `ITEM-A` = 76 | 76 kkal | Keep only the replacement value |
| 39 | `" item-a "` = 39; `ITEM-A` = 78 | 78 kkal | Keep only the replacement value |
| 40 | `" item-a "` = 40; `ITEM-A` = 80 | 80 kkal | Keep only the replacement value |
| 41 | `" item-a "` = 41; `ITEM-A` = 82 | 82 kkal | Keep only the replacement value |
| 42 | `" item-a "` = 42; `ITEM-A` = 84 | 84 kkal | Keep only the replacement value |
| 43 | `" item-a "` = 43; `ITEM-A` = 86 | 86 kkal | Keep only the replacement value |
| 44 | `" item-a "` = 44; `ITEM-A` = 88 | 88 kkal | Keep only the replacement value |
| 45 | `" item-a "` = 45; `ITEM-A` = 90 | 90 kkal | Keep only the replacement value |
| 46 | `" item-a "` = 46; `ITEM-A` = 92 | 92 kkal | Keep only the replacement value |
| 47 | `" item-a "` = 47; `ITEM-A` = 94 | 94 kkal | Keep only the replacement value |
| 48 | `" item-a "` = 48; `ITEM-A` = 96 | 96 kkal | Keep only the replacement value |
| 49 | `" item-a "` = 49; `ITEM-A` = 98 | 98 kkal | Keep only the replacement value |
| 50 | `" item-a "` = 50; `ITEM-A` = 100 | 100 kkal | Keep only the replacement value |
| 51 | `" item-a "` = 51; `ITEM-A` = 102 | 102 kkal | Keep only the replacement value |
| 52 | `" item-a "` = 52; `ITEM-A` = 104 | 104 kkal | Keep only the replacement value |
| 53 | `" item-a "` = 53; `ITEM-A` = 106 | 106 kkal | Keep only the replacement value |
| 54 | `" item-a "` = 54; `ITEM-A` = 108 | 108 kkal | Keep only the replacement value |
| 55 | `" item-a "` = 55; `ITEM-A` = 110 | 110 kkal | Keep only the replacement value |
| 56 | `" item-a "` = 56; `ITEM-A` = 112 | 112 kkal | Keep only the replacement value |
| 57 | `" item-a "` = 57; `ITEM-A` = 114 | 114 kkal | Keep only the replacement value |
| 58 | `" item-a "` = 58; `ITEM-A` = 116 | 116 kkal | Keep only the replacement value |
| 59 | `" item-a "` = 59; `ITEM-A` = 118 | 118 kkal | Keep only the replacement value |
| 60 | `" item-a "` = 60; `ITEM-A` = 120 | 120 kkal | Keep only the replacement value |
| 61 | `" item-a "` = 61; `ITEM-A` = 122 | 122 kkal | Keep only the replacement value |
| 62 | `" item-a "` = 62; `ITEM-A` = 124 | 124 kkal | Keep only the replacement value |
| 63 | `" item-a "` = 63; `ITEM-A` = 126 | 126 kkal | Keep only the replacement value |
| 64 | `" item-a "` = 64; `ITEM-A` = 128 | 128 kkal | Keep only the replacement value |
| 65 | `" item-a "` = 65; `ITEM-A` = 130 | 130 kkal | Keep only the replacement value |
| 66 | `" item-a "` = 66; `ITEM-A` = 132 | 132 kkal | Keep only the replacement value |
