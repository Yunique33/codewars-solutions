# [Count of positives / sum of negatives](https://www.codewars.com/kata/576bb71bbbcf0951d5000044)

# Description
Given an array of integers.

Return an array, where the first element is the count of positives numbers and the second element is sum of negative 
numbers. 0 is neither positive nor negative.

If the input is an empty array or is null, return an empty array.

## Example
For input <code>[1, 2, 3, 4, 5, 6, 7, 8, 9, 10, -11, -12, -13, -14, -15]</code>, you should return 
<code>[10, -65]</code>.

# My Solution
```ruby
def count_positives_sum_negatives(lst)
  return [] if lst.empty?
  positive, negative = lst.partition(&:positive?)
  [positive.count, negative.sum]
end
```