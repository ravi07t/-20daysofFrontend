Today’s Focus:
1.	What is a Promise in JavaScript?
Promises provide a structured way to manage asynchronous code without deeply nested callbacks. A Promise in JavaScript is an object that represents success or failure of an asynchronous operation and its results value. They help avoid callback hell and make the code cleaner, more readable, and easier to handle errors.

2.	What are the states of Promise? Or Promise lifecycle summary?
Every Promise in JavaScript goes through three distinct states during its lifecycle: 
Pending State: This is the initial state of a Promise when it is created and the asynchronous operation has not yet completed.
Fulfilled (Resolved) State: A Promise moves into the fulfilled state when the asynchronous operation completes successfully. In this state, the operation is completed, and the Promise delivers the expected value.
Rejected State: A Promise enters the rejected state when the asynchronous operation fails.

3.	How to Handling Promise Results?
.then() - Used when the Promise is fulfilled. It allows access to the value returned by the asynchronous task.
.catch() - Used when the Promise is rejected. It allows handling of errors or exceptions that occurred during the operation.
.finally() - Executes after the Promise is settled, regardless of whether it was fulfilled or rejected. It is generally used for cleanup operations.

4.	What is async/await in JavaScript?
It’s syntactic sugar over Promises, It allows writing asynchronous code in a synchronous style. await pauses execution of an async function until the Promise resolves.

5.	Output based questions like examples:
console.log("A");
setTimeout(() => console.log("B"), 0);
Promise.resolve().then(() => console.log("C"));
console.log("D");
