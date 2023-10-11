# [Geometry Basics: Distance between points in 2D](https://www.codewars.com/kata/58dced7b702b805b200000be/ruby)

# Description
This series of katas will introduce you to basics of doing geometry with computers.

`Point` objects have attributes `x` and `y`.

Write a function calculating distance between `Point a` and `Point b`.

Tests compare expected result and actual answer with tolerance of `1e-6`.

```ruby
def distance_between_points(a, b)
  return 0 # your code here
end
```

# My Solution
```ruby
def distance_between_points(a, b)
  Math.sqrt((a.x - b.x)**2 + (a.y - b.y)**2)
end
```

# Better/Alternative solution from Codewars
```ruby
def distance_between_points(a, b)
  Math.hypot(b.x - a.x, b.y - a.y)
end
```
