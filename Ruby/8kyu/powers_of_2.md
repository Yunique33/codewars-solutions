# [Powers of 2](https://www.codewars.com/kata/57a083a57cb1f31db7000028)

# Description
Complete the function that takes a non-negative integer <code>n</code> as input, and returns a list of all the powers of
<code>2</code> with the exponent ranging from <code>0</code> to <code>n</code> (inclusive).

## Examples
>n = 0  ==> [1]        # [2^0]\
n = 1  ==> [1, 2]     # [2^0, 2^1]\
n = 2  ==> [1, 2, 4]  # [2^0, 2^1, 2^2]

# My Solution
```ruby
def powers_of_two(n)
  (0..n).map { |n| 2**n }
end
```
