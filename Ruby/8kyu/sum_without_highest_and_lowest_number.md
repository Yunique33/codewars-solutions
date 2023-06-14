# [Sum without highest and lowest number](https://www.codewars.com/kata/576b93db1129fcf2200001e6)

# Description
## Task
Sum all the numbers of a given array ( cq. list ), except the highest and the lowest element ( by value, not by 
index! ).

The highest or lowest element respectively is a single element at each edge, even if there are more than one with the 
same value.

Mind the input validation.

## Example
>{ 6, 2, 1, 8, 10 } => 16\
{ 1, 1, 11, 2, 3 } => 6

## Input validation
If an empty value (<code>null</code>, <code>None</code>, <code>Nothing</code> etc. ) is given instead of an array, or 
the given array is an empty list or a list with only <code>1</code> element, return <code>0</code>.
# My Solution
```ruby
def sum_array(arr)
  return 0 if arr.nil? || arr.size <= 1
  arr.sum - (arr.min + arr.max)
end
```
