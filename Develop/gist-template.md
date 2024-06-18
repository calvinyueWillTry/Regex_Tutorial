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
Matching an email Value: `[/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/]`
### Anchors
It begins and ends with a backtick and forward slash because everything in between are considered "literals", so the `/ literal values /` have to be wrapped here.
The characters ^ and $ are both considered to be anchors.  The Circumflex ^ anchors the beginning of the sequences, and the dollar $ anchors the end.
### Quantifiers
The curly brackets { n } have a number. In this case, it's a Greedy quantifier that sets the parameter that the last portion of the domain after the period . needs to be between 2-6 characters {2, 6}, also lower-cased.
### Grouping Constructs
The 1st set of square brackets [] wrapped within the parantheses () is the email prefix (username) to the left of the @ symbol. The 2nd set of square brackets [] wrapped within the parantheses () is the domain name, which is always to the right of the @ symbol, with the same parameters as the username. Afer the forward slash \ is a period that indicates a separation within the domain name. The 3rd set is the last portion of the domain. This one is structured uniqely, because the parantheses () indicates that this part only pertains to the domain "last name" portion, yet the sequence ends with this set, hence why the $/ needs to end within that part of the bracket. ] 
### Bracket Expressions
the brackets [ ] state that within this section, [a-f] means that it needs to be an American alphebetical letters. [0-9] means that the numbers need to be between 0-9.
This is a range of characters that need to be matched in the future when inputting the local part of the email address.
After the {curly brackets}, [letters and numbers] occurs again, because of the email domain section. 
### Character Classes
The # symbol indicates a hashing of a large quantity of ongoing written dialogues.
The ? symbol demonstrates a query, because this address will need to be queried whenever one wants access to it. 
These symbols_\.- within the 1st set of square brackets [] indicate that these are acceptable sybols to have in the username or the domain name. 
The @ symbol divides the username from the domain. 
### The OR Operator

### Flags

### Character Escapes

## Author
A short section about the author with a link to the author's GitHub profile:
Calvin Yue 
(Github username: calvinyueWillTry )
https://github.com/calvinyueWillTry 