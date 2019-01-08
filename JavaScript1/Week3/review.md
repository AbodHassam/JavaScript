# REVIEW JavaScript week 3

## Objects

Variables that are objects also contain a list of things, but instead of them being in some specific order, they can be assigned to words, called "keys". Instead of "elements" the things that are inside objects are called "properties".


```js
let obj = {name: 'John', age: 24};
```

This object has two properties: `name` and `age`. The "value" of the property `name` is the string `'John'`. The "value" of the property `age` is the number `24`.

When accessing object properties, you can use the dot-notation: `obj.name` or the bracket-notation: `obj["name"]`. Note that the latter looks a lot like the way to access array elements. However, here what's inside the bracket (called "key" for objects, instead of "index") must be a string.

```js
console.log(obj.name); // -> 'John'
console.log(obj['name']); // -> 'John'
```

Just like with arrays, you can also use a variable to access properties, as long as these variables are strings. In this case you cannot use the dot-notation!

```js
var ageKey = 'age';
console.log(obj[ageKey]); // -> 24
```

Remember that there is a very big difference between `obj[name]` and `obj["name"]`.

> Note:
>
> Thinking back of arrays, the length of an array can be retrieved by `arr.length`. So as mentioned before, arrays are just like other JavaScript objects. You could even write `arr['length']` to access the `length` property of the array. JavaScript will look: is what we put between brackets a number? Then it is an index and we'll look up the correct array element. If it's a string, it's a key and we will look up the corresponding property.



## Functions
```js
console.log("script loaded");

function cakeLogger(numberOfCakes) {
    return 'Delicious cake!';
}

const cakeStringResult = cakeLogger();



const cakeLoggerConst = function(numberOfCakes) {
    return 'Delicious cake!';
}

//console.log(cakeLoggerConst());



function testFunctionA(functionToCall, numberOfCakes) {
    //console.log(functionToCall);
    const cakeString = functionToCall(numberOfCakes);
    testFunctionB(functionToCall, numberOfCakes);

    return cakeString;
}


function testFunctionB(functionToCall2, numberOfCakes2) {
    functionToCall2(numberOfCakes2);
}

// testFunctionA(cakeLoggerConst, 2);

const test = function() {
    return "test";
}

//console.log(test());

/*context execution */



function a() {
    // add to call stack
    b();

    return 'a';
    // remove from call stack
}


function b() {
    //throw 'hello';
    return 'b';
}

a();


// http://latentflip.com/loupe

function pickUpKids() {
   
}

function buyCarrots() {
    console.log('I am buying carrots');
}

function buyVegetables() {
    buyCarrots();
}

function getGroceries() {
    buyVegetables();
}

function doWork() {
    
}

pickUpKids();
getGroceries();
doWork();
```

## HTML interaction

Interacting with the HTML DOM is done through the document object in the browser. With the document object we can get html elements and change them.


For the next js part we use this html.

```html
<html>
    <body>
        <h1>
            Javascript week 3
        </h1>
        <div class="queue"></div>
        <div id="test-id"></div>
        <script src="js/review.js"></script>
    </body>
</html>
```


```js
// use the querySelector to select elements just like in css
const testIdElement = document.querySelector('#test-id');
console.log(testIdElement); // logs the html element with id "test-id"

// Change the inner html of the test-id element
testIdElement.innerHTML = 'test';
// Change the background-color of the test-id element. Inline css changes is done via the style attribute on the element
testIdElement.style.backgroundColor = 'blue';


// It is also possible to create html elements
// Create a div element
const div = document.createElement('div');
// Change its inner html
div.innerHTML = 'We created this div!!!';

// Lest append it to the div with the class queue
const queueDiv = document.querySelector('.queue');
queueDiv.appendChild(div);
```



## Code Commenting
First the straightforward part: how do we place comments in our code?

### JavaScript
Single line comments
```js
// Change heading:
document.getElementById("myH").innerHTML = "My First Page";
```

Single line comments at end of the line:
```js
const x = 5;      // Declare x, give it the value of 5
```

Coding **well** in JavaScript: [JSDoc](http://usejsdoc.org/)

### HTML
[W3Schools](https://www.w3schools.com/html/html_comments.asp)
Comments
```html
<!-- Write 
your comments here -->

<!-- Write your comments here -->
```


### CSS
[MDN on CSS comments](https://developer.mozilla.org/en-US/docs/Web/CSS/Comments)
```css
/* Comment */

/*
A comment
which stretches
over several
lines
*/
```

### When to comment?
Now for the hard part: when to comment? When you work for different companies, you will see different styles. Embrace something you like, and then learn to let go. Google on "when to comment code?" and you'll find a big bunch of different opinions. 

The general concept is, however, that it is there to help make the code more easy to understand. Note, however, that comments can also make code more difficult to understand when not applied properly. 









