---
layout: page
title: Counting Bases
permalink: /puzzle/counting bases
hide: false
week: 6
term: "Fall 2016-17"
solutions: week6_countingbases
---

Sometimes it's useful to go through a list and tally up how many of each
type of thing is found. Today, we'll do just that.

## Functions to Add to Your Code Library

```c++
map<char, int> count_chars(string input);
```
The above function should take a string of text, and count up how many of
each letter there is. The return value should be a map/dictionary/associative
array (depending on your programming language of choice) that maps characters
to the number of occurrences in the string.

It should be easy to support both alphanumeric characters and non-alphanumeric
characters, so try to do both!

Examples:

```python
count_chars("ABCDAB") #=> {"A": 2, "B": 2, "C": 1, "D": 1}
count_chars("AB BA") #=> {"A": 2, "B": 2, " ": 1}
```

## Puzzle

Rosalind's first bioinformatics programming problem deals with counting up
DNA base pairs:

[Rosalind: Counting DNA Nucleotides](http://rosalind.info/problems/dna/)

## Mini Project Ideas

If you'd like something more advanced than the above, try one of these
project ideas! Feel free to make up your own project idea, but try to involve
this week's theme of counting characters in a string

* Take a paragraph of text as a single string. Determine which are the top
    five most common letters in the paragraph. Print these five letters out
    along with how many times they occurred.
* Write a program that takes a single string of text. If the number of 'A's
    in the string is bigger than the number of 'E's, print "You Win!".
    Otherwise, print "You Lose!"
* Pretend you are a professor trying to compute the class average based on
    letter grades alone. You get a list of grades like this: `"AABCAABDAFDBCC"`.
    Using this map of
    [Grade to Grade Points](http://drexel.edu/provost/policies/grades/), and
    the `count_chars()` function, compute the average class grade points. You
    can assume that all grades are one of `{A, B, C, D, F}`, no pluses or
    minuses.
