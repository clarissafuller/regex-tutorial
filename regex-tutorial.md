# Regex, the least regular thing about coding

Regular expressions, often abbreviated as "regex" or "regexp," are a powerful and flexible tool for pattern matching and text manipulation in computer science and programming. They provide a concise and highly expressive way to define search patterns within strings of text. Regular expressions are widely used in a variety of applications, including text processing, data validation, searching and replacing text, and more.

## Summary

While regular expressions can be a powerful tool, they can also be complex and challenging to master. It's essential to strike a balance between their capabilities and their potential for complexity. Learning regular expressions can be highly rewarding for those who work with text processing, as it enables efficient and precise manipulation of textual data in a wide range of applications.

Regular expressions can be made of multiple components that will be explained below.

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

Anchors are special characters that specify the position within the input string where a match must occur. Two common anchors are the caret (^), which matches the beginning of a line or string, and the dollar sign ($), which matches the end of a line or string.

ex: `match_start = re.search(r'^Hello', text)`

### Quantifiers

Quantifiers determine how many times a preceding character or group of characters must be repeated to constitute a valid match. Common quantifiers include the asterisk (\*), which matches zero or more occurrences, and the plus sign (+), which matches one or more occurrences.

ex: `text = "ab abbb abbbbb" 
pattern=r"ab*"`

### Grouping Constructs

Grouping constructs are used to group characters or subpatterns together, allowing you to apply quantifiers or other operations to the entire group. Parentheses () are commonly used for grouping in regular expressions.

ex: `text = "Debby Ryan (disneyqueen2000@disney.com) and Salena Gomez (salena@wizards.com) cant sing 
pattern = /\((.*?)\)/g"`

### Bracket Expressions

Bracket expressions, also known as character classes, allow you to specify a set of characters that should match at a particular position. For example, [a-zA-z] matches any uppercase or lowercase letter.

ex: `text = "If we were a movie you'd be the right guy and I'd be the best friend that you fall in love with" 
const pattern = /\b[AEIOUaeiou]+\b/g`

### Character Classes

Character classes are predefined sets of characters that match specific categories, such as digits (\d) for numbers, word characters (\w) for alphanumeric characters, or whitespace (\s) for spaces and tabs.

ex: `text = "Birds are not real" const pattern = /\s/g`

### The OR Operator

The OR operator (|) allows you to specify alternative patterns. It matches any one of the patterns on either side of the operator. For example, "cat|dog" matches either "cat" or "dog."

ex:`text = "The color of my clothes is always either green or black" const pattern = /green|black/g

### Flags

Flags are optional modifiers that can be added to the end of a regular expression to change its behavior. Common flags include "i" for case-insensitive matching and "g" for global matching (to find all matches in the input string).

### Character Escapes

Character escapes are used to match specific characters that would otherwise be treated as special characters in regular expressions. For example, "." is used to match a literal period (.), and "\d" is used to match the digit "d" instead of the special character for a digit.

## Author

Clarissa Fuller
email: clarissafuller5@yahoo.com



