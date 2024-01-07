# [Decibel Scale](https://www.codewars.com/kata/5612a42e746aa62de100001a)

# Description
The following formula is called the Decibel Scale:

<img alt="Decibel Scale Formula" src="http://i.imgur.com/EikMPFO.png">

The Decibel Scale is used to determine the loudness of a sound, measured in dB:

* **β** is the result we want, defined in dB;
* We multiply the result of the logarithmic operation by 10, otherwise it'll be called "Bel Scale";
* We provide `I`, the `intensity` of the sound wave we need to find the loudness of, which is, for the purposes of this 
Kata, measured in 2D space and, hence, in `Watts per square meter`;
* Finally, we divide the intensity by the `threshold of human hearing`, also measured in `Watts per square meter`. This 
is the softest possible sound a human ear can hear;
* Since the threshold of human hearing involves an extremely small, long number, we need to utilize a logarithmic 
operation that will provide us the result in a convenient way.

Your task is to simply calculate the loudness of a sound wave, given its intensity as a parameter to the 
`dBScale/db_scale` function.

_Results are automatically rounded to the `nearest integer` by the test cases._

# My Solution
```ruby
def dBScale(i)
  10 * Math.log((i/(10 ** -12)), 10)
end
```

# Better/Alternative solution from Codewars
```ruby
def dBScale(i)
  10 * (12 + Math::log10(i))
end
```
