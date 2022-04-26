[Home](README.md) > [Code 201 Topic Notes](201topicNotes.md)

# Class 12

## Chart.js & Canvas

### Chart.js

Charts are (generally) much more visually appealing for conveying information to users than tables are.
**Chart.js** is a JavaScript plugin that uses HTML5's canvas element to draw graphs onto pages.
We use the `<canvas>` element in HTML to create the charts and populate them with data using JavaScript.

[Web Designer Depot](https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/)  and [Chartjs.org](https://www.chartjs.org/docs/latest/) have some great examples of this.

### Canvas

The `<canvas>` element really only has two attributes: width and height.
If you don't specify these, they will automatically be 300 x 150.
You can use CSS, but the image may not end up being rendered appropriately and it can be distorted.
So...specify it in the tag itself!

You can style the element in CSS, just like any other element, but it doesn't actually affect the "drawing" on the canvas.
If there no CSS elements applied, it will be fully transparent by default.

Providing *fallback* content is important, because if users are using older browsers that are not compatible with canvas, they will be shown *something*.
An example would be a text explanation of what the graph is showing.
`<canvas>` creates a drawing surface that exposes one or more **rendering contexts**, which are what create or manipulate the data you are presenting.
There is a method called `getContext('2d')` that is used to obtain the rendering context.
In my example, I used the parameter '2d'.
This method only has the one parameter.
You can use an if/else statement to check for canvas support and whether or not to use fallback content.

MDN has tutorials on how to do things such as draw shapes, apply styles and colors, and draw text here:

- [MDN Canvas Shapes](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes)
- [MDN Canvas Styles & Colors](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors)
- [MDN Drawing Text with Canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text)
