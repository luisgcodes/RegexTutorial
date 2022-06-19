# Regex Tutorial
A Regex which is short for regular expression, is a string of text that allows you to create patterns to match character combinations. Regex can help in many ways such as being able to verify an email address, a phone number and matching passwords as well.

## Summary

There are quite a bit of areas where Regex can be used but today we'll be going over being able to verify an email address. To begin we need to understand that a regular expression that matches all the possible valid email addresses does not exist. The best approach when validating is to limit the user's input from the beginning. Below is a snipit of what an email regex can look like.

```
'^([a-z0-9]+@[a-z]+\.[a-z]{2,3})$'
```

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors
Anchors are special characters have a particular job when it comes to regular expressions. They match a position before or after the characters. For example, The carrot anchor (^) matches the beginning of the text where the dollar sign ($) matches the end of the text.

### Quantifiers
When it comes to regular expression quantifiers, they match a number of instances of a character, group, or character class in a string. An example of a simple quantifier is a number in curly braces {n}. When the user appends it to a character, it specifies how many characters the user would want to match. Here is an example of that:
 /\d{4}/ matches a four-digit number.
### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
