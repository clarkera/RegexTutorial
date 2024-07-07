# Regex Tutorial: Matching Hex Value

Regular expressions are patterns used to match character combinations in strings.In a regular expression the metacharacter ^ means "not". For example, if "a" means "match lowercase a", "^a" means "do NOT match lowercase a".

## Summary

I will be explaining and breaking down the components of a regular expression used to match Hex Values.Hexadecimal code is a system by which any specific color can be described accurately to a computer. This ensures consistency and accuracy in an electronic display. A hexadecimal color value is a six-digit code preceded by a # sign; it defines a color that is used in a website or a computer program. The following is the regular expression for matching a hexadecimal color value that we will be examining in this tutorial: /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors

/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
The Anchors in a regex string are the ^ and $, the ^ will represent the start of the string and the $ represents the end of the string.
Everything in between the ^ and $ will be representing what the regex is looking for. Anchors do not match any character at all. Instead, they match a position before, after, or between characters.They can be used to “anchor” the regex match at a certain position.

### Quantifiers

/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
Quantifiers are used to communicate how many characters will be matched.By default, quantifiers are greedy, and will match as many characters as possible. If the ",+,?,{}" characters are found within regular expressions, they are considered quantifiers.The + indicates that the element may be repeated 1 or more times.The ? indicates that the element is optional, matching 0 or 1 occurrences.The {n} indicates a quantity, either a single number or a range of numbers.

### OR Operator

/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
The "or" operator within a regular expression is defined using the | element. The or operator indicates that it could either of the components that we are separating with the |. For our hex value regular expression we have ([a-f0-9]{6}`|`[a-f0-9]{3}). Note the or operator separating these 2 components. This means that our hex value could either be 6 characters [a-f0-9]{6} or 3 characters [a-f0-9]{3}.

### Character Classes

/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
Character classes are components within our regular expression that tells us what type of characters to expect. In our example our character classes are confined within brackets []. For our example we have 2 character classes: [a-f0-9] and [a-f0-9] which searches for the same values. We will be breaking down what the characters are searching within these character classes. a-f searches for letters a-f and 0-9 searches for digits 0-9.

### Bracket Expressions

/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
Matches any character in the square brackets. For example [nN] [oO] matches no, nO, No, and NO. gr[ae]y matches both spellings of the word 'grey'; that is, gray and grey.

### Greedy and Lazy Match

/^#?([a-f0-9]{6}|[a-f0-9]{3})$/
A greedy match tries to match an element as many times as possible. Whereas, a lazy match tries to match an element as few times as possible. In our example we have ? which signifies lazy quantifier. This is referred to a lazy quantifier because it causes the regular expression engine to match as few occurances as possible. We can simply turn this lazy match into a greedy one by adding a ?.

## Author

Hi I'm Rachael Clarke, I'm a full-stack developer student looking to expand my knowledge as much as possible.I am just as ambitious as I am curious about everything web-related!
GitHub:https://github.com/clarkera
