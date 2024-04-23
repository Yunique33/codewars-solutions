# [Incorrect division method](https://www.codewars.com/kata/54d1c59aba326343c80000e7)

## Description
This method, which is supposed to return the result of dividing its first argument by its second, isn't always returning 
correct values. Fix it.

```ruby
def divide_numbers x, y
  x / y
end
```

## My Solution
```ruby
def divide_numbers(x, y)
  x / y.to_f
end
```

## Better/Alternative solution from Codewars
```ruby
def divide_numbers x, y
  x.fdiv y
end
```
