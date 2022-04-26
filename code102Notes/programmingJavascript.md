[Home](README.md) > [Code 102 Topic Notes](102topicNotes.md)

# Programming With JavaScript

## Week 02 Day 01

Today we dive another few feet down the 'well' of JavaScript.
To begin, I'm going to define some important points we went over during the lesson:

- `'use strict'` should be at the top of every JS file. This will make sure everything behaves as it should
- `Let blank =` or `var blank =` define variables (variable declaration)
- On that note, you must define variables *before* using them in a function
- `||` means 'or', meaning only one of the conditions has to be true
- `&&` means 'and', meaning both or all conditions have to be true
- `==` is a comparison operator, it loosely means 'equal to'...it will convert strings to numbers
- `===` is a strict equal to. Will not convert string to number
- You must declare functions and invoke them
- Functions are invoked with () and will not run until called
- When JavaScript reaches a 'return' statement, it will stop executing

Most of our lesson was based around the importance of functions in JavaScript.
Bottom line: functions are pretty dope!
They let us reuse code. You define it once, and you're able to reuse it many times within a webpage.
You can also use the same code with different arguments to get different results.
Here's an example of a function used in my code:

```
function userName(){
let name = prompt('What is your name?');
console.log('Hello, ' + name);
return name;
}
```

More to come later.