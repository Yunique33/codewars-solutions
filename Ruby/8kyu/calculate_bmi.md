# [Calculate BMI](https://www.codewars.com/kata/57a429e253ba3381850000fb)

# Description
Write function bmi that calculates body mass index (bmi = weight / height<sup>2</sup>).

if bmi <= 18.5 return "Underweight"

if bmi <= 25.0 return "Normal"

if bmi <= 30.0 return "Overweight"

if bmi > 30 return "Obese"

# My Solution
```ruby
def bmi(weight, height)
  case weight/height**2
  when 0..18.5
    'Underweight'
  when 18.6..25.0
    'Normal'
  when 25.0..30.0
    'Overweight'
  else
    'Obese'
  end
end
```
