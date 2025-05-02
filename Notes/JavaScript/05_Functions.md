

### Function Declaration
Defines a named function.

#### **Syntax:**
```js
function greet(name) {
  return "Hello, " + name;
}
```

#### **Example:**
```js
console.log(greet("John"));
```

---

### Function Expression
Assigns an anonymous function to a variable.

#### **Example:**
```js
const add = function(x, y) {
  return x + y;
};
console.log(add(3, 4));
```

---

### Parameters and Return Values

- Functions can accept parameters and return results.
- `return` sends a value back to the caller.

#### **Example:**
```js
function square(num) {
  return num * num;
}
console.log(square(5));
// Output: 25
```

---