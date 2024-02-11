# [Grasshopper - Debug](https://www.codewars.com/kata/55cb854deb36f11f130000e1)

# Description
## Debug celsius converter
Your friend is traveling abroad to the United States so he wrote a program to convert fahrenheit to celsius. 
Unfortunately his code has some bugs.

Find the errors in the code to get the celsius converter working properly.

To convert fahrenheit to celsius:

> celsius = (fahrenheit - 32) * (5/9)

Please round to 5dp (use `.round(5)`)

```ruby
def weather_info (temp)
  c : convert(temp)
  if (c > 0)
    return (c.round(5) + " is freezing temperature")
  else
    return (c.round(5) + " is above freezing temperature")
  end
end

def convertToCelsius (temperature)
  var celsius = ((tempertur) - 32 + (5/9)).round(5)
  return temperature
end
```

# My Solution
```ruby
def weather_info (temp)
  result = ((temp - 32) * (5/9.to_f)).round(5)
  result.positive? ? "#{result} is above freezing temperature" : "#{result} is freezing temperature"
end
```
