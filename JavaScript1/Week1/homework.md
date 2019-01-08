# Homework week 1

![Hacking](https://media.giphy.com/media/eCqFYAVjjDksg/giphy.gif)
## Step 1: Before you start with the homework:
1. Watch: [What is programming](https://www.khanacademy.org/computing/computer-programming/programming/intro-to-programming/v/programming-intro) Just watch the 2 min video, you do not have to do the entire JavaScript course (It could be useful later on though). 

## Why should i do this homework?


## Step 2: Javascript warm up part one
Lets get started with some warm up exercises: On freeCodeCamp.com please do the [Basic JavaScript](https://learn.freecodecamp.org/javascript-algorithms-and-data-structures/basic-javascript) exercises up and until the **"Shopping List"** exercise (there are some topics we did not cover but you can do it).

Please add your freecodecamp username as answer for this exercise!

## Step 3: Javascript warm up part two
1. Write a `console.log` statement saying "Hello World!" for each language that you know.

For example:
```
Halo, dunia! // Indonesian
Ciao, mondo! // Italian
Hola, mundo! // Spanish
```

2. Create a variable that rounds the number 7.25, to the nearest integer (i.e., whole number)  

3. Working with arrays
* Declare an empty array. Make sure that the name you choose indicates 'plurality', because an array is capable of containing more than one element. (See [Naming conventions](https://github.com/HackYourFuture/fundamentals/blob/master/fundamentals/naming_conventions.md)).  
* Write a `console.log` statement that explains in words what you think the value of the array is.  
* `console.log` your array.  
* Create an array that has your favorite animals inside (see if you can find a good name that exactly describes what this variable will hold).  
* Log your array.  

4. Working with strings

Checkout [this article](https://www.digitalocean.com/community/tutorials/how-to-index-split-and-manipulate-strings-in-javascript) for help with working with strings
Let's consider the following string: `const testString = "this is a test"`.
  * Find a way to get the length of `testString`.  
  * `console.log` the length of `testString`.  
  * `console.log` the last character in the string using character indexes

5. Working with variable types
* First declare at least four variables and assign them different variable types.  
* For each variable write a `console.log` statement that logs the value
  ```js
  let foo = 3;
  console.log('The value of my variable foo is: ' + foo);
  ```

6. Working with typeof
* Now write a `console.log` statement wherein you first explain in words what you think the _type_ of your variables is.  
* Now use `typeof` to log the actual _type_ of your variables.  

---

You have finished the warmup exercises, well done!

## Step 4: Smart-ease - We help where we can
Enough warm up, lets get to the real problems! We will assume a real world business case where you (the developer) needs to help a business that is starting up (a startup) with solving some of their problems related to JavaScript! Here we go:

---

Lets imagine that we have just started a cool new tech startup called **Smart-ease**. And lets imagine we even have this cool website url: [smart-ease.io](smart-ease.io) Now we are in business!

At **Smart-ease** we focus on solving real world problems. We venture into the world to help people, and by helping people, we create a sustainable business.

Cool now lets venture into the world and see which problems we can solve:

![Adventure](https://media.giphy.com/media/oj2GhTqAIoNIk/giphy.gif)

### Age-ify (A future age calculator)
> You are talking to a friend who suddently looks at you and asks: "How old will you be in 2045?" Hmm you remember the year you were born and try to do some calculation: Born in 1987 + 3 that's 1990. 90 - 40 is 50 + 5 thats 58. I will be 58! Wow that was painful! Let's fix that by making some code that automatically does this!

Create two variables called yearOfBirth and yearFuture. Assign these your own age and a futureYear.
What type will these two variables be? Now calculate the age and store that in a variable called age. Log out this string:
"You will be 40 years old in 2027". With 40 being the result of the age variable and 2027 being the yearFuture variable. (Hint use string concatenation)

### Goodboy-Oldboy (A dog age calculator)
> The same friend (who by the way loves dogs) asks how old his dog will be in 2045. Hmm you think, lets make this into a product as well!
Dogs age can either be measured in dog years or in human years, this we want to take into consideration! 

Like before lets create three variables but this time we call them dogYearOfBirth, dogYearFuture and dogYear. We add an extra variable called shouldShowResultInDogYears. If it is true we should show the result in dog years, if it is false we should show it in human years. What do we call this type of variable? Now log this string out:
"Your dog will be 10 human years old in 2027"
or 
"Your dog will be 70 dog years old in 2027"

### Housey pricey (A house price estimator)
> Two of your friends are considering buying a house, but cannot figure out what the right price should be. Your friends know the width, the height and the depth of the house and the garden size. Lets help them figure out if they paid too much:

We have made our own formula for calculating the price of a house. This formula is VERY simplified and not at all close to the real calculation which can get [quite complicated](https://www.kaggle.com/erick5/predicting-house-prices-with-machine-learning):
```js
housePrice = volumeInMeters * 2.5 * 1000 + gardenSizeInM2 * 300
```

Your friend Peter is considering a house that is 8m wide, 10m deep and 10m high. The garden size is 100m2. The house costs 2.500.000.
Your friend Julia is considering a house that is 5m wide, 11m deep and 8m high. The garden size is 70m2. This house costs 1.000.000.

Figure out if Peter and Julia are paying too much or too little using javascript and the formula specified above.

### Ez Namey (Startup name generator) (Optional)
> At a meetup you overhear a conversation between two developers. It went something like this: "Man i wish picking a startup name was easier! You need to be creative, funny and interesting, its nearly impossible!" Another problem to solve, awesome!

Lets help people who struggle finding a startup name by creating some code!

Create two arrays called firstWords, secondWords. The arrays should have 10 elements containing strings of possible startup names. Some examples could be: "Easy", "Awesome", "Corporate".
Create a variable called startupName that will contain created startup name.  
Using a random index (you choose) of the arrays and concatenation of strings, create and log the new startup name and the number of characters in it. 
An example could be: "The startup: "Easy Corporation" contains 16 characters"

Hint: you can use this code to generate a random number from 0-9, if you dont want to specify the indexes yourself.
```js
const randomNumber = Math.floor(Math.random() * 10) + 0
```
---

4 projects from one startup, thats incredible! Lets hope one or more of these projects actually becomes popular!

To be continued...


## Step 5: Hand in Homework:

Steps:
* Use the hyf-homework repo and add your homework files in the javascript/javascript1/week1 folder
* If you dont have the repo, fork it from here: https://github.com/HackYourFuture-CPH/hyf-homework
* Make your commits for the homework. Remember to seperate the code into meaningful commits!
* Push the changes to github
* To finish the homework:
  * Fill in the form for the relevant week. The link to the form can be found at the top of your classes slack channel. 
  * Share the github link to your classes slack channel. 

---

And thats it your are done 🎉
