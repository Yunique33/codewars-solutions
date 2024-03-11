# [Enumerable Magic #16 - Sort that List!](https://www.codewars.com/kata/545ac54161aa4c339a0010dd)

## Description
Create a method **sort** that accepts a list and a block. The block should define how **sort** compares two items on the
list. It should return a new, sorted version of the list.

If you need help, here's a reference:

http://www.rubycuts.com/enum-sort

## My Solution
```ruby
def sort(list, &block)
  list.sort(&block)
end
```
