# [Regexp Basics - is it a digit?](https://www.codewars.com/kata/567bf4f7ee34510f69000032)

# Description
Implement `String#digit?` (in Java `StringUtils.isDigit(String)`), which should return `true` if given object is a 
digit (0-9), `false` otherwise.

```ruby
class String
  def digit?
    # your code goes here
  end
end
```

# My Solution
```ruby
class String
  def digit?
    self.match?(/\A\d\z/)
  end
end
```

# Better/Alternative solution from Codewars
```ruby
class String
  def digit?
    /\A\d\z/ === self
  end
end
```
