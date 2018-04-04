---
layout: page
title: "Linked Lists"
permalink: /puzzle/linked_lists_2
hide: false
week: 3
term: "Winter 2017-18"
---

Today we have a couple of problems involving singly linked lists, which are basic
data-structures that consist of nodes, each with some value and a link to
another node (or null).

A visualization of this can be seen here: [Visualization of Linked Lists](https://cdn-images-1.medium.com/max/800/1*1B4X5Jbe5LNXeZNWx2msyw.gif)

A Python linked list node could be:

```
    class Node(object):

      def __init__(self, value=None, next=None):
        self.value = value
        self.next = next

```

However, this structure can be written in any language you'd like to use. All you
should make sure to have is some way to create a node with a link to the next
node (or null if it's the end of the list).

# Problem 1
Given the head node of a linked list, print the values of its elements in order,
one element per line. If the head node is null (indicating the list is empty),
print '(empty)'.

## Sample Input

```
    NULL  

    1->2->3->NULL

    5->4->3->2->NULL
```

Each row is a separate linked list and consists a set of node values, separated
by '->', which indicates a link to another node.

## Sample Output

```
    (empty)  

    1
    2
    3

    5
    4
    3
    2
```

Each list's values are printed on separate lines in-order. If the head node is
null (indicating the list is empty), print '(empty)'.

# Problem 2

Given the head node of a linked list, reverse the order of elements, and then
print the values of its elements in the new order, one element per line. As
before if the head node is null (indicating the list is empty), print '(empty)'.

## Sample Input

```
    NULL  

    1->2->3->NULL

    5->4->3->2->NULL
```

## Sample Output

```
    (empty)  

    3
    2
    1

    2
    3
    4
    5
```

# Problem 3

Given two sorted linked lists, merge the two linked lists, preserving order.
Print out the new linked list in order, one element per line. If both lists are
null, then print '(empty)'. Take note of whether or not you are distorting the
original lists or are creating a new list with copied data.

## Sample Input

```
    1 -> 3 -> 5 -> 6 -> NULL
    2 -> 4 -> 7 -> NULL

    15 -> NULL
    12 -> NULL

    NULL
    1 -> 2 -> NULL
```

## Sample Output

```
    1 -> 2 -> 3 -> 4 -> 5 -> 6 -> 7 -> NULL
    12 -> 15 -> NULL
    1 -> 2 -> NULL
```

# Problem 4

Given a sorted linked list, remove duplicate elements. Bonus points if you extend
your code to do the same with an unsorted linked list. Print the list after
removing duplicates.

## Sample Input

```
    1 -> 1 -> 3 -> 3 -> 5 -> 6 -> NULL
    NULL
```

## Sample Output
```
    1 -> 3 -> 5 -> 6 -> NULL
    NULL
```

# Problem 5 - Challenge Problem

Given a linked list, detect and output whether or not there is a cycle in the
list. This will require that you create multiple linked lists, some where they
are linear and some where they point back to a previous node, creating a cycle.
Output whether there is a cycle or not (1 if cycle is present, 0 if not).

[Reference Image](https://s3.amazonaws.com/hr-challenge-images/1163/1463778594-900a0ae522-inputs.png)
