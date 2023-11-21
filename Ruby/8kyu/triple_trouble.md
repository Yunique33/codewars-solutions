# [Triple Trouble](https://www.codewars.com/kata/5704aea738428f4d30000914)

# Description
## Triple Trouble
Create a function that will return a string that combines all of the letters of the three inputed strings in groups. 
Taking the first letter of all of the inputs and grouping them next to each other. Do this for every letter, see example
below!

**E.g. Input: "aa", "bb" , "cc" => Output: "abcabc"**

_Note: You can expect all of the inputs to be the same length._

# My Solution

```ruby
def triple_trouble(one, two, three)
  [one, two, three].map(&:chars).transpose.join
end
```

# Better/Alternative solution from Codewars
```ruby
def triple_trouble(one, two, three)
  one.chars.zip(two.chars, three.chars).join("")
end
```
