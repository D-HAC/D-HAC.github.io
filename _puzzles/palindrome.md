---
layout: page
title: Palindromes
permalink: /puzzle/palindromes
hide: true
week: 4
solutions: week4_palindromes
---

A palindrome is a word or phrase that is the same spelled forwards and
backwards. Examples:

`racecar`, `level`, `A man, a plan, a canal, Panama!`

Note that we ignore whitespace, punctuation and case-sensitivity.

## Functions to Add to Your Code Library

```c++
bool is_palindrome(string str);
```

This function takes a string and checks if it reads the same both forwards
and backwards.

In a previous week we wrote `removeCharFromString()`. Thus, you can handle
removing whitespace/punctuation outside of `is_palindrome()` if you wish.

Examples:

```python
is_palindrome('a') #=> True
is_palindrome('aa') #=> True
is_palindrome('ab') #=> False
is_palindrome('racecar') #=> True
is_palindrome('deleted') #=> False
# Note: this assumes that we already handled whitespace/punctuation
is_palindrome('amanaplanacanalpanama') #=> True
```

## Puzzle

Our puzzle is to check for palindromes given a phrase of text that may span
several lines:
[/r/dailyprogrammer: Palindromes](https://www.reddit.com/r/dailyprogrammer/comments/3kx6oh/20150914_challenge_232_easy_palindromes/)

## Mini Project Ideas

If you'd like something more advanced than the above, try one of these
project ideas! Feel free to make up your own project idea, but try to involve
this week's theme of Palindromes

* Try finding palindromes a different way. How would you do this recursively?
* Generate palindromes by taking a string and appending a reversed copy of it.
    Example:

```
'abd' -> 'abddba' -> 'abddbaabddba' ->
```
