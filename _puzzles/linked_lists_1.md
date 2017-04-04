---
layout: page
title: Linked Lists 1
permalink: /puzzle/linked-lists-1
hide: false
week: 1
term: "Sprint 2016-17"
solutions: "week1_linked-lists-1"
---

Fun with Linked Lists

This week's puzzle is based on a couple of problems on Hacker Rank:
[Hacker Rank: Linked Lists](https://www.hackerrank.com/domains/data-structures/linked-lists)

Today we have a couple of problems involving singly linked lists, which are basic
data-structures that consist of nodes, each with some value and a link to
another node (or null)

A Python linked list node could be:

    class Node(object):

      def __init__(self, value=None, next=None):
        self.value = value
        self.next = next

# Problem 1
Given the head node of a linked list, print the values of its elements in order,
one element per line. If the head node is null (indicating the list is empty),
print '(empty)'.

## Sample Input

    NULL  

    1->2->3->NULL

    5->4->3->2->NULL

Each row is a separate linked list and consists a set of node values, separated
by '->', which indicates a link to another node.

## Sample Output

    (empty)  

    1
    2
    3

    5
    4
    3
    2

Each list's values are printed on separate lines in-order. If the head node is
null (indicating the list is empty), print '(empty)'.

# Problem 2

Given the head node of a linked list, reverse the order of elements, and then
print the values of its elements in the new order, one element per line. As
before if the head node is null (indicating the list is empty), print '(empty)'.

## Sample Input

    NULL  

    1->2->3->NULL

    5->4->3->2->NULL

## Sample Output

    (empty)  

    3
    2
    1

    2
    3
    4
    5
