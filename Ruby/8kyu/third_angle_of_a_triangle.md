# [Third Angle of a Triangle](https://www.codewars.com/kata/5a023c426975981341000014)

# Description
You are given two interior angles (in degrees) of a triangle.

Write a function to return the 3rd.

Note: only positive integers will be tested.

https://en.wikipedia.org/wiki/Triangle

# My Solution
```ruby
def other_angle(a, b)
  180-(a+b)
end
```
# Better/Alternative solution from Codewars
```ruby
def first_non_consecutive(arr)
  arr.each_index do |i|
    return arr[i + 1] if arr[i].next != arr[i + 1]
  end
end
```
