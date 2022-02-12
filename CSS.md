[Home](README.md) > [Code 102 Topic Notes](102topicNotes.md)

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

Some other important features of CSS:

We can style elements based on their HTML element names, class attributes, location in a document, their state, *and* by comibining these together.
For example:

```
p {
    text-align: center;
}
```

Here we stylized the paragraph HTML elements.

```
p, h1 {
    text-align: center;
}
```

Here we combined multiple elements to style the same.

To add a class to style:

```
<p class="intro">
```

Now to style that class:

```
.intro {
    font-weight: bold;
}
```

You can also go further and combine element names and class names.

Additional examples can be found online!

This is just scratching the surface of **CSS* basics and what the language can do.