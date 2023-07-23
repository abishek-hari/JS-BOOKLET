# Strings Math Date

### Strings

A string is a data type representing a sequence of characters that may consist of letters, numbers, symbols, words, or sentences.

```js
let js = "30 days of JavaScript";
let jsx = js[js.length - 1];

console.log(js.length);

console.log(jsx);

console.log(js.toUpperCase());

console.log(js.toLowerCase());

// substr(): It takes two arguments, the starting index and number of characters to slice.
console.log(js.substr(2, 5));

// substring(): It takes two arguments, the starting index and the stopping index but it doesn't include the character at the stopping index.
console.log(js.substring(4, 10));

// split(): The split method splits a string at a specified place.
console.log(js.split(""));

// trim(): Removes trailing space in the beginning or the end of a string.
console.log(js.trim());

// includes(): It takes a substring argument and it checks if substring argument exists in the string. includes() returns a boolean. If a substring exist in a string, it returns true, otherwise it returns false.
console.log(js.includes("days"));

// replace(): takes as a parameter the old substring and a new substring.
console.log(js.replace("JavaScript", "golang"));

//  Takes index and it returns the value at that index
console.log(js.charAt(5));

// charCodeAt(): Takes index and it returns char code (ASCII number) of the value at that index
console.log(js.charCodeAt(5));

// indexOf(): Takes a substring and if the substring exists in a string it returns the first position of the substring if does not exist it returns -1
console.log(js.indexOf("f"));

// lastIndexOf(): Takes a substring and if the substring exists in a string it returns the last position of the substring if it does not exist it returns -1
console.log(js.lastIndexOf("pt"));

// concat(): it takes many substrings and joins them.
console.log(js.concat(" and you can finish"));

// startsWith: it takes a substring as an argument and it checks if the string starts with that specified substring. It returns a boolean(true or false).
console.log(js.startsWith("30"));

// endsWith: it takes a substring as an argument and it checks if the string ends with that specified substring. It returns a boolean(true or false).
console.log(js.endsWith("JavaScript"));

// search: it takes a substring as an argument and it returns the index of the first match. The search value can be a string or a regular expression pattern.
console.log(js.search("of"));

// match: it takes a substring or regular expression pattern as an argument and it returns an array if there is match if not it returns null.
console.log(js.match("days"));

// repeat(): it takes a number as argument and it returns the repeated version of the string.
console.log(js.repeat(3));
```

### Math

```js
// Round
console.log(Math.round(PI)); // 3 to round values to the nearest number

console.log(Math.round(9.81)); // 10

// Floor
console.log(Math.floor(2.7)); // 2 rounding down

// Ceil
console.log(Math.ceil(5.2)); // 6 rounding up

// Min
console.log(Math.min(-5, 3, 20, 4, 5, 10)); // -5, returns the minimum value

// Max
console.log(Math.max(-5, 3, 20, 4, 5, 10)); // 20, returns the maximum value

//Absolute value
console.log(Math.abs(-10)); // 10

//Square root
console.log(Math.sqrt(100)); // 10

// Power
console.log(Math.pow(3, 2)); // 9
```

#### Random generator

```js
// 1. Generate a random number between 0 and 100 inclusively.

let randomNum = Math.floor(Math.random() * 10);
console.log(randomNum);

// 2. Generate a random number between 50 and 100 inclusively.

let random = Math.floor(Math.random() * (100 - 50 + 1)) + 50;
console.log(random);

//   Access the 'JavaScript' string characters using a random number.

let string = "javascript";
let randomIndex = Math.floor(Math.random() * string.length);
let randomCharacter = string.charAt(randomIndex);
console.log(randomCharacter);
```

### Date

Date Methods:

- getFullYear(), getMonth(), getDate(), getDay(), getHours(), getMinutes, getSeconds(), getMilliseconds(), getTime(), getDay()

#### Time

Human Readable Time Format

```js
const date = new Date();
const year_s = date.getFullYear();
const month = String(date.getMonth() + 1).padStart(2, "0");
const dates = String(date.getDate()).padStart(2, "0");
const hour = String(date.getHours()).padStart(2, "0");
const minutes = String(date.getMinutes()).padStart(2, "0");

console.log(`${year_s}-${month}-${dates} ${hour}:${minutes}`);
```
