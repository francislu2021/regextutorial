# Regex Tutorial Starter Code

Regex-Tutorial by Luknator-the full stacker

### Summary
This is a brief tutorial breakdown on how to use Regex rules for matching a Hex Value in a body of text. /^#?([a-f0-9]{6}|[a-f0-9]{3})$/ is the syntax that I will be applying for demonstration purpose.

Hex Code is a way to identify color. It is usually in a 6-digit alphanumeric sequence.

The regex string I am using will return a # Number sign character followed by either a 6 or 3 character length code with only lowercase letters a,b,c,d,e,or f or numbers 0,1,2,3,4,5,6,7,8, or 9.


### Table of Contents
1. Anchors
2. Quantifiers
3. OR Operator
4. Character Classes
5. Grouping and Capturing
6. Greedy and Lazy Match
7. Boundaries

### Regex Components
## Anchors
The starting ^ caret and ending $ dollar sign are both anchors in the example string. /^#?([a-f0-9]{6}|[a-f0-9]{3})$/
1. The ^caret matches at the start of the string the regex pattern is applied to.
2. The # Number Sign following the starting ^caret is a literal character and a #Number Sign MUST be at the start of the string.
3. The $ dollar sign matches at the end of the string the regex pattern is applied to. This signifies the end of the string.

### Quantifiers
Each quanifier denotes how many times the previous token will be matched. There are 3 quanitfiers in the example syntax. /^#?([a-f0-9]{6}|[a-f0-9]{3})$/
1. The first $ Dollar Sign ( which I will also go over in the Greedy section) This signifies that the # Number Sign will match 0-1 times.
2. {6} This signifies that the previous token [a-f0-9] will have 6 characters match within that set.
3. {3} This signifies that the previous token [a-f0-9] will have 3 characters match within that set.

### OR Operator
The example syntax uses an OR operator known as | Vertical line or pipe. There is a | Pipe between two characters classes. This creates 2 alternative groups. This allows the search to find and match either group.

/^#?([a-f0-9]{6}|[a-f0-9]{3})$/

1. The first alternative is before the | pipe [a-f0-9] will return 6 characters.

2. The second alternative after the | Pipe will return 3 characters.

### Character Classes
Character classes are found betwen [...] square brackets. They are used to create a list of allowable characters. In the example syntax there are two character classes. They look exactly the same because they are, however the quantifier is what makes each class return a different number of characters.

The example uses [a-f0-9]

1) a-f = This is the range that matches a case sensitive single character of: a,b,c,d,e, or f.
2) 0-9 = This is the range that matches a case sensitive single digit of: 0,1,2,3,4,5,6,7,8, or 9

### Grouping and Capturing
Anything found inside of ( round brackets ) creates a capture group. Everything inside that (...) is treated as a single unit. So with the example syntax /^#?([a-f0-9]{6}|[a-f0-9]{3})$/ there is one capture group with two characters sets seperated by an OR Operator.

### Greedy and Lazy Match
The single ? by defult is considered greedy. This means it will match as many occurrences of the given pattern as possible. A lazy match would be denoted as a double ??. Lazy means as few occurrences of the pattern as possible, however our example syntax is considered greedy not lazy.

### Boundaries
Boundries used are the ^caret to siginify the start of the string and the $ dollar sign signifies the end of the string.

If you still have any questions, please feel free to contact me. thank you!

Luknator tutorial
