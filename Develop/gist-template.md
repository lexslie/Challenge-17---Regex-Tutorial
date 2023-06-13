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

the quantifiers are present in `([a-z0-9_\.-]+)`. It specifies that it will match any string containing a-z, 0-9, _, ., or -. The quantifier `+` present at the end of the snippet interprets that the email has to contain at least one of the quantifiers listed in order to have a match.


### Grouping Constructs

Grouping constructs delineate the subexpressions of a regex and capture the substrings of an input string. Grouping constructs can be used to:
* Match a subexpression that is repeated in the input string.
* Apply a quantifier to a subexpression that has multiple regex language elements.
* Include a subexpression in the string that is returned by the `Regex.Replace` and `Match.Result` methods.
* Retrieve individual subexpressions from the `Match.Groups` property and process them separately from the matched text as a whole.
Referring back to our example for matching an email, we can divide our regex into three segments. `([a-z0-9_\.-]+)` as the first group, `([\da-z\.-]+)` as our second group, and `([a-z\.]{2,6})` as our third group. The first segment/group must be true before moving on to "match" the next part of the code.


### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

Flags are a set of instructions that modify the behavior of a regex, such as making the regex case sensitive or allowing it to match multiple lines. A regex flag is not present in the example code we are using in this tutorial. Flags are typically present after the slash in cases where the regular expression is in the common form of `/regex/`.

Flags: 
* g : "global", allows for matching all the instances within a string that follow the matching guidelines set in the regex
* m : "multiline", searches line by line instead of searching through a string as a whole
* i : "insensitive", makes the regex case-insensitive, which means that capital and lower-case letters will not deture the matching


### Character Escapes

## Author

This gist tutorial was created by Leslie Sanchez.
As a junior developer fresh out of Web Development bootcamp, I am always open to new opportunities and any form of feedback.
Please feel welcomed to contact me or visit any of my profiles provided below!

[GitHub](https://github.com/lexslie)

[Email](lesliiee727@gmail.com)

[LinkedIn](https://www.linkedin.com/in/leslie-sanchez-903241167/)
