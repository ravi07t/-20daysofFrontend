
Today’s Focus:
6.	What is JSON? Difference between JSON.parse() & JSON.stringify()?
JSON (JavaScript Object Notation) is a lightweight data format used for storing and exchanging data between a server and a web application.
JSON.stringify() - Converts a JavaScript object or array into a JSON string (text format).
When to use You need to send data to a server or store it (e.g., in localStorage or API calls).
JSON.parse() - Converts a JSON string back into a JavaScript object.
When to use You receive JSON data (like from an API or localStorage) and want to use it as a JavaScript object.

7.	map(), filter(), reduce() in JavaScript?
map() - Creates a new array by applying a function to each element of an existing array. Does not change the original array.
const numbers = [1, 2, 3, 4];
const doubled = numbers.map(num => num * 2);
console.log(doubled); // [2, 4, 6, 8]

filter() - Creates a new array with only those elements that pass a condition (returns true). Does not change the original array.
const numbers = [1, 2, 3, 4, 5, 6];
const even = numbers.filter(num => num % 2 === 0);
console.log(even); // [2, 4, 6]

reduce() - Executes a reducer function on each array element and returns a single accumulated result (like sum, average, total, etc.).
const numbers = [1, 2, 3, 4];
const sum = numbers.reduce((acc, curr) => acc + curr, 0);
console.log(sum); // 10

8.	Difference between map() and forEach() in JavaScript?
Both are used to iterate over arrays, But their purpose and behavior are different.
map() - Used to transform elements and return a new array with modified values. It returns a new array with transformed values.

forEach() - Used to loop through an array and perform some action for each element. It does not return anything (always undefined)

9.	What is Browser Storage?
There are mainly 3 types of browser storage:
Cookies - Small pieces of data (usually < 4KB) stored by the browser and sent with every HTTP request to the server.

localStorage - Stores data permanently (until manually cleared). Data is saved in the browser and not sent to the server. Storage limit: 5-10 MB

sessionStorage - Stores data for one browser session it’s cleared when the browser tab or window is closed. Storage limit: ~5MB.

10.	What is the prototype of a function in JavaScript?
Every function in JavaScript has a prototype property (used when creating instances). However, the function itself is also an object, so it has its own __proto__ (which points to Function.prototype).
