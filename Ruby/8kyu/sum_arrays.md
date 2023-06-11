# [Sum Arrays](https://www.codewars.com/kata/53dc54212259ed3d4f00071c)

# Description

Write a function that takes an array of numbers and returns the sum of the numbers. The numbers can be negative or 
non-integer. If the array does not contain any numbers then you should return 0.

### Examples
Input: <code>[1, 5.2, 4, 0, -1]</code>\
Output: <code>9.2</code>

Input: <code>[]</code>\
Output: <code>0</code>

Input: <code>[-2.398]</code>\
Output: <code>-2.398</code>

### Assumptions

* You can assume that you are only given numbers.
* You cannot assume the size of the array.
* You can assume that you do get an array and if the array is empty, return 0.

### What We're Testing
We're testing basic loops and math operations. This is for beginners who are just learning loops and math operations.
Advanced users may find this extremely easy and can easily write this in one line.

# My Solution

```ruby
def sum(numbers)
  numbers.sum
end
```
