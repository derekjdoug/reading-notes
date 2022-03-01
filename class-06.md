[Home](README.md)

# Class 06

## Problem Domain, Objects, and the DOM

### Object Literals

**Objects** group together sets of variables and functions to represent/model something we would see in the real world.
For instance, an object could represent a motorcycle dealership and their inventory.
Variables that are a part of an object are known as **properties**.
Properties tell us more about an object, for instance: what the name of the motorcycle dealership is, what motorcycles they have in stock, etc.
Functions that are included in objects are called **methods**.
Methods can be thought to represent tasks that are associated with an object.
For example: a method that represents the motorcycle dealership's current number of motorcycles in inventory.

Properties and methods have *names* and *values*.
Names are called a **key** in objects.
Objects can't have multiple keys with the same name because keys are used to access values.
The actual value of a key could be one of many different data types:

- string
- number
- Boolean
- array
- another object

A method's value, by definition is always going to be a function.

There are a few different ways to create objects, but the most popular way is **literal notation**.
In literal notation, the object is stored in a variable, contained within curly braces.
Keys are separated from their values using colons.
Each property (and method) are separated with commas after--with the exception of the last one.
We can access the properties/methods of an object by using **dot notation** or **square brackets**.
For example:

```
let dealerName = dealer.name;
let currentStock = dealer.checkStock();

let dealerName = dealer['name'];
```

Dot notation is more common, but using brackets may be used when the property is a number (not usually recommended) or if a variable is being used in place of the property name.

### Document Object Model

The **Document Object Model** (DOM) tells browsers how they should create the model of an HTML page and how JavaScript can interact with and update the web page while it is in a browser window.
The DOM is *not* HTML or JavaScript, rather it is an additional set of rules that covers two different areas:

- The DOM creates a model of the page in memory and specifies how to structure this model using a **DOM Tree**. Each object that comprises the DOM represents a different part of the web page.
- The DOM also figures out a set of rules to update what the user sees in the model.
- The DOM is called an **Application Programming Interface (API). That is a fancy acronym for the idea that something like DOM is built to let programs and scripts interact with each other.

When visualizing the DOM Tree, you can think of it as an HTML family tree for the web page.
It begins with the 'document' and progresses down through descendants with things that are called **nodes**.
The four different nodes are:

- document node
- element node
- attribute node (these are *not* children of the element node, they are actually a part of that element--think about their nodes as going off to the side and not below as children in a family tree)
- text node

It is important to note that when a page is loaded in a browser, scripts access and update the DOM Tree, and not the source HTML file itself.
Changes made to the DOM Tree can be seen, and are reflected in, the browser.

To work with the DOM Tree, you first must locate the node you want to work with.
Then use that node's text content, child elements, and attributes.

Information taken from notes while reading *JAVASCRIPT&JQUERY* by Jon Duckett.
