# [Remove First and Last Character](https://www.codewars.com/kata/56bc28ad5bdaeb48760009b0)

## Description
It's pretty straightforward. Your goal is to create a function that removes the first and last characters of a string. 
You're given one parameter, the original string. You don't have to worry with strings with less than two characters.

## My Solution
```ruby
def remove_char(s)
  s[1..-2]
end
```
## Better/Alternative solution from Codewars
```ruby
def remove_char(s)
  s[1...-1]
end
```
