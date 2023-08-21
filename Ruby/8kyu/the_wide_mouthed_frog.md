# [The Wide-Mouthed frog!](https://www.codewars.com/kata/57ec8bd8f670e9a47a000f89)

# Description
If you can't sleep, just count sheep!!

### Task:
The wide-mouth frog is particularly interested in the eating habits of other creatures.

He just can't stop asking the creatures he encounters what they like to eat. But, then he meets the alligator who just 
LOVES to eat wide-mouthed frogs!

When he meets the alligator, it then makes a tiny mouth.

Your goal in this kata is to create complete the `mouth_size` method this method takes one argument `animal` which 
corresponds to the animal encountered by the frog. If this one is an `alligator` (case-insensitive) return `small` 
otherwise return `wide`.

# My Solution
```ruby
def mouth_size(animal)
  animal.downcase == 'alligator' ? 'small' : 'wide'
end
```

# Better/Alternative solution from Codewars
```ruby
def billboard(name, price = 30)
  name.size / (1.0 / price)
end
```
