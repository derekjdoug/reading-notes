[Home](README.md) > [Code 201 Topic Notes](201topicNotes.md)

# Class 08

## More CSS Layout

CSS wasn't as involved or as complicated as it is today.
As technology has evolved, the ability to change the look of a site without ever touching the CSS has increased dramatically.

The `display` property determines if the element it is applied to acts inline or as a block.
Inline elements can be thought of like words in a sentence (meaning they do *not* start on a new line).
Block elements start on new lines, and their margins will be respected on all sides of the box they represent.
Finally, `display` also determines how an element's children will behave (flex being an example).

There are two main layout properties that create rules for multiple elements, these being `flexbox` and `grid`.
`Flexbox` will align an element's children next to each other, either horizontally or vertically.
This means that items will all stay on the same axis, and they will not wrap when the end up running out of space.
Child items of an element end up becoming *flex items* meaning that you can alter their rules on how they are oriented inside of a *flex container* (alignment, order, and justification are examples).
`Grid` is similar to`flexbox`, but controls multi-axis layouts instead of single-axis ones.
With is property, you can essentially create column and rows of grid items.

If you don't choose to use either of these layouts, your elements will display in *normal flow*.
Some properties we can use to manipulate layout here are:

- `inline-block` gives you some characteristics of a block-level element, but still flow inline with a level of text
- `float` think of a newspaper article with a picture, and the story wrapping around one edge of the photo to include it in the layout (space has to maximized, eh?)
- `column-count` and `column-gap` can be used to be split long list items into separate columns. With this, you can define heights and widths so that more columns will be added if the browser viewport becomes wider.
- `position` alters how elements behave when in the normal flow of the document. The options are: (`relative`, `absolute`, `fixed`, and `sticky`. `Static` is the default).

My main takeaway here is that CSS continues to be a mystical world of crazy things we can do with the display of a website within a browser, all with minimal--or no--changes to the HTML itself.

### Learn CSS - Layout

This chapter builds on the ideas of the site we read for the first half of this page of notes and goes into more depth.

Some items of note:

- `z-index` controls which elements will display on top of the other when their is overlap
- `clear` has something to do with clearing `floats` (meaning no side of an element will contact a specified side of a box)

The rest of the chapter dives into a breakdown of layouts.
We can base our decisions for designing layouts on a few different ideas.
Screen resolution (or device used) and browser size are important consideration, especially if you want your layouts designed for computers and mobile devices.
There are also layouts that are static or liquid, meaning they either adjust themselves, or don't, based on the browser viewport changing size.
Really, you need to look at the needs of the site and the end users and decide from there how you can design the site and convey the necessary information for all.

### Layout

Information taken from notes while reading *HTML&CSS* by Jon Duckett.
