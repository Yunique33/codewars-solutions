# [Playing with cubes I](https://www.codewars.com/kata/55c0a79e20be94c91400014b )

# Description
Create a public class called **Cube _without_** a constructor which gets one single private integer variable **Side**, a
getter **GetSide()** and a setter **SetSide(int num)** method for this property. Actually, getter and setter methods are
not the common way to write this code in C#. In the next kata of this series, we gonna refactor the code and make it a 
bit more professional...

Notes:
* There's no need to check for negative values!
* initialise the side to 0.

# My Solution
```ruby
class Cube
  def get_side
    @side.to_i
  end

  def set_side(side)
    @side = side
  end
end
```
