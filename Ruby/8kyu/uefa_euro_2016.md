# [UEFA EURO 2016](https://www.codewars.com/kata/57613fb1033d766171000d60)

# Description
Finish the uefaEuro2016() function so it return string just like in the examples below:

```
uefa_euro_2016(['Germany', 'Ukraine'],[2, 0]) # "At match Germany - Ukraine, Germany won!"
uefa_euro_2016(['Belgium', 'Italy'],[0, 2]) # "At match Belgium - Italy, Italy won!"
uefa_euro_2016(['Portugal', 'Iceland'],[1, 1]) # "At match Portugal - Iceland, teams played draw."
```

# My Solution
```ruby
def uefa_euro_2016(teams, scores)
  if scores.first > scores.last
    "At match #{teams.first} - #{teams.last}, #{teams.first} won!"
  elsif scores.first < scores.last
    "At match #{teams.first} - #{teams.last}, #{teams.last} won!"
  else
    "At match #{teams.first} - #{teams.last}, teams played draw."
  end
end
```

# Better/Alternative solution from Codewars
```ruby
def uefa_euro_2016(teams, scores)
  outcome = case scores.inject(:<=>)
            when 0
              "teams played draw."
            when 1
              "#{teams.first} won!"
            else
              "#{teams.last} won!"
            end

  "At match #{teams.join(' - ')}, #{outcome}"
end
```
