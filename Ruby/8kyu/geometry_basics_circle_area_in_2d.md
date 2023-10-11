# [Geometry Basics: Circle Area in 2D](https://www.codewars.com/kata/58e3f824a33b52c1dc0001c0)

# Description

This series of katas will introduce you to basics of doing geometry with computers.

Write the function `circleArea`/`CircleArea` which takes in a `Circle` object and calculates the area of that circle.
The Circle class can be seen below:

```ruby
# Represents a Circle where center is a Point and radius is a Number
class Circle
  attr_accessor :center, :radius

  def initialize(center, radius)
    @center = center
    @radius = radius
  end
end
```

And the `Point` class can be seen below:

```ruby
# Represents a Point where x and y are Numbers
class Point
  attr_accessor :x, :y

  def initialize(x, y)
    @x = x
    @y = y
  end
end
```

Tests round answers to 6 decimal places.

# My Solution

```ruby
def circle_area(circle)
  Math::PI * circle.radius**2
end
```
