# [Find Maximum and Minimum Values of a List](https://www.codewars.com/kata/577a98a6ae28071780000989)

# Description
Your task is to make two functions (<code>max</code> and <code>min</code>, or <code>maximum</code> and 
<code>minimum</code>, etc., depending on the language) that receive a list of integers as input, and return the largest 
and lowest number in that list, respectively.

### Examples (Input -> Output)
&ast; [4,6,2,1,9,63,-134,566]         -> max = 566, min = -134\
&ast; [-52, 56, 30, 29, -54, 0, -110] -> min = -110, max = 56\
&ast; [42, 54, 65, 87, 0]             -> min = 0, max = 87]\
&ast; [5]                             -> min = 5, max = 5

### Notes
* You may consider that there will not be any empty arrays/vectors.

# My Solution
```ruby
def min(list)
  list.min
end

def max(list)
  list.max
end
```
