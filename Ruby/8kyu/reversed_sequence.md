# [Reversed sequence](https://www.codewars.com/kata/5a00e05cc374cb34d100000d)

# Description
Build a function that returns an array of integers from n to 1 where <code>n>0</code>.

Example : <code>n=5</code> --> <code>[5,4,3,2,1]</code>

# My Solution
```ruby
def reverse_seq(n)
  n.downto(1).to_a
end
```
