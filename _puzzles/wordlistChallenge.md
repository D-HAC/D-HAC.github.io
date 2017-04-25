---
layout: page
title: Wordlist
permalink: /puzzle/wordlist
hide: false
week: 4
term: "Spring 2016-17"
solutions: week4_wordlist
---

Generate a Wordlist
Word lists are lists of strings, often used in password cracking attempts. 
List items are usually composed of capital and lowercase letters, numbers, and symbols, and are designed to resemble real passwords.
Many people make passwords by switching out certain characters in a word, so our wordlist will account for this.

## The Challenge

Given a list of words and a list of single-character replacements, produce a list of every replacement permutation for those words.
For Example, Given a list containing the word "PASSWORD" and a replacement set of `{S:$, A:4, O:0}`, the program should produce:

PASSWORD  
PA$$WORD  
PA$SWORD  
PAS$WORD  
PASSWORD  
P4$$WORD  
P4$SWORD  
P4S$WORD  
P4SSWORD  
PASSW0RD  
PA$$W0RD  
PA$SW0RD  
PAS$W0RD  
PASSW0RD  
P4$$W0RD  
P4$SW0RD  
P4S$W0RD  
P4SSW0RD  

Input:

 `[password, amazon, letmein, qwerty, baseball, iamroot, facebook]`

 Substitutions:

 `{a:@, e:3, i:!, l:1, o:0, s:$, t:+}`

## Bonus Challenges 

1) Many passwords require capitalization, but people capitalize erratically. Extend your code to create all capitalization permutations of each word.

2) Some characters have more than one possible substitution. Modify your program to deal with this, and output all permutations for the substitution list below:

	`{a:4, a:@, b:6, b:8, e:3, i:!, i:1, l:1, o:0, t:+}`