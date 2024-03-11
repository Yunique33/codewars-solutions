# [Crash Override](https://www.codewars.com/kata/578c1e2edaa01a9a02000b7f)

## Description
<img style="width:463px;height:200px;" src="https://media.giphy.com/media/13AN8X7jBIm15m/giphy.gif">

Every budding hacker needs an alias! `The Phantom Phreak`, `Acid Burn`, `Zero Cool` and `Crash Override` are some 
notable examples from the film `Hackers`.

Your task is to create a function that, given a proper first and last name, will return the correct alias.

### Notes:
* Two objects that return a one word name in response to the first letter of the first name and one for the first letter
of the surname are already given. See the examples below for further details.

* If the first character of either of the names given to the function is not a letter from `A - Z`, you should return 
`"Your name must start with a letter from A - Z."`

* Sometimes people might forget to capitalize the first letter of their name so your function should accommodate for
---

### Examples
```ruby
# These two hashes are preloaded, you need to use them in your code
FIRST_NAME = {'A': 'Alpha', 'B': 'Beta', 'C': 'Cache', ...}
SURNAME = {'A': 'Analogue', 'B': 'Bomb', 'C': 'Catalyst' ...}

alias_gen('Larry', 'Brentwood') == 'Logic Bomb'
alias_gen('123abc', 'Petrovic') == 'Your name must start with a letter from A - Z.'
```

Happy hacking!

## My Solution
```ruby
def alias_gen(first_name, surname)
  name_first_letter = first_name[0].upcase
  surname_first_letter = surname[0].upcase
  if name_first_letter =~ /[^A-Z]/ || surname_first_letter =~ /[^A-Z]/
    return 'Your name must start with a letter from A - Z.'
  end
  "#{FIRST_NAME[name_first_letter]} #{SURNAME[surname_first_letter]}"
end
```

## Better/Alternative solution from Codewars
```ruby
def alias_gen first, sur
  f = FIRST_NAME[first[0].upcase]
  l = SURNAME[sur[0].upcase]
  f && l ? "#{f} #{l}" : "Your name must start with a letter from A - Z."
end
```
