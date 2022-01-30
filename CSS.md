[Home](README.md)>[Topic Notes](topicNotes.md)

# Design Web Pages With CSS

## Week 01 Day 05

## CSS

**CSS** stands for Cascading Style Sheets.
It's a language used for altering the presentation of a document written in a markup language--HTML for example.

**CSS** is a rule-based language.
We define the rules we want to appear on our web page or to affect specific elements of HTML by making our styles.css file and linking it to the HTML file.

CSS rules open with a *selector* and then have a set of *curly braces* `{ }` that will contain declarations.
Declarations state a property, and the value of that property.
To include multiple declarations inside of our `{}` we must include a `;` after the values of each line.
For example:

```
body {
    background-color: cyan;
    font-size: 20px;
}
```