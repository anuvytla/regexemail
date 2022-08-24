# Regex Tutorial on Matching an Email

A regular expression, or regex, is a sequence of characters that illustrate or define a search pattern. They are used to find, match, replace, or validate input in strings. This regex matches character information for valid e-mail addresses.

## Summary

The following is the regular expression for matching a email address

```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{1,3})$/
```

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Author](#Author)

## Regex Components


### Anchors

Our regex is enclosed by anchors on both ends, indicating that the match will span the entire string

- The `^` symbol marks the beginning of the string.
- The `$` symbol marks the end of the string.

In our example, you can see that the text we are matching will begin after the `^` and end at `$`.

### Quantifiers

Quantifiers specify the number of characters to match. They are located to the right of the expression or characters in question.

- The `+` indicates that the element may be repeated 1 or more times
- The `*` indicates that the element may be repeated 1 or more times, as well as 0 times
- The `?` indicates that the element is optional, matching 0 or 1 occurrences
- The `{n}` indicates a quantity, either a single number or a range of numbers

n this example, we used `+` to communicate there is another sequence to be matched as a greedy quantifier. We also used `{1,3}` as another greedy quantifer to specify the input should be a minimum of 1 characrtors to a maximum of 3 characters.

### Character Classes

The charactor class `/d` is used which in Javasctipt classifies the use of any digit from 0 to 9 which we used in this example.

### Grouping and Capturing



### Bracket Expressions



### Greedy and Lazy Match


## Author
