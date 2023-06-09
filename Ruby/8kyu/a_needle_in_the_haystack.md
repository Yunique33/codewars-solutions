# [A Needle in the Haystack](https://www.codewars.com/kata/56676e8fabd2d1ff3000000c)

# Description
Can you find the needle in the haystack?

Write a function <code>findNeedle()</code> that takes an <code>array</code> full of junk but containing 
one <code>"needle"</code>

After your function finds the needle it should return a message (as a string) that says:

<code>"found the needle at position "</code> plus the <code>index</code> it found the needle, so:

**Example(Input --> Output)**
>["hay", "junk", "hay", "hay", "moreJunk", "needle", "randomJunk"] --> "found the needle at position 5"


# My Solution
```ruby
def find_needle(haystack)
  "found the needle at position #{haystack.index('needle')}"
end
```