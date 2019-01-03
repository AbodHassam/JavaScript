# Homework Week 7

## Why should i even do this homework?
Working with json and api's is the way modern **javascript application's communicate with servers**. That can be either getting some data but also updating or creating new data. 

It is how autocomplete can receive suggestions for a search query and how infinite scroll can keep loading new posts. 

## Create your own json file
Create your own json file with something that **interests you**. Maybe that could be computers, pets, music etc.

Remember to validat the json using a tool like fx this: https://jsonlint.com/

## Github data fetching site

Make a website that fetches (= to get) data asynchronously.

1) Create a new website with external js file

2) Add a button (e.g. 'click me') that when clicked `console.logs` 'you clicked me!'

3) Create a function that fetches repositories from https://api.github.com/orgs/HackYourFuture-CPH/repos) using the fetch api. 

4) Display the data that you get from the Github API on your web page. That could fx be the **repo title, the url, when it was created etc.**

5) Now link the two together: When you click the button -> get the data from the Github API and display it on your website

6) Make all the repositories link their own page in Github. Use the value of the key: `name` to make this work (hint: Github urls always look like this https://api.github.com/repos/HackYourFuture-CPH/[repositoryName] where [repositoryName] would be replaced by the actual `name` of the repository, for example `CommandLine`). Make sure the link opens in a new tab.

- Add map, filter to your existing app to build an application that loads data from github, filters out based on a certain value. Fx you could filter based on something a user wrote in an input field. 

- Add a readme to your repo explaining  what your app does and how to use your app. Here's a [template](https://gist.github.com/jxson/1784669) and here you can see how to make [your readme awesome](https://gist.github.com/rrgayhart/91bba7bb39ea60136e5c).

## Find a cool api
Find a cool api and **explain how it works** and what kind of **json data** the api responds with. Is it an array, an object, a string. How is the data structure. Is it fx an array of objects or how is it structured. 

There are a few examples of apis here:
https://github.com/HackYourFuture/teaching_tips_tricks#javascript-apis

## Giphy api
Create a site where a **user can search for any word**. When searching a word the application will **find a gif** using the **searched word** using the giphy api: https://developers.giphy.com/docs/
Here is how it is going to work: The user can write some text indicating the gif he is looking for, click a button and then a gif will be found (using the searched word) and the gif will be displayed to the user. 

Try break this problem into **smaller problems** and write down how you are going to solve the problem **BEFORE you start coding.** 

![Coding](https://media.giphy.com/media/1C8bHHJturSx2/giphy.gif)

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
