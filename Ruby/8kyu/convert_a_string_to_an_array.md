# [Convert a string to an array](https://www.codewars.com/kata/57e76bc428d6fbc2d500036d)

# Description
Note: This kata is inspired
by [Convert a Number to a String!](http://www.codewars.com/kata/convert-a-number-to-a-string/). Try that one too.

## Description
We need a function that can transform a string into a number. What ways of achieving this do you know?

### Examples (Input ==> Output):
> "Robin Singh" ==> ["Robin", "Singh"]
> 
> "I love arrays they are my favorite" ==> ["I", "love", "arrays", "they", "are", "my", "favorite"]

# My Solution
```ruby
def string_to_array(string)
  string.split
end
```
