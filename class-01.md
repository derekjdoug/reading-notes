[Home](README.md) > [Code 201 Topic Notes](201topicNotes.md)

# Class 01

## HTML Structure

How we structure webpages is *extremely* important because it helps the user make sense of the hierarchy of information being displayed.
HTML is what describes that structure. HTML structure is defined by elements, which are usually comprised of two tags: an opening and a closing.

- Opening: `<p>`
- Closing: `</p>`

You can imagine tags like containers for information to go in.
They tell you something about the content that's within the tags.
We can further define tags with the use of attributes.
They are made of two parts: the name and value.
Example: `<h1 lang="en">`. *lang* (language) is the name and *en* (english) is the value.

Some of the major elements that define structure within HTML are the `<body>`, `<head>`, and `<title>`.
Everything within the **body** is what is going to be shown within the main browser window--what the user will see.
The **head** contains information about the page itself.
Within the head lies the title.
The **title** is what will show up at the top of the browser or in a browser tab.

## Extra Markup

The first thing we write on an HTML file is the **DOCTYPE**.
It's important to specify DOCTYPE at the top of the page because there have been several versions of HTML throughout the years.
`<!DOCTYPE html>` indicates to the browser that we are using HTML5.
Moving on, we can annotate **comments** in HTML--notes that are shown in the source code, but not in the browser page--by writing: `<!-- -->`.
Using comments is a good practice, because it helps you figure out what's going on with a page's code if you are not the original author or if you've been away from it for some time.
Diving further into HTML **elements**, we have some **attributes** that we can apply to give them identifiers to link for CSS or JavaScript code.
An **ID attribute** is a unique identifier for an HTML element.
It can only be used with *one* element on a page.
A class attribute is broader in the sense that you can apply it to *multiple* elements to give them all the same effects you defined.
**Block elements** are defined as appearing to start on a new line in the browser, while **inline elements** continue on the same line.
There are methods (elements) you can use to group items in a block and inline.
We can add a window into our page with the `<iframe>` element--showing a map application, for instance.
Further information about the page (for SEO and other reasons) can be added within the head under `<meta>`.

## HTML5 Layout

The take away here is that HTML5 was improved over past iterations of HTML by being easier and clearer to use.
It differentiates block level code instead of needing to use `<div>` elements to do so.
What this means is that it's easier to divide up the parts of a page, the structure--basically what HTML is all about.
Some specific examples I want to mention are **articles** and **asides**.
An `<article>` could be thought of as a stand alone section of a website--a blog post, for example.
An `<aside>` is used for a sidebar for information that is related to what is on the page, but not essential for its overall meaning.
An example here could be a glossary or notes referencing the page.
A danger with using some of these new HTML5 elements is that users with older browsers may run into compatibility issues.
There are codes that you can include to fix some compatibility issues, but they may not fix everything, possibly rendering some HTML5 items unviewable.

## HTML Process and Design

Just because you *can* create or make something doesn't necessarily mean you *should*.
Good websites are created for the user and their goals.
For this reason, we need to do some thinking based around:

- Who is the target audience for our site?
- Why do people visit the site?
    - We can now think about things such as navigation, contact means, etc.
- What are the visitors trying to gain?
- What info the users need
    - We can prioritize the structure of our website accordingly
- How often will people visit the site?
    - Does it need to be frequently updated?
    - What percentage of users return within a certain timeframe
- After we have done this research, we can decide what information needs to be contained within the site and create a site map.
- A great way to visualize this process in a very basic way of what the site should look like and how it should operate is with a wireframe. A wireframe is a rough sketch of the site design and UI.
- After the structure is defined, we can look at things like visual hierarchy, grouping, and designing navigation.
    - These are important  because users are unlikely to read everything that is on a page. We must design so scanning/skimming/navigation is easy

## ABCs of Programming

Coming soon!

Source: Notes were taken and paraphrased from reading *HTML & CSS* and *JAVASCRIPT & JQUERY* by Jon Duckett.