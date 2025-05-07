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
    console.log(element);
    element.innerText = "Clicked!";
    element.style.backgroundColor = "yellow";
  }
</script>
```
---

## Text and Font

| Property         | Description                       |
|------------------|-----------------------------------|
| `color`          | Text color                        |
| `fontSize`       | Size of the text (`"16px"`, etc.) |
| `fontWeight`     | Boldness (`"bold"`, `"normal"`)   |
| `fontFamily`     | Font style (`"Arial"`, etc.)      |
| `textAlign`      | Alignment (`"center"`, `"right"`) |
| `textDecoration` | Underline, line-through, etc.     |

---

## Background and Borders

| Property             | Description                         |
|----------------------|-------------------------------------|
| `backgroundColor`    | Background color                    |
| `border`             | Full border definition              |
| `borderWidth`        | Width of the border                 |
| `borderStyle`        | Solid, dashed, dotted, etc.         |
| `borderColor`        | Border color                        |
| `borderRadius`       | Rounded corners                     |

---

## Layout and Box Model

| Property         | Description                          |
|------------------|--------------------------------------|
| `width`          | Width of the element (`"100px"`)     |
| `height`         | Height of the element                |
| `padding`        | Space inside border                  |
| `margin`         | Space outside border                 |
| `display`        | Box behavior (`"block"`, `"none"`)   |
| `visibility`     | `"visible"` or `"hidden"`            |

---

## Positioning

| Property       | Description                            |
|----------------|----------------------------------------|
| `position`     | `"static"`, `"relative"`, `"absolute"` |
| `top`          | Distance from top                      |
| `left`         | Distance from left                     |
| `right`        | Distance from right                    |
| `bottom`       | Distance from bottom                   |
| `zIndex`       | Stack order                            |

---

## Flexbox (basic)

| Property         | Description                          |
|------------------|--------------------------------------|
| `display`        | `"flex"` to start flex container     |
| `justifyContent` | Align items horizontally             |
| `alignItems`     | Align items vertically               |
| `flexDirection`  | Row or column layout                 |

---

## Other Useful Properties

| Property       | Description                       |
|----------------|-----------------------------------|
| `cursor`       | Pointer type (`"pointer"`, etc.)  |
| `opacity`      | Transparency (`0` to `1`)         |
| `boxShadow`    | Shadow effect                     |
| `overflow`     | Scroll behavior (`"auto"`, etc.)  |
| `transition`   | Smooth animation of changes       |

---