[Home](README.md) > [Code 201 Topic Notes](201topicNotes.md)

# Class 09

## Forms and JS Events

### Forms

Forms allow users to perform functions on a site (signing up to become a member, searching, entering comments, etc.).

There are different types of form controls that you can use to collect information from site users:

- Add text: (single-line text input, password input, text area/box)
- Make choices: (radio butons-select one of a number of options, checkboxes-select one or multiple options, and drop-downs)
- Submitting forms: (submit buttons, image buttons, file uploads)

Forms can have several (or many, really) form controls to gather different information.
The server needs to know which piece of inputted data the user submitted corresponds to which form element.
What this means is that information is sent from the browser back to the server using our classic name/value pairs.
If the form control is text input, the value of the form control is what the user typed in.
If the form control lets the user pick from a fixed set of choices, the web page author writes code that gives each option their automatically assigned value.

Form controls are written using the `<form>` element.
`<form>` tags require an *action* attribute, its value being the URL for the server page that will receive the form info when submitted.
The *method* attribute will also usually be present.
There are two different methods to send forms: *get* or *post*
In the get method, values of the form are added to the end of the URL specified in the action attribute.
This makes it ideal for: short forms (such as a seach), retrieving data from a web server, etc.
Post values are sent in **HTTP headers**.
Post should be used when allowing users to upload files, long entries, sensitive data is involved (like passwords), or if the entry adds information to, or deletes information from, a database.

`<input>` element is used for several different form controls, including text.
The element using attributes like: *type*, *name*, and *maxlength*.
You may also see *size* in older code, but it should no longer be specified in HTML, but rather CSS.

Other form controls are implemented much the same, though may send additonal information or values.
These examples include: password input, text area, radio buttons, checkboxes, drop-down lists, multiple-select boxes, file input, submit buttons, image buttons, etc.

Labelling form controls is important to do, as it makes forms accessible for vision impaired users.
Each form control should have its own label.
There are two different ways you can apply a label to a form control:
You can wrap around the text description and the form input *or* you can use the *for* attribute, which specifies which from control the label applies to.

For longer forms, you can group them together using the `<fieldset>` element.
In most browsers, a box will appear around the grouped form controls, indicating their relation.
The box appearance can be edited using CSS.
Additionally, the `<legend>` element can be placed right after the opening `<fieldset>` tag and contains a caption that helps identify the purpose of the group of form controls.

HTML5 is beginning to incorporate something called **form validation**, which essentially ensures the user is filling out the form properly, and prompting them if that is not the case.
Traditonally, this was done using JavaScript, but more and more HTML5 browsers are reducing the legwork and adding compatbility for this HTML5 feature.
HTML5 also has incorporated ways to standardize certain iformation such as date input.
This would be indicated with the `type="date"` attribute.
There are also specific `type=""` options available for email & url input, as well as searches.

### Lists, Tables, & Forms

In addition to forms, CSS has the ability to manipulate the appearance of tables and lists in HTML as well.

These include:

- Bullet-point styles (both for `<ul>`--shapes--and `<ol>`--decimals, alphas, or romans, etc.)
- Images for bullets (by referencing an img url)
- Positioning the marker (is the bullet point indented outside of the content, or within?)
- There is the *list-style* CSS property, which allows you to use shorthand and express several list properties together
- A gigantic list of *table properites* that can manipulate just about every aspect of a table imaginable
- The *empty-cells* property specifies whether the borders of empty cells are visible or not
- *Border-spacing* and *border-collapse* specifiy whether or not there are gaps between cells
- Pages 341 - 347 outline examples of how to use CSS to style forms, including submit buttons, fieldsets and legends, aligning form controls, and cursor styles

### Events

Events are a way to make your site more interactive.
Basically, when a specified event/interaction occurs (we call this the event being **fired** or **raised**), code is **triggered** and ran!
There are many different event types that we can use to trigger code (the list is on pages 246 and 247).
When events trigger code, the steps involved are called **event handling**.

1. Select element node you want script/code to respond to
2. Indicate which event on that selected node will trigger the response
3. Select the code you want to run when the event occurs

There are also three different ways to 'bind' events to elements:

1. HTML event handlers (not good practice, does not separate HTML and JS)
2. Traditonal DOM Event Handler (good, put an event can only trigger one function with this method. Trying to trigger additional functions on the same page may cause errors)
3. DOM Level 2 Event Listeners (preferred method, multiple functions can be used for single event; ex: validating form and submitting when user does specified event)

Here is a syntax example for traditional DOM event handlers:

- `element.on*event* = *functionName*;` 'element' refers to the DOM element node to target, 'on*event*' refers to the event bound to the node to trigger, and '*functionName*' is the code that will be run

There is a great example of this on page 253 of *JAVASCRIPT&JQUERY*.

Event listener syntax is as follows:

- `*element*.addEventListener('*event*', *functionName* [, *Boolean*]);` *element* is the DOM node to target, '*event*' binds the node, *functionName* is the function to call, and the last part is for the **event flow**, indicating something called *capture* . . . usually set to false

The rest of the chapter dives into more specific ways to write code and manipulate the syntax for different effect.
Basically, adding details to these ideas.

Information taken from notes while reading *HTML&CSS* and *JAVASCRIPT&JQUERY* by Jon Duckett.
