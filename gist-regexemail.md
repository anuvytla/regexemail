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

A regex captures characters by using parenthesis () to group them.
There are three groups captured in this example. Group #1 is the username of the e-mail account `[a-z0-9_\.-]`. The second group captures the domain name or e-mail service being used `[\da-z\.-]`.Lastly, the third group captures the domain extention (i.e .com or .net) `[a-z\.]{1,3}`

### Bracket Expressions

Brackets are used in this regex to define the character sets. The information in the bracket expressions is opened and closed between brackets like this `[]`. This indentifies which information is allowed to be matched.

In this example they are 3 bracket expressions being used

- `[a-z0-9_\.-]` - includes case sensitive characters from a-z, numbers from 0-9 an underscore, periods and hyphens.
- `[\da-z\.-]` - includes all digits, case sensitive characters from a-z, periods and hyphens.
- `[a-z\.]` - includes case sensitive characters from a-z and periods.


### Greedy and Lazy Match

In this example we  used greedy quantifiers `+` and `{}`, meaning that it will allow the match to expand as long as it neess to go. If these quantifiers were lazy quantifiers, they would appear as `+?` or `{}?`, this will direct the system to make the shortest match.

## Author

This is Anusha, full stack developer with an expertise in `MERN` stack.

[Github Profile Link](#https://github.com/anuvytla/)
