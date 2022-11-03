# Regex Tutorial Matching a Hex Value by Terry Kim

This is a standard tutorial in order to understand the concept of Regex, aka regular expression. Regex is a special text string for describing a search pattern. Inside a code or search algorithms,
regular expressions can be used to find a specific pattern of characters within the string.

## Summary

We will be discussing individual components of Regex and also matching Hex Values.

We will use the following regex expression to define and determine its individual components.

        /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

This will be our example for matching a Hex Value.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)


## Regex Components

 
### Anchors

The anchors are components to start and end a string. By themselves, they dont match any regular expression, but instead assert something about the string based on whatever is next to the anchor. 

In our example expression, the ^ will be our anchor to start this string. And at the end of our string, $ is ending the string.

### Quantifiers

Quantifiers are components that communicate with the regex engine and must match the quantity of the characters of the expression going to the left.

Quantifiers trys to match any patterns an X amount of times, depending on which quantifiers used.

There are two types of quantifiers: Greedy and Lazy

A greedy quantifier tries to match the pattern at a specific position then repeats to the next position, while lazy quantifiers try to minialize the amount of position used to match.

Our quantifiers with the example is ? and {n}, in our case where n = 6 and 3. Our ? quantifier is matching any preceding characters maximum 1 time. Since our ? is preceded by a #, our expression will try to match a string that begins with a # or not.

Our {n} quantifier is a meta character that is trying to match exactly the preceding characters n amount of times, in our case 6 and 3. So with {6}, it will try to match a string that contains 6 consecutive numbers such as 000011.

### OR Operator

The OR operator is a boolean that matches with either the left or the right of the expression. 

Our OR Operator for our expression is a |, which in our case is inside a big group. ([a-f0-9]{6}|[a-f0-9]{3}) is our big group that contains our OR operator, which splits the expression into 
[a-f0-9]{6} and [a-f0-9]{3}. This means that our regex will match either or of these expression.

### Grouping and Capturing

Grouping and Capturing component is usually defined with (). This groups the expression between them and treats them as a single unit. 

Our grouping component in our expression is ([a-f0-9]{6}|[a-f0-9]{3}). This grouping is also using a combination with an OR Operator. Please see ### OR Operator for explanation.

### Bracket Expressions
 
Bracket expression that matches a specific pattern of characters within the brackets. Inside the brackets, a hypen will be used to define the range of set characters like [a-z] for alphabet characters from letters a to z.

In our expression, we are using [a-f0-9] multiple times to have a literal letter from a - f and a literal number from 0-9.

## Author
 
https://github.com/TeryKing

