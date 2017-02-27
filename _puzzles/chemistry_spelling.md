---
layout: page
title: Spelling with Chemistry
permalink: /puzzle/chemistry-spelling
hide: false
term: "Winter 2016-17"
week: 8
---
The periodic table of elements is a table of all the chemical elements that have been discovered and classified, and is something that we all have a bit of familiarity with. Today's challenge involves using that table of elements that we all know and love to spell words that are inputted by a user.

## The Challenge
Today's goal is to spell user-inputted words with elements from the periodic table by using their 1-2 letter chemical symbol. For example, given the input:

```
luck
functions
bacon
poison
sickness
ticklish
```

The program should output:

```
LuCK (lutetium, carbon, potassium)
FUNCTiONS (flourine, uranium, nitrogen, carbon, titanium, oxygen, nitrogen, sulfur)
BaCoN (barium, cobalt, nitrogen)
POISON (phosphorus, oxygen, iodine, sulfur, oxygen, nitrogen)
SiCKNeSS (silicon, carbon, potassium, neon, sulfur, sulfur)
TiCKLiSH (titanium, carbon, potassium, lithium, sulfur, hydrogen)
```

Some words will be impossible to spell. If that is the case, let the user know.

Here is a list of elements for reference: [List of Chemical Elements](https://en.wikipedia.org/wiki/List_of_chemical_elements)

## Bonus Challenge 1
Some words can be spelled multiple ways. Print out every combination of chemical symbols that can be used to create the user-specified word.

## Bonus Challenge 2
Since some words can be spelled multiple ways, there can be a way to determine which spelling is a 'better' one to use. Use other properties of the elements such as atomic weight, density, and melting point to determine which elements would be the best combination to spell the word based on the lowest or highest summation of the property chosen to make the distinction.

Adapted (slightly) from [/r/dailyprogrammer](https://www.reddit.com/r/dailyprogrammer/comments/5seexn/20170206_challenge_302_easy_spelling_with/).
