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
