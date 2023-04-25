# Module 17 Regex

Introductory paragraph (replace this with your text)

## Summary

I will be explaining how you match a URl utilizing this regex, `/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`. 
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
In the regex example I have chosen there are anchors, an optional capturing group that gets the url, capturing group that matches the top-level domain, and a capturing group that matches the path of the URL, allowing for zero or more occurrences of forward slashes. 
### Anchors
The `^` symbol starts the string anchor, which specifies that the regex pattern should match the start of the string. This ensures that the pattern matches the entire URL from the beginning to the end.The `$` symbol is the end of string anchor, which specifies that the regex pattern should match the end of the string.
### Quantifiers
the quantifiers in the regex `/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/` are `?`, `*`, and `{2,6}`. The `?` quantifier makes the preceding element optional, the * quantifier matches the preceding element zero or more times, and the {2,6} quantifier matches the preceding element between 2 and 6 times. No + or {n} quantifiers are used in this regex.
### OR Operator
The OR operator `|` is not used in this regex, but there is a forward slash `/` operator used to delimit the regular expression pattern. The forward slash `/` is used to indicate the start and end of the regex pattern, similar to how quotation marks are used to delimit strings in programming languages.
### Character Classes
The character classes in the regex are `[\da-z\.-]` and `[a-z\.]`. The first character class matches any digit, lowercase letter, dot, or hyphen character, while the 2nd character class matches any lowercase letter or dot character. The backslash `\` is used to escape special characters like `.` and `/`. T
### Flags
There are no flags in this regex expression
### Grouping and Capturing
There are four capturing groups used in this regex: one for the optional protocol, one for the domain name, one for the top-level domain, and one for the path. The use of capturing groups allows for the extraction of specific parts of the matched string. Additionally, the regex also uses non-capturing groups, such as the forward slashes and optional trailing slash, which do not store matched text as a separate result.
### Bracket Expressions
There are two bracket expressions used in this regex: one that matches any digit, lowercase letter, dot, or hyphen character, and another that matches any lowercase letter or dot character. These character classes are used to match different parts of the URL. Backslashes are used to escape some special characters in the character classes. Bracket expressions can be used to make a regex more specific by limiting what it matches.
### Greedy and Lazy Match
The `*` quantifier used in the regex is greedy, meaning it matches as many occurrences of the preceding character class as possible, resulting in the longest possible match. However, the `*` quantifier is also lazy by default, meaning it matches as few occurrences of the preceding character class as possible. This is because it is applied to a capturing group that can match any number of forward slashes, alphanumeric characters, spaces, dots, or hyphens. The use of greedy and lazy quantifiers allows for more flexible matching of patterns in the regex.
### Boundaries
There are two boundary anchors used in this regex: the start of string anchor `^` and the end of string anchor `$`. These anchors specify that the regex pattern should match only at the beginning and end of the string, respectively. Boundaries can be useful when you want to match a pattern only if it appears at the beginning or end of a line or word, or if it is surrounded by certain characters.
### Back-references
There are none
### Look-ahead and Look-behind
There are none in this expression. 
## Author
Cole Roberts
