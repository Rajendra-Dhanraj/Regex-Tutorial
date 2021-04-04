# Email RegEx Parameters

Welcome to this page that will explain what RegEx is, and how its used with examples. 

RegEx or "Regular Expression," serves the purpose to help you dissect characters from a string. As it searches through the string, it will look for: numbers, letters, white space and special characters. In addition RegEx allows you to search for specific patterns of characters within a string.

RegEx is often used to validate inputs, for example: emails, passwords, phone numbers, postal codes.

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

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
- [Back-references](#back-references)

## Regex Components

### Anchors

RegEx expressions are contained in "Anchors," they are used at the beginning and ending of Regular Expression as shown below:

`/^`([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})`$/`

### Quantifiers

Quantifiers are used within the RegEx expression in order to specify: amount of characters, groups or character classes for a match to be fufilled. Quantifiers are represented by: +, *, ?, {}.

The highlighted portion of the expression below represents the quantifiers. The highlighted text indicates " match between 2 and 6 of the group. The "group" indentifies letters between "a" and "z."

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

()

### Bracket Expressions

Matches a single character contained within `[]`. Matching any single character within the brackets. When the first character in the square brackets is a `"^"` the opposite premise is created, meaning anything not in the list will be matched. 

Example:

`[abc]` : Matches a, b, c characters.
`[^abc]` : Matches characters that are NOT a, b, c.
 
### Greedy and Lazy Match 

### Back-references

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)

[GitHub Profile](https://github.com/Rajendra-Dhanraj)

