# Regex Tutorial

Regex, which is short for regular expressions, are a group of characters that can be used to find and validate emails, usernames, urls, or html tags. In this tutorial I will explain each of the components in a regular expression for emails.

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.
In this tutorial I will be explaining a regex for emails and what each components searches for in this regex:

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

This regex checks whether an email entered by the user follows the guidelines in the regex.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Back-references](#back-references)

## Regex Components

### Anchors

In a regex anchors are always represented by two different symbols and come up first and last in a regex. The first character ^ signifies the beginning of the string and the $ signifies the end of the string. Since both are in place everything inside the regex must match the string.

### Quantifiers

A regex expression has four different symbols that are quantifies these are *, +, ?,  and the {} symbols. This regex has two quantifiers in it which are + and {2,6}. The + in the first part of it which is [a-z0-9_\.-]+ which means any character or number between a-z and 0-9 has to appear at least once. The same thing goes for the other part of the regex which is [\da-z\.-]. Inside the curly brackets are [a-z\.]{2,6} which indicates that the charcters a-z should have a minimum of 2 character and maximum of 6 characters.

### Character Classes

Character classes are used to shorten regular expressions and point to a set of charcters. In this regex the character class \d is used to look for anything between 0-9.

### Grouping and Capturing

In this regex we use a () to seperate the diffrent sections from each other.

The first section is ([a-z0-9_\.-]+) is trying to match the charcter a-z, the numbers 0-9 and the characters _, ., and - in the first part of the email.

The second section is ([\da-z\.-]+) this section targets the email's domain(gmail, outlook, hotmail). It uses a character class which targets the numbers 0-9, the letters a-z and the character . and - to match them.

The third section is ([a-z\.]{2,6}). This section get the final part of the email and looks for charcters a-z and . that are between 2-6 characters long.

### Bracket Expressions

Bracket Expressions are used to determine what the regex should include in the pattern and to seperate what each section should match for. The regex has three different sections which are [a-z0-9_\.-], [\da-z\.-], and [a-z\.].

## Author

My name is Joaquin Godina and I'm enrolled in the UCSD coding bootcamp. https://github.com/JoaquinGodina0 