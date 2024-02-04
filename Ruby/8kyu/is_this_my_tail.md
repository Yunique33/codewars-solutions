# [Is this my tail?](https://www.codewars.com/kata/56f695399400f5d9ef000af5)

# Description
Some new animals have arrived at the zoo. The zoo keeper is concerned that perhaps the animals do not have the right 
tails. To help her, you must correct the broken function to make sure that the second argument (tail), is the same as 
the last letter of the first argument (body) - otherwise the tail wouldn't fit!

If the tail is right return true, else return false.

The arguments will always be non empty strings, and normal letters.

```ruby
def correct_tail(body, tail)
   sub = body.substr(body.length-(tail.length)
  
  if sub = tail) then
    return true
  
  else 
    return false
    end
```

# My Solution
```ruby
def correct_tail(body, tail)
  body[-1] == tail
end  
```
