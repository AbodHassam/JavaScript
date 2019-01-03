# Homework Week 8

## Why should i even do this homework?
Promises creates a **pleasant way of working with asynchronous code**. It will make your asynchronous code nearly look synchronous. It is possible to compose promises further developing the function part of javascript. 

Since promises is becoming standard in javascript, new browser api's use promises for interacting with them. getUserMedia for accessing webcam, Navigator.getBattery() for getting battery level, Bluetooth.requestDevice(), serviceWorker or USB.requestDevice(). 

So lets learn some promises :)

## Exercises with promises
### Create promise that resolves after set time
Create a function that has one parameter: SecondsToResolve. **Calling this function** will **return a promise** that resolves after the millisecondsToResolve. 

Here is an example: `getPromise(3000)` will return a promise that resolves after 3 seconds.

Use the `getPromise` to log out the string `I am called asynchronously` after 6 seconde.

### Transforming div
Create a div that has a transition on 3 seconds on the `tranform` attribute (in css). 
If we now manually in the devtools change the `transform` to `translateX(1000px)` we will see the div move 1000 pixels to the right. Lets create that functionality when clicking on the div. So a user clicks the div and it slides to the right. Cool. 

Now what if we after the div had slided out wanted to create some functionality. That could fx be slide another div to the right. Lets use promises for that and lets use the function we already created! When a user clicks the div, lets call the `getPromise(3000)` assign the return (which is a promise) that to a variable. In the resolve of that promise we want to log out the following: "Div has slided to the right!". 

So what we as developers see is we click a div. It slides 1000px to the right and then exactly when it is done, we log out the text "Div has slided to the right!".

#### Optional part
- What if we changed the transition of the div in css. Now they are going to be out of sync. How can we fix this problem?
- After we have slided the first div to the right. Lets slide a new div to the right using promises and cahining.

### Fetch promise exercise
Only using promises
1. Fetch some data from an api.
1. Wait 3 seconds
1. Log out the data from the api

#### Optional part
Use promise chaining

## Feedback giving time!
Find a student to give feedback using this site: https://hyf-peer-review.herokuapp.com/
The feedback should be given after the homework has been handed in preferably latest two days after.
 
To help you get started we have created some ressources about giving feedback. Find them here: https://github.com/HackYourFuture-CPH/curriculum/tree/master/review

## Hand in Homework:
Go over your homework one last time:

- Does every file run without errors and with the correct results?
- Have you used `const` and `let` and avoided `var`?
- Do the variable, function and argument names you created follow the [Naming Conventions](https://github.com/HackYourFuture/fundamentals/blob/master/fundamentals/naming_conventions.md)?
- Is your code well-formatted (see [Code Formatting](https://github.com/HackYourFuture/fundamentals/blob/master/fundamentals/naming_conventions.md))?  
![](https://media.giphy.com/media/l4EpblDY4msVtKAOk/giphy.gif)  
If you can answer yes to the above questions then you are ready to hand in the homework:<br/>
- Find the hyf-homework git repo (that you have forked from [here](https://github.com/HackYourFuture-CPH/hyf-homework)) the link will be https://github.com/YOUR-ACCOUNT/hyf-homework
- Add your homework files in the Javascript/javascript3/week7 folder
- To finish the homework post the link for your repo and the rendered index.html on your classes slack channel
---

🎉