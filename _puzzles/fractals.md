---
layout: page
title: "Fractals"
permalink: /puzzle/fractals
hide: false
week: 7
term: "Fall 2017-18"
---

# It's November!
It is now the month of November, and the focus of this month's theme is going to be "Visuals." We're going to try and have a diverse set of puzzles that focus on making something interactive and/or visually engaging. This week we are looking at Turtle Graphics and Fractals (though use anything you want to, if you have a different idea of how you'd like to make fractals).

## Setup

Python comes with a cool built-in turtle graphics module called `turtle`.
[Python Downloads](https://www.python.org/downloads/) - I'd recommend choosing
Python 3

## Turtle Graphics

Turtle graphics is an old method of generating graphics. It dates all the way
back to the [Logo programming language, first released in 1967](http://el.media.mit.edu/logo-foundation/what_is_logo/history.html).

You start with the "Turtle", a fictional robot that drags a pen across paper
(or in our case, the screen). It can be controlled by simple commands.

In Python:

```python
import turtle
t = turtle.Turtle() # make a new turtle
```

The turtle has a position on the screen and has some orientation angle
in degrees.

Here are the basic commands to control the turtle:

The basic commands:

| Command          | Description |
|------------------|-------------|
| `t.forward(x)`   | Move forward `x` pixels |
| `t.backward(x)`  | Move backwards `x` pixels |
| `t.left(angle)`  | Turn in place `angle` degrees to the left |
| `t.right(angle)` | Turn in place `angle` degrees to the right |
| `t.penup()`      | Lift the pen from the "paper". This allows moving without drawing a line |
| `t.pendown()`    | Press the pen down onto the "paper". Now the turtle will resume drawing lines |

There are several other commands, but I'll let you
[read the docs](https://docs.python.org/2/library/turtle.html).

## Example Program:

```python
import turtle

# Create our turtle
t = turtle.Turtle()

# Draw a cool pattern by drawing straight lines then making sharp
# angled turns
for i in range(9):
    # Move 300 pixels forward
    t.forward(300)
    # Turn to the right 200 degrees
    t.right(200)

# This keeps the turtle window open at the end of the program
turtle.mainloop()
```

This produces a design like this:

![Turtle Design]({{site_url}}/images/turtle_example.png)

## Puzzle

Try as many of these as you can manage:

* Draw a square
* Draw a hexagon
* Draw a triangle
* Let the user type a number of sides and generate a polygon with that many
    sides
* Draw a square spiral
* Draw a pattern with circles (hint: [read the docs](https://docs.python.org/2/library/turtle.html).)
* Try changing the pen color (again, read the docs!)

When you feel satisfied with the above, get creative and make your own design.

## The Challenge: Fractals

There is class of fractals that are easily drawn with turtle graphics. Here's
an example, the von Koch Snowflake:

Step 0: Start with a triangle. Turtle commands:
1. Move forwards some amount of pixels (start with a big number)
2. Turn left 120°
3. Repeat steps 1 and 2 twice more

![Initiator]({{site_url}}/images/koch0.png)

Step 1: Replace every forward command with the following:
1. Move forward 1/3 of the old distance
2. Turn right 60°
3. Move forward 1/3 of the old distance
4. Turn left 120°
5. Move forward 1/3 of the old distance
6. Move Turn right 60°
7. Move forward 1/3 of the old distance
![Iteration 1]({{site_url}}/images/koch1.png)

Step 2: Do the same thing as Step 1, dividing the distance for each
segment by three each time
![Iteration 2]({{site_url}}/images/koch2.png)

This can be repeated an infinite number of times (theoretically). Here's the
snowflake after 5 iterations.
![Iteration 5]({{site_url}}/images/koch5.png)

For the curious, [L-Systems](https://en.wikipedia.org/wiki/L-system) are useful
in making this type of fractal.

If you liked this challenge, try making these other similar fractals:
* [Lévy C Curve](https://en.wikipedia.org/wiki/L%C3%A9vy_C_curve)
* [Dragon Curve](https://en.wikipedia.org/wiki/Dragon_curve)

Or try designing your own!
