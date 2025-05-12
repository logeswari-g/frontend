JavaScript provides built-in **popup dialog functions** that interact with users:

| Function    | Purpose                         | Returns              |
|-------------|----------------------------------|----------------------|
| `alert()`   | Display a message                | `undefined`          |
| `prompt()`  | Ask the user to enter input      | String or `null`     |
| `confirm()` | Ask for confirmation (OK/Cancel) | `true` or `false`    |

---

## 1. `alert()`

### Purpose
Displays a **popup message** to the user with an OK button.

### Syntax
```javascript
alert("Message to show");
````

### Example

```javascript
alert("Welcome to Student Registration!");
```

---

## 2. `prompt()`

### Purpose

Displays a **dialog box asking for user input**. It returns the value entered by the user (as a string).

### Syntax

```javascript
let result = prompt("Message", "Default value");
```

### Example

```javascript
let name = prompt("Enter your name:", "Student");
```

---

## 3. `confirm()`

### Purpose

Displays a **confirmation box** with OK and Cancel buttons.
Returns `true` if the user clicks OK, and `false` if Cancel.

### Syntax

```javascript
let choice = confirm("Are you sure?");
```

### Example

```javascript
let isConfirmed = confirm("Do you want to submit?");
```

---