---
layout: page
title: Light Switches
permalink: /puzzle/light-switches
hide: false
week: 3
term: "Spring 2016-17"
---

## Background
This challenge is all about the flipping of light switches. Input will specify the number of light switches available and then the order in which light switches are flipped. The goal is to determine the number of lights that will be on after a series of light switches have been flickered on and off. The challenge explains in detail what this input looks like.

## The Challenge
The first line of input will always start with the number of light switches, N. The subsequent lines will feature a range of switches, 0 - N-1, that will be flipped. They can be in ascending or descending order. When there is no more input, the program must determine how many lights are currently on. A sample input would look this:
```
10
3 6
0 4
7 3
9 9
```
Which would give an output of:
```
7
```
Since there are 7 lights on at the end of this sequence of light flipping.

A visualization of why this is 7 is shown here:
```
    0123456789
    ..........
3-6    ||||
    ...XXXX...
0-4 |||||
    XXX..XX...
7-3    |||||
    XXXXX..X..
9-9          |
    XXXXX..X.X
```

## Bonus 1
Create a program that outputs the steps taken in switching the lights, similar to the graphical representation given in the above example.

## Bonus 2
Make your program as effecient as possible and try to parse the lights switches found in [this](https://raw.githubusercontent.com/fsufitch/dailyprogrammer/master/ideas/switches/lots_of_switches.txt) text file with 5,000,000 light switches and 200,000 light switch ranges.

Puzzle from [/r/dailyprogrammer](https://www.reddit.com/r/dailyprogrammer/comments/46zm8m/20160222_challenge_255_easy_playing_with_light/).
