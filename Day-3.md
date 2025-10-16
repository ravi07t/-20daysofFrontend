1.	What is JavaScript?
JavaScript is Synchronous single threaded language, JavaScript is prototype-based with first-class functions. It is a interpreted, full-fledged programming language that enables dynamic interactivity on websites when applied to HTML document.

2.	What are datatypes in JavaScript?
1. Primitive Data Types: Primitive means single, immutable (cannot be changed)	
	string, number, Boolean, undefined, null, symbol, bigint
2. Non-Primitive Data Types: hold multiple values and are mutable (changeable).	
	object, array, function
3.	What is the difference between undefined and null?
Undefined - Variable declared but value not assigned, undefined is a default state.
Null – null means nothing, Variable assigned with an empty or intentional “no value” choice made by the developer 
4.	What is Scope in JavaScript?
Scope defines where you can access a variable in your program
Global scope - If a variable is declared outside any function or block, it is globally scoped. That variable can access from anywhere in the code.
Function scope - Variable accessible only inside a function, Variables declared inside a function are accessible only inside that function not outside.
Block scope - Variable accessible only inside a block{ }, Introduced in ES6, variables declared with let and const have block-level scope.
Lexical scope - Inner functions can access outer variables Lexical Scope, a function can access variables from its parent (outer) scope.
NOTE: Thus, we say *let* and *const* are BLOCK SCOPED. They are stored in a separate memory space which is reserved for this block. Also, they can't be accessed outside this block. But *var* a can be accessed anywhere as it is in global scope. Thus, we can't access them outside the Block.

5.	var vs let vs const
var - var declarations are function-scoped. This means a variable declared with var is accessible throughout the entire function in which it is declared, regardless of block-level scopes (like if statements or for loops).
let - let declarations are block-scoped. This means a variable declared with let is only accessible within the block (e.g., if block, for loop, or any {}) where it is defined.
const - const declarations are also block-scoped, similar to let.
