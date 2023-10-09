# [Area of a Square](https://www.codewars.com/kata/5748838ce2fab90b86001b1a)

# Description
Complete the function that calculates the area of the red square, when the length of the circular arc `A` is given as 
the input. Return the result rounded to two decimals.

<img src="http://i.imgur.com/nJrae8n.png">

Note: use the π value provided in your language (`Math::PI`, `M_PI`, `math.pi`, etc)

# My Solution
```ruby
def square_area(arc)
  ((2 * arc /  Math::PI) ** 2).round(2)
end
```
