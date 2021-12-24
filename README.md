# JavaScript Principles

- To run some code we need the thread of execution, going through the code line by line. We also need the memory to store things. Those two things together form the execution context.

- The call stack starts with global, the whole execution context. When JavaScript executes a function, it adds it on top of the call stack, when it is done with the function, that which is on top of the call stack gets taken off.

# Functions & Callbacks

- Functions in JavaScript are first class objects, they can be treated as with any other object.

- Everytime a function gets called in JavaScript, a new execution context that gets created with its own thread of execution and local memory.

- What we refer as closure in JavaScript, is a function's ability to remember its "surrounding" when called elsewhere, i.e. the variables it had access to. It is being able to remember its lexical scope, even though it gets called elsewhere. This really shines when you return a function from a function, and continous onwards.

# Web API

- When we Web API gets used in JavaScript, the Web Browser takes cares of that operation. When it is done, the Web Browser sends the output to the callback queue, and then the Event Loop, who's job is to continously check if the callstack is empty and no thread of execution is running, then allows that which is in the callback queue to get pushed into the callstack.
