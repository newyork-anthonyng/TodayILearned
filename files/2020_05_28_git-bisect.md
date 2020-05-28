`git bisect` lets you find out which commit broke your app.

```
# start the git bisect process
git bisect start

# mark that the current commit is bad
git bisect bad

# mark that a previous commit is good
git bisect good SOME_COMMIT_HASH
```

Then, git finds the midway point between the two commits. See if the application works or not.
If it works, then run `git bisect good`.
If it doesn't work, then run `git bisect bad`.

This process is repeated until the bad commit is found.

[Git bisect documentation](https://git-scm.com/docs/git-bisect)
