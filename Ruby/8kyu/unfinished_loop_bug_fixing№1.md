# [Unfinished Loop - Bug Fixing #1](https://www.codewars.com/kata/55c28f7304e3eaebef0000da)

# Description
### Unfinished Loop - Bug Fixing #1
Oh no, Timmy's created an infinite loop! Help Timmy find and fix the bug in his unfinished for loop!
```ruby
def create_array(n)
  res=[]
  i=1
  while i<=n
    res+=[i]
  end
  return res
end
```
# My Solution
```ruby
def create_array(n)
  res=[]
  i=1
  while i<=n
    res+=[i]
    i+=1
  end
  return res
end
```
