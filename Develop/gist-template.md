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
The characters ^ and $ are both considered to be anchors.  The Circumflex ^ anchors the beginning of the sequences, and the dollar $ is asserted at the end of a line to anchor the end.
### Quantifiers
The curly brackets { n } have a number. In this case, it's a Greedy quantifier that sets the parameter that the last portion of the domain after the period . needs to be between 2-6 characters {2, 6}, also lower-cased.
### Grouping Constructs
The 1st set of square brackets [] (normally meaning needs to be matched within here) wrapped within the parantheses () is the email prefix (username) to the left of the @ symbol. The 2nd set of square brackets [] wrapped within the parantheses () is the domain name, which is always to the right of the @ symbol, with the same parameters as the username. Afer the forward slash \ is a period that indicates a separation within the domain name. The 3rd set is the last portion of the domain. This one is structured uniqely, because the parantheses () indicates that this part only pertains to the domain "last name" portion, yet the sequence ends with this set, hence why the $/ needs to end within that part of the bracket. ] 
Because of the combination of paranthesis+square bracket ([]), everything in between must match the single characters in the index list of acceptable characters (also case sensitive). 
"\d" mean to match a digit, or another way to state "0-9". 
### Bracket Expressions
the brackets [ ] state that within this section, [a-f] (the hyphen "-" representing a range) means that it needs to be an American alphebetical letters between a through f, lower-case (unless there is an "i" at the end of the syntax to indicate "ignore casing"). [0-9] means that the numbers need to be between 0-9.
This is a range of characters that need to be matched in the future when inputting the local part of the email address.
{curly brackets} allow us to set limits for a match, includes either {number} (match the pattern exactly that "number" of times), {number,} (match the pattern at least that "number" of times), and {number, otherNumber} (match the pattern between the minimum of "number" of times to a maximum of "otherNumber" of times). After the {curly brackets}, [letters and numbers] occurs again, because of the email domain section. 
### Character Classes
The # symbol indicates a hashing of a large quantity of ongoing written dialogues.
The ? symbol demonstrates a query, because this address will need to be queried whenever one wants access to it. 
These symbols_\.- within the 1st set of square brackets [] indicate that these are acceptable sybols to have matched in the username or the domain name. 
The @ symbol divides the username from the domain. 
### The OR Operator
The most prominent OR operator is the "vertical bar pipe |," tell it to match either what is before or after the | . For example, a | b means match either a or b. In order to use it in a phrase, it needs to be in its own ( a | b ), but will then produce one of those results within the code.
### Flags
Flags modify how a regex pattern behaves when encountering matching text. These are appended at the end of the regular expression and can be combined with other flags in any order (which doesn't matter). The 3 most common ones that are utilized include: #1: "i" for "ignore case", means that the pattern is case-insensitive, so "ignore upper or lower case". #2: "g" for "global scope", so search for all matches, instead of only returning the first one (search/find on webpages for text are an example of this). #3: "m" for "multi-line", to take in specified elements from multiple lines. For example, In the following array
[ 1,
2,
3 ];
Adding a "mg" to the end of the regex will tell it to take in all 3 numbers (g) from multiple lines (m). 
### Character Escapes
It begins and ends with a backtick and forward slash because everything in between are considered "literals", so the `/ literal values /` have to be wrapped here.
A backward slash \ would indicate that it need to match the character literally (i.e. case sensitive).
"+" matches the previous token 1+ (unlimited), or as many times as possible, giving back as needed (greedy quantifier only). 
Other related "quantifier" characters include: * (matches 0+ times), ? (match 0 or 1 times), 
## Author
A short section about the author with a link to the author's GitHub profile:
Calvin Yue 
(Github username: calvinyueWillTry )
https://github.com/calvinyueWillTry 