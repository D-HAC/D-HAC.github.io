---
layout: page
title: "Game of Threes: Integer Divisibility"
permalink: /puzzle/game-of-threes
hide: false
---

Integer divisibility might sound boring, but it is actually quite
useful in a variety of situations. The biggest example is determining
whether a number is odd or even. A number is even when it is divisible
by two.

**Hint**: the remainder operator--aka modulo (symbol: `%`)--is important here!
    If this is new to you, let us know and we'll help you!

## Functions to Add to Your Code Library

```C
bool is_divisible_by(int x, int n);
```

This method returns true if x is divisible by n, and false otherwise.
Assume `x >= 0` and `n > 0`.

Examples:

```python
is_divisible_by(4, 2) #=> True
is_divisible_by(3, 2) #=> False
is_divisible_by(6, 4) #=> False
is_divisible_by(6, 2) #=> True
```

## Puzzles

Today we have two

* [Game of Threes](https://www.reddit.com/r/dailyprogrammer/comments/3r7wxz/20151102_challenge_239_easy_a_game_of_threes/)
* [FizzBuzz](https://www.reddit.com/r/dailyprogrammer/comments/s6bas/4122012_challenge_39_easy/)

## Mini Project Ideas

* Stripes - write a console program that displays stripes. Every Nth line,
    print a line of different characters. Examples:

```
N=2
============================
----------------------------
============================
----------------------------
============================
----------------------------
```

```
N=3
============================
----------------------------
----------------------------
============================
----------------------------
```

* TICK. TOCK. - Make a program/web page that starts with 'TICK' in the
    middle of the screen. Every second, get the current seconds on the clock.
    If the number of seconds is divisible by 4 (or whatever number of seconds
    you would like), toggle the text once between 'TICK' and 'TOCK'. Also
    change the text/background color for effect.
* Bonus Puzzle: [Making Change](https://www.codewars.com/kata/making-change) - Note, this
    requires a CodeWars account (or GitHub)
