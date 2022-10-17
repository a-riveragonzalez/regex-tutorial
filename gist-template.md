# Regex Tutorial for Matching a Hex Value
---

Regex, also known as regular expressions, define a **search pattern** by utilizing a series of characters. 


When using Regex, you look at each character and translate what they mean. 
For example : "Cat" is a captical "C" followed by a lowercase "a" and lowercase "t". In this case, each of these characters are **literal characters**. We can also use **meta characters**, which refers to a general pattern rather than a literal character. Using the above example of "Cat", we want a uppercase alphabetical character followed by two lowercase alphabetical characters. 


When included in code or search algorithms, regular expressions can be used to find certain patterns of characters within a string, or to find and replace a character or sequence of characters within a string. They are also frequently used to validate input. 

## Summary
---

In this tutorial, we will use an example to match a hexcode. A hex code is a format to identify colors with a six custom characters. The example regex we will use is: 

`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`



## Table of Contents
---

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Summary](#summary)
- [Author](#author)

## Regex Components
---
### Anchors
---
**Anchors** are used to signify the the start and end to a string. Both "^" and "$" are anchors. 

In our example : `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`
- The "^" anchor is used to start the string
- The "$" anchor is used to end the string

### Quantifiers
---
**Quantifiers** set the length of sections of the string. They can set the minimum, maximum, and/or the exact amount of characters a string can have. 

In our example : `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`
- The "?" matches the pattern zero or one time
- The "{6}" and "{3}" signify that the length of that part of the string will be what is inside the curly brackets

### OR Operator
---
The **OR operator** means that either expression on both sides of the "|" will be true. 

In our example : `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`
- The "|" means that the string can either be `[a-f0-9]{6}` or `[a-f0-9]{3}`

### Grouping and Capturing
---
Grouping helps break the string into smaller sections to fulfill different requirements. "()" are used to create sections, also known as **subexpressions**. 


In our example : `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`
- The "( )" are used to start and end of a group, or subexpression



### Bracket Expressions
---
**Bracket Expressions**, or positive character groups, are held inside "[]" and represent a range of characters we want to match. The "-" can be used to set a range for numerical or alphabetical characters. 


In our example :  `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`
- The "[ ]" indicates what we want to include in our regex
- The "a-f" means it can have any letter a-f
- The "0-9" means it can have any number 0-9


### Summary
---

Here is a quick summary of what these characters represent : 
`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

- "^" anchor used to start the string
- "#" Literal character, the hex code will start with this
- "?" matches the pattern zero or one time
- "( )" start and end of a group, or subexpression
- "[ ]" start and end of a bracket expression
- "a-f" string can have any letter a-f
- "0-9" string can have any number 0-9
- "{ }" length of that part of the string will be what is inside the curly brackets
- "|" or operator
- "$" anchor is used to end the string



## Author
---

💻 I am a junior full stack web developer based in Los Angeles. 

👾 Check out what else I'm up to on [my github](https://github.com/a-riveragonzalez)
