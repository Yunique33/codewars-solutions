# [Name on billboard](https://www.codewars.com/kata/570e8ec4127ad143660001fd)

# Description
If you can't sleep, just count sheep!!

### Task:
You can print your name on a billboard ad. Find out how much it will cost you. Each character has a default price of 
£30, but that can be different if you are given 2 parameters instead of 1 (allways 2 for Java).

You can not use multiplier "*" operator.

If your name would be Jeong-Ho Aristotelis, ad would cost £600. 20 leters * 30 = 600 (Space counts as a character).

# My Solution
```ruby
def billboard(name, price = 30)
  name.size.times.inject(0) {|sum, _|  sum += price}
end
```

# Better/Alternative solution from Codewars
```ruby
def billboard(name, price = 30)
  name.size / (1.0 / price)
end
```
