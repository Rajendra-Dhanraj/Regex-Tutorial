# RegEx Tutorial: Email

Welcome to this page that will explain what RegEx is and how its used with examples. 

RegEx or "Regular Expression," serves the purpose to help you search and dissect characters from a string. As it searches through the string, it will look for: numbers, letters, white space and special characters. In addition RegEx allows you to search for specific patterns of characters within a string.

RegEx is often used to validate inputs, for example: emails, passwords, phone numbers, postal codes.

## Summary

We will be examining a Regular Expression used to validate an email address as follows:

`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

Traditional email addresses contain a username, @ symbol, domain. 

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors

RegEx expressions are contained in "Anchors," they are used at the beginning and ending of Regular Expression as shown below:

/`^`([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})`$`/

### Quantifiers

Quantifiers are used within the RegEx expression in order to specify: amount of characters, groups or character classes for a match to be fufilled. Quantifiers are represented by: +, *, ?, {}.

The highlighted portion of the expression below represents the quantifiers. The highlighted text indicates: match between 2 and 6 of the group. The "group" indentifies the punctuation character "." letters between "a" & "z."

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]`{2,6}`)$/

### Character Classes

Character classes define the possible characters that can be searched. As highlighted below, there are many different classes which we will explore:

* `[a-z]` : Matches any character between a and z.
* `[0-9]` : Matches any number from 0-9.
* `_` : Matches "_" character.
* `\.` : Matches "." character.
* `-` : Matches "-" character.
* `\d` : Matches any digit character.

/^(`[a-z0-9_\.-]`+)@(`[\da-z\.-]`+)\.(`[a-z\.]`{2,6})$/

### Grouping and Capturing

Capturing allows the collection within the `()` to treat more than one character as a single group. In our example below, each highlighted section is its own "Capturing Group," the expression contains (3) groups, which are numbered in order from left to right.

/^`([a-z0-9_\.-]+)`@`([\da-z\.-]+)`\.`([a-z\.]{2,6})`$/

### Bracket Expressions

Matches a single character contained within `[]`. Matching any single character within the brackets. When the first character in the square brackets is a `"^"` the opposite premise is created, meaning anything not in the list will be matched. 

Example:

* `[abc]` : Matches a, b, c characters.
* `[^abc]` : Matches characters that are NOT a, b, c.
 
### Greedy and Lazy Match 

* **Greedy Search** will try to match the longest possible string, only giving back as neccessary to match the remainder of the regex.
* **Lazy Search** will try to match as few of the input characters possible and then proceed to the next token in the regular expression pattern.

## Author

Created with ❤️ by Rajendra Dhanraj, aspiring Full Stack Web Developer studying at the University of Toronto.

[Click to view my GitHub Profile!](https://github.com/Rajendra-Dhanraj)

