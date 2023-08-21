# [Is your period late?](https://www.codewars.com/kata/578a8a01e9fd1549e50001f1)

# Description
In this kata, we will make a function to test whether a period is late.

Our function will take three parameters:

last - The Date object with the date of the last period

today - The Date object with the date of the check

cycleLength - Integer representing the length of the cycle in days

Return true if the number of days passed from last to today is greater than cycleLength. Otherwise, return false.

# My Solution
```ruby
def period_is_late(last,today,cycle_length)
  today - last > cycle_length
end
```
