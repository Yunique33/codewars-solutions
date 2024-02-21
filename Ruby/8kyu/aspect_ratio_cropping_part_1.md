# [Aspect Ratio Cropping - Part 1](https://www.codewars.com/kata/596e4ef7b61e25981200009f)

## Description
The aspect ratio of an image describes the proportional relationship between its width and its height. Most video shown 
on the internet uses a 16:9 aspect ratio, which means that for every pixel in the Y, there are roughly 1.77 pixels in 
the X (where 1.77 ~= 16/9). As an example, 1080p video with an aspect ratio of 16:9 would have an X resolution of 1920, 
however 1080p video with an aspect ratio of 4:3 would have an X resolution of 1440.

Write a function that accepts arbitrary X and Y resolutions and converts them into resolutions with a 16:9 aspect ratio 
that maintain equal height. Round your answers up to the nearest integer.

This kata is part of a series 
with [Aspect Ratio Cropping - Part 2](https://www.codewars.com/kata/aspect-ratio-cropping-part-2).

### Example

_374 × 280 pixel image with a 4:3 aspect ratio._

![Aspect ratio 4 3 example](https://upload.wikimedia.org/wikipedia/commons/4/43/Aspect_ratio_4_3_example.jpg)

_500 × 280 pixel image with a 16:9 aspect ratio._

![Aspect ratio 16 9 example3](https://upload.wikimedia.org/wikipedia/commons/2/2c/Aspect_ratio_16_9_example3.jpg)

## My Solution
```ruby
def aspect_ratio(x, y)
  [(y.to_f / 9 * 16).ceil, y]
end
```

## Better/Alternative solution from Codewars
```ruby
def aspect_ratio(x, y)
  [(y * 16 + 8) / 9 , y]
end
```
