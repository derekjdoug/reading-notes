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
