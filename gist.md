# Hex-RegexTutorial

My goal is to go over and explain a regular expression. The regular expression we will be dealing with today is a hex. Hex codes are a positional numeral system that uses 16 distinc symbols. One of the many uses for hex regular expressions is hex colors. Developers use these hex codes for manipulating colors on a webpage.

Some examples of hex codes are: #000000, #fddd36, #b12651, #1dcd65

## Summary

The regex that we are going to be solving is: `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs and OR Operator](#grouping-constructs)
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

This regex has one big group: `([a-f0-9]{6}|[a-f0-9]{3})`. This grouping also uses an OR operator `|`. This divides the expression into two parts `[a-f0-9]{6}` and `[a-f0-9]{3}`. So the regex will match any of the two expressions.

OR operators are also used to validate email domains like .com, .net, etc...

### Character Classes

This regex uses one character class but it is repeated twice: `[a-f0-9]`. This character class will match any other character enclosed in the brakets. For example: [iop] with match "i", "o" and "p". The regex has two ranges: `a-f` and `0-9`. So any character "a-f" and "0-9" will match.

## Author

- Ian Irwin
- Github: https://github.com/Ianirwin18
