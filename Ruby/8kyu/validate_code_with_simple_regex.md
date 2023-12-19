# [validate code with simple regex](https://www.codewars.com/kata/56a25ba95df27b7743000016)

# Description
Basic regex tasks. Write a function that takes in a numeric code of any length. The function should check if the code 
begins with 1, 2, or 3 and return `true` if so. Return `false` otherwise.

You can assume the input will always be a number.

# My Solution
```ruby
def validate_code(code)
  /^[123]/.match?(code.to_s)
end
```

# Better/Alternative solution from Codewars
```ruby
def validate_code(code)
  /\A[123]/ === code.to_s
end
```
