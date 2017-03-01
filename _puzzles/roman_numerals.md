---
layout: page
title: "Roman Numerals"
permalink: /puzzle/roman-numerals
# If true, this puzzle won't show up on the puzzle page
hide: false
week: 9
# Make sure to match this format in order for the puzzles page
# to group puzzles properly
term: "Winter 2016-17"
---

Let's go back in time to way before we had integers and floats. Before we
had base-10 numerals. Let's go to ancient Rome and do as the Romans do: Use
Roman Numerals.

## Roman Numeral Refresher

Just in case anyone needs a refresher on how roman numerals work, here's a
description

Roman numerals are written with the following letters:

| Letter | Value |
|--------|-------|
| I      |     1 |
| V      |     5 |
| X      |    10 |
| L      |    50 |
| C      |   100 |
| D      |   500 |
| M      |  1000 |

Normally, you list these letters in descending order of value and add their
values:

```
VII = 5 + 1 + 1 = 7
CLV = 100 + 50 + 5 = 155
MMXVII = 2 * 1000 + 10 + 5 + 2 * 1 = 2017
```

However, this would make numbers like 9 super long: `VIIII`. So instead, we
can use some subtraction rules:

* `I` before `V` or `X` means one less than the value. Example: `IV = 4` and
  `IX = 9`
* `X` before `L` or `C` means ten less than the value. Example: `XL = 40` and
  `XC = 90`
* `C` before `D` or `M` means 100 less than the value. Example: `CD = 400` and
  `CM = 900`

## Basic Challenge

Write two functions:

```c
int roman2dec(str roman); //Convert Roman Numerals to integer
```

Examples:

```python
roman2dec("VII") # => 7
roman2dec("MCDIV") # => 1404
roman2dec("MMXVII") # => 2017
```

```c
str dec2roman(int dec); //Convert (positive) integer to roman numerals
```

Examples:

```python
dec2roman(7) # => "VII"
dec2roman(1404) # => "MCDIV"
dec2roman(2017) # => "MMXVII"
```

## Puzzles Online

Here are some puzzles online that deal with roman numerals

* [CodeWars: Roman Numerals Decoder](https://www.codewars.com/kata/roman-numerals-decoder)
* [CodeWars: Roman Numerals Encoder](https://www.codewars.com/kata/roman-numerals-encoder)
* [CodeWars: Roman Numerals Helper](https://www.codewars.com/kata/roman-numerals-helper)
* [Project Euler 89](https://projecteuler.net/problem=89) - Examine some
  malformed roman numerals and see how much longer they are than the correct
  representation
