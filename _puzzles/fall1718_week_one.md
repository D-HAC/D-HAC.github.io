---
layout: page
title: Welcome to D-HAC
permalink: /puzzle/welcome1718
hide: false
week: 1
term: "Fall 2017-18"
---
# Drexel Hackathon and Coding Club
Welcome to the Drexel Hackathon and Coding Club! Here, we work on weekly coding challenges based around monthly themes. While you are free to work on your own projects during this hacking time, we encourage you to try our weekly puzzles and come up with creative, new solutions. Feel free to grab a partner and try them out or go it alone and see what you can create!

## What This Club is About
We are all about creating a hacking space and an environment where people can come together, create new things, learn new skills, be mentors, and become mentors. We wish to promote a love of programming and just create an club that people want to attend to hang out, talk, and have a good time. Feel free to use this club to talk to people to get advice on classes and coop.

## Our First Puzzle - Integer Divisibility

Integer divisibility might sound boring, but it is actually quite useful in a variety of situations (potentially during an interview!). The biggest example is determining whether a number is odd or even. A number is even when it is divisible by two.

**Hint**: the remainder operator--aka modulo (symbol: `%`)--is important here! If this is new to you, let us know and we'll help you!

## Functions to Write (They'll help!)

```C
bool is_divisible_by(int x, int n);
```

This method returns true if x is divisible by n, and false otherwise.
Assume `x >= 0` and `n > 0`.

Examples:

```C
is_divisible_by(4, 2); //=> True
is_divisible_by(3, 2); //=> False
is_divisible_by(6, 4); //=> False
is_divisible_by(6, 2); //=> True
```

## Puzzles

Once you've written the above function, try your hand at one (or both) of these two puzzles:

* [Game of Threes](https://www.reddit.com/r/dailyprogrammer/comments/3r7wxz/20151102_challenge_239_easy_a_game_of_threes/) - A basic printing puzzle based on divisibility. See if you can replicate the output shown in the puzzle!
* [FizzBuzz](https://www.reddit.com/r/dailyprogrammer/comments/s6bas/4122012_challenge_39_easy/) - This is a common programming puzzle that is used from time to time in interviews (or a variant of it).

If you are struggling with either of these, let someone know and we'll help you talk and work through the puzzles!

## Mini Project Ideas

If you'd like something more advanced than the above, try one of these project ideas! Feel free to make up your own project idea, but try to involve this week's theme of integer divisibility.

* Stripes - write a console program that displays stripes. Every Nth line, print a line of different characters. Examples:

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

* TICK. TOCK. - Make a program/web page that starts with 'TICK' in the middle of the screen. Every second, get the current seconds on the clock. If the number of seconds is divisible by 4 (or whatever number of seconds you would like), toggle the text once between 'TICK' and 'TOCK'. Also change the text/background color for effect.
* Bonus Puzzle: [Making Change](https://www.codewars.com/kata/making-change) - Note, this requires a CodeWars account (or GitHub)
