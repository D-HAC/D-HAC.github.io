---
layout: page
title: "DNA to RNA to Protein"
permalink: /puzzle/dna2protein
hide: false
week: 4
term: "Fall 2017-18"
---
# October Week 3
We are still working on fun, text-based puzzles but this one has a biological twist! Enjoy!

## Background
This week let's take a look into genetics. Specifically, DNA transcription (transcribing DNA into RNA) and RNA translation (translating RNA to proteins).

## Write Code to Transcribe DNA to RNA
DNA has the bases ATCG, whereas RNA has the bases AUCG. Here is a key for that transcription:

```
DNA -> RNA
 A  ->  U
 T  ->  A
 C  ->  G
 G  ->  C
```

The first goal is to take a string of DNA and transcribe it to RNA:

```
Input: ACGTACT
Output: UGCAUGA
```

## Write Code to Translate RNA to proteins
The next step is to take that RNA and turn it into a protein. Every three bases of RNA (called a codon) is translated to a single amino acid. If you chain these amino acids together, you get a protein.

[Here is a table](http://rosalind.info/glossary/rna-codon-table/) of codons and the amino acids they produce. This will be used in today's puzzle

### Functions to Write

```c++
String[] by_threes(String text);
```
This function takes a string and splits it into groups of three. If the length of the string is not divisible by three, the last group can be shorter than three characters.

Examples:

```c++
by_threes("abcdefghi");   //=> ["abc", "def", "ghi"]
by_threes("Hello World"); //=> ["Hel", "lo ", "Wor", "ld"]
```

### Puzzle - Split and Translate

Today's puzzle is take an RNA strand, split it into threes, and translate to a protein string: [ROSALIND - Translating RNA into Protein](http://rosalind.info/problems/prot/)

## Mini Project Ideas

If you'd like something more advanced than the above, try one of these project ideas! Feel free to make up your own project idea, but try to involve this week's theme of DNA and RNA.

* If you used Python and have never used generators, try to write `by_threes()` using a generator to lazily generate the groups of three!
* Take a 1D array of `[text, red, blue, green, text, red, blue, green, ...]` and display each string of text in the RGB color specified. Example: `["Hello", 255, 0, 0, "World", 0, 0, 255]` would print "Hello" in red followed by "World" in blue. I recommend doing this in JavaScript in a web browser, though any programming environment that can display rich text could work.
