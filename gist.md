Computer Science Regex Tutorial

Regular Expression or regex for short, are a series of special characters that define a search pattern. In essense, regex can be used to find and/or replace a set of characters within a string. Since regex are a series of special characters, it can be universal and used within all programming languages.

## Summary

The regex I will be providing a tutorial for is:
<br />
![Screenshot of Email regex](https://gist.github.com/ItsMARPON/3de0eb86a1e2e3bbc75c401b539556e6/raw/dd0f5aaefc313c5fbcf08ec7c88db22f9091d6c0/email-regexex1.png)
<br />
This regex matches email addresses that is broken down into three groups. The first group signified by parenthesis `()`, may contain only lowercase letters, digits, underscores, dots, and hyphens before the `@` symbol. The second group may contain only lowercase letters, digits, dots, and hyphens after the @ symbol. In the last group, after the `\.` symbol, it may contain any lowercase letters or dots with further limiting the possible value of characters to a minimum and maximum of 2 and 6, respectively.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)

## Regex Components

### Anchors

The anchor characters ^ and $ are both considered to be anchors. The ^ character signifies a
string that begins with the characters that follow it. This could be in one of two formats:
An exact string match, such as ^The, where the strings "The" or "The person" match, but "the" and "the person" do not.
This is because a regex is case-sensitive.
A range of possible matches, displayed using bracket expressions. this tutorial will discuss this in the next section.
The $ character signifies a string that ends with the characters that precede it. Just as with the ^ character,
it can be preceded by an exact string or a range of possible matches.

### Quantifiers

Quantifiers set the limits of the string that your regex matches (or an individual section of the string).
They frequently include the minimum and maximum number of characters that your regex is looking for.
{}—Curly brackets can provide three different ways to set limits for a match.

### Bracket Expressions

[a-z]—The string can contain any lowercase letter between a–z. Keep in mind that this looks for lowercase characters only.
If we wanted to include uppercase characters, we would need to change the expression to [a-zA-Z].
[0-9]—The string can contain any number between 0–9
If we put all of these expressions together so that our pattern is [a-z0-9_-], this will match any string that includes any combination of lowercase letters between a and z, any number between 0 and 9.
Keep in mind that these characters can be in any order. It's also important to note that this pattern does not require the string to meet all of these requirements; it can meet any of them.

### Character Classes

A character class in a regex defines a set of characters, any one of which can occur in an input string to fulfill a match.
We've actually already discussed some character classes.
The bracket expressions outlined previously, including positive and negative character groups, are considered character classes.
\d— Matches any Arabic numeral digit. This class is equivalent to the bracket expression [0-9].

## Author

Carisse Barr
I used the following as a reference: [https://coding-boot-camp.github.io/full-stack/](https://coding-boot-camp.github.io/full-stack/)

[Carisse Barr](https://github.com/carissella)

You can visit my Github Profile here: [Carissella](https://github.com/carissella) 
  If you have any questions please email me at carissebarr.swe@gmail.com