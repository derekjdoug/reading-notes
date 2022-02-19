[Home](README.md) > [Code 201 Topic Notes](201topicNotes.md)

# Class 03

## HTML Lists, Control Flow with JS, and the CSS Box Model

### HTML Lists

There are three different types of lists on HTML:

- Ordered lists (each item in the list is numbered)
- Unordered lists (List items begin with a bullet point instead of number)
- Definition lists (define a term with its definition)

Here are some example elements:

- `<ol>` ordered list
- `<li>` list item
- `<ul>` unordered list
- `<dl>` definition list
- `<dt>` definition term
- `<dd>` definition
- These also have closing tags that must be used
- You can nest lists inside of each other for sub-bullets (further indentation)

### CSS Boxes

We can imagine that CSS treats HTML elements as if they are a box that surrounds them.
With that in mind, there are many modifications we can perform using CSS to manipulate the box and its contents.
Some examples are:

- Controlling dimensions, colors, fonts
- Creating borders (literal visual boxes)
- Manipulate margins and padding
- Show or hide different "boxes"

For manipulating dimension (such as *width* and *height*), there are a few different ways to go about it.
Some common measurements are **pixels**, **percentages**, and **ems**.
Pixels were very popular because they allow the designer exact control over the size of a box, but percentages have been used more because they translate better across different types of devices.
If the content contained within a box is larger than the box itself for whatever reason we can use the `overflow` property to tell the browser what to do.
Overflow can do things like choose to hide the content or have the user scroll to reveal.

Boxes have three very important properties that are adjusted to control their appearance.
They are:

- Border (separates the edge of one box from another)
- Margin (beyond the border, creates space between them)
- Padding (space between the content and the border of the box)

Adjusting these properties will manipulate space between boxes, which is crucial in aiding the positioning and readability of the content.
The margins will also control where content is justified on a page.
There are many attributes that you can set for all of these different properties.
I will not list them here because they are numerous and easy to reference.

Also of note in this section is the ability to use the `display` property to make inline elements behave like a block-level elements and vice versa.
An example for this would be getting a list to display horizontally instead of vertically (think page navigation).
You can also choose to hide boxes with the `visibility` property.
Anything hidden with the property *will* be visible in the source code that's available to everyone with browser development tools.

A few extra cool things are described at the end of the chapter like making border images, box shadows, and rounded or elliptical corners for borders.

### Basic JavaScript Instructions

**Arrays** are a type of variable in JavaScript.
Essentially, they are a *list* or set of variables that are *related* to each other.
The technique for creatign an array is called an **array literal**.

Example:

`let teams;`
`teams = ['Sabres', 'Canadiens', 'Maple Leafs'];`

You can also use an **array constructor**

`let teams = new Array('Sabres', 'Canadiens', 'Maple Leafs');`

Values in arrays are given numerical values as if they were in a numbered list.
Important to note on this point is that the numbers *start counting on zero*.
You can alter the value of an item in an array just like you would with any other variable.
You can also reference the array variables *index number*.

### Switch Statements

This current information is a placeholder and will be updated with more notes tomorrow.

All information taken from notes while reading *HTML&CSS* and *JAVASCRIPT&JQUERY* by Jon Duckett.
