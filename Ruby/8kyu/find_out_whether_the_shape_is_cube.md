# [Find out whether the shape is a cube](https://www.codewars.com/kata/58d248c7012397a81800005c)

# Description
To find the volume (centimeters cubed) of a cuboid you use the formula:

<code>volume = Length * Width * Height</code>

But someone forgot to use proper record keeping, so we only have the volume, and the length of a single side!

It's up to you to find out whether the cuboid has equal sides (= is a cube).

Return <code>true</code> if the cuboid could have equal sides, return <code>false</code> otherwise.

Return <code>false</code> for invalid numbers too (e.g volume or side is less than or equal to 0).



# My Solution
```ruby
def cube_checker(volume, side)
  volume == side**3 && volume > 0
end
```
