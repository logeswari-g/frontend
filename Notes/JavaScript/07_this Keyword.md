### What is `this`?

In JavaScript, the `this` keyword refers to the **object that is currently calling the function**. Its value depends on the **context in which it is used**.

---

### 1. In an Object Method  
Inside a method, `this` refers to the **object the method belongs to**.

```js
let person = {
  name: "Asha",
  greet: function () {
    console.log("Hello, my name is " + this.name);
  }
};

person.greet();
```

### 2. In a Regular Function

In a normal function (not inside an object), `this` refers to the **global object** (`window` in browser).

```js
function show() {
  console.log(this);
}

show();
```

---

### 3. In an Event Listener

In an event listener, `this` refers to the **HTML element** that triggered the event.

```html
<button onclick="showMessage(this)">Click me</button>

<script>
  function showMessage(element) {
    console.log(this);
    element.innerText = "Clicked!";
    this.style.background-color = "yellow";
  }
</script>
```

---