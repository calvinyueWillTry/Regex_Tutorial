# Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)
- [Author](#author)

## Regex Components
Matching a Hex Value (email): `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`
### Anchors
It begins and ends with a backtick and forward slash because everything in between are considered "literals", so the `/ literal values /` have to be wrapped here.
The characters ^ and $ are both considered to be anchors.  The Circumflex ^ anchors the beginning of the sequences, and the dollar $ anchors the end.
### Quantifiers
The curly brackets { n } have a number. In this case, it's a Greedy quantifier that sets the parameter that the username has to be at least 6 characters, but apparently lower-case letter menaing that all of those letters need to be lower-cased {6}. For the domain, it needs to have at least 3 characters {3}, also lower-cased.
### Grouping Constructs

### Bracket Expressions
the brackets [ ] state that within this section, [a-f] means that it needs to be an American alphebetical letters. [0-9] means that the numbers need to be between 0-9.
This is a range of characters that need to be matched in the future when inputting the local part of the email address.
After the {curly brackets}, [letters and numbers] occurs again, because of the email domain section. 
### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile:
Calvin Yue 
(Github username: calvinyueWillTry )
https://github.com/calvinyueWillTry 