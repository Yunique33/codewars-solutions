# [Convert to Binary](https://www.codewars.com/kata/59fca81a5712f9fa4700159a)

# Description
Given a non-negative integer `n`, write a function `to_binary`/`ToBinary` which returns that number in a binary format.

Example:

```
to_binary(1)  # should return 1
to_binary(5)  # should return 101
to_binary(11) # should return 1011
```

# My Solution
```ruby
def to_binary(n)
  n.to_s(2).to_i
end
```
