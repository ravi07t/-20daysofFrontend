Today’s Focus:
1.	What is the difference between call(), apply(), and bind()?
call(), apply(), and bind() in JavaScript they all help you control the value of ‘this’ inside a function. It doesn’t return new function. 
call() - Calls the function immediately, setting this to the specified object. Arguments are passed individually.
const person = {
  fullName: function (city, country) {
    return `${this.firstName} ${this.lastName} from ${city}, ${country}`;
  }
};

const user = { firstName: "Ravi", lastName: "Kumar" };
console.log(person.fullName.call(user, "Nellore", "India"));

apply() - Just like call(), Calls the function immediately but arguments are passed as an array. It doesn’t return new function.
const person = {
  fullName: function (city, country) {
    return `${this.firstName} ${this.lastName} from ${city}, ${country}`;
  }
};

const user = { firstName: "Ravi", lastName: "Kumar" };
console.log(person.fullName.apply(user, ["Nellore", "India"]));

bind() - Does not call immediately, but returns a new function with this permanently bound.
const person = {
  fullName: function () {
    return `${this.firstName} ${this.lastName}`;
  }
};

const user = { firstName: "Ravi", lastName: "Kumar" };

const boundFunc = person.fullName.bind(user);
console.log(boundFunc());

2.	What is Closures in JavaScript?
A closure in JavaScript is a combination of a function and the lexical environment, it allows inner function to access variables from its outer scope, even after the outer function has finished executing.

3.	What is an IIFE?
IIFE stands for Immediately Invoked Function Expression. It’s a JavaScript function that runs as soon as it is defined. Instead of calling the function later, an IIFE executes immediately and creates a new scope, helping to avoid polluting the global namespace. IIFE was widely used before ES6 for modules and scope management, but now ES6 modules and let/const.

4.	Callbacks in Javascript?
A callback function is a function passed as an argument to another function and is executed after some operation. Callbacks allow JavaScript to handle asynchronous tasks without blocking code execution.

