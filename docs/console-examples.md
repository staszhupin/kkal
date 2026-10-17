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
