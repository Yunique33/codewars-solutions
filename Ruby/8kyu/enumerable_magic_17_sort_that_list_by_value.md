# [Enumerable Magic #17 - Sort that List by Value!](https://www.codewars.com/kata/545ac6fe85166a42c8000f37)

# Description
Create a method `sort_by` that accepts a list and a block, and returns a new list sorted by the return values of the block.

If you need help, here's a reference:

http://www.rubycuts.com/enum-sort-by

# My Solution
```ruby
def sort_by(list, &block)
  list.sort_by(&block)
end
```
