# Regex Introduction

Hi, this is my summary of Regex and the way it works.

## Summary

In Summary, Regex is a great way of searching through large bodies of text with high accuracy for anything you need. Like If i wanted to search for a phone number but didn't want to have to search through entire website just to find it. I could do "\d\d\d-\d\d\d-\d\d\d\d" to search for any phone number and even if by chance it has Parenthese around the area code you simply add \( \) around the hypothetical area code. It is extremely useful and can even have applications in coding so it is a helpful skill to have and knowledge to gold.

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
Regex is considered a literal so they need to start and be wrapped with "//". Javascript does have another way of writing a regex object but that is a RegExp constructor that puts it in quotes.
### Anchors
 anchors signify a string that begins with the characters that follows it which can be in one of two formats an exact string match or a range of possible matches
### Quantifiers
 sets the limit of how long your string can be. So if youre looking for a username you set the quantifier {3,16} searching for any string that is 3 characters long to 16 characters long. This teamed up with bracket expressions can narrow down your search.
### Grouping Constructs
 Grouping constructs check multiple parts of a string to determine that different sections fulfill different requirements. The main way you group a section of a regex is by using parentheses (()). Each section within parentheses is known as a subexpression. Subexpressions are much more strict in that they will only accept what is exactly input unless told otherwise. so (abc):(xyz) would literally only pull a string that matches "abc:xyz" and nothing else.
### Bracket Expressions
bracket expression are within a bracket and whatever we put into those brackets is what we are searching for. so [a-z] would search for a string with any letter a-z and you can put them together with other inputs like [0-9] searching for any string with a number 0-9 in it. Doing this will display a string that displays any of the requirements so if it has a number or letter it will appear.
### Character Classes
 A character class in a regex defines a set of characters, any one of which can occur in an input string to fulfill a match.Bracket expressions are considered character classes and here are a few more.
 .-matches any character besides the new line character
 /d-stands for any digit, basically the same as [0-9]
 /w- is basically any letter in the alphabet upper or lower case including the underscore
 /s- matches a single white space character so tab or space, or a line break
### The OR Operator
 Gives another way of specifying besides using brackets. for example from the grouping constructs which would only return (abc):(xyz) or "abc:xyz" you could write it as (a|b|c):(x|y|z) and it would now include any mix of those three letters within their respective groupings.
### Flags
Placed at the end of a Regex expression and define any extra limitors there are six but youll only typically see these three.
g- means global, test against every possible string
i- means case sensitivity is turned off.
m- treats a multiple line string as multiple lines
### Character Escapes
the backslash '\' would escape a character. Meaning that it would search for the character without counting it as a regex object or expression. for example if you put a '{' it would think youre starting a quantifier but by putting the backslash in front '\{' it would now search for it instead. Any special character loses it's inherent value this way making them searchable.
## Author

Hi, I'm Nicolas Alonzo and I'm the author of this summary of Regex. Here's a link to my Github : https://github.com/DewYourWorst
See ya Around! 
