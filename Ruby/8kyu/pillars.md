# [Pillars](https://www.codewars.com/kata/5bb0c58f484fcd170700063d)

# Description
There are pillars near the road. The distance between the pillars is the same and the width of the pillars is the same. 
Your function accepts three arguments:

1. number of pillars (≥ 1);
2. distance between pillars (10 - 30 meters);
3. width of the pillar (10 - 50 centimeters).

Calculate the distance between the first and the last pillar in centimeters (without the width of the first and last pillar).

# My Solution
```ruby
def pillars(num_of_pillars, distance, width)
  return 0 if num_of_pillars < 2
  distance * (num_of_pillars - 1) * 100  + (num_of_pillars - 2) * width
end
```
