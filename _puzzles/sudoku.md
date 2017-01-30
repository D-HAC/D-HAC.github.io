---
layout: page
title: Sudoku
permalink: /puzzle/sudoku
# If true, this puzzle won't show up on the puzzle page
hide: false
# Make sure to match this format in order for the puzzles page
# to group puzzles properly
term: "Winter 2016-17"
week: 4
---

## Background

Sudoku is a numerical puzzle game that involves placing numbers in blocks within a grid. In a 
standard sudoku board the grid is 9x9 blocks. This 9x9 grid is then split up further into 9 3x3 
grid contained within. Each row and column of the 9x9 grid must contain 1 of each number from 1 to 9.
Additionally, each of the smaller 3x3 grids must contain 1 of each number 1 to 9. This means no number 
can appear twice in a row, column, or smaller grid. 

Here are two links that have example sudoku puzzles

[Easy 4x4 grid](http://1sudoku.com/play/sudoku-kids-free/sudoku-4x4/)
[Hard Standard 9x9 grid](http://1sudoku.com/play/sudoku-free-online/) 

## Easy Challenge

The first step in writing a solver is to determine if a board is 
solved and valid. Boards are valid if all of the spaces are filled in and
no row, column, or subgrid have a number written twice. For example:

```
1 2 3 4
4 3 2 1
3 1 4 2 
2 4 1 3

is a valid 4x4 board

1 2 4 3
3 4 1 2
2 3 3 1
4 1 2 4

is not a valid 4x4 board
```

Write a program that will return true if a board is valid and false if it is not. 

## Medium Challenge

Write a program that will solve a 4x4 sudoku puzzle. 

## Hard Challenge

Write a program that will solve a 9x9 sudoku puzzle.


## Hint

For input to your program consider using a Comma Seperated Value (CSV) file or a 
Whitespace Seperated Value (WSV) file. These are very common file formats and 
writing programs that interpret it can be a very valueable skill on co-op. 
