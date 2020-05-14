Ruby has keyword arguments. This allows you to pass arguments to a function without worrying about its order.

```ruby
def write(file:, data:)
	puts "file: #{file}"
	puts "data: #{data}"
end

write file: "first.csv", data: "type/csv"
# => file: first.csv
# => data: type/csv

# you can reorder arguments
write data: "type/csv", file: "first.csv"
# => file: first.csv
# => data: type/csv
```