# [Exclamation marks series #2: Remove all exclamation marks from the end of sentence](https://www.codewars.com/kata/57faece99610ced690000165)

# Description
## Description:
Remove all exclamation marks from the end of sentence.

## Examples
```
remove("Hi!") === "Hi"
remove("Hi!!!") === "Hi"
remove("!Hi") === "!Hi"
remove("!Hi!") === "!Hi"
remove("Hi! Hi!") === "Hi! Hi"
remove("Hi") === "Hi"
```

# My Solution
```ruby
def remove(s)
  s.gsub(/!+$/, '')
end
```
