# [Simple validation of a username with regex](https://www.codewars.com/kata/56a3f08aa9a6cc9b75000023)

# Description
Write a simple regex to validate a username. Allowed characters are:

* lowercase letters,
* numbers,
* underscore

Length should be between 4 and 16 characters (both included).

# My Solution
```ruby
def validate_usr(username)
  (/^[a-z0-9_]{4,16}$/).match?(username)
end
```

# Better/Alternative solution from Codewars
```ruby
def validate_usr(username)
  !!username[/\A[a-z0-9_]{4,16}\z/]
end
```
