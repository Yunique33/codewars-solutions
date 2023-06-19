# [To square(root) or not to square(root)](https://www.codewars.com/kata/57f6ad55cca6e045d2000627)

# Description   
Write a method, that will get an integer array as parameter and will process every number from this array.

Return a new array with processing every number of the input-array like this:

If the number has an integer square root, take this, otherwise square the number.

### Example
>[4,3,9,7,2,1] -> [2,9,3,49,4,1]

### Notes
The input array will always contain only positive numbers, and will never be empty or null.

# My Solution
```ruby
def square_or_square_root(arr)
  arr.map do |el|
    res = Math.sqrt(el)
    res == res.to_i ? res : el**2
  end
end
```
# Better/Alternative solution from Codewars
```ruby
def square_or_square_root(arr)
  arr.map do |n|
    sqrt = Math.sqrt(n)
    sqrt % 1 == 0 ? sqrt : n**2
  end
end
```