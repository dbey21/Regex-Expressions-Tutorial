# Regex Expression Tutoial

The goal of this gist is to dawdle over what a common word is and in what manner to employ them. common Expressions(Regex) might be utilized when one is testing to match a definite character mixture within a string. This is noteworthy for dragging out data from a given body of programming language along with being utilized for validation. For example, this tutorial will succeed an instance programming language snippet that is able to be utilized to match an email. This tutorial will succeed the distinct elements of common expressions.

## Summary


The following code will be utilized all over the tutorial to donate particular illustrations for how the elements of regex could be utilized. The after programming language could be utilized for matching electronic mail. One use for this programming language is that it might be utilized to verify to ensure that an email follows the accurate layout.

Matching Email-

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/


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
Anchors indicate a position to match strings, usually the beginning or the end.

^ anchor matches at the beginning of a string. $ ancher matches at the end of a string

### Quantifiers
Quantifiers indicate how many instances a character to match in a string and is appended to a character or an range of characters, e.g. [...], more on that later.

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
In our example, we used:

1.{2,6} quantifier, we have set an range of 2 to 6 times to match what's denoted in [...].
2.+ quanifier at the end of [...], this indicates we are matching between one and unlimited times. Both quantifiers matches as many time as possible giving back as needed.

### Grouping Constructs
Grouping is denoted by by parentheses, it unifies a pattern or string to be matched in a complete block.

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

In our example we have 3 groups ([a-z0-9_\.-]+), ([\da-z\.-]+) and ([a-z\.]{2,6}). Below we will talk about them more and break them down.

### Bracket Expressions
Brackets indicate a character class or an range of characters we want to match.

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
In our example:

1.[a-z0-9_\.-] indicates we are looking for lowercase "a-z" a through z, "0-9" 0 through 9, and we literal match special characters "_" underscore, "\." dot, and "-" hyphen.
2.[\da-z\.-] indicates we are looking for "\d" 0 through 9, "a-z" a through z, "\." dot, and "-" hyphen.
3.[a-z\.] indicates we are looking for "a-z" a through z, and  "\." dot.

### Character Classes
As mentioned above a character class is range of characters denoted in [...] of what we want to match .
### The OR Operator

### Flags

### Character Escapes
Backslash "" is the escape character in regex, escaping a character prevents a character from beging interpreted as a literal character.

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
In our example: "\." is in several places, using the backsplash denotes that we want to find just the dot.
## Author

Dahn Bey is a student at UC Berkeley extension Coding Bootcamp summer 2023. Locate me on Github:https://github.com/dbey21
