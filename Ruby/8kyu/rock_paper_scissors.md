# [Rock Paper Scissors!](https://www.codewars.com/kata/5672a98bdbdd995fad00000f)

# Description
## Rock Paper Scissors
Let's play! You have to return which player won! In case of a draw return <code>Draw</code>!.

### Examples(Input1, Input2 --> Output):

>"scissors", "paper" --> "Player 1 won!"\
"scissors", "rock" --> "Player 2 won!"\
"paper", "paper" --> "Draw!"

![rockpaperscissors](http://i.imgur.com/aimOQVX.png)
# My Solution

```ruby
def rps(p1, p2)
  options = %w[scissors paper rock]
  result = options.index(p1) - options.index(p2)
  if result == -1 || result == 2
    'Player 1 won!'
  elsif result.zero?
    'Draw!'
  else
    'Player 2 won!'
  end
end
```

# Better/Alternative solution from Codewars
```ruby
def rps(p1, p2)
  beatmap = { 'scissors' => 'paper', 'paper' => 'rock', 'rock' => 'scissors' }

  if p1 == p2
    "Draw!"
  elsif beatmap[p1] == p2
    "Player 1 won!"
  else
    "Player 2 won!"
  end
end
```