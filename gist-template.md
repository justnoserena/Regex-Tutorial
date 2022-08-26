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

**Regular expressions**, also known as regex, contains both literal and meta-characters. Which specifies a search pattern and can form arbitrarily complex expressions. The syntax of meta-characters give regular expressions the ability to vary the precision of pattern matching from exact to a very general similarity. Such patterns are commonly used in string-searching algorithms for "find" or "find and replace" operations, as well as input validation. Most general-purpose programming languages include regex support, allowing the expression to useful in a command prompt. Leaving regex to be widely used in search engines, word processors, and text editors. The following is an example of a **regular expression**, that is used to identify text that matches the pattern of an email address:
```
    /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
``` 
**Regular expressions** describes regular languages using the formal language theory, which is rooted in the mathematical field of computer science. The formal language theory can be viewed as what dictates a programming language's grammar. Meaning it matches words or semantics with its associated meaning. Explaining why regular expression can be visually complexing at first. However to the trained eye, it can be easily broken down into three parts:
```
    1.  ^([a-z0-9_\.-]+)@
```
The initial section of the expression defines the pattern of the email string before the '`@`' character, meaning that it will identify strings that match at least one of the preceding tokens:

- Any lowercased alphabetic letter from a to z
- Any character from 0 to 9
- A '`_`' character
- A '`.`' character
- A '`-`' character

Needs to include a '`@`' character after entering at least one of the previous tokens. 
```
    2.  ([\da-z\.-]+)\.
```
The mid section of the expression defines the pattern of the email string after the '@' character, before the '`.`' meaning that it will identify strings that continue to match at least one of the preceding tokens:

- Any digit character from 0 to 9
- Any lowercased alphabetic letter from a to z
- A '`.`' character
- A '`-`' character 

Needs to include the '`.`' character after entering at least one of the previous tokens.
```
    3.  ([a-z\.]{2,6})$
```
The final section of the expression defines the ending pattern of the email string after the '`.`' character, meaning that it will identify strings that continue to match between 2 to 6 of the proceeding tokens:

- Any lowercased alphabetic letter from a to z
- A '`.`' character

All three sections of the email must be included in order for the pattern algorithm to identify the string; otherwise, the email will not meet the parameters requirements. 

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
After learning what the our specific regex pattern is searching for, it's time to explore and define the various components of our expression.

```
    /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```
**Note:** Javascript uses both literal, as shown above, and RegExp constructor when creating a regex object. With literal using slashes and constructor function using quotation marks in place of the slashes.

### Anchors
***
**Anchors** are unique tokens found within **regular expressions** that are not characters but an assertion. It allows the expression to specifically assert locations within a string, where certain characters are to be. In our email expression there are two **anchors**.
```
    / ^ ([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6}) $ /
```

- '`^`' - This token asserts the beginning of the string. In our example that means our expression will only match with strings that begin with 

- '`$`' -

Although not shown in our own expression, there **anchors** that are still extremely helpful to know and understand.  

### Quantifiers
***
```
    /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```
### Grouping Constructs
***
```
    /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```
### Bracket Expressions
***
```
    /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```
### Character Classes
***
```
    /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```
### The OR Operator
***
```
    /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```
### Flags
***
```
    /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```
### Character Escapes
***
```
    /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```
## Author
***
A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
//Link to profile 