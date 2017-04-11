---
layout: page
title: mazes
permalink: /puzzle/mazes
hide: true
week: 2
term: "Spring 2016-17"
---

## Background

This week we are going to work on writing programs to solve mazes! There are lots of great algorithms for solving a maze, see if you can implement multiple solving methods. A good place to start might be the Wikipedia page, [Maze solving algorithm](https://en.wikipedia.org/wiki/Maze_solving_algorithm).

## The Challenge

Given a file containing a maze that looks like this:
```
+--+--+--+--+--+
   |           |
+  +  +--+--+  +
|     |  |     |
+--+--+  +  +--+
|     |     |  |
+  +  +--+  +  +
|  |        |  |
+  +--+--+--+  +
|               
+--+--+--+--+--+
```


```bash
./mazesolver maze1.txt
```

Output:

```
+--+--+--+--+--+
###|###########|
+##+##+--+--+##+
|#####|  |#####|
+--+--+  +##+--+
|#####|   ##|  |
+##+##+--+##+  +
|##|########|  |
+##+--+--+--+  +
|###############
+--+--+--+--+--+
```


## Maze generating site
[Maze generator](http://www.delorie.com/game-room/mazes/genmaze.cgi)

## Bonus Challenge 1

Write a program that generates maze text files that you can feed into your maze solving program.

## Bonus Challenge 2

If you've written multiple maze solving methods, write a program that analyzes which method is the most efficient for solving a given maze. See if you can discover if certain methods are more effective for a particular type of maze, and if there is a certain method that is the most efficient in general.
