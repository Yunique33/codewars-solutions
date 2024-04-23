# [Get Planet Name By ID](https://www.codewars.com/kata/515e188a311df01cba000003)

## Description
The function is not returning the correct values. Can you figure out why?

Example **(Input --> Output )**:

```
3 --> "Earth"
```

## My Solution
```ruby
def get_planet_name(id)
  case id
  when 1 then "Mercury"
  when 2 then "Venus"
  when 3 then "Earth"
  when 4 then "Mars"
  when 5 then "Jupiter"
  when 6 then "Saturn"
  when 7 then "Uranus"
  when 8 then "Neptune"
  end
end
```

## Better/Alternative solution from Codewars
```ruby
def get_planet_name(id)
  %w[0 Mercury Venus Earth Mars Jupiter Saturn Uranus Neptune][id]
end
```
