# [Function 1 - hello world](https://www.codewars.com/kata/523b4ff7adca849afe000035)

# Description
Make a simple function called <code>greet</code> that returns the most-famous "hello world!".

### Style Points

Sure, this is about as easy as it gets. But how clever can you be to create the most creative "hello world" you can think of? What is a "hello world" solution you would want to show your friends?
# My Solution
```ruby
def greet
  [104, 101, 108, 108, 111, 32, 119, 111, 114, 108, 100, 33].map(&:chr).join
end  
```
# Better/Alternative solution from Codewars
```ruby
module Kernel
  def method_missing(*args)
    return "hello world!"
  end
end
```
