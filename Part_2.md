# Hack School: Part 2 - Javascript/Node.js (10/22)

Workshop Recording: (__insert-link-here__)

In this workshop, we learned about Javascript and Node.js. Specifically, we learned about **variables**, **loops**, **arrow functions**, and **promises**.


We used these ideas to:
- [x] Create pokemon
- [x] Create attack functions
- [x] Determine how much damage each attack does



## What is JavaScript and NodeJS?

JavaScript is a scripting language (meaning: it has its own terminology, etc.). It is used to make applications dynamic and interactive.

Node.js is an environment that sits in between a server and the client-side (what you see). It allows an application to process JavaScript commands asynchronously (through asynchronous programming).

In Hack School, we will be using JavaScript and Node.js to make our Pokemon game move/change. JavaScript and Node.js handles every dialogue box, every change in HP, every user command, etc., and updates accordingly.



### Variables

Variables are objects that store information in variable names.

In JavaScript, you can assign variable names in several different ways:

#### `let`

`let` is a command that is **block scoped**. A block is a chunk of code bounded by curly braces {}.

This means that `let` defines variables within the scope of a block (or outside of the block):

```
let apple = 6

if (1 < 2) {
  let apple = 10 \\ This will create a "new" variable `apple` inside the block.
  console.log(apple) \\ This will return 10.
}

console.log(apple) \\ Since apple outside of the block is defined as 6, this will return 6
```
Note that the second console.log returned 6. JavaScript considers  `apple` outside of the block to be an entirely different variable than `apple` inside the block, because inside of the block is a new scope.


`let` variables can also be re-assigned. However, they cannot be re-declared:
```
let apple = 6
apple = 7
```
This is re-assigning the variable apple to the number 7. JavaScript realizes that the previously-defined variable  `apple` is being updated. This is okay!

```
let apple = 6
let apple = 7
```
This is re-declaring the variable apple. The use of `let` makes JavaScript expects `apple` to be a new variable. Since it's not, JavaScript will throw an error.

#### `const`

`const` is also a command that is block scoped. However, it cannot be re-assigned or re-declared.

This means that:
```
let apple = 6
apple = 7
```
will return an error, because re-assignemnt is not allowed.

This also means that:
```
let apple = 6
let apple = 7
```
will return an error, becuase re-declaration is not allowed.


### Main Idea 2

Main Idea 1 is (explanation).

Some examples of Main Idea 1 are:

#### `(Code Command #1)`

`Code Command #1` is a (insert descriptor here). It takes (input) and (does output).

```
example code here
```

### Main Idea 3

Main Idea 1 is (explanation).

Some examples of Main Idea 1 are:

#### `(Code Command #1)`

`Code Command #1` is a (insert descriptor here). It takes (input) and (does output).

```
example code here
```

## Project Implementation

### Task 1

We want to do (insert task here) for our Pokemon generator.

For that, we use **main idea 1** and **main idea 2**.

```
example code here
```

## Simple Resources:

**Main Idea 1**:

Site #1: (link)

Site #2: (link)
