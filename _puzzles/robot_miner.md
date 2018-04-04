---
layout: page
title: "Robot in a Minefield"
permalink: /puzzle/robot_miner
hide: false
week: 1
term: "Winter 2017-18"
---
# Welcome Back!
Welcome back to the Drexel Hackathon and Coding Club! It's time for a new year and new set of puzzles. We hope you'll enjoy what we have selected for you all.

# Today's Challenge
The goal of today's challenge is to a build a text-based simulator for a robot traveling through a minefield. For example, given a minefield like this:
```
At start:
+++++++++++++
+???????????
+???????????+
+???????????+
+???????????+
+???????????+
R???????????+
+++++++++++++

Revealed:
+++++++++++++
+000000*0000
+00000000000+
+00000*00000+
+00000000000+
+0*000000000+
R000000000*0+
+++++++++++++

Key:
+ = wall
? = unknown space
0 = safe space
* = mine
R = robot
  = either exit or entrance (leave these open)
```
The goal would be to move the robot through the minefield with a series of commands, getting it safely from the entrance to the exit. This is done through issuing it a command sequence to tell it to move:
```
Input: DDW
```
would move the robot right twice and up once (following the WASD method of moving the robot). In the end, you might have a sequence that looks like this:
```
Welcome!

+++++++++++++
+???????????
+???????????+
+???????????+
+???????????+
+???????????+
R???????????+
+++++++++++++
Input: DDWWWWWDDDDDDDDDD

+++++++++++++
+???????????
+???????????+
+???????????+
+???????????+
+?*?????????+
 00?????????+
+++++++++++++
Output: Robot exploded!
```
## Making the Map
Having a good representation for the minefield will make your life easier. Think of potential ways you could represent your minefield such as arrays, lists, or other data structures. Once you have a good way of representing the minefield, write a function to print it to the console:
```
# Takes a field and prints it out to the console. Returns nothing
def printMinefield(field):
```
## Taking Note
Things you should think about how you wish to handle:
* Saving the robot location
* Saving locations of the mines (to check as the robot moves)
* Processing robot moves (you might want to stop if you hit a mine)

Some functions you might want to write:
```
# Potential function that could take the field, robot position and an input string to move the robot
def moveRobot(field, robot, input_str):

# Potential function that could check if a move is valid. Could have a return based on wall, mine, or open space
def checkMove(move, field):
```

## Want to Add More?
Here are a few ideas to make things even more complex:
* Allow users to type how big they want their minefield to be
* Randomly generate mines (make sure the exit and entrance are unblocked though!)
* Have difficulty options for number of mines (maybe percentage of field covered based on difficulty)
* Want more than just mines, walls, and open spaces? Maybe add holes or complex map shapes

Adapted from [/r/dailyprogrammer](https://www.reddit.com/r/dailyprogrammer/comments/7d4yoe/20171114_challenge_340_intermediate_walk_in_a/)
