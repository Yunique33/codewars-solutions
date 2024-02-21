# [Century From Year](https://www.codewars.com/kata/5a3fe3dde1ce0e8ed6000097)

# Description
## Introduction
The first century spans from the **year 1** up to _and including_ the year 100, the second century - from the year 101 
up to _and including_ the year 200, etc.

## Task
Given a year, return the century it is in.

## Examples
```
1705 --> 18
1900 --> 19
1601 --> 17
2000 --> 20
2742 --> 28
```

Note: this kata uses strict construction as shown in the description and the examples, you can read more about 
it [here](https://en.wikipedia.org/wiki/Century)

# My Solution
```ruby
def century(year)
  (year/100.0).ceil
end
```
