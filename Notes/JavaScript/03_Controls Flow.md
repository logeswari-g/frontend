
## Control Flow

### `if`, `else if`, `else`

Used for decision-making in your code. The `if` block is executed if the condition is **true**, while `else` and `else if` provide alternative actions when the condition is **false** or another condition is **true**.

#### **Syntax:**
```js
if (condition) {
  // code block if condition is true
} else if (anotherCondition) {
  // code block if another condition is true
} else {
  // code block if all conditions are false
}
```

#### **Example:**
```js
let age = 20;

if (age < 13) {
  console.log("Child");
} else if (age >= 13 && age < 18) {
  console.log("Teenager");
} else {
  console.log("Adult");
}
// Output: "Adult"
```

---

### `switch` Statement

The `switch` statement is a more **efficient** way to handle multiple conditions compared to a long series of `if...else` statements.

#### **Syntax:**
```js
switch (expression) {
  case value1:
    // code block if expression === value1
    break;
  case value2:
    // code block if expression === value2
    break;
  default:
    // code block if no case matches
}
```

#### **Example:**
```js
let fruit = "banana";

switch (fruit) {
  case "apple":
    console.log("This is an apple.");
    break;
  case "banana":
    console.log("This is a banana.");
    break;
  default:
    console.log("Unknown fruit.");
}
// Output: "This is a banana."
```

---

### Ternary Operator (`condition ? true : false`)

A shorter way to write **if-else** conditions, making code cleaner and more concise. It is used for simple decisions.

#### **Syntax:**
```js
condition ? expressionIfTrue : expressionIfFalse;
```

#### **Example:**
```js
let age = 16;
let result = (age >= 18) ? "Adult" : "Minor";
console.log(result);

---