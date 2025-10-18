1.	JavaScript Execution context?
Everything in JS happens inside the execution context. Imagine a container inside which JS runs. In the container the first component is memory component and the 2nd one is code component, Memory component has all the variables and functions in key value pairs. It is also called Variable environment. Code component is the place where code is executed one line at a time. It is also called the Thread of Execution.

2.	What happens during the creation phase of an Execution Context?
Memory is allocated for variables and functions. Functions are hoisted with their full code. Variables are hoisted with value undefined. *this* keyword is set.

3.	What is the role of the *this* keyword in Execution Context?
In Global Context - this refers to window (in browser)
In Function Context - depends on how function is called.

4.	How does the Call Stack manage multiple Execution Contexts?
The Call Stack stores all the execution contexts created during the execution of a JavaScript program. When a function is called, a new execution context is created and pushed onto the stack. When the function returns, its context is popped off the stack.

5.	How ‘this’ works in JavaScript?
In JavaScript, this refers to the object that is currently executing the code. Its value depends on how the function is called.
- In global scope, it refers to the global object (window in browsers).
- Inside an object method, it refers to that object.
- In regular functions, it’s undefined in strict mode or window in non-strict mode.
- Arrow functions don’t have their own this; they inherit it from their parent scope.
- In classes, this refers to the class instance.
- And using call, apply, or bind, we can explicitly set what this should refer to.


