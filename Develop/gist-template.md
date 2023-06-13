# Title Regular Expressions Tutorial

This gist has been created to explain what a regular expression (Regex) is while walking you through how to use the Regex. One would typically use regular expressions to match a certain character combination a specific string, which is ideal ideally for validation or to pull information out of a body of code. This tutorial will demonstrate the various components of regular expressions through an example code snippet that can be used to match an email.

## Summary

The regex that will be described can be used for matching emails. This tutorial will explain how this code can be used to validate that an email is following the correct format. The code that will be used throughout the tutorial is provided below:

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors

The anchors match the start and end points of a string or line.
In the matching email code snippet we are using for the tutorial, 

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

the anchors are `^` (starting the regex) and `$` (ending the regex).


### Quantifiers

The quantifiers allow you to specify how many of a character or character class should be matched.
Using our code, 

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/` 

the quantifiers are present in `([a-z0-9_\.-]+)`. It specifies that it will match any string containing a-z, 0-9, _, ., or -. The quantifier `+` present at the end of the snippet interprets that the email had to contain at least one of the quantifiers listed in order to have a match.


### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

This gist tutorial was created by Leslie Sanchez.
As a junior developer fresh out of Web Development bootcamp, I am always open to new opportunities and any form of feedback.
Please feel welcomed to contact me or visit any of my profiles provided below!

[GitHub](https://github.com/lexslie)

[Email](lesliiee727@gmail.com)

[LinkedIn](https://www.linkedin.com/in/leslie-sanchez-903241167/)
