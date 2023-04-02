# Matching a URL regex
A URL (Uniform Resource Locator) is a reference to a web resource that specifies its location on a computer network and the protocol used to access it. Matching a URL using regex is a common task in web development. In this article, we will discuss the basic components of a URL and provide a regular expression pattern to match a URL.

## Summary
In this article, we will explain how to match a URL using a regular expression in different scenarios. The regular expression pattern we will be using is:

- /^https?:\/\/(?:[a-z0-9-]+\.)+[a-z]{2,}$/i
This pattern matches URLs starting with either http:// or https://, followed by one or more subdomains, and ending with a top-level domain name such as .com, .org, or .net.

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
The ^ and $ anchors are used to match the start and end of the string, respectively. In our pattern, ^ matches the start of the URL string, while $ matches the end of the string.

### Quantifiers
The + quantifier matches one or more of the preceding character or group. In our pattern, (?:[a-z0-9-]+\.)+ matches one or more subdomains.

The {} quantifier matches a specified number of occurrences of the preceding character or group. In our pattern, {2,} matches two or more characters in the top-level domain name.

### Grouping Constructs
The (?:) non-capturing group is used to group multiple characters or groups together without capturing the match. In our pattern, (?:[a-z0-9-]+\.)+ groups one or more subdomains together.

### Bracket Expressions
The [] bracket expression is used to match a single character from a set of characters. In our pattern, [a-z0-9-] matches any lowercase letter, digit, or hyphen.

### Character Classes
The \w character class matches any word character (letter, digit, or underscore). In our pattern, it is not used explicitly, but it is implied in the bracket expression [a-z0-9-].

### The OR Operator
The | operator matches either the expression on the left or the expression on the right. In our pattern, it is not used explicitly.

### Flags
The i flag is used to make the pattern case-insensitive. In our pattern, it is used to match URLs regardless of whether the protocol and domain names are in uppercase or lowercase letters.

### Character Escapes
The \/ escape sequence is used to match a forward slash character. In our pattern, it is used to match the forward slashes in the http:// and https:// protocols.

### Author
Alyshia Kandler is a full stack developer with a passion for web developement and programming.
https://github.com/alyshiak
