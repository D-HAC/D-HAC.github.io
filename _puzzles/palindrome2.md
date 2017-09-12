---
layout: page
title: Palindromes
permalink: /puzzle/palindromes_fa1718
hide: false
week: 2
term: "Fall 2017-18"
---
# It's October!
It is now the month of October, and the focus of this first month's theme is going to be "Text and Text-based Puzzles!" Welcome to our first set of puzzles in this theme.

# Background
Today, we are going to work with something called a palindrome. A palindrome is a word or phrase that is the same spelled forwards and backwards. For example:

`racecar`, `level`, `A man, a plan, a canal, Panama!`

Note that we ignore whitespace, punctuation and case-sensitivity in our particular examples, however, you can decided to handle it any way you like!.

## Functions to Write

```c++
bool is_palindrome(string str);
```

This function takes a string and checks if it reads the same both forwards and backwards.

**Hint:** Something that might be helpful is to write a function called `removeCharFromString(char c, string str)` which will take in a character and a string, and remove all instances of that character from the string and return the new version. This would be good for cleaning up inputs of symbols and whitespace.

Examples:

```c++
is_palindrome('a');                     //=> True
is_palindrome('aa');                    //=> True
is_palindrome('ab');                    //=> False
is_palindrome('racecar');               //=> True
is_palindrome('deleted');               //=> False
// Note: this assumes that we already handled whitespace/punctuation
is_palindrome('amanaplanacanalpanama'); //=> True
```

## Puzzle

Our puzzle is to check for palindromes given a phrase of text that may span
several lines: [/r/dailyprogrammer: Palindromes](https://www.reddit.com/r/dailyprogrammer/comments/3kx6oh/20150914_challenge_232_easy_palindromes/)

## Mini Project Ideas

If you'd like something more advanced than the above, try one of these project ideas! Feel free to make up your own project idea, but try to involve this week's theme of Palindromes.

* Try finding palindromes a different way. How would you do this recursively? (If you don't know what recursion is, try Googling it!)
* Generate palindromes by taking a string and appending a reversed copy of it. Example:

```
'abd' -> 'abddba' -> 'abddbaabddba' ->
```
