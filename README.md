# Regex-URL-gist

This gist describes the procces of matching URL's with a regular expression set.

## Summary

This regular expression (or regex for short) allows for matching URL's. It uses anchors, quanitfiers, grouping constructs, bracket expressions, character classes and character escapes to do so.<br>

Matching a URL: `/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`<br>

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
This regex for identifying URL's uses anchors on either side of the expression to define the beginging and end of the search characters<br>

![Anchors](./Media/anchors.png)

### Quantifiers

There are a number of quantifiers used in this regular expression. 
Qunatifiers can be used in a similar way of and/or gates. They can allow the programer to write a regex that can specify: <br>
- "* - zero-or-more"<br>
- "+ - one-or-more"<br>
- "? - zero-or-one"<br>
- "{4} - a specific quantity such as four"<br>
- "{4,} - more than four"<br>
- "{1,4} - or between one and three"<br>

![Quantifiers](./Media/quantifiers.png)


### Grouping Constructs

By grouping elements within round brackets we can act on them with quantifiers, refer back to them later or specifiy the preceeding or suceeding values.<br>

![Grouping Constructs](./Media/grouping.png)


### Bracket Expressions

Bracket expressions are any set of items wraps by brackets. Round brackets create [Grouping Constructs](#grouping-constructs) square brackets create [Character Classes](#character-classes) and curly brackets can act as [Quantifiers](#quantifiers).<br>

![Bracket Expressions](./Media/bracket%20expressions.png)

### Character Classes

Character classes enable us to select a range of values. 
They use square brackets to capture these values<br>
There is also the option to speficiy characters classes with simplier notation.<br>
- \d matches a single digit<br>
- \w matches a single word character<br>
- \s matches a whitespace<br>
<br>

The URL regex uses \d and \w

![Character Classes](./Media/charater%20class.png)

### The OR Operator

OR opperators in Regex allow for multiple options to be considered valid. <br>
For example [color | colour] <br>
This URL regex does not use an OR opperator. If someone wanted to specifiy only URL's from particular addesses, it would be reasonable to use it as follows:
<br>
[com | gov | edu | ru | nu]

### Flags

flags allow us to sepcifiy a number of things regarding how we treat the contents that are being searched.
Such as case sensitivity (/i) or if the item being seached has multiple lines (/m).
<br>
<br>
There are no flags on this regex however if it were bing used to search a document for URL's the /m (multiline) and /g (global), should be included.<br>
![Flags](./Media/flags.png)

### Character Escapes

Native charaters such as . / * | } ] ) ? to list a few cannot be used literaly unless escaped. <br>
Placing a forward slash ( \ ) infront fo the character allows it to be used litteraly.

![Character Escapes](./Media/charater%20escapes.png)

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)

Please email any questions about this project to: Chrisw1096(you know it)gmail.com
or contact me though my github: 
[Wollemipines:](https://github.com/Wollemipines)
