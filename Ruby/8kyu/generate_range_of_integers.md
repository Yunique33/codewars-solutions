# [Generate range of integers](https://www.codewars.com/kata/55eca815d0d20962e1000106)

# Description
Implement the function `generateRange` which takes three arguments `(start, stop, step)` and returns the range of 
integers from `start` to `stop` (inclusive) in increments of `step`.

## Examples
```
(1, 10, 1) -> [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
(-10, 1, 1) -> [-10, -9, -8, -7, -6, -5, -4, -3, -2, -1, 0, 1]
(1, 15, 20) -> [1]
```

## Note
* start < stop
* step > 0

# My Solution
```ruby
def generate_range(min, max, step)
  min.step(max, step).to_a
end
```

# Better/Alternative solution from Codewars
```ruby
def generate_range(min, max, step)
  (min..max).step(step).to_a
end
```
