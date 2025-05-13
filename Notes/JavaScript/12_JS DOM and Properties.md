# JavaScript DOM: Methods and Properties

The **Document Object Model (DOM)** represents the structure of a web page in a tree-like format. JavaScript uses **DOM methods and properties** to access, change, add, or delete HTML elements.

---

## DOM Access Methods

| Method                    | Description                                   | Example                                 |
|---------------------------|-----------------------------------------------|-----------------------------------------|
| `getElementById()`        | Selects one element by ID                     | `document.getElementById("myDiv")`      |
| `getElementsByClassName()`| Selects elements by class (HTMLCollection)    | `document.getElementsByClassName("box")`|
| `getElementsByTagName()`  | Selects elements by tag name                  | `document.getElementsByTagName("p")`    |
| `querySelector()`         | Returns the first matching CSS selector       | `document.querySelector(".menu")`       |
| `querySelectorAll()`      | Returns all matches of a CSS selector         | `document.querySelectorAll("div.box")`  |

---

## Example:

```html
<div id="greet" class="message">Hello</div>

<script>
  let msg = document.getElementById("greet");
  console.log(msg.textContent); // Output: Hello
</script>
```

---

## DOM Element Properties

| Property       | Description                             | Example                           |
|----------------|-----------------------------------------|-----------------------------------|
| `innerHTML`    | Gets/sets HTML content of an element    | `el.innerHTML = "<b>Hi</b>"`      |
| `textContent`  | Gets/sets plain text content            | `el.textContent = "Hello"`        |
| `value`        | Gets/sets value of form input fields    | `input.value`                     |
| `id`           | Gets/sets the `id` of an element        | `el.id = "newId"`                 |
| `className`    | Gets/sets full class string             | `el.className = "red bold"`       |
| `classList`    | Access to class methods (add, remove)   | `el.classList.add("active")`      |
| `style`        | Access to inline CSS styles             | `el.style.color = "blue"`         |
| `href`, `src`  | Gets/sets link or image path            | `img.src = "img.jpg"`             |

---

## Common DOM Modification Methods

| Method             | Purpose                                 | Example                                 |
|--------------------|------------------------------------------|-----------------------------------------|
| `createElement()`  | Create a new HTML element                | `document.createElement("p")`           |
| `appendChild()`    | Add a child element                      | `parent.appendChild(child)`             |
| `removeChild()`    | Remove a child element                   | `parent.removeChild(child)`             |
| `setAttribute()`   | Set any attribute (e.g., `id`, `href`)   | `el.setAttribute("id", "box")`          |
| `getAttribute()`   | Get value of an attribute                | `el.getAttribute("href")`               |
| `replaceChild()`   | Replace one child with another           | `parent.replaceChild(newEl, oldEl)`     |

---

## Example: Create and Add New Element

```javascript
let newPara = document.createElement("p");         // create
newPara.textContent = "New paragraph added";       // edit
document.body.appendChild(newPara);                // add
```

---

## Summary

| Category        | Examples                                      |
|----------------|-----------------------------------------------|
| Access Elements| `getElementById`, `querySelector`             |
| Read/Write Data| `innerHTML`, `textContent`, `value`           |
| Modify Elements| `setAttribute`, `classList.add()`             |
| Create/Remove  | `createElement`, `appendChild`, `removeChild` |
