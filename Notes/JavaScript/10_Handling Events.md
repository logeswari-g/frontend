# Handling Events

## What is an Event?

An **event** is something that happens in the browser (user action or browser action) that JavaScript can respond to.

Examples:
- Mouse click
- Key press
- Page load
- Input change

---

## Ways to Handle Events

### 1. Inline Event Handling (HTML Attribute)

Attaching JavaScript directly in the HTML tag.

```html
<button onclick="sayHello()">Click Me</button>

<script>
  function sayHello() {
    alert("Hello!");
  }
</script>
````

---

### 2. DOM Property Method

Assigning a function to an element's event property.

```html
<button id="btn">Click Me</button>

<script>
  document.getElementById("btn").onclick = function() {
    alert("You clicked the button!");
  };
</script>
```

**Note**: Only one function can be assigned per event type using this method.

---

### 3. Using `addEventListener()`

Attach multiple event handlers without overwriting previous ones.

```html
<button id="btn">Click Me</button>

<script>
  function handler1() {
    console.log("Handler 1 executed");
  }

  function handler2() {
    console.log("Handler 2 executed");
  }

  const button = document.getElementById("btn");

  button.addEventListener("click", handler1);
  button.addEventListener("click", handler2);
</script>
```

**Note**: Both `handler1` and `handler2` will run when the button is clicked.

---

## Event Object

An **event object** is automatically passed to the event handler and contains details about the event.

```javascript
button.addEventListener("click", function(event) {
  console.log("Event type:", event.type);
  console.log("Clicked element ID:", event.target.id);
});
```

---

## Multiple Events on the Same Element

```html
<button id="myBtn">Hover or Click</button>

<script>
  const btn = document.getElementById("myBtn");

  btn.addEventListener("click", () => {
    alert("Button clicked!");
  });

  btn.addEventListener("mouseover", () => {
    console.log("Mouse is over the button");
  });

  btn.addEventListener("mouseout", () => {
    console.log("Mouse left the button");
  });
</script>
```

---

## Removing Event Handlers

```javascript
function greet() {
  console.log("Hello");
}

btn.addEventListener("click", greet);

// Later...
btn.removeEventListener("click", greet);
```

**Note**: You can remove event listeners only if the function is **named** (not anonymous).

---

## Common Event Types

| Event Type  | Description                    |
| ----------- | ------------------------------ |
| `click`     | Mouse click                    |
| `dblclick`  | Double-click                   |
| `mouseover` | Cursor enters the element      |
| `mouseout`  | Cursor leaves the element      |
| `keydown`   | Key is pressed down            |
| `keyup`     | Key is released                |
| `submit`    | Form is submitted              |
| `change`    | Input value changes            |
| `load`      | Page or image finishes loading |

---