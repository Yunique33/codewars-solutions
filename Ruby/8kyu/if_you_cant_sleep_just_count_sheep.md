# [If you can't sleep, just count sheep!!](https://www.codewars.com/kata/5b077ebdaf15be5c7f000077)

# Description
If you can't sleep, just count sheep!!

### Task:
Given a non-negative integer, <code>3</code> for example, return a string with a murmur: <code>"1 sheep...2 sheep...3 
sheep..."</code>. Input will always be valid, i.e. no negative integers.

# My Solution
```ruby
def count_sheep(num)
  str = ''
  num.times {|n| str << "#{n+1} sheep..." }
  str
end
```
