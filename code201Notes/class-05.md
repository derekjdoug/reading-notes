[Home](README.md) > [Code 201 Topic Notes](201topicNotes.md)

# Class 05

## Images, Color, and Text

### Images

Images are important because they help establish the tone for the site.
If you do not have your own images to source, a good method is to uses a *stock photos* website, since all images are subject to copyright.
Images should be many things, but *especially* relevant and match your site (including color palette).
It is a good practice to keep your images in a separate folder, including subfolders, as necessary.

Images are added to pages using the `<img>` element.
It is an empty element, meaning there is no closing tag used.
Image elements contain:

- `src` (where the site can find the image file, usually a relative URL)
- `alt` (the alternate text; this is used be screen readers and search engines to describe the image)
- `title` (this is optional; most browsers will display the title if you hover over the image with the mouse)
- `<img src="images/example.jpg" alt="This is an example image" title="This image is giving us an example of how to use the image element.">`

You can specify the height and width of images in the `<img>` element, however it is probably a better practice to do this in CSS.

Where you place the image element in your HTML is signficant, and will alter the structure of your page.
Here are three additional important things to keep in mind when adding images to your page:

- images are best in the jpeg, gif, or png formats (they may not be as sharp as they could be, otherwise)
- make sure to save images as the correct size
- measure image height and width in pixels

HTML5 has added the `<figure>` and `<figcaption>` elements so that web authors can add a caption to the image and have the two be associated.

### Color

The *color property* specifies the color of text inside an element.
There are a few different ways to specify specific colors:

- RGB values
- Hex codes
- Color names (most browsers recognize 147 predefined names)
- HSLA (hue, saturation, lightness, alpha...beware, older browsers may not support this)

The *background-color property* controls the color of the background color for each element's box it is used in.
If you do not specify a color, it will default to transparent.

It is important to have good contrast between colors when creating a page.
Not only does this make your page more readable, it also helps your website accessibility with users who have vision disabilities.

You can control **opacity** with the *rgba property*.
This adds a forth value to the mix (which is a decimal), to control the opacity of elements and any child elements.
This is a newer CSS feature, so it may not work with all browsers, especially older versions.

### Text

Here is some helpful *typeface* terminology:

- **serif:** extra details on the ends of main strokes known as serifs. They look a little fancier
- **sans-serif:** cleaner font. No fancy details at the end of main strokes
- **monospace:** every letter has the same width (even an 'i' and 'm')
- **weight:** can add emphasis (how bold does the typeface look?), also effects whitespace and contrast of a page
- **style:** is it normal or italicized?
- **stretch:** how far apart are the letters?

When choosing a typeface (font) there are quite a few options to pick from, but it is important to note that the browser will only display that font if the user has it installed on their computer.
There are techniques available to increase the amount of typefaces available for a site, but they all have their own drawbacks or limitations.
These include: prompting the user to download the fonts, using an image with the text/font you want instead of text in HTML,siFR, and cufon (the later two deal with JavaScript and/or Flash).

Finally, there are many properties that deal with manipulating text. Whether you want to change the font-family, size, use a different font format, change the font weight, style, decoration, height, spacing, alignment, and indent, these choices (and more) are available to you in CSS. Most are fairly obvious, but there are some cool use cases out there!

### Which Image Format?

- **JPEG:** natural scenes, photography, images with high variation in color and intensity
- **PNG:** images that need transparant backgrounds, images with text or that need high contrast edges (think logos)
- **GIF:** animation images (is it gif or gif?!)

Information taken from notes while reading *HTML&CSS* by Jon Duckett.

*Which Image Format* notes taken from: [*JPEG vs PNG vs GIF — which image format to use and when?*](https://blog.imagekit.io/jpeg-vs-png-vs-gif-which-image-format-to-use-and-when-c8913ae3e01d) by Rahul Nanwani.
