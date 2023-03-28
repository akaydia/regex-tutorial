# Email Regex Tutorial

Regular expressions are a powerful tool for finding patterns in strings. In this tutorial, we'll focus on the regular expression that matches an email address, which is a common use case for regular expressions.
## Summary
This tutorial provides an in-depth explanation of the regular expression used to match email addresses: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/. We'll break down each component of the regular expression, explaining what it does and how it works. Additionally, we'll cover some related topics, such as anchors, quantifiers, grouping constructs, bracket expressions, character classes, the OR operator, flags, and character escapes.
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
- `^` matches the beginning of the string.
- `(?:[a-z0-9_\.-]+)` this is the first capture group that matches one or more of any lowercase letter, digit, underscore, dot or hypen characters.
- `@` matches the literal @ symbol.
- `([\da-z\.-]+)` this is the second capture group that matches one or more of any digit, lowercase letter, dot or hypen characters.
- `\.` matches the literal dot symbol.
- `([a-z\.]{2,6})` this is the third capture group that matches two to six of any lowercase letter or dot characters.
- `$` matches the end of the string to make sure it ends in the correct format.

### Anchors
Anchors help match certain parts of a string using regular expressions. The caret `^` matches the beginning of a string, while the dollar sign `$` matches the end of a string. For example, if we use the regex `^a`, it matches any string that starts with `a`. Similarly, the regex `a$` matches any string that ends with `a`. And, if we use the regex `^a$`, it matches any string that only contains the letter `a`.

### Quantifiers
The quantifiers in this email regex are:

- `+` means "one or more of the preceding item". For the first and second capture groups, it matches one or more of any lowercase letter, digit, underscore, dot or hyphen characters. For the third capture group, it matches two to six of any lowercase letter or dot characters.
- `{2,6}` means "between two and six of the preceding item". For the third capture group, it matches two to six of any lowercase letter or dot characters.

### Grouping Constructs
The parentheses `()` define capture groups. This email regular expression has 3 capture groups in total:

- The first capture group matches the username, which consists of one or more of any lowercase letter, digit, underscore, dot, or hyphen characters.
- The second capture group matches the domain name, which can consist of one or more digits, lowercase letters, dots or hyphen characters.
- The third capture group matches the domain extension, which can consist of two to six of any lowercase letter or dot characters.

### Bracket Expressions
The square brackets `[]` define a bracket expression. This email regular expression has 3 bracket expressions in total:

- `[a-z0-9_\.-]` matches one or more of any lowercase letter, digit, underscore, dot, or hyphen characters.
- `[\d]` matches any digit equivalent to `[0-9]`.
- `[a-z\.]` matches any lowercase letter or dot equivalent to `[a-z\.]`.

### Character Classes
Character classes match any character that is within a certain set of characters. The following character classes apply to this regular expression:

- `[a-z0-9_\.-]` matches any lowercase letter, digit, underscore, dot or hyphen.
- `[\d]` matches any digit equivalent to `[0-9]`.
- `[a-z\.]` matches any lowercase letter or dot equivalent to `[a-z\.]`.

### The OR Operator
The OR operator `|` can be used to match multiple patterns. For example, the regex `cat|dog` matches the string `cat` or `dog`.

### Flags
Flags can be used to modify the regex. For example, the `i` flag is used to match the string `cat` or `dog` regardless of case. The regex `cat|dog` with `i` flag will match `cat`, `CAT`, `dog` and `DOG`.

### Character Escapes

Escape sequences match literal characters rather than using their special meaning as a wildcard or operator. The following escape sequences apply to this regular expression:

- `\.` matches a literal dot character (".") rather than using its special meaning as a wildcard character that matches any single character except newline.
- `\-` matches a literal hyphen character ("-") rather than using its special meaning inside a character class as a range operator.
- `\_` matches a literal underscore character ("_") rather than using its special meaning as a word boundary marker in some regex flavors.

## Author
Hi there, I'm Ricky and I'm an aspiring software engineer. I enjoy learning about new technologies and implementing them in fullstack projects. From styling a website to building a backend API, I enjoy all these different aspects in software development. I hope to learn more algorithms and data structures in the future.
This tutorial was written by [Ricky](https://github.com/akaydia).
