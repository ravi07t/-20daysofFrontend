
Today’s Focus:
1.	What is Event loop in JavaScript?
JavaScript runs on a single thread, meaning it can execute only one piece of code at a time. But web apps do many things like fetching data, waiting for user clicks, or reading files. So how can JavaScript handle all these tasks without freezing the page, That’s where the Event Loop comes in it manages what to execute next and when.

2.	How it works?
JavaScript starts executing the global code and fills the call stack. When it encounters an asynchronous operation, such as a setTimeout() or fetch() call, that task is delegated to the Web API. Once the Web API finishes, the callback function is placed in the Callback Queue or Microtask Queue (depending on the type of task). The Event Loop checks whether the call stack is empty. If empty, it first processes all microtasks (like Promise callbacks). After all microtasks are executed, it moves to the Callback Queue and executes one microtask. This cycle repeats continuously as long as the program is running.

3.	What is Call stack?
The call stack is where the JavaScript engine keeps track of the current executing functions. When a function is invoked, it is pushed onto the stack, and when it finishes execution, it is popped off.

4.	What is Callback Queue?
Once the Web API completes its task (for example, after a timer ends), the associated callback function is placed in the Callback Queue. These callbacks wait until the call stack is empty before they can be executed.

5.	What are the different types of queues in the event loop?
Microtask Queue: Handles Promises (.then, .catch, .finally), process.nextTick (Node.js).
Macrotask Queue: Handles tasks like setTimeout, setInterval, setImmediate, DOM events.


