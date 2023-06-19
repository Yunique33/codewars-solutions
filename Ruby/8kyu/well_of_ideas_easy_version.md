# [Well of Ideas - Easy Version](https://www.codewars.com/kata/57f222ce69e09c3630000212)

# Description
For every good kata idea there seem to be quite a few bad ones!

In this kata you need to check the provided array (x) for good ideas 'good' and bad ideas 'bad'. If there are one or two
good ideas, return 'Publish!', if there are more than 2 return 'I smell a series!'. If there are no good ideas, as is 
often the case, return 'Fail!'.

# My Solution
```ruby
def well(x)
  case x.count('good')
  when 0 then 'Fail!'
  when 1..2 then 'Publish!'
  else  'I smell a series!'
  end
end
```
# Better/Alternative solution from Codewars
```ruby
def get_age(age)
  age.to_i
end
```
