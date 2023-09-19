# [Barking mad](https://www.codewars.com/kata/54dba07f03e88a4cec000caf)

# Description
Teach snoopy and scooby doo how to bark using object methods. Currently only snoopy can bark and not scooby doo.

```ruby
snoopy.bark() #return "Woof"
scoobydoo.bark() #doesn't work yet
```

Use method prototypes to enable all Dogs to bark.

```ruby
class Dog
  def initialize(breed)
    @breed=breed
  end
end

snoopy=Dog.new("Beagle")

def snoopy.bark()
  "Woof"
end

scoobydoo=Dog.new("Great Dane")
```

# My Solution
```ruby
class Dog
  def initialize(breed)
    @breed = breed
  end

  def bark
    'Woof'
  end
end

snoopy = Dog.new("Beagle")
scoobydoo = Dog.new("Great Dane")
```
