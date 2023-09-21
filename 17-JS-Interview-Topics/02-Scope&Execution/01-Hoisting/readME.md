# Hoisting

JavaScript hoisting occurs during the creation phase of the execution context that moves the variable and function declarations to the top of the script.
The JavaScript engine hoists the variables declared using the let keyword, but it doesn’t initialize them as the variables declared with the var keyword.
The JavaScript engine doesn’t hoist the function expressions and arrow functions.

```js
a();
b();
console.log(x);
var x = 1;

function a() {
  var x = 10;
  console.log(x);
}

function b() {
  var x = 100;
  console.log(x);
}
```
