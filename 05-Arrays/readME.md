# Arrays

An array is a collection of different data types which are ordered and changeable(modifiable).

```js
const arr = [];
console.log(arr);
```

#### Creating an array using split

Using split you can convert String to Array

```js
let js = "JavaScript";
const charsInJavaScript = js.split("");

console.log(charsInJavaScript); // ["J", "a", "v", "a", "S", "c", "r", "i", "p", "t"]

let companiesString = "Facebook, Google, Microsoft, Apple, IBM, Oracle, Amazon";
const companies = companiesString.split(",");

console.log(companies); // ["Facebook", " Google", " Microsoft", " Apple", " IBM", " Oracle", " Amazon"]
let txt =
  "I love teaching and empowering people. I teach HTML, CSS, JS, React, Python.";
const words = txt.split(" ");

console.log(words);

// ["I", "love", "teaching", "and", "empowering", "people.", "I", "teach", "HTML,", "CSS,", "JS,", "React,", "Python"]
```

### Methods to manipulate array

There are different methods to manipulate an array. These are some of the available methods to deal with arrays:Array, length, concat, indexOf, slice, splice, join, toString, includes, lastIndexOf, isArray, fill, push, pop, shift, unshift, reverse, sort

#### ARRAY METHODS

```js
// Array Constructor

const arr = Array();
console.log(arr);

const eightEmptyValue = Array(8);
console.log(eightEmptyValue);
```

```js
// Creating static values with fill

const eight5values = Array(8).fill(5);
console.log(eight5values);
```

```js
// Concatenating array using concat

const firstList = [1, 2, 3];
const secondList = [4, 5, 6];
const thirdList = firstList.concat(secondList);
console.log(thirdList);
```

```js
// Getting array length
const flat = ["flatmap", "setmap", "harshmap"];
console.log(flat.length);
```

```js
// IndexOf

const fruits = ["banana", "orange", "mango", "lemon"];
console.log(fruits.indexOf("banana"));
```

```js
// lastIndexOf

const numbers = [1, 2, 3, 4, 5, 3, 1, 2];
console.log(numbers.lastIndexOf(2));
console.log(numbers.lastIndexOf(0));
```

```js
// Includes

const webTechs = [
  "HTML",
  "CSS",
  "JavaScript",
  "React",
  "Redux",
  "Node",
  "MongoDB",
];

console.log(webTechs.includes("React"));
```

```js
// Checking array

const number = [1, 2, 3, 4, 5];
console.log(Array.isArray(number)); //true
```

```js
// Converting array to string

const names = ["Asabeneh", "Mathias", "Elias", "Brook"];
console.log(names.toString()); // Asabeneh,Mathias,Elias,Brook
```

```js
// joining array elements
const webTech = [
  "HTML",
  "CSS",
  "JavaScript",
  "React",
  "Redux",
  "Node",
  "MongoDB",
]; // List of web technologies

console.log(webTechs.join());
console.log(webTechs.join(" # "));
```

```js
// Slice array elements
const num = [1, 2, 3, 4, 5];
console.log(num.slice(1));
```

```js
// Splice method in array
const nums = [1, 2, 3, 4, 5, 6, 7];
nums.splice(1, 5, 3, 8, 9);
console.log(nums);
```

```js
// Adding item to an array using push
const fruit = ["banana", "orange", "mango", "lemon", "apple"];
fruit.push("grapes");
console.log(fruit);
```

```js
// Removing the end element using pop
console.log(fruit.pop());
```

```js
// Removing an element from the beginning
console.log(fruit.unshift("pearl"));
```

```js
// Add an element from the beginning
console.log(fruit.shift("pearl"));
```

```js
// Reversing array order
const numb = [1, 2, 3, 4, 5];
numb.reverse();
console.log(numb);
```

```js
// Sorting elements in array
const webTechnology = [
  "HTML",
  "CSS",
  "JavaScript",
  "React",
  "Redux",
  "Node",
  "MongoDB",
];

webTechnology.sort();
console.log(webTechnology);
```
