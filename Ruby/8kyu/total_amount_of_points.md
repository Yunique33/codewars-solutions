# [Total amount of points](https://www.codewars.com/kata/5bb904724c47249b10000131/ruby)

# Description
Our football team has finished the championship.

Our team's match results are recorded in a collection of strings. Each match is represented by a string in the 
format <code>"x:y"</code>, where <code>x</code> is our team's score and <code>y</code> is our opponents score.

For example: <code>["3:1", "2:2", "0:1", ...]</code>

Points are awarded for each match as follows:

* if x > y: 3 points (win)
* if x < y: 0 points (loss)
* if x = y: 1 point (tie)

We need to write a function that takes this collection and returns the number of points our team <code>(x)</code> got 
in the championship by the rules given above.

Notes:

* our team always plays 10 matches in the championship
* 0 <= x <= 4
* 0 <= y <= 4

# My Solution
```ruby
def points(games)
  games.map do |match|
    first = match[0]
    second = match[-1]
    if first > second
      3
    elsif first < second
      0
    else
      1
    end
  end.sum
end
```
# Better/Alternative solution from Codewars
```ruby
def points(games)
  games.sum { |score| [1, 3, 0][score[0] <=> score[2]] }
end
```
