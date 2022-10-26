# EMAIL REGEX

I will be doing a tutorial on Email Regex /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Summary

An email regex can be a tough cookie if you dont know what you're looking for. In this gist I will be breaking down each section of an email regex.

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
The anchors used in this regex expression for matching an email are ^ , which indicates the beginning of the string and $to indicate the ending of the string.

### Quantifiers
Quantifiers in this regex includes the + operator, which will connect the users email name + email service + .com. Another quantifier for this regex includes {2,6}, which will allow a match range of 2-6 characters for the character set of [a-z\.].

### Grouping Constructs
A part of a pattern can be enclosed in parentheses (...). This is called a “capturing group”. It allows to get a part of the match as a separate item in the result array.
If we put a quantifier after the parentheses, it applies to the parentheses as a whole.

### Bracket Expressions
Bracked expressios for email validation includes the character sets of [a-z0-9_\.-], which is matching any letter a-z and is case senstive. It also matches a character 0-9 and matches the characters "_" , "-" , and "."; [\da-z\.-], which is matching a single digit from 0-9, any character a-z (case senstive), and the characters "." and "-".; [a-z\.] matches any character a-z(case senstive) and the character ".".

### Character Classes
The character class in this expression is \d, which matches a single characters that is a digit from 0-9. It will only match a single digit such as "4", but not "44".

### The OR Operator
The OR Operator uses this syntax "|" to group and differentiate constructs.

An example would be:
(a|b|c):(x|y|z)

### Flags
Flags are placed at the end of a regex, after the second slash, and they define additional functionality or limits for the regex.

/.../

This is used for every aspect of string.

### Character Escapes
The backslash in a regular expression precedes a literal character. If you put a backslash after a curly bracket for instance, it'll look for the curly bracket.
## Author
This Regex was created by 
Cory Carroll https://github.com/CoryCarroll 