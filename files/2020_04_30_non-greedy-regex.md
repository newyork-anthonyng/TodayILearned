## non-greedy regular expressions

You have the below string:
```
import/some-random-hash/stonemaier-import.csv
```

You want to get the last segment of the CSV: `stonemaier-import.csv`

I tried using this regular expression, `\/.*\.csv`
But it's greedy. It returns `/some-random-hash/stonemaier-import.csv`.

Instead, use this regular expression, `[^\/]*\.csv`.
The `[^\/]*` captures everything that is not a `/` character.
