## Git

4/21/2020
`git merge no-ff`. The `no-ff` flag prevents `git merge` from executing a "fast-forward". This forces git to create a `merge commit`, even if it could've done the merge without it.


## Ruby

4/21/2020
You can't add an attribute to an existing has like this:
```ruby
my_hash = { name: "Anthony" }
my_hash.age = 30
# => undefined method 'age='
```
You need to use `merge`:
```ruby
my_hash = { name: "Anthony" }
my_hash.merge! name: 30
```
