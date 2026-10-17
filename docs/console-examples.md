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
