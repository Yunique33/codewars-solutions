# [Find Nearest square number](https://www.codewars.com/kata/5a805d8cafa10f8b930005ba)

## Description
Your task is to find the nearest square number, `nearest_sq(n)` or `nearestSq(n)`, of a positive integer `n`.

For example, if `n = 111`, then `nearest\_sq(n)` `(nearestSq(n))` equals 121, since 111 is closer to 121, the square of 
11, than 100, the square of 10.

If the `n` is already the perfect square (e.g. `n = 144`, `n = 81`, etc.), you need to just return `n`.

Good luck :)

## My Solution
```ruby
def nearest_sq(n)
  Math.sqrt(n).round ** 2
end
```
