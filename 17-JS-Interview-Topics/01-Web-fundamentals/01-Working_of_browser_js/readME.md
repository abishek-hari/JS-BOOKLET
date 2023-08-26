# Working Of Javascript

What is javascript?
JavaScript is a dynamic typed single-threaded language. It was developed by Brendan Eich in september 1995.Initially, it was called Mocha, then LiveScript, and was later renamed JavaScript.

#### How javscript code works in browser?

JAVASCRIPT CODE ----> PARSER ----> JS ENGINE

- Javscript code - The code that is written in the Script.js
- Parser - Parser go through line by line and check if the syntax of the code is correct
- JS Engine - Js Engine is computer program that executes javascript code and converts it into computer understandable language (Machine Code)

Firstly the Jscode is parsed and check if the syntax of the code is correct.Now the browser doesn't understand the high level of JS code, so it is send to JS Engine.When the JS Engine scans a script file it makes an environment called Execution Context that handles the entire tranformation and execution of the code.

![THREAD OF EXECUTION](../../../Images/ThreadOfExecution.png)

#### What is Execution Context?

When the JS Engine scans a script file it makes an environment called Execution Context that handles the entire tranformation and execution of the code.

There are two types of Execution Context:

- Global Execution Context
- Function Execution Context

Global Execution Context:
The global execution context is created when a JavaScript script first starts to run, and it represents the global scope in JavaScript.

Function Execution Context:
A function execution context is created whenever a function is called, representing the function's local scope.

When a javascript file is created there will be only one Global Execution Context but there could be many Function Execution Context.

#### How Execution Context is created?

There will be two phases when a Execution Context is created, One is Creation Phase and the other one is Execution Phase

Creation Phase:
During this phase, JavaScript allocates memory for variables and assigns them an initial value of undefined. It also stores functions in memory (hoisting) and sets up the scope chain and this value.

Execution Phase:
In this phase, JavaScript executes the code line by line, performing assignments, computations, and function calls. Functions are executed within their own execution contexts.

![EXECUTION CONTEXT](../../../Images/Execution-context.png)
![EXECUTION CONTEXT](../../../Images/Execution-context-info.png)

Execution Context has many Function Execution Context and it is managed by Execution Stack.

#### What is Call stack?

A Call Stack is a stack with LIFO(Last In First Out) structure, which is used to store all the Execution Context created during the code Execution.

Function Calls: When a function is called in JavaScript, a new execution context for that function is created, which includes information about the function's arguments, local variables, and its scope.

Push onto Stack: This newly created execution context is pushed onto the top of the call stack.

Execution: The function's code is executed within its context. If this function calls other functions, their contexts are also pushed onto the stack, creating a chain of contexts.

Pop from Stack: When a function finishes executing, its context is popped (removed) from the top of the call stack.

Other Names For Call Stack:

- Execution context Stack
- Program Stack
- Control Stack
- Runtime stack
- machine Stack

![CALL STACK](../../../Images/CallStack.png)
![CALL STACK](../../../Images/callStackEg.png)

#### Event Loop
