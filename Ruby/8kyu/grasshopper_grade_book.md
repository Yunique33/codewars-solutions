# [Grasshopper - Grade book](https://www.codewars.com/kata/55cbd4ba903825f7970000f5)

## Description
### Grade book
Complete the function so that it finds the average of the three scores passed to it and returns the letter value 
associated with that grade.


| Numerical Score    | 	Letter Grade |
| ------------------ | ------------------ |
| 90 <= score <= 100 |          'A'  |
| 80 <= score < 90   | 	        'B'  |
| 70 <= score < 80   | 	        'C'  |
| 60 <= score < 70   | 	        'D'  |
| 0 <= score < 60    |          'F'  |

Tested values are all between 0 and 100. Theres is no need to check for negative values or values greater than 100.

## My Solution
```ruby
def get_grade(s1, s2, s3)
  case (s1 + s2 + s3)/3
  when 90..100
    'A'
  when 80..89
    'B'
  when 70..79
    'C'
  when 60..69
    'D'
  else
    'F'
  end
end  
```

## Better/Alternative solution from Codewars
```ruby
def get_grade(s1, s2, s3)
  m = (s1 + s2 + s3)/3.to_f
  m >= 90 ? 'A' : m >= 80 ? 'B' : m >= 70 ? 'C' : m >= 60 ? 'D' : 'F'
end
```
