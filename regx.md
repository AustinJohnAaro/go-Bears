# rooyale_With_Cheese

This tutorial will show one example of a regular expression (or regex) that was written to validate an email address. I will then break down the regex into it's component pieces and explain the function of each piece. 

## Summary

This expression uses anchors, quantifiers, character classes, grouping, and bracket expressions. The forward slashes at the beginning and end of the regex are there to delimit the search pattern and are not explained below as components of the regex. Use the table of contents below for explanation and examples of each of these components of the regular expression above. 

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
The anchors included in this regex are the ^ and the $ shown at the beginning and end of the line of code shown below:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

### Quantifiers
The quantifiers in this regex are the + and the {3,6} in the expression below:
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
Quantifiers indicate the amount of characters the regex will match.

The + quantifier will match 1 or more characters. The * quantifier will match 0 or more characters. The ? quantifier will match 0 or 1 characters. The {n} quantifier will match n characters. The {a,b} quantifier will match an expression that is at least a characters, but no more than b characters.

The quantifier often follows a character class or bracket expression that defines what characters the regex will match, as in the example below from the regex above:

[a-z0-9_\.-]+
In this example, ([a-z\.]{2,6}), a matching expression will be anywhere from 2 to 6 characters in length composed of characters as defined by the bracket expression that precedes the {} quantifier. 

### OR Operator

### Character Classes
The characters within the braces define what the regex will match, while the quantifier indicates how many.

Character Classes
The character class in regex below is the \d within the second set of braces.

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
The \d character class will match a single digit. The \w character class will match a single alphanumeric character or underscore. The \s character class will match a single white space such as a space or tab.

Capitalizing the letter will negate the character class so case is important when using these in your regex. For example, \D would match any character that is NOT a digit. 
### Flags

### Grouping and Capturing
Parenthesis are used for grouping in the regex below. In this particular regex, grouping is used to separate meta characters from literal characters. Grouping or capturing can also be used to isolate part of a string to back reference or to replace a part of the string.

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
([a-z0-9_\.-]+) and ([\da-z\.-]+) and ([a-z\.]{2,6}) are all groups found in the regex above. 
### Bracket Expressions
Bracket expressions are used to define what characters the regex will match. An example of a bracket expression from the regex we have been examining is:

[a-z0-9_\.-]
The characters that will match this bracket include the letters a-z, the numbers 0-9, an underscore, a period, and a dash.

Note that the backslash is not included in the matching characters stated. That is because the . on it's own represents a character class that will match any character. So in the case that we want to include a literal . as a matching character in our bracket expression, we must first type a \ to indicate an escaped character. The backslash that precedes the period differentiates the meta ., which represents a character class, from the literal . that we want to include as a possible matching character in the bracket expression.

Given the following bracket expression:

[a-z0-9_\.-]
brown_cow. //returns true
fre$h*m!lk //returns false
All characters in the first expression are included in the bracket expression and would therefore be matched. The second expression contains the special characters $*! which are not defined as matching by the bracket expression, and therefore would not be matched by the regex.

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

Hi, I’m @AustinJohnAaro

👀 I’m interested in Computer Engineering, Computer Programming and Computer Coding.

🌱 I’m currently learning Full Stack Computer Programming.

💞️ I’m looking to collaborate on electric Trucks.

 <https://github.com/AustinJohnAaro>
 
 