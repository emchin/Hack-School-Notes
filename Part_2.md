# Hack School: Part 2 - Javascript/Node.js (10/22)

Workshop Recording: (__insert-link-here__)

REPL Link: (__insert-link-here__)

In this workshop, we learned about Javascript and Node.js. Specifically, we learned about **variables**, **objects**, **arrow functions**, and **promises**.


We used these ideas to:
- [x] Create pokemon
- [x] Create attack functions
- [x] Determine how much damage each attack does



## What is JavaScript and Node.js?

JavaScript is a scripting language (meaning: it has its own terminology, etc.). It is used to make applications dynamic and interactive.

If you remember the house metaphor from Part 1, you can say that JavaScript is like the electricity in the house: it allows for light, running water, A/C, heat, dishwashers, etc.

Node.js is an environment that sits in between a server (the computer) and the client-side (what you see). It allows an application to process JavaScript commands asynchronously (through asynchronous programming).

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

`const` is also a command that is **block scoped**. 

However, *unlike* the `let` command, `const` CANNOT re-assign OR re-declare variables.

This means that:
```
let apple = 6
apple = 7
```
will return an error, because re-assigned is not allowed.

This also means that:
```
let apple = 6
let apple = 7
```
will return an error, becuase re-declaration is not allowed.

#### `var`

DON'T USE `var`.

(Basically, `var` is the command that JavaScript used to define variables pre-ES6 (before JavaScript was standardized). The problem is, `var` is not block scoped; it's globally or locally-scoped.

That means if a `var` variable was defined outside of a block, it is considered globally scoped, and can be used anywhere.

But if a `var` variable was defined INSIDE a block, it is considered locally-scoped, and only accessible in the scope of that block.

`var` variables can also be re-assigned AND re-declared, either inside or outside of a block.

Long story short?

For your sanity and ours...

PLEASE. DON'T. USE. `var`.)


### Objects

Everything in JavaScript is an object. It's like the cake thing on TikTok (rip TikTok).

In our project, though, one important object is our pokemon!

Let's take a look at our Pikachu example from the slides:

```
let Pikachu = {
	name : 'pika',
	type : 'electric',
	power : 50,
hp : 150,
	attacks :  ['Thunder Shock','Tail Whip','Spark'],
	attack : function (attacker) {
		return (attacker.hp - this.power);
	}
};
```

In this code, we use `let` to define an object with variable name Pikachu. 

That object, Pikachu, has **properties**. Properties are characteristics of an object. These properties can be accessed with `.property` For example, printing `Pikachu.power` would return `50`.

Objects can also have **methods**. Methods are functions that an object can execute. These methods can be accessed with `.method_name()`. For example, `Pikachu.attack()` would cause the Pikachu to attack.

Methods often use `this` to call an object's own properties in its method. For example, Pikachu's "attack" method calls for `this.power`.

<img src="https://img00.deviantart.net/6b98/i/2011/166/1/1/pikachu_thunderbolt_by_ajl03-d3izb66.png" alt="Pikachu using Thunderbolt!">


### Callback and Higher-Order Functions

Functions are considered objects in JavaScript. 

A callback function is a function that is passed as an object for another function (which is called the higher-order function).

For example:

```
function multNum (num1, num2, pokemon, callback) {
console.log('your pokemon will heal ' + (num1 * num2) + ' hp');
	callback(pokemon, num1 * num2);
}
```

This is a higher-order function `multNum` that asks a general callback function `callback` to do something with `(pokemon, num1*num2)`.

Later, we pass `heal` as the callback function:

```
multNum (5, 6, pikachu, heal);
```

As you can see, in this instance, the higher-order function `MultNum` takes the callback function `heal` as a callback function.


## Project Implementation

### Task 1

We want to do (insert task here) for our Pokemon generator.

For that, we use **main idea 1** and **main idea 2**.

```
example code here
```

<details> 
  <summary> Hint 1: Where to begin? </summary>
	Start with this: <code>this code here</code>
</details>

## Simple Resources:

<img src="https://external-content.duckduckgo.com/iu/?u=https%3A%2F%2Fi.ytimg.com%2Fvi%2FggUcrIWgKNI%2Fmaxresdefault.jpg&f=1&nofb=1" alt="brock-crying" height=50% width=50%>

We've all learned JavaScript. We've all been there. If any of you are feeling like Brock right now, please go find a mentor for help.

About `let`, `var` and `const`: [freecodecamp article](https://www.freecodecamp.org/news/var-let-and-const-whats-the-difference/)

JavaScript object properties: [W3Schools article](https://www.w3schools.com/js/js_object_properties.asp)

About `this` and a how-to on arrow functions: [W3Schools article](https://www.w3schools.com/Js/js_arrow_function.asp)

JavaScript promises: [Mozilla article](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Using_promises)
