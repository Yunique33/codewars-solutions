# [Surface Area and Volume of a Box](https://www.codewars.com/kata/565f5825379664a26b00007c)

# Description
Write a function that returns the total surface area and volume of a box as an array: `[area, volume]`

# My Solution
```ruby
def get_size(w,h,d)
  [2 * (w * d + h * d + w * h), w * h * d]
end
```
