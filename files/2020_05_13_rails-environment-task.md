Inside Rails rake tasks, your Rails environment (such as models and service classes) aren't automatically loaded.

You have to pass `:environment` as an argument to your rake task.

```ruby
desc "Pick a random user as the winner"
task :winner => :environment do
  puts "Winner: #{pick(User).name}"
end

# :environment gives you access to your User model
```

[StackOverflow](https://stackoverflow.com/questions/7044714/whats-the-environment-task-in-rake)