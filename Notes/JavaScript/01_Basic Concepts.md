### What is JavaScript?
JavaScript is a high-level, dynamic programming language used to create interactive effects within web browsers.

---

### History and Evolution (brief)
JavaScript was created in 1995 by Brendan Eich at Netscape.  
Key milestones:
- 1995: Originally called Mocha, renamed to LiveScript, then JavaScript.
- 2009: Node.js introduced for server-side JS.
- 2015: ES6 introduced modern syntax and features.

---

### How JS is used in web development
JavaScript makes websites interactive (e.g., form validation, animations).

**Example:**
```html
<h2 id="message">Welcome!</h2>
<button onclick="changeMessage()">Click Me</button>

<script>
function changeMessage() {
    document.getElementById("message").innerText = "You clicked the button!";
}
</script>
```

---

### Adding JS to HTML: `<script>` tag
JavaScript can be added directly in HTML or linked externally.

**Example:**
```html
<!-- Inline JS -->
<script>
  function changeMessage() {
    document.getElementById("message").innerText = "You clicked the button!";
}
</script>

<!-- External JS -->
<script src="script.js"></script>
```

---

## 2. Basics of JavaScript Syntax

### Statements and Semicolons
Statements are instructions. Semicolons (`;`) mark the end of a statement.

**Example:**
```js
console.log(document.getElementById("message").innerText);
```

---

### 🔹 Comments (`//`, `/* */`)
Used to explain code:
- `//` for single-line
- `/* ... */` for multi-line

**Example:**
```js
// This is a single-line comment
/*
  This is a 
  multi-line comment
*/
```

---

### 🔹 Console output: `console.log()`
Displays output in the browser’s developer console.

**Example:**
```js
console.log("Hello from console!");
```

---

## 3. JavaScript Execution Placement

### 1. JavaScript in `<head>` (without `defer` or `async`)

- Blocks HTML rendering until the script finishes executing.
- DOM elements **below the script tag** may not exist yet when the script runs.

### Example:
```html
<!DOCTYPE html>
<html>
<head>
  <script>
    // This runs before the body is parsed
    console.log(document.getElementById("demo")); // Outputs: null
  </script>
</head>
<body>
  <p id="demo">Hello from body</p>
</body>
</html>
```

### 2. JavaScript in <head> with defer

- defer tells the browser to download the script during parsing, but run it after the HTML is fully parsed.

### Example:
```html
<!DOCTYPE html>
<html>
<head>
  <script defer>
    document.addEventListener("DOMContentLoaded", function () {
        console.log(document.getElementById("demo").innerText);
    });
  </script>
</head>
<body>
  <p id="demo">Hello from body</p>
</body>
</html>
```

### 3. JavaScript in <body> (at the end)

- Since HTML is already loaded, scripts can safely access DOM elements.

### Example:
```html
<!DOCTYPE html>
<html>
<head>
<title>Test</title>
</head>
<body>
  <p id="demo">Hello from body</p>
  <script>
    console.log(document.getElementById("demo").innerText); // Outputs: Hello from body
  </script>
</body>
</html>
```

### 4. External JavaScript File

- Keeps JS code in a separate file, improving modularity and maintainability.
- Use with defer to ensure it executes after HTML is parsed.

### Example:
```html
<!DOCTYPE html>
<html>
<head>
  <script src="script.js" defer></script>
</head>
<body>
  <p id="demo">Hello from external script</p>
</body>
</html>
```

---

## 3. Variables and Data Types

JavaScript provides **three** ways to declare variables:
- `var`
- `let`
- `const`

---

### 1. `var`

- Only accessible within the function it is declared in.
- Can be **re-declared** and **updated**.

### 2. `let`

- Only accessible within `{ ... }` where it was declared.
- Can be **updated**, but **not re-declared** in the same scope.

### 3. `const`

- **Block-scoped**, like `let`.
- Must be **initialized** at the time of declaration.
- Cannot be **reassigned**.
- Good for values that should not change.

### Primitive types: `String`, `Number`, `Boolean`, `null`, `undefined`, `Symbol`
Basic data types that are not objects.

**Example:**
```js
let name = "Alice";         // String
let age = 25;               // Number
let isStudent = true;       // Boolean
let empty = null;           // null
let notDefined;             // undefined
let uniqueId = Symbol();    // Symbol
```

---

### 🔹 Type Checking: `typeof`
Checks the type of a value.

**Example:**
```js
console.log(typeof 123);         // "number"
console.log(typeof "hello");     // "string"
console.log(typeof true);        // "boolean"
```

---
