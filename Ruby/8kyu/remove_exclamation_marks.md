# [Remove exclamation marks](https://www.codewars.com/kata/57a0885cbb9944e24c00008e)

# Description
Write function RemoveExclamationMarks which removes all exclamation marks from a given string.

# My Solution

```ruby
def remove_exclamation_marks(s)
  s.delete('!')
end
```

# Better/Alternative solution from Codewars
```ruby
def remove_exclamation_marks(s)
  s.gsub(/!/, '')
end
```
