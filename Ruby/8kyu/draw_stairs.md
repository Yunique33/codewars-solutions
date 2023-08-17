# [Draw stairs](https://www.codewars.com/kata/5b4e779c578c6a898e0005c5)

# Description
Given a number `n`, draw stairs using the letter `"I"`, `n` tall and `n` wide, with the tallest in the top left.

For example `n = 3` result in:

`"I\n I\n  I"`

or printed:
```
I
 I
  I
```

Another example, a 7-step stairs should be drawn like this:
```
I
 I
  I
   I
    I
     I
      I
```

# My Solution
```ruby
def draw_stairs(n)
  n.times.map { |el| "#{ ' ' * el }I" }.join("\n")
end
```
