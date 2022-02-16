[Home](README.md) > [Code 201 Topic Notes](201topicNotes.md)

# Class 02

## HTML Text

When we create a webpage, we use **markdown** (tags) to the contents to provide meaning and allow browsers to show the correct structure we are trying to convey to the user.
There is **structural** markup and **semantic** markup.
Structural markup are elements used to plot out the foundation of a webpage.
Semantic markup provides extra information to the content, such as emphasis, something is a quote, acronym, etc.
Some examples of structural markup:

- `<h1>This is the main heading</h1>`
- `<h2>level 2 heading</h2>`
- `<p>paragraphs go here.</p>`
- `<b>bold words</b>`
- `<i>italic words</i>`
- `<sup>superscript</s>`
- `<sub>subscript</sub>`
- `<br />` this is a line break (when formatting a poem, for example)
- `<hr />` this is a horizontal rule to make a break in the page.

Some examples of semantic markup:

- `<strong>Caution</strong>` indicates importance, browsers will usually make bold
- `<em>emphasis that changes meaning of sentence</em>`

There are two different types of quotes that can include citations:

- `<blockquote>` and `<q>`

These are but a few of the many semantic markup elements we can use in HTML to more accurately represent meaning of content on a webpage.

## Introducing CSS

CSS applies rules to HTML elements to dictate how they will *appear*.
You can visualize them as *boxes* around content that determine how the content looks.
CSS rules contain two parts: the **selector** and the **declaration**.
Multiple elements can be included with a single rule if you separate them using commas.
Declarations are what actually describes how an element will be styled.
There are two parts to a declaration: the **property** and the **value**.
You can specify *multiple* properties in a single declaration, provided you separate them with semicolons.
You can use **external CSS** (CSS that lives on its own sheet) or **internal CSS** (CSS that is incorporated directly with HTML).
It is a better practice to use an external CSS file, especially when working with sites that are multiple pages.
**CSS selectors** let you target specific elements or sets of elements within an HTML document.
*Important*: they are case sensitive.
This allows you to be very specific in how you apply rules to sets of content.
CSS rules **cascade**, meaning certain rules take precedence over others.
It's important to understand how this works so you can override rules as necessary.

## Basic JavaScript Instructions

A **script** is like a recipe or list of procedures to follow.
A computer will follow them, line-by-line, one-by-one.
Each step is called a **statement**.
Statements end with a semicolon--much like CSS properties within a declaration.
**Code blocks** are indicated with *curly braces*.
Important to note is that JS is case sensitive.
Statements should be organized into code blocks.
This helps programmers make their code more readable and organized.
Additionally, it is good practice to include comments with your code
This helps you or others quickly figure out or remember what the function a specific code block was written to perform.
**Multi-line comments** are written as: `/* This is a multi-line comment */` and **single-line comments** are written as: `//`.

**Variables** define different values that the computer will remember and temporarily store when performing a function.
This concept is similar to algebra.
When writing scripts, we must give computers explicit instructions because they will carry out instructions (or not) exactly as you have written them.
The data stored within a variable can change within a function, which the computer can then calculate.
Before we can actually use a variable, we have to create it and give it a name.
t looks like this: `let quantity;`.
In this example, `let` is the variable keyword and `quantity` is the variable name.
Once we have created a variable, we can use **assignment operators** to assign a value to the variable.
If there is no value, the variable is *undefined*.

Three basic data types are:  **numerals, strings, and booleans** (true or false).
For numerals, no commas are used, you can represent negative numbers, and decimals are ok.
Strings are letters and other characters that are enclosed within quotes.
Example: `'This is a string.'`. Booleans can be thought of a light switch: on or off.

**Arrays** are variable types that store a list of values.
An **expression** assigns a value to a variable or it can combine multiple values into a single values (for example `let distance = 9 * 5`).
We can use **operators** (both arithmetic and string) to create a single value from one or more.
There is much more information on this topic, but I will leave that to reference when needed.

## Decisions and Loops

Most scripts have multiple possible paths.
Meaning the coder has to learn how to control the flow of data in order to handle different situations.
There are three main ways we can do this: evaluations, decisions, and loops.

- **Evaluations** analyze values in a script to see if they match the expected results
- **Decisions** use the result of evals to determine which path the script should go down
- **Loops** are used when we want a script to perform the same set of steps repeatedly (or multiple times depending on if conditions are met or not.

You can evaluate situations in code with **comparison operators**.
This is done by comparing a value in a script to what we expect it to be.
The code can then progress from there depending on the result. **Expressions** are often enclosed in brackets.
They usually contain one **comparison operator** and two **operands**.
For example: `(run >= pass)`.
Operands do not have to be a *single value*, in fact, they could be an *entire expression* that we are comparing against another expression.
While comparison operators usually return a true or false, we can use logical operators to compare the results of more than one comparison operator (for example: for this to be true, this expression and that expression must both be true).
Finally, we can use **if** and **if…else** statements in our code.
This simply means that if this condition is met (or not) then the following code in the script will be run.
The if…else statement is just a more complex script to run.
