# Regex-URL-gist

This gist describes the procces of matching URL's with a regular expression set.

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

Matching a URL: `/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`

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
The regex expression used to match URL's...
 `/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`
...uses anchors on either end to define what charaters URL's typically begin or end with.

![Anchors](./Media/anchors.png)

### Quantifiers

There are a number of quantifiers used in this regular expression. 
Qunatifiers can be used in a similar way of and/or gates. They can allow the programer to write a regex that can specify: 
- "* - zero-or-more"
- "+ - one-or-more"
- "? - zero-or-one"
- "{4} - a specific quantity such as four"
- "{4,} - more than four"
- "{1,4} - or between one and three"

![Quantifiers](./Media/quantifiers.png)


### Grouping Constructs

By grouping elements within round brackets we can act on them with quantifiers, refer back to them later or specifiy the preceeding or suceeding values.

![Grouping Constructs](./Media/grouping.png)


### Bracket Expressions

Bracket expressions are any set of items wraps by brackets. Round brackets create [Grouping Constructs](#grouping-constructs) square brackets create [Character Classes](#character-classes) and curly brackets can act as [Quantifiers](#quantifiers).

![Bracket Expressions](./Media/bracket%20expressions.png)

### Character Classes

Character classes enable us to select a range of values. They use square brackets to capture these values

![Character Classes](./Media/charater%20class.png)

### The OR Operator

![](./Media/quantifiers.png)

### Flags

![](./Media/quantifiers.png)

### Character Escapes

![](./Media/quantifiers.png)

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)

Please email any questions about this project to: Chrisw1096(you know it)gmail.com
or contact me though my github: 
[Wollemipines:](https://github.com/Wollemipines)
