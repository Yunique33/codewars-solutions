# [Playing with cubes II](https://www.codewars.com/kata/55c0ac142326fdf18d0000af)

# Description
Hey Codewarrior!

You already implemented a **Cube** class, but now we need your help again! I'm talking about constructors. We don't have
one. Let's code two: One taking an integer and one handling no given arguments!

Also we got a problem with negative values. Correct the code so negative values will be switched to positive ones!

The constructor taking no arguments should assign 0 to Cube's Side property.

```ruby
class Cube
  # This cube needs help
	# Define a constructor which takes one integer, or handles no args
  
  def get_side()
    return @_side
  end
  
  def set_side(new_side)
    @_side = new_side.abs
  end
end
```

# My Solution
```ruby
class Cube
  def initialize(side = 0)
    @side = side
  end

  def get_side()
    @side
  end

  def set_side(new_side)
    @side = new_side.abs
  end
end
```

# Better/Alternative solution from Codewars
```ruby
class Cube
  attr_accessor :side
  alias_method :get_side, :side
  alias_method :set_side, :side=

  def initialize(side = 0)
    @side = side
  end
end
```
