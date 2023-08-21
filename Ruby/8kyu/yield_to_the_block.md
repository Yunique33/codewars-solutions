# [Yield to the Block](https://www.codewars.com/kata/5253d3a24f16f061cd000228)

# Description
Complete the Compute method/function so that if a block is given it will run else it returns "Do not compute".

```ruby
def compute
  yield
end
```

# My Solution
```ruby
def compute
  block_given? ? yield : "Do not compute"
end
```
