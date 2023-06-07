# [Square(n) Sum](https://www.codewars.com/kata/515e271a311df0350d00000f)

# Description
Complete the square sum function so that it squares each number passed into it and then sums the results together.

For example, for <code>[1, 2, 2]</code> it should 
return <code>9</code> because 1<sup>2</sup>+2<sup>2</sup>+2<sup>2</sup>=9.

# My Solution
```ruby
def square_sum(numbers)
  numbers.sum{ |num| num**2 }
end
```
# Better/Alternative solution from Codewars
```ruby
def squareSum(numbers)
  numbers.map {|n| n*n}.reduce(:+)
end
```
