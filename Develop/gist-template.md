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
The following symbol, (|) represents the OR Operator which either matches what's to the left or right of the that symbol. Below is an example using the pipe symbol.

```
'^[A-Z0-9_!#$%&'*+/=?`{|}~^.-]+@[A-Z0-9.-]+$'
```
### Character Classes
Character classes are commonly used when it comes to regular expressions. With the character classes, you can tell the regex to soley match one out of several characters and even use a hyphen to specify a range of charaacters which can be seen in our previous example.
```
'...[A-Z0-9.-]+$'
```
### Flags
Regular expressions have optional flags which allow for global searching, case-insensitive searching and more. For example, '/\w+\s/g' creates a regex that searches for one or more characters which is then followed by a space and looks for a combination within the string.

### Grouping and Capturing
Grouping and capturing tend to be used in a regex with parenthesis to seperate a series of criteria or for creating blocks of patterns to apply repetitions or modifiers as a whole. 

### Bracket Expressions
Regular expressions can contain brackets so that they can indicate a set of characters to match. Now if a set is to be defined, a hyphen needs to be used. An example of this can be seen from our code used previously under 'Summary': 
```
'...[A-Z0-9.-]'
```
### Greedy and Lazy Match
Within regular expressions, we can also see "Greedy and Lazy match". 'Greedy' matches the longest possible string while 'Lazy' matches the shortest. By default, all quantifiers are greedy and to make them 'Lazy', the user needs to append a question mark, '?'. An example of this is shown below: 
```
'{0,5}?'
```
### Boundaries
Regex boundries are used with the '\b' symbol. Its an anchor just like the caret symbol '^' and the dollar sign '$'. It allows the user to search for 'whole words only' 

### Back-references
Back-references are used to matach same text that was previously matched by capturing a group. To do this, the user needs to put an openeing tag into a backreference so that the user can reuse the name of the tag for the closing tag. 
### Look-ahead and Look-behind
Now so that the user can discover ocurring patterns, 'look-ahead' and 'look-behind' can be used. When it comes to 'look-ahead', the user should use '?=' and for 'look-behind', '?<=' needs to be used. 

## Author

My name is Luis Gutierrez. I am a front-end developer who is currently enrolled in a UCR Coding bootcamp extension on the mission to develop my skills. Below is a link to my Github with some of the work I have done. 
https://github.com/luisgcodes