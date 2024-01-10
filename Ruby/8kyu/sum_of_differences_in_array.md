# [Sum of differences in array](https://www.codewars.com/kata/5b73fe9fb3d9776fbf00009e)

# Description
Your task is to sum the differences between consecutive pairs in the array in descending order.

## Example
```
[2, 1, 10]  -->  9
```

In descending order: `[10, 2, 1]`

Sum: `(10 - 2) + (2 - 1) = 8 + 1 = 9`

If the array is empty or the array has only one element the result should be `0` (`Nothing` in Haskell, `None` in Rust).

# My Solution
```ruby
def sum_of_differences(arr)
  arr.sort.reverse.each_cons(2).map { |a, b| a - b }.sum
end
```

# Better/Alternative solution from Codewars
```ruby
def sum_of_differences(arr)
  arr.empty? ? 0 : arr.max - arr.min
end
```
