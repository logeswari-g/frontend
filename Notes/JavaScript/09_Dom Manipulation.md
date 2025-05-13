# JavaScript DOM Element Selection
DOM stands for Document Object Model.

It is a programming interface provided by the browser that allows JavaScript to interact with, modify, and manipulate HTML and CSS on a web page.

When a web page loads, the browser converts the HTML into a tree-like structure of objects — this structure is the DOM.

## 1. `getElementById()`

* Selects **one** element by its `id`.

```js
let title = document.getElementById("main-title");
console.log(title.textContent);
```

---

## 2. `getElementsByClassName()`

* Selects **all** elements with a given class (returns an list).

```js
let paragraphs = document.getElementsByClassName("info");
console.log(paragraphs[0].textContent);
```

---

## 3. `getElementsByTagName()`

* Selects all elements with a given tag name.

```js
let listItems = document.getElementsByTagName("li");
console.log(listItems[1].textContent);
```

---

## 4. `querySelector()`

* Selects the **first** matching element using a **CSS selector**.

```js
let firstItem = document.querySelector(".item");
console.log(firstItem.textContent);
```

---

## 5. `querySelectorAll()`

* Selects **all** matching elements using a **CSS selector** (returns a NodeList).

```js
let allParagraphs = document.querySelectorAll(".info");
allParagraphs.forEach(p => console.log(p.textContent));
```

---

## Selecting Nested Elements

```js
let nestedSpan = document.querySelector("#container span");
console.log(nestedSpan.textContent);
```
---
