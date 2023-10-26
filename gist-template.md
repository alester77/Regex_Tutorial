# Regex Tutorial

Welcome to this Regex tutorial where we unravel the mysteries behind validating email addresses using Regular Expressions (Regex). By the end of this tutorial, you will have a clearer understanding of how different components of a regex come together to perform a powerful email validation.

## Summary

In this tutorial, we will dissect the following regex used for email validation.
Matching an Email – /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

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

Anchors `^` and `$` are used to match the start and end of a line, respectively. In our email regex, these anchors help ensure the matched pattern represents the entire email address.

### Quantifiers

In our email regex, quantifiers such as `+` and `{2,6}` specify the number of times a character or group of characters may appear. For example, `[a-z0-9_.-]+` ensures that the username part of the email has one or more valid characters.

### Character Classes

Character classes, like `\d` and `[a-z]`, match a specific set of characters. In our case, `\d` matches digits, and `[a-z]` matches lowercase letters, contributing to the flexibility of the domain part matching.

### Flags

While not explicitly used in our email regex, flags like `i` could be added to make the email matching case-insensitive, for example, `/email regex/i`.

### Grouping and Capturing

Parentheses `()` create groups in our email regex, capturing the username, domain, and top-level domain (TLD) parts of the email for potential back-references or separate extraction.

### Bracket Expressions

Bracket expressions `[ ]` define a set of characters of which only one needs to be matched. In our email regex, various bracket expressions, like `[a-z0-9_.-]`, specify the allowable characters in different parts of the email address.

### Greedy and Lazy Match

Greedy matches capture as much as possible, while lazy matches capture the smallest amount possible, influencing the overall matching behavior.

### Boundaries

Boundaries, like `\b`, assist in defining the edges of words or sequences within the text to ensure precise matches.

### Back-references

Back-references refer to previously matched groups, allowing for consistency and repetition checks within the pattern.

### Look-ahead and Look-behind

Look-aheads and look-behinds perform assertions to check for the presence or absence of patterns before or after the current matching point without including them in the match.

## Author

This tutorial was made by Alexa Lester during the DU Coding boot camp.
Github: alester77@github.com
Linked In: https://www.linkedin.com/in/alexa-lester-a23143189/
Email: alester0284@gmail.com

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
