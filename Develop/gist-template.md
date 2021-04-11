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
Also known as Alternation Operators, OR Operators match between a choice of regular expressions.  

Examples of OR Operators:
```
(|)         matches a string that is followed by the value on the left or the right of the veritcal bar

[]          matches a string that is not followed by the value indicated in the brackets
```

Examples:
```
a(b|c)     matches a string that has a followed by b or c (and captures b or c)

a[bc]      same as previous, but without capturing b or c
```


### Character Classes
Character Classes tell the regex engine to search for specifically indicated characters such as numbers, words, or spaces.

Examples of Character Classes:
```
`\d`      matches a single character that is a digit

`\w`      matches a word character (any alphanumeric character plus underscore)

`\s`      matches a whitespace character (including tabs and line brakes)

`.`       matches any character the capital case for any aformentioned characters will inverse the match
```

Examples:
```
\d         matches a single character that is a digit

\w         matches a word character (alphanumeric character plus underscore)

\s         matches a whitespace character (includes tabs and line breaks)

.          matches any character

\D         matches a single non-digit character

\W         matches a single any non-character that is a-z

\S         matches a single non-` `

```
### Flags
Flags are special tags that alter a search to return different results.

Examples of Flags:
```
`g`         (global), makes the expression serach for all occurrences

`m`         (multi-line), makes the boundary characters '^' and '$' match the beginning and ending of every single line instead of the beginning and ending of the whole string.

`i`         (insensitive), mmakes the expression search case-insensitively
```

Examples:
```
/Hello/g   matches all characters `Hello` in the test

/Hello/m   matches the beginning and ending of each line with `Hello`, rather than the whole string `Hello` itself

/Hello/i   matches all `hello` regardless of case (Hello, hEllo, heLlo, hellO, hello, HELLO would all return in the search)
```


### Grouping and Capturing
Grouping creates a unified string so that it is matched completely.

Examples of Grouping:
```
()          characters inside parentheses indicates a captured group

(?:)        using ?: disables the captured group

(?<>)       using ?<> names the group
```

Examples:
```
a(bc)           parentheses create a capturing group with value bc

a(?:bc)*        using ?: we disable the capturing group

a(?<foo>bc)     using ?<foo> we put a name to the group
```

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
