
# CSS Positioning

CSS positioning allows you to control how elements are placed in the document flow.

## Types of Positioning

### 1. `static` (default)
**Elements are placed according to the normal document flow.**
```css
div {
  position: static;
}
```
- You can't use `top`, `left`, `right`, or `bottom` with static.

---

### 2. `relative`
**Element is positioned relative to its normal position.**
```css
div {
  position: relative;
  top: 10px;
  left: 20px;
}
```
- Space for the element is still reserved in the layout.
- Moves **without affecting** other elements.

---

### 3. `absolute`
**Element is positioned relative to the nearest positioned ancestor (not static).**
```css
.parent {
  position: relative;
}

.child {
  position: absolute;
  top: 0;
  right: 0;
}
```
- If no positioned ancestor exists, it's relative to `<body>`.
- It’s removed from the normal document flow.

---

### 4. `fixed`
**Element is positioned relative to the viewport (browser window).**
```css
div {
  position: fixed;
  bottom: 0;
  right: 0;
}
```
- Stays in place even when scrolling.
- Commonly used for sticky headers/footers.

---

### 5. `sticky`
**Toggles between `relative` and `fixed` based on scroll.**
```css
div {
  position: sticky;
  top: 0;
}
```
- Sticks to a position when you scroll past it.
- Requires a defined `top`, `left`, etc.

---
