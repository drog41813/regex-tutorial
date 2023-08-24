# Matching hex values

In this regex tutorial, we will touch upon the regular expression that pertains to matching hex values.  

## Summary
The regex that will be targeted in this tutorial will be the /^#?([a-f0-9]{6}|[a-f0-9]{3})$/. This expression is mainly used to match hex values. Hex values are typically formatted in a hexadecimal manner and is utilized to identify a particularly specific color. From this point forward, I will be going in depth as to the various components that this regex contains as well as the purpose it serves within the expression itself. 


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
The two anchors are placed at the beginning and end of the expression. This is because these anchors are used as an indicator as to where the start and end of the expression will be, which in this case the /^ indicates the beginning of the expression whereas the $/ indicates the end. 

The Anchors in this expression are the /^ and $/. 

### Quantifiers
The quantifiers that are contained within this expression are the ?, {6}, and {3} respectively. A quantifier is essentially an indicator as to how many times a certain character, character class, and/or group must occur within the input for a match to be identified. The ? quantifier represents that the expression in question should match either 0 or 1 time(s). The {6} and {3} quantifiers indicate the type of format the hex will use, which in this case is the Hex triplet ({6}) or the shorthand hex ({3}).

### Grouping Constructs
The Grouping constructs within this expression is ([a-f0-9]{6}|[a-f0-9]{3}). Grouping constructsare what allow for the expression to particularly target the substrings of a string that is inputed. The [a-f0-9]{6} represents that there will be 6 instances of the [a-f0-9] mentioned and the [a-f0-9]{3} represents that there will be 3 values of [a-f0-9], which is then capped off with an or (|) which indicates that it will choose between one or the other dependent on input. 
### Bracket Expressions
The Bracket expressions that are contained within this regex are the 2 instances of [a-f0-9]. These expressions are utilized to group up a specific selection of characters and can range from alphabetic, special, or numeric characters and will contain a ( - ) to indicate the range. With this particular expression, it will match with any lowercase character between the letters a through f as well as numbers 0 through 9. 
### Character Classes
The character classes in this expression are the characters that are contained within the 2 brackets, which are a-f0-9. The character class represents a specific set of characters that can be compared with any string that is inputed when looking for a match. This specific character class represents looking for characters between a and f as well as the numbers 0 through 9. 
### The OR Operator
The OR operator that is contained within this regex expression is the |. This operator is utilized in order to allow for the expression to check for multiple instances and/or occurrences of the set of characters before and after the | symbol itself. In this expression, the OR operator is showing that the specific hex value will either be the {6} indicated, which translates into 6 characters OR( | ) the {3}, which translates to 3 characters. 
### Flags
This regex expression does not contain any instances of flags.
### Character Escapes
This expression does not contain any instances of Character escapes. 
## Author

Daniel Lee

GitHub Link: https://github.com/drog41813
