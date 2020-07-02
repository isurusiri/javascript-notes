# Core Elements of JavaScript

- Thread of execution
- Functions
- Call stack

When JavaScript compiler runs the code, it goes through the code line by line and executes each line. This is know as _Thread of execution_.

JavaScript stores data in its memory. This data includes 'strings', 'numbers', and 'arrays', so that we can reuse what's in the memory later on. It also stores it's code inside the memory as functions, which allows us to reuse these code blocks later on in our programs.

When a function is executing in JavaScript, a logical area called `Execution Context` will be created. Main purpose of execution context is to run JavaScript code and it has two main parts,

- Thread of execution
- Memory

Since JavaScript applications can have multiple function, these applications will have multiple threads of execution specific to each function / function call. To keep track of the current execution context, JavaScript maintains a call stack.

Call stack maintains a stack of function calls, or in more precisely a stack of references to execution contexts, where latest execution context will alway be on top and pop it out once the scope of that function is over.

Executing a function in JavaScript means pushing a new execution context to the call stack and returning from a function makes that function pop out from the call stack.
