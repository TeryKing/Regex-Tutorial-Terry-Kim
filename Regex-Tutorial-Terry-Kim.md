# Regex Tutorial by Terry Kim

This is a standard tutorial in order to understand the concept of Regex, aka regular expression. Regex is a special text string for describing a search pattern. Inside a code or search algorithms,
regular expressions can be used to find a specific pattern of characters within the string.

## Summary

We will be discussing individual components of Regex and also Hex Values.

We will use the following regex expression to define and determine its individual components.



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

## Regex Components

### Anchors

The anchors are components to start and end a string. By themselves, they dont match any regular expression, but instead assert something about the string based on whatever is next to the anchor. 

### Quantifiers

Quantifiers are components that communicate with the regex engine and must match the quantity of the characters of the expression going to the left.

Quantifiers trys to match any patterns an X amount of times, depending on which quantifiers used.

There are two types of quantifiers: Greedy and Lazy

A greedy quantifier tries to match the pattern at a specific position then repeats to the next position, while lazy quantifiers try to minialize the amount of position used to match.

### OR Operator

The OR operator is a boolean that matches with either the left or the right of the expression. 

### Character Classes

Character classes are just ways to match a specific amount of set characters. A hyphen can be used to define a range of characters rather than a specific single unit.

### Flags

A flag is a parameter that allows the regex to modify the way it searches. There are a total of 6 flags that serve different purpose.
i - ignoring case
g - Global
s - Dot all
m - Multiline
y - Sticky
u - Unicode

Flags are utilized using two forward slashes: // 
The pattern of what the flag will modify will be within those two forward slashes.

### Grouping and Capturing

Grouping and Capturing component is usually defined with (). This groups the expression between them and treats them as a single unit. 

### Bracket Expressions

Bracket expression that matches a specific pattern of characters within the brackets. Inside the brackets, a hypen will be used to define the range of set characters like [a-z] for alphabet characters from letters a to z.

### Greedy and Lazy Match

A greedy match just means that it will try to match the longest possible string, while a lazy match will try to match the shortest string.

### Boundaries



### Back-references



### Look-ahead and Look-behind



## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)