# [Be Concise I - The Ternary Operator](https://www.codewars.com/kata/56f3f6a82010832b02000f38)

# Description
## Be Concise I - The Ternary Operator
You are given a function `describeAge` / `describe_age` that takes a parameter `age` (which will always be a 
**positive integer**) and does the following:

1. If the age is `12` or lower, it `return "You're a(n) kid"`
2. If the age is anything between `13` and `17` (inclusive), it `return "You're a(n) teenager"`
3. If the age is anything between `18` and `64` (inclusive), it `return "You're a(n) adult"`
4. If the age is `65` or above, it `return "You're a(n) elderly"`

Your task is to shorten the code as much as possible. Note that submitting the given code will not work because there is
a character limit of **137**.

I'll give you a few hints:

1. The title itself is a hint - if you're not sure what to do, **always** research any terminology in this description 
that you have not heard of!
2. Don't you think the whole `"You're a(n) <insert_something_here>"` is very repetitive? ;) Perhaps we can shorten it?
3. Write everything in one line, `\n` and other whitespaces counts.

**Whatever you do, do not change what the function does.** Good luck :)

```ruby
def describe_age(age)
  if age <= 12
    "You're a(n) kid"
  elsif age >= 13 && age <= 17
    "You're a(n) teenager"
  elsif age >= 18 && age <= 64
    "You're a(n) adult"
  else
    "You're a(n) elderly"
  end
end
```

# My Solution
```ruby
def describe_age(age)
  "You're a(n) #{age < 13 ? 'kid' : (13..17) === age ? 'teenager' : (18..64) === age ? 'adult' : 'elderly'}"
end
```

# Better/Alternative solution from Codewars
```ruby
def describe_age(age)
  "You're a(n) " + (age <= 12 ? "kid" : age <= 17 ? "teenager" : age <= 64 ? "adult" : "elderly")
end
```
