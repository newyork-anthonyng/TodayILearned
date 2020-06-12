https://apidock.com/rails/ActiveRecord/QueryMethods/where

In Rails, you can treat your SQL as a template. The `?` are placeholders that are replaced.

For example,
```ruby
User.where(["name = ? and email = ?", "Joe", "joe@example.com"])
# name = Joe and email = joe@example.com
```

You can also use named placeholders in the template. This is convenient when you have a lot of placeholders.
```ruby
User.where(["name = :name and email = :email", { name: "Joe", email: "joe@example.com" }])
# name = Joe and email = joe@example.com
