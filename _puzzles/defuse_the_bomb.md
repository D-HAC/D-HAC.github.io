---
layout: page
title: Defuse the Bomb
permalink: /puzzle/defuse-the-bomb
hide: false
term: "Winter 2016-17"
week: 6
---

To disarm a bomb, one must cut some wires. The order in which the wires are cut is very important; cut the wires in the wrong order and the bomb will explode. Here are the rules for how the wires should be cut:
```
If you cut a white wire you can't cut white or black wire.
If you cut a red wire you have to cut a green one.
If you cut a black wire, you are not allowed to cut a white, green or orange one.
If you cut a orange wire, you should cut a red or black one.
If you cut a green one, you have to cut a orange or white one.
If you cut a purple wire, you can't cut a purple, green, orange or white wire.
```
There can be multiple wires with the same color, however, only one wire may be cut at a time.

## The Challenge
The goal today is to write a program that receives a sequence of wires to be cut and determines, based off of the rules, whether or not the bomb will explode.

Example 1:

```
white
red
green
white

BOMB DEFUSED
```

Example 2:

```
white
orange
green
white

BOOM
```

Hint: [State Machines](https://en.wikipedia.org/wiki/Finite-state_machine)

## Hard Challenge
The challenge is ultimately the same, only this time, when the program starts, it requests a set of rules that must be entered by the user. It parses those rules, and then takes wire cutting inputs to determine if that input will cause the bomb to explode based on the new, custom rules.

Good luck!
