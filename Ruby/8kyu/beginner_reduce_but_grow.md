# [Fake Binary](https://www.codewars.com/kata/57eae65a4321032ce000002d)

# Description
Given a non-empty array of integers, return the result of multiplying the values together in order. Example:

>[1, 2, 3, 4] => 1 * 2 * 3 * 4 = 24

# My Solution
```ruby
def grow(x)
  x.inject(:*)
end
```
