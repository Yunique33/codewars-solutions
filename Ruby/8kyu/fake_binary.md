# [Fake Binary](https://www.codewars.com/kata/57eae65a4321032ce000002d)

# Description
Given a string of digits, you should replace any digit below 5 with '0' and any digit 5 and above with '1'. Return the 
resulting string.

### Note: input will never be an empty string

# My Solution
```ruby
def fake_bin(s)
  s.tr('01234', '0').tr('56789', '1')
end
```

# Better/Alternative solution from Codewars
```ruby
def fake_bin(s)
  s.tr('1-9', '00001')
end
```
