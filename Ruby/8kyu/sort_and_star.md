# [Sort and Star](https://www.codewars.com/kata/57cfdf34902f6ba3d300001e/train/ruby)

# Description
You will be given a list of strings. You must sort it alphabetically (case-sensitive, and based on the ASCII values of 
the chars) and then return the first value.

The returned value must be a string, and have <code>"***"</code> between each of its letters.

You should not remove or add elements from/to the array.

# My Solution
```ruby
def two_sort(s)
  s.sort.first.chars.join('***')
end
```
# Better/Alternative solution from Codewars
```ruby
def two_sort(s)
  s.min.chars.join('***')
end
```