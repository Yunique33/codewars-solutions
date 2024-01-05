# [Merging sorted integer arrays (without duplicates)](https://www.codewars.com/kata/573f5c61e7752709df0005d2)

# Description
Write a function that merges two sorted arrays into a single one. The arrays only contain integers. Also, the final 
outcome must be sorted and not have any duplicate.

# My Solution
```ruby
def merge_arrays(a, b)
  (a + b).uniq.sort
end
```

# Better/Alternative solution from Codewars
```ruby
def merge_arrays(a, b)
  (a | b).sort
end
```
