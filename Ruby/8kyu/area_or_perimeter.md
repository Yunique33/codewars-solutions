# [Area or Perimeter](https://www.codewars.com/kata/5ab6538b379d20ad880000ab)

# Description
You are given the <code>length</code> and <code>width</code> of a 4-sided polygon. The polygon can either be a rectangle
or a square.
If it is a square, return its area. If it is a rectangle, return its perimeter.

### Example(Input1, Input2 --> Output):

>6, 10 --> 32\
3, 3 --> 9

**Note:** for the purposes of this kata you will assume that it is a square if its <code>length</code> and 
<code>width</code> are equal, otherwise it is a rectangle.

# My Solution

```ruby
def area_or_perimeter(l , w)
  l == w ? l*w : (l+w)*2
end
```
