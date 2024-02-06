# [101 Dalmatians - squash the bugs, not the dogs!](https://www.codewars.com/kata/56f6919a6b88de18ff000b36)

# Description
Your friend has been out shopping for puppies (what a time to be alive!)... He arrives back with multiple dogs, and you 
simply do not know how to respond!

By repairing the function provided, you will find out exactly how you should respond, depending on the number of dogs he
has.

The number of dogs will always be a number and there will always be at least 1 dog.

> Good luck!

```ruby
def how_many_dalmatians(n)
  dogs ["Hardly any", "More than a handful!", "Woah that's a lot of dogs!", "101 DALMATIONS!!!"];

  respond = number <= 10 ? dogs[0] (number <= 50 ? dogs[1] : (number = 101  dogs[3] : dogs[2]

  return respond
  end
```

# My Solution
```ruby
def how_many_dalmatians(n)
  dogs = ["Hardly any", "More than a handful!", "Woah that's a lot of dogs!", "101 DALMATIONS!!!"]

  case n
  when 0..10
    dogs[0]
  when 11..50
    dogs[1]
  when 101
    dogs[3]
  else
    dogs[2]
  end
end
```

# Better/Alternative solution from Codewars
```ruby
def how_many_dalmatians(n)
  case
  when n <= 10 then "Hardly any"
  when n <= 50 then "More than a handful!"
  when n == 101 then "101 DALMATIONS!!!"
  else "Woah that's a lot of dogs!"
  end
end
```
