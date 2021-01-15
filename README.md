# Programming Foundations Lesson 2.4: Functions

## Exercise 1

Make a function, with an apropriate name, that given one parameter, console logs out the value of that parameter plus some descriptive comment. 

Invoke the function with a string as its argument.

## Exercise 2

a) Make a function, isItOdd() that given a numeric parameter, returns `true` if the number passed in is odd, and false if it's not.

b) Invoke the function with a string as its argument. Console log the result.

c) Expand the function to return NaN if the argument passed in is not a valid number.

d) Invoke the function with a string as its argument. Console log the result.

## Exercise 3

Temperatures can be given in Celsius or Farenheit, depending on where we live in the World.

Mathematically you can calculate one from the other in these ways:
```
°F = °C x 9/5 + 32

°C = °F - 32
     -------
       9/5
```
a) Make a function `toFarenheit()` that given one argument, the temperature in celsius, returns the corresponding temperature in farenheit.

Console.log out the corrsponding degrees in farenheit, for the following degrees in calsius `-40`, `0`, `37` and `100`.

b)
a) Make a function `toCelsius()` that given one argument, the temperature in farenheit, returns the corresponding temperature in celsius.

Console.log out the corrsponding degrees in celsius, for the following degrees in farenheit `-40`, `32`, `98.6` and `212`.

> Tip: Mind your parenthesis, and note that the solution to one of these can be found on [W3School](https://www.w3schools.com/js/js_functions.asp).


## Exercise 4

Given two paragraphs in your HTML, with the ids `emptyParagraph` and `anotherParagraph`:

```html
<p id="emptyParagraph"></p>
<p id="anotherParagraph"></p>
```

a) Make a function called `writeToPage()`, that takes one argument, and writes that value of the argument at text inside the `p#emptyParagraph` element.

Invoke the function with an appropriate argument.

b) Extend the function from a to take a second argument, `element`, use the value of that parameter to target any element with that name.

Invole the new/extended function, with an appropriate first argument and "anotherParagraph" as the second argument.

c) [Level 2] If the element given in b doesn't exist, make a console **error**, with the text: `"The given element, " + element + ", doesn't exist."`

Invole the new/extended function, with an appropriate first argument and "whatever" as the second argument. 

## Exercise 5

Given a button and an empty ordered list in your HTML, like this: 

```html
<button onclick="listItems()">Press Me, I dare you</button>
<ol id="myList"></ol>
```

And a list of programming languages.

```js
let programmingLanguages = [
    "Python",
    "JavaScript", 
    "Java", 
    "C#", 
    "C", 
    "C++", 
    "Go", 
    "R", 
    "Swift", 
    "PHP"
];
```

Make a function `listItems()` that sorts the list `programmingLanguages` alfabetically, and list them in individual list items in the `ol#myList` element on the page.

Press the button on the webpage to invoke the function.

> Hint: To make a list element it's sufficient here to make something like `"<li>" + value + "</li>"`;

## Exercise 6

Note: In 3a the result from toFarenheit(37), or another value, may be logged out as `98.60000000000001`. Normally we don't want that many decimal points.

a) Based on `toFarenheit()`, make a new function `toFarenheitPrecise()`, that takes two arguments, the temperature in celsius, and the precision (the numbers of decimal points), that returns a float with the required level of precision.
(Level 2: Make the default value for the precision 2)

Console.log out the corrsponding degrees in farenheit, for the following degrees in calsius `-40`, `0`, `37` and `100`.

b) Do the same based on `toCelsius()`, in a new `toCelsiusPrecise()` function.

Console.log out the corrsponding degrees in celsius, for the following degrees in farenheit `-40`, `32`, `98.6` and `212`.

> Tip: Use [Number.toFixed()](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number/toFixed)