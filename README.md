# Simple calorie checker

A small Python console script that records food names and integer calorie
values, then prints the stored entries and their total. The source is in
[`checker`](checker).

## Run

Run the script with Python 3:

```sh
python3 checker
```

Enter a food name, then an integer calorie value. Enter `done` at the food-name
prompt to print the summary and finish. No third-party packages are required.

## Input behavior

- Food names are trimmed and converted to lowercase.
- Entering the same normalized food name replaces its previous calorie value.
- An invalid integer prints an error and returns to the food-name prompt.
- Zero and negative integer values are accepted by the current script.
- Entries are stored in memory and are not saved between runs.

## Examples

The [console examples](docs/console-examples.md) cover totals for distinct food
names, replacement of repeated names, and recovery after invalid numeric input.
The supplied numbers are synthetic inputs for demonstrating the script; they
are not nutritional measurements.
