Ruby has a `starship` operator; `<=>`

It's a comparator operator, similar to `<` and `>`.
```ruby
a <=> b

  if a < b then return -1
  if a == b then return 0
  if a > b then return 1
  if a and b are not comparable then return nil
```

[StackOverflow](https://stackoverflow.com/questions/827649/what-is-the-ruby-spaceship-operator)
