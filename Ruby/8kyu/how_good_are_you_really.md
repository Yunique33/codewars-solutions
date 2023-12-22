# [How good are you really?](https://www.codewars.com/kata/5601409514fc93442500010b )

# Description
There was a test in your class and you passed it. Congratulations!
But you're an ambitious person. You want to know if you're better than the average student in your class.

You receive an array with your peers' test scores. Now calculate the average and compare your score!

Return <code>True</code> if you're better, else <code>False</code>!

## Note
Your points are not included in the array of your class's points. For calculating the average point you may add your
point to the given array!

# My Solution
```ruby
def better_than_average(arr, points)
  arr.push(points).sum/arr.size < points
end
```
