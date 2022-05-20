[Home](../README.md) > [Code 201 Topic Notes](../201topicNotes.md)

# Class 14

## CSS Transforms, Transitions, and Animations

### CSS Transforms

Transforms were introduced with CSS3 as new ways to position and affect images.
You can you use the **transform propery** in two different settings: 2D (on the x and y axes) and 3D (on the x, y, and z axes).
Important to note: browser support for `transform` is currently not great, you may need to use a nightly build of Chrome to implement.

For 2D, here are some of the values you can use with the transform property:

- `transform: rotate(10deg);`
- `transform: rotate(-10deg);`
- `transform: scale(.5);` (make smaller)
- `transform: scale(1.5);` (make bigger)
- `transform: scale(.5, 1.5);` (x axis, y axis)
- `transform: translateX(-10px);` (move to the left from original position)
- `transform: translateY(50%);` (move down by 50%)
- `transform: translate(-10px, 50%);` (affect both)
- `transform: skew(5deg,-5deg);` (distorts elements on both axes)
- `transform-origin:` (default is the center of an element, with this we can set where we want the transform of an element to originate from)
- There is also the *perspective* value, which can be thought of as a vanishing point for each.

For 3D transforms, we want to specify values not only for the x and y axes, but also for the z as well.
You can also combine transforms to make shapes; for example, a cube!

Source:[Shay Howe, Transforms](https://learn.shayhowe.com/advanced-html-css/css-transforms/)

### CSS Transitions and Animations

Transitions and animations allow front end developers to alter element and appearance and behavior without having to use JavaScript or Flash.

For a **transition** to take place, an element must have a change of state, and different styles must be identified for those states.
These pseudo-classes can be used to do so:

- `:hover`
- `:focus`
- `:active`
- `:target`

There are four different transition related properties:

1. `transition-property:` (determines what properties will actually be altered; multiple can be separated by a comma)
2. `transition-duration:` (the duration of the transition, either in seconds or milliseconds; commas can be used to separate different duration times for different properties, but their order must match what is used in the transition-property value)
3. `transition-timing-function:` (sets the speed with which a transition will *move*)
4. `transition-delay:` (how long to stall a transition before executing)

Not all properties can be transitioned, *only properties that have an identifiable midway point can be . . . like colors, font sizes, etc.

You can use shorthand by writing: `transition: transition-property, transition-duration, transition-function-timing, and transition-delay` in that order.

**Animations** are used where more control is required, and when transitions need to have multiple states.
Using the *keyframe rule*, you can set multiple points at which an element should undergo a transition.
The *animation name* is how we can assign a keyframe to an element.
You can then use *animation duration, timing function, and delay* just as you would with the transition property.
You can further customize animations with *animation direction, play state, and fill mode*.

Source: [Shay Howe, Transitions & Animations](https://learn.shayhowe.com/advanced-html-css/transitions-animations/)

8 very simple and popular CSS transitions are covered at: [Web Designer Depot](https://www.webdesignerdepot.com/2014/05/8-simple-css3-transitions-that-will-wow-your-users)

Included is the ability to: fade in an element, change color, grow or shrink, rotate elements, change shape from square to circle, create a 3D shadow, swing (shake) an element, and to create an inset border.

[6 Buttons Animated](https://codepen.io/retyui/pen/ByoaXV) has some code examples for animating buttons.

[akshaychauhan](https://codepen.io/akshaychauhan/pen/dyBqVo) includes a great example of code for CSS3 keyframes animation.

[kieranfivestars](https://codepen.io/kieranfivestars/pen/MYdQxX) has an example of '404' being animated.

[dp_lewis](https://codepen.io/dp_lewis/pen/QWMxRR) has a code example of a bouncing ball animation.

### What Google Learned . . .

In 2012, Google started an iniative, called **Project Aristotle** to study Google's team and understand why some of them were very effective, and some were not.
In the beginning, Project Aristotle struggled to find any patterns at all.
Groups that were comprimised seemingly the same had differing levels of success.
What Google ultimately settled on investigating further was *group norms*, basically what rules (spoken or unspoken) did groups reinforce and follow.
On good teams, it was found that members all spoke in relatively equal proportion and that the members tended to have high "average social sensitivity".
This was explored further by Harvard Business School professor Amy Edmondson as being aspects of what's known as *pyschological safety*.
She specifically defines it as being: a "shared belief held by members of a team that the team is safe for interpersonal risk-taking."
Google identified this as being a safe work space where people feel empowered to take risks as needed.

Source: [NY Times](https://www.nytimes.com/2016/02/28/magazine/what-google-learned-from-its-quest-to-build-the-perfect-team.html)
