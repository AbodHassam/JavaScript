# Homework Week 8

## Exercises with promises
### Create promise that resolves after set time
Create a function that has one parameter: SecondsToResolve. Calling this function will return a promise that resolves after the millisecondsToResolve. Calling this `getPromise(3000)` will return a promise that resolves after 3 seconds.

### Transforming div
Create a div that has a transition on 3 seconds on the `tranform` attribute (in css). 
If we now manually in the devtools change the `transform` to `translateX(1000px)` we will see the div move 1000px to the right. Lets create that functionality when clicking on the div. So a user clicks the div and it slides to the right. Cool. 

Now what if we after the div had slided out wanted to create some functionality. That could fx be slide another div to the right. Lets use promises for that and lets use the function we already created! When a user clicks the div, lets call the `getPromise(3000)` assign the return (which is a promise) that to a variable. In the resolve of that promise we want to log out the following: "Div has slided to the right!". 

So what we as developers see is we click a div. It slides 1000px to the right and then exactly when it is done, we log out the text "Div has slided to the right!".

#### Optional part
- What if we changed the transition of the div in css. Now they are going to be out of sync. How can we fix this problem?
- After we have slided the first div to the right. Lets slide a new div to the right using promises and cahining.

### Fetch promise exercise
ONLY USING PROMISES
1. Fetch some data from an api.
1. Wait 3 seconds
1. Log out the data from the api

#### Optional part
Use only chaining

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

If you can answer yes to the above questions then you are ready to hand in the homework:
* Find the hyf-homework git repo (that you have forked from [here](https://github.com/HackYourFuture-CPH/hyf-homework)) the link will be https://github.com/YOUR-ACCOUNT/hyf-homework
* Add your homework files in the Javascript/javascript3/week8 folder
* To finish the homework post the link for your repo and the rendered index.html on your classes slack channel