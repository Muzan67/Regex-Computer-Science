## Summary - The basic international phone number validation

The regex below validates a string against a valid international phone number format without delimiters and with an optional plus sign:

/^\+?[1-9][0-9]{7,14}$/

While validation of phone numbers using regex can give a possibility to check the format of the phone number, it does not guarantee that the number exists.

There might be also an option to leave a phone number field without any validation since some users might have:

- More complex phone numbers with extensions
- The different phone numbers for calling them on a different time of day

# Phone Number Regex

The basic international phone number validation

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

While the regex to validate a string against a valid international phone number expression may seem obscure upon initial inspection, we can break down eacah individual component in order to understand how the sequence works.

## Anchors

Anchors have special meaning in regular expressions. They do not match any character. Instead, they match a position before or after characters:

– ^ The caret anchor matches the beginning of the text.

– $ The dollar anchor matches the end of the text.

## Quantifiers

We often use the quantifiers to form complex regular expressions. The following shows some regular expression examples that include quantifiers:

Whole numbers:/^\d+$/

Decimal numbers:/^\d\*.\d+$/

Whole numbers and decimal numbers:/^\d\*(.\d+)?$/

Negative, positive whole numbers & decimal numbers:/^-?\d\*(.\d+)?$/

## Flags

A regex usually comes within this form /abc/, where the search pattern is delimited by two slash characters /.
At the end we can specify a flag with these values (we can also combine them each other):

m (multi-line) when enabled ^ and $ will match the start and end of a line, instead of the whole string.

## Grouping and Capturing

The square brackets can contain character ranges. For example, [0-9] is a digit from 0 to 9. The [^0-9] matches any character except a digit.

Typically, you use a backslash to escape a special character e.g., \.. However, in square brackets, you don’t need to escape most of the special characters except they have a meaning for the square brackets.

For example, if the caret (^) is at the beginning of a string, you need to escape it. If the caret is not at the beginning of a string (^), you do not need to escape.

Use the - inside a set to construct a range to match any character in the range.
Use the ^ to negate a range.

## Bracket Expressions

The square brackets can contain character ranges. For example, [0-9] is a digit from 0 to 9.

- Excluding ranges
  To make a range ineffective , you use the excluding range like: [^...].

- Escape special characters
  Typically, you use a backslash to escape a special character e.g., \.. However, in square brackets, you don’t need to escape most of the special characters except they have a meaning for the square brackets.

For example, if the caret (^) is at the beginning of a string, you need to escape it:
[\^#$]

Code language: JavaScript (javascript)
If the caret is not at the beginning of a string (^), you do not need to escape:
[#^$]

For example, [^0-9] matches any character except a digit. It is the same as \D.

- Summary
  Use the - inside a set to construct a range to match any character in the range.
  Use the ^ to make ineffective a range.

## Greedy and Lazy Match

In the greedy mode, quantifiers (expressions) try to match as many as possible and return the largest matches. When quantifiers (expressions) use the greedy mode, they are called greedy quantifiers.

In the lazy mode, the quantifiers (expressions) match their previous elements as few as possible and return the smallest matches. When quantifiers use the lazy mode, they’re often referred to as non-greedy quantifiers or lazy quantifiers.

Lazy quantifiers match their previous elements as few as possible to return the smallest possible matches.

Use a question mark (?) to transform a greedy quantifier into a lazy quantifier.

## Regex Gist

https://gist.github.com/Muzan67/278ea3140ca007db065b95a1e871acac

## Regex repository

https://github.com/Muzan67/Regex-Computer-Science

## Author

This regex tutorial was created by Alejandro Cortez

Github: https://github.com/Muzan67

## Alejandro Cortez - BIO

I am currently enrolled in Columbia Engineering Boot Camp to become a Full Stack Web Developer which has given me the foundation and tools to be both a Frontend and Backend Developer. I am developing while reinforcing newly developed skills and technologies which include HTML5, JavaScript, CSS, JQuery, Express.js, React.js, Node.js, responsive web design and applications, agile methodology, computer science, database theory, MongoDB, and MySQL.

I am also certified as an Amazon Web Service Cloud Practitioner which allows me to work with the AWS Cloud Management Console to access a broad collection of resources and services while managing information to perform AWS related tasks

🌍 Born and raised in NYC

⚡I am a professional Chef, Enthustiatic Travelor, Melomaniac, collector of the Polo Bear clothing attire from Ralph Lauren, Anime Otaku.


