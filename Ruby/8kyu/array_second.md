# [Array#secon](https://www.codewars.com/kata/536c6f2349aa8b16520002e0)

# Description
Define a new instance method on the `Array` class called `second`, which returns the second item in an array (similar 
to the way `.first` and `.last` work in Ruby).

If there is no element with index `1` in the array, return `nil`.

```ruby
class Array

end
```

# Examples
```ruby
[3, 4, 5].second  #  => 4 
[].second         #  => nil
````

# My Solution
```ruby
class Array
  def second
    self[1]
  end
end
```

# Better/Alternative solution from Codewars
```ruby
class Array
  def second
    self.at(1)
  end
end
```
