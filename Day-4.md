Today’s Focus:
1.	Hoisting in JavaScript?
Hoisting behavior where variable and function declarations are moved to the top of their scope (global or local) before the code is executed. ‘var’ declarations are hoisted to the top of their function scope. This means you can use a var variable before its declaration in the code, though its value will be undefined until the actual declaration is reached, ‘let’ and ‘const’ are not hoisted.
console.log(a); // undefined (not error)
var a = 10;

2.	What is Temporal Dead Zone (or) Does hoisting happen with let and const??
We see before let and const are not hoisted, Thus, let and const are also hoisted but where different from the var, different memory space that is called Temporal Dead Zone(TDZ). let and const are also hoisted, but they don’t get initialized until their declaration line. The time between entering scope (global or local) and declaration is called the TDZ.
console.log(b); // ❌ ReferenceError
let b = 20;

3.	What is Function Hoisting?
Function declarations are fully hoisted - you can call them before they appear in the code.
greet();
function greet() {
  console.log("Hello!");
}
With Function Expression are not hoisted only the variable (var sayHello) is hoisted, not the function assignment
sayHello();
var sayHello = function() {
  console.log("Hi!");
};
To avoid this use variable ‘let’ or ‘const’ instead of var.

4.	Why is it a good practice to declare variables at the top of their scope even though hoisting exists?
When JavaScript hoists variables, it only hoists declarations, not initializations. This means that if you use a variable before it’s assigned a value, you might get undefined or even ReferenceError - which can cause confusing bugs. Better we use declare variables at top its predictable and it doesn’t depend on hoisting behavior.

5.	How does hoisting work inside a function scope?
Hoisting inside a function works just like in the global scope but it’s limited to that function’s local execution context. Variables declared inside a function are not associable outside, and their hoisting is independent of the global scope.
function demo() {
  console.log(x); // undefined
  var x = 10;
  console.log(x); // 10
}

demo();
