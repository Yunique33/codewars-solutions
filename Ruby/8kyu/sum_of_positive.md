# [Sum of positive](https://www.codewars.com/kata/5715eaedb436cf5606000381  )

# Description
You get an array of numbers, return the sum of all of the positives ones.\
Example <code>[1,-4,7,12]</code> => <code>1 + 7 + 12 = 20</code>\
Note: if there is nothing to sum, the sum is default to <code>0</code>.

# My Solution
```ruby
def positive_sum(arr)
  arr.select(&:positive?).sum
end
```
# Better/Alternative solution from Codewars
```ruby
def positive_sum(arr)
  arr.select{|x| x > 0}.reduce(0, :+)
end
```
