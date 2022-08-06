# Regular Expression Tutorial

Scripting languages such as JavaScript are designed with methods that can check strings for specific characters or elements when listed within the parameter, for example:
```
    str.includes(char)); 
```
*Which returns true or false, given weather or not the listed character or element is within the string.* 
```
    str.indexOf(char));
```
*Which returns the index of the string where the character can be located or -1 if the character is not* found.

Looking at these examples, one might conclude that listing each specific character is the simplest way to scan a finite set of strings for any words or characters. This, however, would limit the scan to direct matches and, ironically, complicate the code when looking for text that matches a similar pattern but differs in character values. With providing examples and the definition of **Regular expressions**
This tutorial will be explaining and breaking down a more concise way for setting up these parameters.

## Summary
***

**Regular expressions**, also known as regex, contains both literal and meta-characters. Which specifies a search pattern and can form arbitrarily complex expressions. The syntax of meta-characters give regular expressions the ability to vary the precision of pattern matching from exact to a very general similarity. Such patterns are commonly used in string-searching algorithms for "find" or "find and replace" operations, as well as input validation. Most general-purpose programming languages include regex support, allowing the expression to be used in a command prompt. Leaving regex to be widely used in search engines, word processors, and text editors. The following an example of a **regular expression**, that is used to identify text that matches the pattern of an email address:
```
    /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```


## Table of Contents
***
- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components
***
### Anchors
***
### Quantifiers
***
### Grouping Constructs
***
### Bracket Expressions
***
### Character Classes
***
### The OR Operator
***
### Flags
***
### Character Escapes
***
## Author
***
A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
//Link to profile 