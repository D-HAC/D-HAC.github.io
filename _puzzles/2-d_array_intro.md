---
layout: page
title: Find the Path
permalink: /puzzle/2-d_array_intro
hide: false
week: 3
term: "Spring 2017-18"
---


This is a simple puzzle to get you used to reading in and working with 2-d arrays (arrays of arrays). It's good practice to separate out the code you use to initialize and manipulate a data structure, and that's especially true in these exercises. All of the 2-d arrays in these puzzles will be square or rectangular. A list of the functions you should develop for reuse are listed below the puzzle.


## Puzzle

Write a program that can read open a file and read the contents into a 2-d array. The file will contain x's and 2 o's. your program should take a file name and output directions on how to get from one o to the other.
Sample input:
<pre>
xxxxxxxxxxxxxx
xxoxxxxxxxxxxx
xxxxxxxxxxxxxx
xxxxxxxxxxoxxx
xxxxxxxxxxxxxx
</pre>
sample output: right 8, down 2

## Functions to save

read_file_to_2-d_array(filename)
get_column_as_array(number)
