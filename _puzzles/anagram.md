---
layout: page
title: "Anagram Detector"
permalink: /puzzle/anagram
hide: true
week: 8
---

String manipulation in general is both very useful and sometimes a little tricky. Before you start hacking away at this challenge look to see if there are any useful libraries that will help you in your language of choice.

Today we are going to try to detect if a phrase is an anagram of another phrase. A phrase a="wisdom" is an anagram of another phrase b="mid sow" if, ignoring spaces, one phrase can be written with the letters of another.

## Functions to Add to Your Code Library


```c
bool containsLetter(char letter, string word);
```

One way to start solving this problem is to check if each letter in phrase a exists in phrase b. However, this solution is not perfect. One requirement of an anagram is that you can not use the letters of phase b in phrase a more than once. For example "Reddit" is not an anagram of "Eat Dirt" even though all of the letters are there 'd' can not be repeated.

Examples:

```python
containsLetter('a', "hello") #=> False
containsLetter('h', "hello") #=> True
```

## Puzzle

Solving the full puzzle will require getting a little more creative. Check out the daily programmer link for more details.


[/r/dailyprogrammer: Anagram Detector](https://www.reddit.com/r/dailyprogrammer/comments/52enht/20160912_challenge_283_easy_anagram_detector/)

## Mini Project Ideas

* To get even crazier, try to generate anagrams based off of a phrase or word. You can google search for a dictionary file or use the unix one to start.
