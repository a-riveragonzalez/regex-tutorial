# Regex Tutorial for Matching a Hex Value
---

Introductory paragraph (replace this with your text)

Regex, also known as regular expressions, define a **search pattern** by utilizing a series of characters. 
When using Regex, you look at each character and translate what they mean. 
For example : "Cat" is a captical "C" followed by a lowercase "a" and lowercase "t". 
- in this case, each of these characters are literal characters 

"Meta" vs. "Literal" characters

Meta character refers to a general pattern rather than a literal character. Using the above example of "Cat", want a Uppercase character followed by two lowercase characters. 
## Summary
---

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

In this tutorial, we will use an example to match a hexcode. A hex code is a format to identify colors with a six custom characters. 

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
Anchors are used to signify the the start and end to a string. Both "^" and "$" are anchors. 

In our example : `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`
- The "^" anchor is used to start the string
- The "$" anchor is used to end the string

### Quantifiers
---
Quantifiers set the length of sections of the string. They can set the minimum, maximum, and/or the exact amount of characters a string can have. 

In our example : `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`
- The "?" matches the pattern zero or one time
- The "{6}" and "{3}" signify that the length of that part of the string will be what is inside the curly brackets

### OR Operator
---
The OR operator means that either expression on both sides of the "|" will be true. 

In our example : `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`
- The "|" means that the string can either be `[a-f0-9]{6}` or `[a-f0-9]{3}`

### Grouping and Capturing
---

In our example : `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`
- "(" ")" start and end of a group 



### Bracket Expressions
---

In our example :  `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`
- "[ ]" everything in this is what we want to include in our regex
- "a-f" any letter a-f
- "0-9" any number 0-9


### Summary
---

Here is a quick summary of what these characters represent : 
`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

- "^" used to start the string
- "#" Literal character, the hex code will start with this
- "?" matches the pattern zero or one time
- "( )" start and end of a group 
- "[ ]" start and end of a bracket expression
- "a-f" any letter a-f
- "0-9" any number 0-9
- "{ }" length of that part of the string will be what is inside the curly brackets
- "|" or operator
- "$" anchor is used to end the string



## Author
---

💻 I am a junior full stack web developer based in Los Angeles. 

👾 Check out what else I'm up to on [my github](https://github.com/a-riveragonzalez)
