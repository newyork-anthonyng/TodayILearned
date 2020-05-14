Ruby's double splt operator (`**`) is similar to JavaScript's [`rest parameter`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/rest_parameters). It gobbles up the end of a functions arguments.

```ruby
def print_list_of(**books)
	# books is an array
	books.each do |book|
		puts book
	end
end

books = ['1984', 'War and Peace']
print_list_of books
# => 1984
# => War and Peace

print_list_of
# Argument list can be empty
```

[More information](https://medium.com/@sologoubalex/parameter-with-double-splat-operator-in-ruby-d944d234de34)