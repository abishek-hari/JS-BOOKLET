# Js-Intro

### JavaScript

JavaScript (JS) is a lightweight interpreted (or just-in-time compiled) programming language with first-class functions, which is also known as the scripting language for webpages.

- Javascript

1. lightweight
2. cross-platform
3. single-threaded
4. Interpreted

### 3 ways to write js

1. Inline
2. Internal
3. External

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>JS-50</title>
  </head>
  <body>
    <section>
      <div>
        <h1>WELCOME TO JS-50</h1>
      </div>
      <!-- Inline Javascript-->
      <button onclick="alert('hello guys')">hello there!</button>
      <button class="btn">random btn</button>
      <button class="btn">random btn</button>
      <button class="btns">random btn</button>
    </section>
    <!-- Internal Javascript-->
    <script>
      const random = document.querySelectorAll(".btn");
      random.forEach((item) =>
        item.addEventListener("click", () => {
          alert("tenet");
        })
      );
    </script>
    <!--External Javascript-->
    <script src="./script.js"></script>
  </body>
</html>
```

### Variables

Variables are containers of data.
Variables are used to store data in a memory location. When a variable is declared, a memory location is reserved.
When a variable is assigned to a value (data), the memory space will be filled with that data.
To declare a variable, we use var, let, or const keywords.

A variable is like abox what we put inside the box is the value that we assign to a variable thats the data and the label that we put on the box is the name of our variable

```js
// Syntax
let name = joe;
```

### Static and Dynamic languages

- static and dynamic languages

1. static languages: when we declare a variable the type of that variable is set and cannot be changed in future
2. Dynamic language : the type of the variable can change at runtime.
