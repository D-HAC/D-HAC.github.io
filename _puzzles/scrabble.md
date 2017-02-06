---
layout: page
title: Scrabble
permalink: /puzzle/scrabble
hide: false
term: "Winter 2016-17"
week: 5
---

## Background

Scrabble is a word game where players are given 7 tiles and take turns strategically placing them to spell words with the highest value. More obscure letters have a higher point value. Today, our challenge involves taking a set of seven tiles and determining if a given word can be spelled using those tiles.

For more on Scrabble: [Wikipedia: Scrabble](https://en.wikipedia.org/wiki/Scrabble)

## Easy Challenge

This challenge simply asks you to write a function that takes a random string of letters and determines if a string input can be spelled using those specific letters. You can randomly generate the tiles or you can just hard code them. The goal of this challenge is to focus on whether a word can be spelled or not.

```
scrabble("ladilmy", "daily") -> true
scrabble("eerriin", "eerie") -> false
scrabble("orrpgma", "program") -> true
scrabble("orppgma", "program") -> false
```

Write a program that will return true if the word can be spelled; otherwise, return false.

## Challenge 1

The extension of this challenge is, given a list of 20 tiles, what is the longest word that can be spelled out of the list of English words found in [this text file](https://storage.googleapis.com/google-code-archive-downloads/v2/code.google.com/dotnetperls-controls/enable1.txt).

```
longest("dcthoyueorza") ->  "coauthored"
longest("uruqrnytrois") -> "turquois"
longest("rryqeiaegicgeo??") -> "greengrocery"
longest("udosjanyuiuebr??") -> "subordinately"
longest("vaakojeaietg????????") -> "ovolactovegetarian"
```

## Challenge 2

Similarly to challenge 1, the goal is to create a word out of 20 tiles. This time though, find the highest scoring word you can create given a set of 20 tiles based off of the scores found on [Wikipedia: Scrabble](https://en.wikipedia.org/wiki/Scrabble).
```
highest("dcthoyueorza") ->  "zydeco"
highest("uruqrnytrois") -> "squinty"
highest("rryqeiaegicgeo??") -> "reacquiring"
highest("udosjanyuiuebr??") -> "jaybirds"
highest("vaakojeaietg????????") -> "straightjacketed"
```

Taken from [/r/dailyprogrammer](https://www.reddit.com/r/dailyprogrammer/comments/5go843/20161205_challenge_294_easy_rack_management_1/)
