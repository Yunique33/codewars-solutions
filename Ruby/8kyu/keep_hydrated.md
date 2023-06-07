# [Keep Hydrated!](https://www.codewars.com/kata/582cb0224e56e068d800003c)

# Description
Nathan loves cycling.

Because Nathan knows it is important to stay hydrated, he drinks 0.5 litres of water per hour of cycling.

You get given the time in hours and you need to return the number of litres Nathan will drink, rounded to the smallest value.

For example:

>hours = 3 ----> liters = 1
> 
>hours = 6.7---> liters = 3
>
>hours = 11.8--> liters = 5

# My Solution
```ruby
def litres(time)
  (time/2).floor
end
```
# Better/Alternative solution from Codewars
```ruby
def litres(time)
  (time * 0.5).floor
end
```
