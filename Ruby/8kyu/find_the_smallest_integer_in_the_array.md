# [Find the smallest integer in the array](https://www.codewars.com/kata/55a2d7ebe362935a210000b2)

# Description
Given an array of integers your solution should find the smallest integer.

For example:

* Given <code>[34, 15, 88, 2]</code> your solution will return <code>2</code>
* Given <code>[34, -345, -1, 100]</code> your solution will return <code>-345</code>

You can assume, for the purpose of this kata, that the supplied array will not be empty.

# My Solution
```ruby
def find_smallest_int(arr)
  arr.min
end
```
