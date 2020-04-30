# 4/21/2020
---
`git merge no-ff`. The `no-ff` flag prevents `git merge` from executing a "fast-forward". This forces git to create a `merge commit`, even if it could've done the merge without it. 
&#35;Git

---
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
&#35;Ruby

# 4/28/2020
---
HereDoc's are a way to write large blocks of string.
```
execute <<-SQL
CREATE TYPE duration_unit AS ENUM ('year', 'month', 'week', 'day', 'hour', 'minute', 'second');
SQL
```
The `<<-{SOME_NAME}` starts the large block. The `{SOME_NAME}` at the end terminates the large block.
&#35;Ruby

---
If you're going to create a public facing API, make sure to version it.
&#35;API

# 4/29/2020
---
In vim visual mode, `gv` gets your last visual selection. This is valuable when I have to do the following:
1. Copy and paste block of code
2. Comment out original block of code
3. Modify the newly pasted block of code
