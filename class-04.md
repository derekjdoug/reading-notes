[Home](README.md) > [Code 201 Topic Notes](201topicNotes.md)

# Class 04

## HTML Links, JS Functions, and Intro to CSS Layout

### Links

Links are kinda the entire idea of what browsing the web is.
After all, we need to be able to navigate from one page to another!

Links come in a few different flavors:

- From one site to another
- From one page to another in the same site
- From one part of a page to another part of the same page
- Links that open in new page
- Email links

This is how a link is written:

- `<a href="url goes here">Link Text</a>`
- Links to an external site must use the absolute URL
- Links to an internal page can use a *relative URL* `example.html`

On larger sites, it's a great idea to organize your code by placing them in folders known sometimes as **directories**.
The top folder that everthing is contained in is called the **root folder**.
Underneath the root, additional folders can be thought of as a *family tree*.
It is important to note that when using *relative URLs* you must reference not only the filename, but also the filepath of what you are trying to link.
This means that you could have to use different URLs to link the same file to different pages.

Email links look like this:

- `<a href="mailto:derek@example.org">Email Derek</a>`

Opening a link in a new window looks like this:

- `<a href="http://www.example.com" target="_blank">Example opens in a new window</a>`

You can also link to specific parts of the same page by using *id attributes* or specific parts of an external page with an absolute URL and id attribute.

### Layout

CSS views HTML elements as being a box.
There are block-level and inline elements.
Block-level elements can be organized into another block called a **containing** or **parent** element (such as `<div>`).

To control the positioning of elements, there are a few different **positioning schemes** we must be aware of:

- Normal flow
- Relative positioning
- Absolute positioning
- Fixed positioning (a type of absolute positioning...helpful if you wanted like a header to stay at the top of the page even while scrolling)
- Floating elements (many layouts place boxes side-by-side...float is one way to do that)
- Clearing floats will make sure that you actually get the box layout you want so it remains consistent
- *overflow property* is one to know for fixing errors with parents of floated elements
- You can create multi-column layouts using floats

If you have overlapping elements with these functions, you can control which element is on top by setting the **z-index** property, otherwise known as **stacking context**.

Using this information, we can design and implement the layout of our site.
Some different factors must be taken into consideration, however, such as:

- device screen size
- screen resolution
- page sizes

There are a few different options at our disposal for layout type:

- Fixed width (width of the main boxes will be specified, usually in pixels)
- Liquid layout (usually percentages, so the layout will stretch depending on browser size)

Finally, designers make their lives easier when designing pages by using different layout grids to organize the content of a webpage.

### Functions, Methods, and Objects

- more to come...

All information taken from notes while reading *HTML&CSS* and *JAVASCRIPT&JQUERY* by Jon Duckett.
