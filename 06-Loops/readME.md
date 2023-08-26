# Loops

Loops are used in JavaScript to perform repeated tasks based on a condition. A Conditions typically return true or false. A loop will continue running until the defined condition returns false.

- For Loop
- While Loop
- Do While Loop
- For Of Loop
- For In Loop
- Break
- Continue

#### For loop

```js
// For loop structure
for(initialization, condition, increment/decrement){
  // code goes here
}

// Example
for(let i = 5; i >= 0; i--){
  console.log(i)
}

// 5 4 3 2 1 0
```

- initialization - This expression runs before the execution of the first loop, and is usually used to create a counter.
- condition - This expression is checked each time before the loop runs. If it evaluates to true, the statement or code in the loop is executed. If it evaluates to false, the loop stops. And if this expression is omitted, it automatically evaluates to true.
- finalExpression - This expression is executed after each iteration of the loop. This is usually used to increment a counter.

#### While loop

```js
let i = 0;
while (i <= 5) {
  console.log(i);
  i++;
}

// 0 1 2 3 4 5
```

#### Do While Loop

```js
let i = 0;
do {
  console.log(i);
  i++;
} while (i <= 5);

// 0 1 2 3 4 5
```

#### For Of Loop

For of loop is mostly used in arrays and For in loop is used in objects.
The for...of loop iterates over the values of many types of iterables, including arrays, and special collection types like Set and Map.

```js
// Adding numbers in an array
const number = [2, 3, 4, 5, 6, 7];

let sum = 0;
for (const num of number) {
  sum += num;
}
console.log(sum);
```

#### For In Loop

```js
const capitals = {
  a: "Athens",
  b: "Belgrade",
  c: "Cairo",
};

for (let key in capitals) {
  console.log(`${key}:${capitals[key]}`);
}

// Output:
// a: Athens
// b: Belgrade
// c: Cairo
```

#### Break

Break is used to interrupt a loop.

```js
for (let i = 0; i <= 5; i++) {
  if (i == 3) {
    break;
  }
  console.log(i);
}

// 0 1 2
```

The above code stops if 3 found in the iteration process.

#### Continue

We use the keyword continue to skip a certain iterations.

```js
for (let i = 0; i <= 5; i++) {
  if (i == 3) {
    continue;
  }
  console.log(i);
}

// 0 1 2 4 5
```

#### Examples

Develop a small script which generate a six characters random id:

```js
let result = "";
const characters =
  "ABCDEFGHIJKLMNOPQRSTUVWXYZabcdefghijklmnopqrstuvwxyz0123456789";

for (let i = 0; i < 6; i++) {
  const randomIndex = Math.floor(Math.random() * characters.length);
  result += characters.charAt(randomIndex);
  // result += characters[randomIndex]; another way
}

console.log("Random ID:", result);
```

// Write a script which generates a random hexadecimal number.

```js
const numbers = "1234567890abcdef";
let hexa = "#";

for (let i = 0; i < 6; i++) {
  const randomHexa = Math.floor(Math.random() * numbers.length);
  hexa += numbers[randomHexa];
}

console.log(hexa);
```

// Using the above countries array, find the country containing the biggest number of characters.

```js
let biggest = "";

for (const big of country) {
  if (big.length > biggest.length) {
    biggest = big;
  }
}
```

```js
// THERE ARE 4 WAYS TO COPY FROM THE ORIGINAL ARRAY

// SPREAD OPERATOR
const copyCountry = [...country];
console.log(copyCountry);

// ARRAY.FROM()
const countriesCopy = Array.from(countries);

// Array.prototype.slice():
const countryCopy = countries.slice();

// Array.prototype.concat():
const countriesCopys = [].concat(countries);
```
