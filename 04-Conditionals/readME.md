# Conditionals

Conditional statements are used for make decisions based on different conditions.statements in JavaScript script executed sequentially from top to bottom.
The sequential flow of execution can be altered in two ways:

- Conditional execution: a block of one or more statements will be executed if a certain expression is true
- Repetitive execution: a block of one or more statements will be repetitively executed as long as a certain expression is true

Conditions can be implementing using the following ways:

- if
- if else
- if else if else
- switch
- ternary operator

#### If

checks specific condition is true

```js
let num = 3;
if (num > 0) {
  console.log(`${num} is a positive number`);
}
//  3 is a positive number
```

#### else

checks specific condition is false

```js
let a = 6;
let b = 5;

if (a > b) {
  console.log(`a is greater than b`);
} else {
  console.log(`a is less than b`);
}
```

#### else if

new condition to test, if the first condition is false

```js
// Student Grades

const marks = Number(prompt("Enter the Marks"));

if (marks > 80) {
  console.log(`great! you got A grade`);
} else if (marks > 70 && marks < 79) {
  console.log(`Very Good! you got B grade`);
} else if (marks > 60 && marks < 69) {
  console.log(`Good! you got c grade`);
} else if (marks > 50 && marks < 59) {
  console.log(`try your best! you got D grade`);
} else if (marks > 0 && marks < 49) {
  console.log(`try to improve! you got F grade`);
} else {
  console.log(`Enter you marks correctly`);
}
```

#### Switch

many alternative blocks of code to be executed

```js
//  Check if the season is Autumn, Winter, Spring or Summer. If the user input is :
// September, October or November, the season is Autumn.
// December, January or February, the season is Winter.
// March, April or May, the season is Spring
// June, July or August, the season is Summer

const userValue = prompt("Enter the month");

if (userValue) {
  const month = userValue.toLowerCase();
  let season;

  switch (month) {
    case "september":
    case "october":
    case "november":
      season = "Autumn";
      break;
    case "december":
    case "january":
    case "february":
      season = "Winter";
      break;
    case "march":
    case "april":
    case "may":
      season = "Spring";
      break;
    case "june":
    case "july":
    case "august":
      season = "Summer";
      break;
    default:
      console.log(`the month is invalid`);
      break;
  }
  if (season) {
    console.log(`The season is ${season}`);
  }
} else {
  console.log(`Invalid type`);
}
```

#### ternary

```js
let num1 = 3;
let num2 = 5;

num1 > num2
  ? console.log(`a is greater than b`)
  : console.log(`a is less than b`);
```
