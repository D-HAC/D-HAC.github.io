---
layout: page
title: Sudoku Checker
permalink: /puzzle/sudoku_checker
# If true, this puzzle won't show up on the puzzle page
hide: false
# Make sure to match this format in order for the puzzles page
# to group puzzles properly
term: "Spring 2017-18"
week: 4
---
### NOTE:

It will probably be easier to do this challenge if you've already done last week's [intro to 2-d arrays](https://d-hac.github.io/puzzle/2-d_array_intro) and have code to reuse from that.

## Background

Sudoku is a numerical puzzle game that involves placing numbers in blocks within a grid. In a
standard sudoku board the grid is 9x9 blocks. This 9x9 grid is then split up further into 9 3x3
grid contained within. Each row and column of the 9x9 grid must contain 1 of each number from 1 to 9.
Additionally, each of the smaller 3x3 grids must contain 1 of each number 1 to 9. This means no number
can appear twice in a row, column, or smaller grid.

Here are two links that have example sudoku puzzles

[Easy 4x4 grid](http://1sudoku.com/play/sudoku-kids-free/sudoku-4x4/)
[Hard Standard 9x9 grid](http://1sudoku.com/play/sudoku-free-online/)

## The Challenge

This week we're writing a checker for sudoku boards. We will be checking for both correctness and completeness. A board is correct if no row, column, or sub-block contains a duplicate number. Is is complete if all of the spaces are filled in:

```
1 2 3 4
4 3   1
3 1 4 2
2   1 3

is a correct, incomplete 4x4 board

1 2 4 3
3 4 1 2
2 3 3 1
4 1 2 4

is an incorrect, complete 4x4 board

4 1 2 3
2 3 4 1
1 4 3 2
3 2 1 4

is a correct, complete 4x4 board
```

Write two functions: one that checks if the board is complete, and one to check if it is correct.
