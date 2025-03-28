# Interview Preparation


- [REACT](#react)
- [JAVASCRIPT](#javascript)
- [HTML-CSS](#html-css)

# React

1.  [what is react?](#what-is-react)
2.  [why use React?](#why-use-react)
3.  [Virtual DOM & Real DOM?](#virtual-dom--real-dom)
4.  [Props](#props)
5.  [state](#state)
6.  [JSX what it is and how it works]()

- Hooks

7.  [useState()](#usestate)
8.  [useEffect()](#useeffect)
9.  [useCallback()]()
10. [useReducer()](#usereducer)
11. [useRef()](#useref)
12. [useMemo()](#usememo)
13. [useLayoutEffect()](#uselayouteffect)
14. [use()]()
15. []()

# Javascript

1. [What are the differences between var, let, and const?](#what-are-the-differences-between-var-let-and-const)
2. [What is the difference between == and ===?](#what-is-the-difference-between--and-)
3. [Explain the difference between null and undefined.](#explain-the-difference-between-null-and-undefined)
4. [What are JavaScript data types?](#what-are-javascript-data-types)
5. [What is the difference between function declaration and function expression?](#what-is-the-difference-between-function-declaration-and-function-expression)
6. [What is hoisting in JavaScript?](#what-is-hoisting-in-javascript)
7. [What is the difference between arrow functions and regular functions?](#what-is-the-difference-between-arrow-functions-and-regular-functions)
8. [What are template literals in JavaScript?](#what-are-template-literals-in-javascript)
9. [What is the difference between map(), filter(), and forEach()?](#what-is-the-difference-between-map-filter-and-foreach)
10. [What is a closure in JavaScript?](#what-is-a-closure-in-javascript)
11. [What are higher-order functions in JavaScript?](#what-are-higher-order-functions-in-javascript)
12. [What is the purpose of call(), apply(), and bind()?](#what-is-the-purpose-of-call-apply-and-bind)
13. [What is the difference between shallow copy and deep copy?](#what-is-the-difference-between-shallow-copy-and-deep-copy)
14. [How does the this keyword work in JavaScript?](#how-does-the-this-keyword-work-in-javascript)
15. [What is prototypal inheritance in JavaScript?](#what-is-prototypal-inheritance-in-javascript)
16. [What are promises and how do they work?](#what-are-promises-and-how-do-they-work)
17. [What is async and await in JavaScript?](#what-is-async-and-await-in-javascript)
18. [What are generators in JavaScript?](#what-are-generators-in-javascript)
19. [What are JavaScript modules? (import and export)](#what-are-javascript-modules-import-and-export)
20. [What is memoization in JavaScript?](#what-is-memoization-in-javascript)
21. [Explain the difference between setTimeout() and setInterval().](#explain-the-difference-between-settimeout-and-setinterval)
22. [What is debouncing and throttling?](#what-is-debouncing-and-throttling)
23. [What is event delegation in JavaScript?](#what-is-event-delegation-in-javascript)
24. [What are WeakMap and WeakSet in JavaScript?](#what-are-weakmap-and-weakset-in-javascript)
25. [What are ES6+ features that you use frequently?](#what-are-es6-features-that-you-use-frequently)
26. [What is the difference between document.querySelector() and getElementById()?](#what-is-the-difference-between-documentqueryselector-and-getelementbyid)
27. [What are event bubbling and event capturing?](#what-are-event-bubbling-and-event-capturing)
28. [What is the difference between localStorage, sessionStorage, and cookies?](#what-is-the-difference-between-localstorage-sessionstorage-and-cookies)
29. [What is the fetch() API?](#what-is-the-fetch-api)
30. [How can you create and trigger a custom event in JavaScript?](#how-can-you-create-and-trigger-a-custom-event-in-javascript)
31. [How does JavaScript handle memory management and garbage collection?](#how-does-javascript-handle-memory-management-and-garbage-collection)
32. [What is the difference between deep cloning and shallow cloning in JavaScript?](#what-is-the-difference-between-deep-cloning-and-shallow-cloning-in-javascript)
33. [What is the difference between Object.freeze() and Object.seal()?](#what-is-the-difference-between-objectfreeze-and-objectseal)
34. [What are Proxy and Reflect in JavaScript?](#what-are-proxy-and-reflect-in-javascript)
35. [What is the typeof operator and what are the possible return values?](#what-is-the-typeof-operator-and-what-are-the-possible-return-values)

36. [Use of stack](#use-of-stack)
37. [new set()](#new-set)

# HTML-CSS

1.  [Explain the difference between absolute, relative, fixed, and sticky positioning.](#explain-the-difference-between-absolute-relative-fixed-and-sticky-positioning)
2.  [What is flexbox and how does it work?](#what-is-flexbox-and-how-does-it-work)

## Answers

### What are the differences between var, let, and const?

```
var: Function-scoped, can be redeclared and updated.
let: Block-scoped, can be updated but not redeclared.
const: Block-scoped, cannot be updated or redeclared.
```

### What is the difference between == and ===?

```
== checks only values (type coercion happens).
=== checks both value and type (strict comparison).
```

### Explain the difference between null and undefined.

```

```

### What are JavaScript data types?

```
Primitive: String, Number, Boolean, Undefined, Null, BigInt, Symbol
Non-Primitive: Object, Array, Function
```

### What is the difference between function declaration and function expression?

```js
Function Declaration: Defined using the `function` keyword at the top level. Can be called before its definition due to hoisting.

Example:
function greet() {
    console.log("Hello");
}

Function Expression: Assigned to a variable. Not hoisted, so it must be defined before use.

Example:
const greet = function() {
    console.log("Hello");
};
```

### What is hoisting in JavaScript?

```js
Hoisting is JavaScript's default behavior of moving variable and function declarations to the top of their scope before code execution.

Example:
console.log(x); // Undefined (var is hoisted but not its value)
var x = 10;

console.log(greet()); // Works because function declarations are fully hoisted
function greet() {
    return "Hello";
}
```

### What is the difference between arrow functions and regular functions?

```js
Arrow Functions:
- Shorter syntax.
- Do not have their own `this` (inherits from parent scope).
- Cannot be used as constructors.

Example:
const add = (a, b) => a + b;

Regular Functions:
- Have their own `this`.
- Can be used as constructors.

Example:
function add(a, b) {
    return a + b;
}
```

### What are template literals in JavaScript?

```js
Template literals allow embedding expressions inside strings using backticks (`).

Example:
const name = "John";
console.log(`Hello, ${name}!`); // Output: Hello, John!
```

**Intermediate JavaScript Questions**

### What is the difference between map(), filter(), and forEach()?

```js
map(): Creates a new array by applying a function to each element.

Example:
const nums = [1, 2, 3];
const squared = nums.map(n => n * n); // [1, 4, 9]

filter(): Creates a new array with elements that meet a condition.

Example:
const evens = nums.filter(n => n % 2 === 0); // [2]

forEach(): Executes a function on each element but does not return a new array.

Example:
nums.forEach(n => console.log(n)); // Logs 1, 2, 3
```

### What is a closure in JavaScript?

```js
A function that has access to its outer functions scope even after the outer function has finished execution.
Example:
function outer() {
    let count = 0;
    return function inner() {
        count++;
        console.log(count);
    };
}

const counter = outer();
counter(); // 1
counter(); // 2
```

### What are higher-order functions in JavaScript?

```js
A higher-order function is a function that takes another function as an argument or returns a function.

Example:
function greet(name) {
    return function(message) {
        console.log(`${message}, ${name}!`);
    };
}

const sayHello = greet("John");
sayHello("Hello"); // Output: Hello, John!
```

### What is the purpose of call(), apply(), and bind()?

```js
call(): Invokes a function with a given `this` value and arguments separately.
apply(): Similar to call(), but takes arguments as an array.
bind(): Returns a new function with `this` set to a specific value.

Example:
function greet(greeting) {
    console.log(`${greeting}, ${this.name}`);
}

const user = { name: "Alice" };
greet.call(user, "Hello"); // Output: Hello, Alice
greet.apply(user, ["Hi"]);
const boundGreet = greet.bind(user);
boundGreet("Hey");

```

### What is the difference between shallow copy and deep copy?

```js
Shallow Copy: Copies only references of nested objects, not the actual objects.

Example:
const obj1 = { a: 1, b: { c: 2 } };
const obj2 = { ...obj1 };
obj2.b.c = 10;
console.log(obj1.b.c); // 10 (Both share same reference)

Deep Copy: Copies everything, including nested objects.

Example:
const obj3 = JSON.parse(JSON.stringify(obj1));
obj3.b.c = 20;
console.log(obj1.b.c); // 10 (Different references)
```

### How does the this keyword work in JavaScript?

```js
The this keyword refers to the object that is calling the function. It behaves differently based on how the function is called:
In a regular function: this refers to the global object (window in browsers, global in Node.js).
In an object method: this refers to the object that owns the method.
In an arrow function: this is inherited from the surrounding function.
In a constructor function or class: this refers to the new instance created.

const person = {
  name: "Yatharth",
  greet() {
    console.log(this.name); // "Yatharth"
  }
};
person.greet();

```

**Advanced JavaScript Questions**

### What is prototypal inheritance in JavaScript?

```js
In JavaScript, objects can inherit properties and methods from another object using prototypes.
 
const animal = { eats: true };
const dog = Object.create(animal);
console.log(dog.eats); // true (inherited from animal)
```

### What are promises and how do they work?

```js
A promise is used for handling asynchronous operations. It has three states: pending, resolved, and rejected.

const fetchData = new Promise((resolve, reject) => {
  setTimeout(() => resolve("Data received"), 2000);
});
fetchData.then(data => console.log(data));
```

### What is async and await in JavaScript?

```js
async and await make working with promises easier by allowing us to write asynchronous code in a synchronous style.

async function fetchData() {
  let data = await fetch("https://jsonplaceholder.typicode.com/todos/1");
  let json = await data.json();
  console.log(json);
}
fetchData();
```

### What are generators in JavaScript?

```

```

### What are JavaScript modules? (import and export)
```
Modules allow us to split code into separate files for better organization.
```
File: module.js
```js
export const name = "Yatharth";
export function greet() {
  return "Hello!";
}
```

File: main.js
```js
import { name, greet } from "./module.js";
console.log(name); // "Yatharth"
console.log(greet()); // "Hello!"
```

### What is memoization in JavaScript?

```

```

### Explain the difference between setTimeout() and setInterval().

```

```

### What is debouncing and throttling?

```

```

### What is event delegation in JavaScript?

```

```

### What are WeakMap and WeakSet in JavaScript?

```

```

### What are ES6+ features that you use frequently?

```

```

**DOM & Browser-Related Questions**

### What is the difference between document.querySelector() and getElementById()?

```

```

### What are event bubbling and event capturing?

```

```

### What is the difference between localStorage, sessionStorage, and cookies?

| Storage          | Expiry        | Scope          | Size |
| ---------------- | ------------- | -------------- | ---- |
| `localStorage`   | Never         | Same origin    | 5MB  |
| `sessionStorage` | On tab close  | Same origin    | 5MB  |
| `cookies`        | Manual expiry | Sent to server | 4KB  |



### What is the fetch() API?

```

```

### How can you create and trigger a custom event in JavaScript?

```

```

**Miscellaneous Questions**

### How does JavaScript handle memory management and garbage collection?

```

```

### What is the difference between deep cloning and shallow cloning in JavaScript?

```

```

### What is the difference between Object.freeze() and Object.seal()?

```

```

### What are Proxy and Reflect in JavaScript?

```

```

### What is the typeof operator and what are the possible return values?

```

```

### use of stack

```

```

### new set()

| Method          | Description                | Example                 |
| --------------- | -------------------------- | ----------------------- |
| `add(value)`    | Adds a new value           | `mySet.add(6);`         |
| `delete(value)` | Removes a value            | `mySet.delete(2);`      |
| `has(value)`    | Checks if value exists     | `mySet.has(3); // true` |
| `size`          | Returns number of elements | `mySet.size; // 5`      |
| `clear()`       | Removes all values         | `mySet.clear();`        |

### what is react?

```
React is a javascript's library for building fast and interactive UI.
```

### why use React?

```
React make the UI development more easier and faster with reusable component and the Virtual DOM
```

### Virtual DOM vs Real DOM

| Virtual DOM                                                                                       | Real DOM                                                    |
| ------------------------------------------------------------------------------------------------- | ----------------------------------------------------------- |
| 🚀 Faster, minimizes changes before updating the Real DOM.                                        | 🐢 Slower, re-renders the entire component.                 |
| 🏗️ A lightweight copy of the Real DOM for faster updates.                                         | 📜 The actual structure of the UI that the browser renders. |
| 🔄 Updates the Virtual DOM first and applies changes only to the necessary parts of the Real DOM. | ✏️ Directly updates the UI, which is less efficient.        |

### props

```
- props is property
- Cant be modified
- read only
- immutable
```

### state

```
- state is part of app that can be changed
- each component have it's state
- mutable
- it is local to the component
```

### useState()

```
Stores and uodate data in fucntional component
```

### useEffect()

```
Runs code when component loads, updates or unmount
```

### useReducer()

```
- used for more complex state management
- it takes a reducer function and initiastate
- returns state and dispatch function
- dispatch which update the state to a different value
```

### useRef()

```
stores reference to an element or value without re-render
```

### useMemo()

```
- improves the app performance
- use memoizationatio to remember values
```

### useLayoutEffect()

```

```

### Explain the difference between absolute, relative, fixed, and sticky positioning.

```
Relative: Moves based on its original position.
Absolute: Moves relative to the nearest positioned parent.
Fixed: Stays in the same position even when scrolling.
Sticky: Sticks when scrolling but stays within its parent
```

### What is flexbox and how does it work?

```
 A CSS layout system that helps align items easily.
```

Example:

```
.container {
 display: flex;
 justify-content: center; //Align horizontally
 align-items: center; //Align vertically
 }
```

<p style="position: fixed; right: 20px; bottom: 20px; z-index: 1000;">
  <a href="#top">
    <img src="https://img.shields.io/badge/🔼-Back_to_Top-blue" alt="Back to Top" 
         style="width: 90px; transition: transform 0.3s ease-in-out;"
         onmouseover="this.style.transform='scale(1.1)'" 
         onmouseout="this.style.transform='scale(1)'">
  </a>
</p>
