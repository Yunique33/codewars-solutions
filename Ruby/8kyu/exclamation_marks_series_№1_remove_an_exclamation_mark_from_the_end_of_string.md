# [Exclamation marks series #1: Remove an exclamation mark from the end of string](https://www.codewars.com/kata/57fae964d80daa229d000126)

## Description
### Description
Remove an exclamation mark from the end of a string. For a beginner kata, you can assume that the input data is always a
string, no need to verify it.

### Examples
```
"Hi!"     ---> "Hi"
"Hi!!!"   ---> "Hi!!"
"!Hi"     ---> "!Hi"
"!Hi!"    ---> "!Hi"
"Hi! Hi!" ---> "Hi! Hi"
"Hi"      ---> "Hi"
```

## My Solution
```ruby
def remove(s)
  s[-1] == '!' ? s[0..-2] : s
end
```

## Better/Alternative solution from Codewars
```ruby
def remove(s)
  s.chomp('!')
end
```
