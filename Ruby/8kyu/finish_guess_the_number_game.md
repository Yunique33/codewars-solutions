# [Finish Guess the Number Game](https://www.codewars.com/kata/568018a64f35f0c613000054)

## Description
Imagine you are creating a game where the user has to guess the correct number. But there is a limit of how many guesses
the user can do.

* If the user tries to guess more than the limit, the function should throw an error.
* If the user guess is right it should return true.
* If the user guess is wrong it should return false and lose a life.

Can you finish the game so all the rules are met?

## My Solution
```ruby
class Guesser
  def initialize(number, lives)
    @number = number
    @lives = lives
  end

  def guess(n)
    raise error if @lives.zero?
    if n != @number
      @lives -= 1
      false
    else
      true
    end
  end
end
```
