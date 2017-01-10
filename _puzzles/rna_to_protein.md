---
layout: page
title: "RNA to Protein"
permalink: /puzzle/rna2protein
hide: true
week: 7
solutions: week7_RNAToBases
---

This week let's take a look into genetics. Specifically, RNA
Translation, the process in our cells where RNA is translated
into proteins.

RNA can be represented by four bases (AUCG). This is nearly the
same as DNA, except that Thymine (T) in DNA becomes Uracil (U)
in RNA.

Every three bases of RNA (called a codon) is translated to a single
amino acid. If you chain these amino acids together, you get a protein.

[Here is a table](http://rosalind.info/glossary/rna-codon-table/) of codons
and the amino acids they produce. This will be used in today's puzzle

## Functions to Add to Your Code Library

```
String[] by_threes(String text);
```
This function takes a string and splits it into groups of three. If the
length of the string is not divisible by three, the last group can be shorter
than three characters

Examples:

```python
by_threes("abcdefghi") #=> ["abc", "def", "ghi"]
by_threes("Hello World") #=> ["Hel", "lo ", "Wor", "ld"]
```

## Puzzle

Today's puzzle is take an RNA strand, split it into threes, and translate
to a protein string:

[ROSALIND: Translating RNA into Protein](http://rosalind.info/problems/prot/)

## Mini Project Ideas

If you'd like something more advanced than the above, try one of these
project ideas! Feel free to make up your own project idea, but try to involve
this week's theme of RNA translation

* If you used Python and have never used generators, try to write `by_threes()`
    using a generator to lazily generate the groups of three!
* Take a 1D array of `[text, red, blue, green, text, red, blue, green, ...]`
    and display each string of text in the RGB color specified. Example:
    `["Hello", 255, 0, 0, "World", 0, 0, 255]` would print "Hello" in red
    followed by "World" in blue. I recommend doing this in JavaScript in a
    web browser, though any programming environment that can display rich text
    could work.
