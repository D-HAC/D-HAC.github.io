---
layout: page
title: 1D and 2D Arrays
permalink: /puzzle/arrays_1d_2d
hide: false
week: 5
solutions: week5_arrays
---

1D Arrays are very common in programming. Often one needs a list of items
of fixed length.

2D arrays are also common for representing fixed-sized grids of items.
Board games and images use these types of data structures.

Sometimes we need to convert between the two. How does one do this?

First, let's examine how we index each type of array:

| Dimensions | How to Index | Index Values in usual order |
|----|-------------------|--------------------------------------------|
| 1D | `array[i]`        | `0, 1, 2, 3, ...`                          |
| 2D | `array[row][col]` | `(0, 0), (0, 1), ..., (1, 0), (1, 1), ...` |

### Converting from 1D -> 2D

Now, how do we convert indices to `(row, col)` pairs? Let's look at a couple
arrays:

```
0 1  2  3
4 5  6  7
8 9 10 11

4 -> (1, 0)

0 1 2
3 4 5
6 7 8

4 -> (1, 1)
```

It's a slightly different conversion depending on the grid size! How do we
handle this? As it turns out, we only need to know the width of the grid
(number of columns). With some integer division/modulo magic, it's actually
pretty simple to convert:

`row = index / num_cols` (Remember: Integer division!)    
`col = index % num_cols`

Why does this work? Examine these when `num_cols = 4`:

`row = index / 4 = 0, 0, 0, 0, 1, 1, 1, 1, 2, 2, 2, 2, ...`  
`col = index % 4 = 0, 1, 2, 3, 0, 1, 2, 3, 0, 1, 2, 3, ...`

Notice how the column number cycles from 0 through 3 and repeats that pattern
over and over like we'd expect. However, the row number is always increasing
as we add each new row. If you look at any particular column, you get the
`(row, col)` value. Neat trick, huh?

### 2D -> 1D

Now for something a bit more straightforward, converting from 2D to 1D.
Let's look at an example grid:

```
(0, 0) (0, 1) (0, 2) (0, 3)     0 1  2  3
(1, 0) (1, 1) (1, 2) (1, 3) --> 4 5  6  7
(2, 0) (2, 1) (2, 2) (2, 3)     8 9 10 11
```

Again, the conversion depends on the width of the grid. Think of it like this:

1. Skip to the first cell of row `row`. How many cells did you skip?
    `row * cells in row`, right?
2. Move to the right `col` cells. You're now at the desired cell `(row, col)`,
    and have now skipped `col` more cells. The number of cells we've skipped
    is the index.

Put it all together:

`index = row * num_cols + col`

## Functions to Add to Your Code Library

**Note**: You may use dynamic arrays (aka vector or ArrayList) if you would
    like, as long as you know how they look in 1D and 2D

### Index Conversions

```c++
pair<int, int> index_to_row_col(int index, int num_cols);
```

Convert a 1D index to a 2D `(row, col)` pair.

Examples:

```python
index_to_row_col(3, 2) #=> (1, 1)
index_to_row_col(3, 4) #=> (0, 3)
```

```c++
int row_col_to_index(int row, int col, int num_cols);
```

Convert a 2D `(row, col)` pair to a 1D index.

Examples:

```python
row_col_to_index(1, 2, 5) #=> 7
row_col_to_index(2, 2, 3) #=> 8
```

### Array Conversions

```c++
vector<vector<int>> arr_1d_to_2d(vector<int> arr, int width);
```

Convert 1D array (or vector) to 2D array

Examples:

```python
arr_1d_to_2d([1, 2, 3, 4, 5, 6], 2) #=> [[1, 2], [3, 4], [5, 6]]
```

```c++
vector<int> arr_2d_to_1d(vector<vector<int>> arr, int width);
```

Convert a 2D array to a 1D array

Examples:

```python
arr_2d_to_1d([ #=> [1, 2, 3, 4, 5, 6, 7, 8, 9]
    [1, 2, 3],
    [4, 5, 6],
    [7, 8, 9]
], 3)
```

## Puzzle

Using the above, You can try this array puzzle. You do not need to use C
unless you want to.

[2D Array Puzzle](https://chortle.ccsu.edu/CPuzzles/PartD/CpuzzlesDsection01.html#D01)

## Mini Project Ideas

If you'd like something more advanced than the above, try one of these
project ideas! Feel free to make up your own project idea, but try to involve
this week's theme of 1D/2D Arrays:

* [Netpbm](https://en.wikipedia.org/wiki/Netpbm_format) is a very simple image
    format designed to be human-readable. However, it is not very efficient
    for storage since it has many whitespace characters in it. Write a program
    that does the following:
    * Read a PBM file and turn it into an array
    * Turn the array into a 1D array
    * Save this 1D array to a binary file format. Without compressing the file,
        find a compact way to store the numbers.
* Write a program that can read a list of numbers and print them in an zig-zag
    order like this:

```
 0  1  2  3  4
 9  8  7  6  5
10 11 12 13 14
```

* Write a program that reads a list of numbers, turns it into a 2D array
    and does some of the following operations that might be useful in puzzle
    games. Pick whichever ones sound fun:
    * Flip the 2D array horizontally/vertically
    * Rotate the 2D array in multiples of 90 degrees
    * Swap rows and columns (transpose)
    * Cycle rows around:

```
0 1 2     1 2 0
3 4 5  -> 4 5 3
6 7 8     7 8 6
```
