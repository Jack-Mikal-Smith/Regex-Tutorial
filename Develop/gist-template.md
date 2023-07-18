# Regex Tutorial

In this Regular Expression tutorial, I will breakdown the components of a matching Email Regex Expression.

## Summary

A Matching Email Regex Expression searches for any instances of data that contain a string of characters that fit the requirements of any email.

Example: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

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
- [Refrences](#references) 

## Regex Components

### Anchors

The "^" anchor specifies that accepted emails begin with the range directly proceeding the anchor.  The "$" anchor specifies that accepted emails end with the range directly before the anchor

### Quantifiers

The Quantifiers in the first two ranges are both "+"; this quantifier matches the given range pattern one or more times.  The quantifier at the end of the expression, "{2,6}", specifies that ending range must be between 2 and 6 characters long.

### OR Operator

There are not any OR Operators in this Regex Expression.

### Character Classes

The first character class, "[a-z0-9_\.-]", specifies that the first string can only include those characters.  The second character class, "[\da-z\.-]" specifies that the range can include any number, letters a-z, back slashes, periods, and hyphens.  The third character class, "[a-z\.]", specifies that the range can only include letters, back slashes, and periods.

### Flags

There are not any Flags in this Regex Expression.

### Grouping and Capturing

This Regex Expression is grouped into three sections.  The first searches for characters before an "@" symbol.  The second and third sections look for characters after the "@" symbol and are seperated by a "." symbol.

### Bracket Expressions

While written two different ways, the first two bracket expressions actually search for the same range of character values.  The third bracket's character range includes all that of the first two, minus numerical characters.

### Greedy and Lazy Match

While not directly specified, the "\d" quantifier is, by default, a Greedy Match.  This means that it will naturally match as many digits as possible.

### Boundaries

There are not any Boundaries in this Regex Expression.

### Back-references

There are not any Back References in this Regex Expression.

### Look-ahead and Look-behind

There are not any Look-ahead or Look-behind tags in this Regex Expression.

## Author

Jack Smith
GitHub: https://github.com/Jack-Mikal-Smith

## References

https://www.regular-expressions.info/backref.html
https://www.rexegg.com/regex-quantifiers.html
https://coding-boot-camp.github.io/full-stack/computer-science/regex-tutorial
