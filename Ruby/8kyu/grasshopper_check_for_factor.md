# [Grasshopper - Check for factor](https://www.codewars.com/kata/55cbc3586671f6aa070000fb)

# Description
This function should test if the <code>factor</code> is a factor of <code>base</code>.

Return <code>true</code> if it is a factor or <code>false</code> if it is not.

## About factors
Factors are numbers you can multiply together to get another number.

2 and 3 are factors of 6 because: <code>2 * 3 = 6</code>

* You can find a factor by dividing numbers. If the remainder is 0 then the number is a factor.
* You can use the mod operator (<code>%</code>) in most languages to check for a remainder

For example 2 is not a factor of 7 because: <code>7 % 2 = 1</code>

Note: <code>base</code> is a non-negative number, <code>factor</code> is a positive number.

# My Solution
```ruby
def check_for_factor(base, factor)
  base % factor == 0
end
```
