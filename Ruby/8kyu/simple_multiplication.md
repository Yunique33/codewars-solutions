# [Simple multiplication](https://www.codewars.com/kata/583710ccaa6717322c000105)

# Description
This kata is about multiplying a given number by eight if it is an even number and by nine otherwise.

# My Solution
```ruby
def simple_multiplication(number)
  number.even? ? number * 8 : number * 9
end
```
