# Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

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
Anchors are sequences that help search for the beginning and end of a string.

Examples of Anchors:
```
^           indicates the starting point of the searched string

$           indicates the ending point of the searched string or word
```

Examples:
```
^The        matches any string that starts with The 

end$        matches a string that ends with end

^The end$   exact string match (starts and ends with The end)

roar        matches any string that has the text roar in it
```

### Quantifiers
Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found. 

Examples of Quantifiers:
```
*           matches a string whose preceeding characters are followed by zero or more of the last character

+           matches a string whose preceeding characters are followed by one or more of the last character

?           matches a string whose preceeding characters are followed by zero or one more of the last character

{}          matches a string whose preceeding characters are followed by x amount (bracketed number) of the last character

()          matches a string whose preceeding characters are followed by zero or x more copies of the parenthesized characters
```

Examples:
```
abc*        matches a string that has ab followed by zero or more c

abc+        matches a string that has ab followed by one or more c

abc?        matches a string that has ab followed by zero or one c

abc{2}      matches a string that has ab followed by 2 c

abc{2,}     matches a string that has ab followed by 2 or more c

abc{2,5}    matches a string that has ab followed by 2 up to 5 c

a(bc)*      matches a string that has a followed by zero or more copies of the sequence bc

a(bc){2,5}  matches a string that has a followed by 2 up to 5 copies of the sequence bc
```

### OR Operator

### Character Classes

### Flags

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
