[Home](../README.md) > [Code 201 Topic Notes](../201topicNotes.md)

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

### Switch Statements to Loops

*Switch* statements begin with a new style of *variable* called the **switch value**.
You create multiple cases of code to run depending on if a variable matches a specificied value.
At the end of each case is the `break;` keyword.
This will tell JavaScript that the switch statement is complete and to run the code that appears after it.
Switch statements can perform better  than *if* statements because it stops the code from continuing to run when it has found a match.

JavaScript is considered to use **weak typing** because it is flexibile when it comes to the data type of a variable.
It can *change*.
Other languages do not allow this interpretation of data types, and are considered to use **strong typing**.
How JavaScript converts data types is called **type coercion**.
For example, if you had the following string: `'42'` JavaScript has the ability to convert the value to a number if appropriate.
The danger here is that it can cause mistakes and errors in your code and cause it to not run correctly.
A way to ensure this doesn't happen is to use the comparative operators of `===` and `!==` as they will check that the value *and* data types match.

Type coercion has interesting consequence for values in JavaScript: they can all be treated as *true* or *false*.
In my understanding, due to the wide variety of data types and that JavaScript checks for true/false, we also have **truthy** and **falsy** values.

- **Falsy** values are not labeled strictly as 'false', but can alse be a number 0, empty value, NaN, or an undefined value
- **Truthy** values comprise pretty much everything else. They could be 'true', numbers other than 0, strings with content, calculations, and even '0' or 'false' written as *strings*!

**Short Circuit Values** reference how *logical operators* are processed--from left to right.
They are considered to 'short-circuit' (or stop) as soon as they come to a result.
This result may not necessarily be *true or false*, but could be a *truthy or falsy* value as well.
For efficiency while programming, we can use this to place objects that are likely to be truthy in the beginning of a statement so the least amount of processing power is used.
Alternately, statements that are false that require additional code to be run that may also be more processing intensive can be put at the end of a statement so they do not run unless needed.

Finally, we have the topic of **Loops**.
Looks are scripts that check a condition.
They will keep looping and running as long as whatever condition being run returns as *true*.
As soon as it returns *false*, it stops running.
There are three different kinds of loops:

- **For** (used when you want a loop to run a speciifc amount of time, most common loop)
- **While** (condition will be something other than a counter, used when you do not know how many times a loop will need to be run. Code will continue to loop as long as the condiiton is true)
- **Do While** (similar to the **while** loop, the difference being that the code between the curly braces is guaranteed to be run *at least once*)

A **for** loop uses a counter to specify the code to run a certain amount of time.
Here are the steps:

- Create a variable, set to 0. Calling it 'i' is a common practice. This will act as the counter.
`let i = 0;`

- Create your condition (how many times the loop will be run)
`i < 5;`

- Chose an *increment operator* that will update the count (you can add or subtract from the count)
`i++`

- When the condition of the counter has been met, the code stops running and moves onto the next block.

**For** loops are really useful for looping through the contents of an array.

All information taken from notes while reading *HTML&CSS* and *JAVASCRIPT&JQUERY* by Jon Duckett.
