[Home](../README.md) > [Code 201 Topic Notes](../201topicNotes.md)

# Class 10

## Debugging

### Error Handling & Debugging

In finding the source of an error in JavaScript, understanding how scripts are processed--and the order in which they are processed--is important.
The order in which code is written, may not be the order in which it is run.

**Execution context** is also critical in writing code.
To put this very simply, some code is *global context* and some is *function context*.
Global code is written in the script, but not within a function (and function context is code more specifically written within a function).
Variable scope is much the same with *global scope* and *function-level scope*.
Global variables can be used anywhere in a script because they are declared outside of a function--in fact, you could pull a global variable in multiple functions if you wanted to.
Function-level variables can only be used within that function.

JavaScript interpreters only process one line of code at a time.
That means that if a *statement* needs data from another function, the new function is piled on top of the current processing **stack**.
Depending on the complexity of the code, this means that many additional functions could be added to the stack to complete the task that was asked of the JavaScript to complete.

Before any code is actually *run*, there are two phases of activity that happen for a script:

1. Preparation: A run through of the code...variables, functions, and arguments are created/noted
2. Execute: values are assigned to variables, reference functions/run their code, and statement execution

What this means is that you can call functions before they are actually declared.
This idea is called **hoisting**, because those prepatory steps get hoisted to the top of the execution context.

Functions in JavaScript are considered to have **lexical scope**, meaning that they are directly linked to the object they are defined within.
For example, their scope is their own *and their parent's execution context*.
Jon Duckett uses a great example of imagining this idea as a nesting doll.
It is critical to note that while a child can borrow from their parent's scope, it does not work the other way around, and pulling to many variable up the chain of execution can negatively impact performance.

When errors happen in JavaScript, they throw an **exception**.
To keep this short and sweet, the interpreter *knows* that there is a problem with the code and stops executing it.
It then looks for exception-handling code to resolve the issue.
If none is available in the current context, it will proceed up the chain all the way to the global-scope level.
If there is still no error handler, the script will stop running and an **Error object** will be created.'

Error objects contain the following properties:

- name of the type of execution
- a description
- JavaScript filename
- Line number of the error

Additonally, there are seven more specific built-in error objects in JavaScript that help futher define what the issue is.
I will not list them here, but they can be found starting on page 459.

The rest of the chapter gives a walkthrough of how to deal with errors yourself, including how to use built in browser and developer tools.
I will reference those pages when I run into my next (inevitable) issue!

Information taken from notes while reading *JAVASCRIPT&JQUERY* by Jon Duckett.
