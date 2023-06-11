# [You only need one - Beginner](https://www.codewars.com/kata/57cc975ed542d3148f00015b)

# Description
You will be given an array <code>a</code> and a value <code>x</code>. All you need to do is check whether the provided 
array contains the value.

Array can contain numbers or strings. X can be either.

Return <code>true</code> if the array contains the value, <code>false</code> if not.

# My Solution
```ruby
def check(arr,element)
  arr.include?(element)
end
```
# Better/Alternative solution from Codewars
```ruby
def positive_sum(arr)
  arr.select{|x| x > 0}.reduce(0, :+)
end
```
