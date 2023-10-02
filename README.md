# arrow-functions

## ES6 Arrow Functions

This assignment is designed to introduce you to some features in ECMAScript 2015, otherwise known as ES6. From this point on, you are expected to use these features.

## Overview: Arrow Functions

By now you should be comfortable writing function expressions and function declarations.
 Arrow functions are a shorter, more concise way to write a JavaScript 
function. The syntax might seem strange at first, so try to use arrow 
functions wherever you can and they will become second nature in no 
time.

There are a few caveats with arrow functions, though. Most importantly, the this context is not reset within an arrow function. The value of this is therefore the same as the this of the enclosing scope (the surrounding non-arrow function). If there isn’t a non-arrow function scope surrounding, the this context will be, in the browser, the global window object.

Why does this happen? It happens because arrow functions retain the this
 value of the enclosing functional scope. Therefore, you will want to 
avoid using an arrow function in a constructor (where we need the 
contextual this to be the object we are building) or any method that needs to use this to behave properly.

## Assignment Tasks

Create a new repo in your GitHub account called arrow-functions. Clone the empty repo to your dev environment.
Download and unzip the starter code onto your computer.
Once you have unzipped the file, copy the contents of the folder named starter-code into your newly-created repo. Make an initial commit with the unchanged starter code.
Proceed to work on a well-named branch. As you work, remember to add, commit, and push regularly.
The app.js
 file contains examples of function expressions, as you are accustomed 
to seeing. Work through steps 1-9, reading the notes and reviewing the 
refactored samples.
For each of these steps, uncomment the console.log line. Open the index.html file in the browser and verify the correct output in the developer console.
To complete step 10, refactor the function expressions one at a 
time. Uncomment the console.log line and use it to check that the output
 is the same after you have completed the refactoring process.
To complete step 11, uncomment the two console.log lines and 
observe the output in the developer console in the browser. Answer the 
corresponding questions.

 1. What is "this" when joe.scope() is invoked?
"this" within the scope function appears be a reference pointing to the joe object
 2. What is "this" when joe.scopeArrow() is invoked?
This refers to the parent which in this case is the global parent which is the browser window.
 3. Explain why "this" is different when an arrow function is used.
The value of this inside an arrow function is determined by where the arrow function is written, it  retains the this value from its parent.
