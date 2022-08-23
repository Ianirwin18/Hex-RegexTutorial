# Hex-RegexTutorial

My goal is to go over and explain a regular expression. The regular expression we will be dealing with today is a hex. Hex codes are a positional numeral system that uses 16 distinc symbols. One of the many uses for hex regular expressions is hex colors. Developers use these hex codes for manipulating colors on a webpage.

Some examples of hex codes are: #000000, #fddd36, #b12651, #1dcd65

## Summary

The regex that we are going to be solving is: `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors

This hex regex is using two anchors: `^` and `$`.

The `^` represents the beginning of string or a line, and the `$` represents the end of a string or a line. For example, `^abc` will match any string or line that begins with abc, while `def$` will match any string or line that ends with def.

The regex we're solving uses these characters to make sure that we are maching the full expresion from beginning to end.

### Quantifiers

This regex uses two types of quantifiers: `?` and `{n}`.

The `?` quantifier matches any preceding character 0 or 1 times. Since `?` is followed by `#`, the expression will match a string that starts with `#`.

The next quantifier used is `{n}`, which is used twice `({6} and {3})`. This meta character matches the preceding character n-times. For example: `{\d{5}}` this regular expresion will match any string that has 5 consecutive digits like 02001 or 11111.

### Grouping Constructs and OR Operator

This regex has one big group: `([a-f0-9]{6}|[a-f0-9]{3})`. This grouping also uses an OR operator.

### Bracket Expressions

### Character Classes

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)