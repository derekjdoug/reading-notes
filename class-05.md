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
