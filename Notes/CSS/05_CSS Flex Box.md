
# CSS Flexbox

CSS Flexbox (Flexible Box Layout) is a layout model designed to distribute space and align items in a container.

---

## Flex Container

To start using Flexbox, apply `display: flex` to a container.

```css
.container {
  display: flex;
}
```

---

## Main Properties of Flex Container

### 1. `flex-direction`
Defines the direction of the main axis (row or column).

```css
.container {
  flex-direction: row | row-reverse | column | column-reverse;
}
```

### 2. `justify-content`
Aligns items along the **main axis**.

```css
.container {
  justify-content: flex-start | flex-end | center | space-between | space-around | space-evenly;
}
```

### 3. `align-items`
Aligns items along the **cross axis**.

```css
.container {
  align-items: stretch | flex-start | flex-end | center;
}
```

### 4. `align-content`
Aligns **multiple rows** of items (when flex-wrap is enabled).

```css
.container {
  align-content: flex-start | flex-end | center | space-between | space-around | stretch;
}
```

### 5. `flex-wrap`
Allows items to wrap onto multiple lines.

```css
.container {
  flex-wrap: nowrap | wrap | wrap-reverse;
}
```

---

## Flex Item Properties

### 1. `flex`
Shorthand for `flex-grow`, `flex-shrink`, and `flex-basis`.

```css
.item {
  flex: 1;
}
```

### 2. `order`
Controls the order of items (default is 0).

```css
.item {
  order: 1;
}
```

### 3. `align-self`
Overrides the container's `align-items` for individual items.

```css
.item {
  align-self: auto | flex-start | flex-end | center | baseline | stretch;
}
```
---
