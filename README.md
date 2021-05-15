# Sprint Challenge - JavaScript Fundamentals

**Read these instructions carefully. Understand exactly what is expected _before_ starting this Sprint Challenge.**

This challenge allows you to practice the concepts and techniques learned over the past week and apply them in project. This Sprint explored JavaScript Fundamentals. During this Sprint, you studied array methods, this keyword, prototypes, and class syntax. In your challenge this week, you will demonstrate proficiency by completing a survey of JavaScript problems.

This is an individual assessment. All work must be your own. Your challenge score is a measure of your ability to work independently using the material covered through this sprint. You need to demonstrate proficiency in the concepts and objectives introduced and practiced in preceding days.

You are not allowed to collaborate during the sprint challenge.

_You have **three hours** to complete this challenge. Plan your time accordingly._

## Introduction

The index.js file contains all of your challenges. Please review it in full before answering the questions. If you complete the stretch goals please leave them in your file but commented out so that they do not affect the MVP tasks

In meeting the minimum viable product (MVP) specifications listed below, you should have all tests passing. You can console.log to check your work and ensure you are submitting the correct results

### Commits

Commit your code regularly and meaningfully. This helps both you (in case you ever need to return to old code for any number of reasons) and your team lead as the evaluate your solution.

## Interview Questions

### (please edit this file and write your answer below each question. In addition, you may also review these questions with your mentor)

Demonstrate your understanding of this week's concepts by answering the following free-form questions.

Edit this document to include your answers after each question. Make sure to leave a blank line above and below your answer so it is clear and easy to read.

1. Briefly compare and contrast `.forEach` & `.map` (2-3 sentences max)

   .forEach and .map both iterate through and execute a function on each item in an array by ascending index. .map requires a return statement that implicitly pushes the results of its function being executed on the original array's items to a new array. .forEach does not require a return statement, does not create a new array (without being told to do so with a push to an empty array), and the callback function within it can mutate the original array.

2. Explain the difference between a callback and a higher order function.

   A callback is a function that is used as an argument inside of another function. A higher order function is the function into which the callback is passed. The higher order function executes its operations on another function, either by using it as an argument or simply returning it.

3. Can you explain what a closure is and how you used it in the counter function?

   A closure is when a function looks outside of its lexical scope to its parent scope for a value. Using the counter function as an example, the counter variable is declared outside of the scope of the loop. Each time the loop runs it reaches outside of its scope to its parent scope to grab the value of counter, a closure. counter's value starts at 0 and is increased by 1 every time the loop runs. The loop runs, and adds 1 to the counter. Since counter is outside of the loop's scope, it is not reset every time the loop runs and is able to be updated by the loop. If it were not for this closure happening, it would be impossible for the loop to access counter AND for counter to not be reset at the start of each new loop.

4. Describe the four principles of the 'this' keyword.

   Principle 1: window/Global Object binding - when in the global scope, 'this' refer to the window/console object. Without context, 'this' binds to the window object in the browser, which is basically everything that is globally avaiilible in javascript.

   Principle 2: Implicit binding - implicit binding happens when 'this' is given context. For example, when a method is called on an object, the object becomes 'this'. In the syntax object.method(), the object preceding the dot automatically becomes what 'this' refers to.

   Principle 3: New Binding - when a constructor function is invoked to create a new instance of an object, that specific instance is what 'this' refers to. Typically in constructors 'this' is used in creating the template for the object keys. When the constructor is used to create a new object, the 'this' from the constructor is passed to that specific new object.

   Principle 4: Explicit Binding - explicit binding is used to override implicit binding using .call, .apply, or .bind. When these methods are used, 'this' is explicity defined. In an example of creating a child constructor from a parent, .call is used to bind the 'this' attributes from the parent to now apply to the child.

5. Why do we need super() in an extended class?

   super works alongside the extends keyword to do the job that .call and object.create() used to do. super takes care of binding and gives the child object access to the parent's 'this' context. Without super we wouldn't have access to the parent's 'this' context and thereby its attributes and prototype.

You are expected to be able to answer questions in these areas. Your responses contribute to your Sprint Challenge grade.

## Instructions

### Task 1: Project Set Up

Follow these steps to set up your project:

1. Fork the repo
2. Clone your forked version of the repo
3. cd into your repo and create a branch with your first and last name
   NOTE: Tests will run for the JavaScript portion of this challenge only
4. open the terminal in your vs code and type `npm install`
5. next type `npm run test:watch` in your terminal
6. Complete your work making regular commits, once you have all your tests passing and you are ready to submit your work please see canvas for instructions on how to submit

### Task 2: Project Requirements

Your finished project must include all of the following requirements

#### Task A: Closure

This challenge takes a look at closures as well as scope.

- [ ] Find this challenge in the index.js file. Read the instructions carefully!

#### Task B: Objects and Arrays

Test your knowledge of advanced array methods and callbacks.

- [ ] Find this challenge in the index.js file. Read the instructions carefully!

#### Task C: Prototypes

Create constructors, bind methods, and create cuboids in this prototypes challenge.

- [ ] Find this challenge in the index.js file. Read the instructions carefully!

#### Task D: Classes

Once you have completed the prototypes challenge, it's time to convert all your hard work into classes.

- Find this challenge in the index.js file. Read the instructions carefully!

In your solutions, it is essential that you follow best practices and produce clean and professional results. Schedule time to review, refine, and assess your work and perform basic professional polishing including spell-checking and grammar-checking on your work. It is better to submit a challenge that meets MVP than one that attempts too much and does not.

### Task 3: Stretch Goals

There are a few stretch problems found throughout the files, don't work on them until you are finished with MVP requirements! Please remember to comment out your stretch goals before you submit

## Submission format

See Canvas for submission instructions
