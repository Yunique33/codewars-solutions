# [Color Ghost](https://www.codewars.com/kata/53f1015fa9fe02cbda00111a)

# Description
## Color Ghost
Create a class Ghost

Ghost objects are instantiated without any arguments.

Ghost objects are given a random color attribute of "white" or "yellow" or "purple" or "red" when instantiated

```ruby
ghost = Ghost.new
ghost.color  #=> "white" or "yellow" or "purple" or "red"
```
# My Solution
```ruby
class Ghost
  def color
    %w(white yellow purple red).sample
  end
end
```
