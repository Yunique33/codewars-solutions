# [Push a hash/an object into array](https://www.codewars.com/kata/527b3cd0492b6b15250060af)

# Description
You are trying to put a hash in ruby or an object in javascript or java into an array, but it always returns error, 
solve it and keep it as simple as possible!

```ruby
items = Array.new
items.push {:a => "b", :c => "d"}
```

# My Solution
```ruby
items = Array.new
items << {:a => "b", :c => "d"}
```
