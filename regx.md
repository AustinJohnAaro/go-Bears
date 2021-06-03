# rooyale_With_Cheese

This tutorial will show example's of a regular expression (or regex) I will next crack down the regex within it's component slice and analyze the function of each unite. 

## Summary

This expression uses anchors, quantifiers, character classes, grouping, and bracket expressions. The forward slashes at the opening and end of the regex are there to specify the search pattern of the regex. Use the table of contents below for explanation and examples of each of these components of the regular expression above. 

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- 
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)



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
| Acts like a boolean OR. Matches the expression before or after the |. It can operate inward a group, or on a whole expression. The patterns will be approved in order. Just as in javaScript will match either set of characters. It will look for this OR that.

### Character Classes
The characters within the braces detail what the regex will meet, while the quantifier indicates how many.

The character class in regex below is the \d within the second set of braces.

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
The \d character class will match a single digit. The \w character class will match a single alphanumeric character or underscore. The \s character class will match a single white space such as a space or tab.

make capital of the letter will cancel out the character class so case is important when using these in your regex. For example, \D would match any character that is NOT a digit. 

### Grouping and Capturing
Parenthesis are used for grouping in the regex below. In this appropriate regex, grouping is used to free meta characters from accurate characters. Grouping or capturing can also be used to disengage part of a string to back reference or to replace a part of the string.

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
([a-z0-9_\.-]+) and ([\da-z\.-]+) and ([a-z\.]{2,6}) are all groups found in the regex above. 

### Bracket Expressions
Bracket expressions are used to define what characters the regex will match. An example of a bracket expression from the regex we have been examining is:

[a-z0-9_\.-]
The characters that will match this bracket include the letters a-z, the numbers 0-9, an underscore, a slash, a period, and a dash.



### Greedy and Lazy Match 
Greedy will consume as much as possible.  <.+> Suppose you have the following: <em>Hello World</em>
You may think that <.+>  would only match the <em> and the </em>, when in reality it will be very impatient, and go from the first < to the last >. It will match <em>Hello World</em> 
Making it lazy (<.+?>) will prevent this. By adding the ? after the +, we tell it to echo as few times as desirable, so the first > it comes across, is where we want to conclusion the matching. 

### Boundaries 
A word boundary, in most regex tongue, is a location between \w and \W (non-word char), or at the beginning or end of a string. If it initiate or completes  with a word character ([0-9A-Za-z_]).


### Back-references
Back-references match the same text as formerly paired by a catching a group.  By focusing the opening tag into a backreference, we can reuse the name of the tag for the closing tag.

### Look-ahead and Look-behind
Lookahead and lookbehind in a class are called “lookaround”, are zero-length declarations just like the start and end of a line. There are positive and negative lookarounds.

## Author

Hi, I’m @AustinJohnAaro

👀 I’m interested in Computer Engineering, Computer Programming and Computer Coding.

🌱 I’m currently learning Full Stack Computer Programming.

💞️ I’m looking to collaborate on electric Trucks.

 <https://github.com/AustinJohnAaro>
 
 