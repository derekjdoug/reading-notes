[Home](README.md) > [Topic Notes](topicNotes.md)

# Operators and Loops

## Week 02 Day 02

Today we learned about comparison and assignment operators in JavaScript.
To simplify assignment operators: they assign a value to their left operand based on the value of their right operand.
For example:

- `x = f()`
- `x += f()` (meaning x = x + f())
-  So and and so forth, you can use this idea with other similiar operations

Comparison operators are just that--they seek to compare operands and return a logical value based on whether or not that comparison is true. 
The operands can be of different types, such as: numerical, strings, logical, or objects.
Usually, JavaScript will try to convert them for comparison (usually numerically).
Exceptions are `===` and `!==` operators, as they perform **strict** equality or inequality comparisons.
Basically, they operands have to match exactly, or no dice.
Examples:

- `==` returns true if operands equal
- `!=` returns true if not equal
- `===` returns true if operands are equal and same type
- `!==` returns true if operands are of same type, but not equal
- `>` returns true if left operand is greater than right operand
- You can also use example of greater than or equal to, less than, etc.

We also learned about three different JavaSCript *loops*.
Loops enable you to code a quick way to do a task repeatedly.
The three types of loops we learned are:

- for (loop repeats until a specified condition is false)
- do. . .while (statement repeats until a specified condition is false **BUT** is guaranteed to be ran at least once)
- while (executes as long as a specified condition is true)

Here are some examples from my code:

for:

```
function displayRating() {

    let output = '';
    let rating = prompt('Scale of 1-5 Olives, how happy are you with our service?');
    for(let i = 0; i < rating; i++){
        output = output + "<img class='olive' src='images/olove.png'/>";
    }
    return document.write(output);
}
```

do. . .while:
```
function guess() {
    let answer;

    do{
        answer = prompt('Guess a number between 1-5');
        if(answer != 5){
            alert('Close, but no olive! Try again!')
        } else{
            alert('That is right on the olive!');
        }
    }while(answer !=5)
}
```