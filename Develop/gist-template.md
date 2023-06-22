# Title (Regex Explained)

HI!! my name is Anthony and I wanted to take a walk with you through Regex. Today we will be going over, What regex? Why do I need to know this? how can I create one? and many more.

## Summary

RegEx also known as "regular expressions" is a set of characters that can create patterns that can be uses to find something in a database for instance * in sql. Another way that I have heard it is " It is engin logic". The one we will be looking at is
 /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/
This is matching a URL.

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
 /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/

-The anchors is what starts and ends the regular expression and it is the ^ at the beggining and the $ at the end

### Quantifiers
-A quantifier is used to see how many times a spacific character or group needs to be there in order to have a match. In this Regex
 /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/ 
 this next part is the quantifiers
[\da-z\.-]+)\.([a-z\.]
and what it is doing is looking for a match

### Grouping Constructs
-In this code there are 4 group sets. lets take a look
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/ 
-The first group set is (https?:\/\/)?
The first group matches the http:// or https:// at the beginning of the string. 
-The second set is ([\da-z\.-]+)
The second group matches the domain name.
-The third set is ([a-z\.]{2,6})
The third group matches the top level domain.
-And the fourth is ([\/\w \.-]*)*
And the fourth set matches the path.

### Bracket Expressions
-Bracket expressions are used to match a single character out of a group of characters. An example from /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/  would be [\da-z\.-] it matches a single character that is a digit, a letter, a period, or a dash. 

### Character Classes
-Character classes are used to match any one of a set of characters.
for example \d will match a single digit and \w will match a single word character.

### The OR Operator
-The OR operator is used to match either the expression before or after the operator an example from our regex /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/ would be the (https?:\/\/)? and it will match either the http:// or https://.

### Flags
-Flags are used to change the way the search is performed for an example the g flag ferforms a global match.

### Character Escapes
-Character Escapes are used to match a character that has a special meaning in the regex for example  /^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/ in this Regex the \. it matches a period.

## Author
-My name is Anthony LaNier I am a junior programmer, Husband, Father of three and I love programming as much as I love chess.
my GitHub is https://github.com/13Blackmagic/Regex
