# Matching an Email Regex Gist Tutorial 

This is a Github Gist that describes how to use a Regular Expressions (Regex) to match an Email address.  
The below Regex is used to identify general an email that follows specific parameters. Those s

```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```

## Summary

Briefly summarize the regex you will be describing and what you will explain.
I will be describing the componenets 

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Bracket Expressions](#bracket-expressions)

## Regex Components

### Anchors
Anchors assert that the Regex current position in the string matches a well-determined location like the beginning or ending of the expression.  The below code written signifies our anchors used in our Regex.  

The "/^" signifies the start of the string and the "$/" signifies the end of the string. Its used to make sure the Regex has a start and a beginning.   

```/^$/```

### Quantifiers
Quantifiers are used to match a character or sequence zero or more times. 

The below code shows where we used a quantifier.  

```{2,6}```
We are making sure at the end of our email we have atleast between two to six characters.  

### Character Classes
Character classes distinguish kinds of characters.  This helps differentiate between numbers and digits.    

When refrencing our email regex we use character classes multiple times.

```a-z``` - this represents any letter from a-z
```0-9``` - this represents any number 0-9

When putting these in your Regex it allows the user to put in any number 0-9 or letter a-z.  


### Flags
Flags allow you to make the case sentive or insensitive.  You can also do this on a global scale.  We didn't input flags anywhere, but this is something you can do to ame the Regex even better/more efficient. 

### Bracket Expressions
A bracket expression matches a specific set of single characters.  It allows you the Regex to return all possiblites for that portion of your expression.  
We used a bracket expression in three places.  
1. Before the @ symbol - our regex makes sure we are only allowing lower case letters, number 0-9, hyphens and underscores. 
```[a-z0-9_\.-]```
2. After the @ symbol - our regex makes sure we are only allowing numbers and any lower case letters and hyphens. 
```[\da-z\.-]```
3. After the "\." - our regex make sure we are only allowing lower case letters a-z. 
```[a-z\.]```

## Author


I am a full stack web developer currently working as a Project Manager. The goal is to continue expanding my knowledge with building websites as well as Technology in general.  Being a CIO is the ultimate goal.  

Github Profile Link: https://github.com/dgib21
