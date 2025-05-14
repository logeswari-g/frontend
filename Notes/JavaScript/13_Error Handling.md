# Error Handling

Error handling in JavaScript is the process of detecting, managing, and responding to runtime errors gracefully, so your code doesn’t crash unexpectedly.

---

## Common JavaScript Errors

| Type             | Description                                           | Example                                |
|------------------|-------------------------------------------------------|----------------------------------------|
| **Syntax Error**  | Incorrect code structure                              | `if (x > 5 {` (missing `)`)            |
| **Reference Error** | Using a variable that hasn’t been declared         | `console.log(a)` when `a` is undefined |
| **Type Error**    | Using a value in an inappropriate way                | `null.toString()`                      |
| **Range Error**   | A number is outside an allowable range               | `new Array(-5)`                        |
| **Eval Error**    | Improper use of `eval()` (rare)                      | `eval('x ===')`                        |
| **URI Error**     | Invalid URI usage in `decodeURI()` or `encodeURI()` | `decodeURI('%')`                       |

---

## try, catch, and finally

### Syntax

```js
try {
  // Code that may cause an error
} catch (error) {
  // Code to handle the error
} finally {
  // (Optional) Always runs, error or not
}
````

---

### Example

```js
try {
  let a = 10;
  let result = a.toUpperCase();
} catch (err) {
  console.log("Error caught:", err.message);
} finally {
  console.log("Execution finished");
}
```

**Output:**

```
Error caught: a.toUpperCase is not a function
Execution finished
```

---

## Purpose of Each Block

| Block     | Description                           |
| --------- | ------------------------------------- |
| `try`     | Contains code that may throw an error |
| `catch`   | Executes if an error occurs           |
| `finally` | Runs always, regardless of error      |

---

## Example

```js
function getUserData(jsonString) {
  try {
    let user = JSON.parse(jsonString); // May throw SyntaxError
    console.log("User name:", user.name);
  } catch (err) {
    console.log("Invalid JSON:", err.message);
  } finally {
    console.log("Finished parsing");
  }
}

getUserData('{"name": "Alice"}');
getUserData('{name: "Alice"}');
```

---