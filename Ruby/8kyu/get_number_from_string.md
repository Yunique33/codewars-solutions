# [Get number from string](https://www.codewars.com/kata/57a37f3cbb99449513000cd8)

# Description
Write a function which removes from string all non-digit characters and parse the remaining to number. 
E.g: "hell5o wor6ld" -> 56

Function:

> get_number_from_string(s)

# My Solution
```ruby
def get_number_from_string(s)
  s.gsub(/[^0-9]/, '').to_i
end
```

# Better/Alternative solution from Codewars
```ruby
def get_number_from_string(s)
  s.scan(/\d+/).join.to_i
end
```
