# Basic Regular Expressions

Regular expressions, or regex, are a powerful tool for pattern matching and searching within text data. Basic Regular Expressions (BRE) are the simplest type of regex and are supported by most Unix utilities like sed and grep. In this article, we will explore the various components of BRE and how they can be used to match patterns within text data.

## Summary

In this article, we will be describing Basic Regular Expressions and explaining its various components. We will cover anchors, quantifiers, grouping constructs, bracket expressions, character classes, the OR operator, flags, and character escapes. Below is a code snippet of the basic regex syntax:

- Matches a string that starts with "hello" and ends with "world"
^hello.*world$


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
Anchors are used to specify the position of the match within the text. The two most commonly used anchors in BRE are ^ and $. The ^ anchor matches the start of a line, while the $ anchor matches the end of a line.

- Matches a string that starts with "hello"
^hello

- Matches a string that ends with "world"
world$

### Quantifiers
Quantifiers are used to specify the number of occurrences of a character or group. The most commonly used quantifiers in BRE are *, +, and ?. The * quantifier matches zero or more occurrences, the + quantifier matches one or more occurrences, and the ? quantifier matches zero or one occurrence.

- Matches a string that contains zero or more "o" characters
o*

- Matches a string that contains one or more "o" characters
o+

- Matches a string that contains zero or one "o" character
o?

### Grouping Constructs
Grouping constructs are used to group together multiple characters or expressions. They are specified using parentheses (). Grouping constructs can also be used to capture the matched text for later use.

- Matches a string that contains "hello" followed by "world"
(hello).*world$

- Captures the "hello" string and the entire matched string
(hello).*world$

### Bracket Expressions
Bracket expressions are used to specify a set of characters to match. They are specified using square brackets []. The characters within the brackets are matched individually.

- Matches a string that contains either "a" or "b"
[a|b]

- Matches a string that contains any character except "a" and "b"
[^ab]

### Character Classes
Character classes are used to match a set of characters with a single character. They are specified using backslash \ followed by a special character.

- Matches any digit character
\d

- Matches any non-digit character
\D

### The OR Operator
The OR operator is used to specify a choice between two or more expressions. It is specified using the vertical bar |.

- Matches a string that contains either "hello" or "world"
hello|world

### Flags
Flags are used to specify additional options for the regex. They are specified using a combination of letters after the closing delimiter of the regular expression. The most commonly used flags in BRE are g and i.

g: Global match flag. Matches all occurrences of the pattern in the string.
i: Case-insensitive match flag. Matches the pattern regardless of case.

- Matches all occurrences of "hello" in the string
/hello/g

- Matches the pattern regardless of case
/HELLO/i

### Character Escapes
Character escapes are used to match special characters within a regular expression. They are specified using a backslash \ followed by a special character. The most commonly used character escapes in BRE are:

\n: Matches a newline character.
\t: Matches a tab character.
\s: Matches any whitespace character.
\S: Matches any non-whitespace character.
\d: Matches any digit character.
\D: Matches any non-digit character.
\w: Matches any word character (letter, digit, or underscore).
\W: Matches any non-word character.

- Matches a string that contains a newline character
\n

- Matches any whitespace character
\s

- Matches any non-word character
\W

## Author

https://github.com/alyshiak -Alyshia Kandler is a full stack developer with a passion for web developement and programming.
