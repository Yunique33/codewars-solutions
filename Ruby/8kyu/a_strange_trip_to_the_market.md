# [A Strange Trip to the Market](https://www.codewars.com/kata/55ccdf1512938ce3ac000056)

# Description
You're on your way to the market when you hear beautiful music coming from a nearby street performer. The notes come 
together like you wouln't believe as the musician puts together patterns of tunes. As you wonder what kind of algorithm 
you could use to shift octaves by 8 pitches or something silly like that, it dawns on you that you have been watching 
the musician for some 10 odd minutes. You ask, _"how much do people normally tip for something like this?"_ The artist 
looks up. _"It's always gonna be about tree fiddy."_

It was then that you realize the musician was a 400 foot tall beast from the paleolithic era! The Loch Ness Monster 
almost tricked you!

There are only 2 guaranteed ways to tell if you are speaking to The Loch Ness Monster: A) it is a 400 foot tall beast 
from the paleolithic era; B) it will ask you for tree fiddy.

Since Nessie is a master of disguise, the only way accurately tell is to look for the phrase `"tree fiddy"`. Since you 
are tired of being grifted by this monster, the time has come to code a solution for finding The Loch Ness Monster. Note
that the phrase can also be written as `"3.50"` or `"three fifty"`. Your function should return true if you're talking 
with The Loch Ness Moster, false otherwise.

# My Solution
```ruby
def is_lock_ness_monster(string)
  ['tree fiddy', '3.50', 'three fifty'].each do |el|
    return true if string.include?(el)
  end
  false
end
```

# Better/Alternative solution from Codewars
```ruby
def is_lock_ness_monster(string)
  string.match? /(tree fiddy)|(3\.5)|(three fifty)/
end
```
