# [Wilson primes](https://www.codewars.com/kata/55dc4520094bbaf50e0000cb)

# Description
[Wilson primes](https://en.wikipedia.org/wiki/Wilson_prime) satisfy the following condition. Let `P` represent a prime 
number.

Then,

```((P-1)! + 1) / (P * P)```

should give a whole number.

Your task is to create a function that returns `true` if the given number is a **Wilson prime**.


# My Solution
```ruby
def am_I_Wilson(p)
  [5,13,563].include? p
end
```
