---
layout: page
title: Goldilocks
permalink: /puzzle/goldilocks
hide: false
week: 2
term: "Winter 2016-17"
solutions: "week2_goldilocks"
---

Find the seat that is 'just right'

This week's puzzle is based on a recent dailyprogrammer challenge:
[/r/dailyprogrammer: Goldilocks' Bear Necessities](https://www.reddit.com/r/dailyprogrammer/comments/5bn0b7/20161107_challenge_291_easy_goldilocks_bear/)

The story so far:
Goldilocks has broken into the Bear family home and finds a table with a set of
chairs and a bowl of porridge at each chair. Goldilocks loves sitting in chairs
and eating porridge, but only if both are 'just right.'

We are going to write programs to help Goldilocks pick the right seat to sit at
and eat porridge.

The chair must support Goldilocks' weight without being to big. This means that,
of all the chairs which can support Goldilocks' weight, Goldilocks prefers the
chair that can support the least weight.

Goldilocks prefers porridge that is as hot as possible, without being hotter
than Goldilocks' heat limit.

The seat at the table which is 'just right' is the seat that minimizes both the
the extra weight the chair can support and the degrees cooler the porridge is
than Goldilocks' heat limit.

## Sample Input
    100 60
    --
    200 20
    50 99
    102 58

Each row consists of a weight and a temperature in Fahrenheit. The first row is
Goldilocks' weight and heat limit. Each row following the '--' is a different
seat at the table, with the maximum weight the chair can support and the
temperature of the porridge.

## Sample Output
    3

The third seat (row) is 'just right.'


## More Sample Input
    150 80
    --
    200 20
    150 99
    102 76
    210 32

## More Sample Output
    4

## Even More Sample Input
    100 100
    --
    50 100
    100 200

## Even More Sample Output
    Try the next house.

In this case, Goldilocks can not sit at any place at the table.


## Advanced Challenges

- Goldilocks' 2 friends, Silverlocks and Bronzelocks, have also broken into the
Bear house. Find the seating arrangement which makes all three as happy as
possible.

- The Bear house is kept as 10 degrees Celsius. Each bowl of porridge has a
surface area and thickness of 1. The thermal conductivity of the porridge is 0.5.
Goldilocks can wait for the porridges to cool down, but each minute of waiting
makes the situation less 'just right.' Output should consist of the place
Goldilocks should sit, followed by the time in minutes Goldilocks should wait
before eating.
