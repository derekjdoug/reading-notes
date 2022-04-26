[Home](README.md) > [Code 201 Topic Notes](201topicNotes.md)

# Class 07

## Object-Oriented Programming and HTML Tables

### Domain Modeling

Domain modeling is all about creating models for a specific problem (or problem domain).
It can gives us the framework to program for certain problems that may be recurring or have many instances.
It's good practice to model attributes that are well defined and initialize properties, while also using small methods that focus on doing individual jobs well--again we should be able to use this as a template for many different, and varied, instances.
Create instances with the `new` keyword (this creates a new object that is based on the domain modeling), then a call to which ever constructor function is used to store the data.

Source: [Domain Modeling](https://github.com/codefellows/domain_modeling#domain-modeling) by Codefellows GitHub

### HTML Tables

Tables are just that . . . a table that displays information (think spreadsheet!).

- `<table></table>` creates (or contains) that table
- `<thead></thead>` creates the top row header...will be of a different style than the rest of the table within most browsers
- `<th></th>` header cells
- `<tbody></tbody>` will establish the main body of the table (the data)
- `<tr></tr>` creates a new table row
- `<td></td>` contains the data for a table cell within a table row
- `<tfooter></tfooter>` creates the footer row

CSS interaction notes:

`border-spacing:` CSS property will give space between table cells if not defined or adjusted.
`padding:` will also make cells look better. If you use *two* elements for padding (or any other CSS property that has a top, bottom, left, and right), first value sets the top and bottom, the second sets the left and right.

Table example:

```
<table>
  <thead>
    <th>Example 1</th>
    <th>Example 2</th>
    <th>Example 3</th>
  </thead>
  <tbody>
    <tr>
      <td>Data 1</td>
      <td>Data 2</td>
      <td>Data 3</td>
    </tr>
  </tbody>
</table>
```

### Functions, Methods, and Objects

- Notes incoming . . .

Information taken from notes while reading *HTML&CSS* and *JAVASCRIPT&JQUERY* by Jon Duckett.
