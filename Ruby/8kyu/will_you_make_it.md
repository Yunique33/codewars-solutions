# [Will you make it?](https://www.codewars.com/kata/5861d28f124b35723e00005e)

# Description
You were camping with your friends far away from home, but when it's time to go back, you realize that your fuel is 
running out and the nearest pump is <code>50</code> miles away! You know that on average, your car runs on about 
<code>25</code> miles per gallon. There are <code>2</code> gallons left.

Considering these factors, write a function that tells you if it is possible to get to the pump or not.

Function should return <code>true</code> if it is possible and <code>false</code> if not.

# My Solution
```ruby
def zero_fuel(distance, mpg, fuel_left)
  distance <= mpg * fuel_left
end
```
