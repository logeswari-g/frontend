# 1. Introduction to CSS

## What is CSS?
CSS (Cascading Style Sheets) is used to style and layout HTML elements.  
It controls how HTML content appears— colors, fonts, spacing, positioning, etc.

## How CSS Works with HTML
CSS can be added to HTML in three ways:
- Inline: Directly inside an HTML tag.
- Internal: Inside a `<style>` tag in the `<head>` section.
- External: In a separate `.css` file linked to the HTML file.

## Types of CSS

### Inline CSS
Applied directly on an element using the `style` attribute.

```html
<p style="color: red;">This is red text.</p>
```

### Internal CSS
Defined in a `<style>` tag inside the HTML document.

```html
<!DOCTYPE html>
<html>
<head>
  <style>
    p {
      color: blue;
    }
  </style>
</head>
<body>
  <p>This is blue text.</p>
</body>
</html>
```

### External CSS
Written in a separate `.css` file and linked to HTML using `<link>`.

```html
<!-- index.html -->
<link rel="stylesheet" href="styles.css">
```

```css
/* styles.css */
p {
  color: green;
}
```

## CSS Syntax

```css
selector {
  property: value;
}
```

Example:

```css
p {
  color: red;
  font-size: 16px;
}
```

---

# 2. CSS Selectors

## Basic Selectors

### Element Selector
Selects all elements of a given type.

```css
p {
  color: purple;
}
```

### Class Selector (`.classname`)
Selects all elements with a specific class.

```html
<p class="note">This is a note.</p>
```

```css
.note {
  color: orange;
}
```

### ID Selector (`#id`)
Selects a specific element with an ID.

```html
<p id="unique">Unique paragraph</p>
```

```css
#unique {
  font-weight: bold;
}
```

## Grouping Selectors
Apply the same styles to multiple elements.

```css
h1, h2, p {
  font-family: Arial;
}
```

## Descendant Selector
Selects elements inside another element.

```css
div p {
  color: brown;
}
```

## Child Selector
Selects only direct children.

```css
div > p {
  color: teal;
}
```

## Pseudo-classes

### `:hover`
Applies styles when mouse hovers over an element.

```css
a:hover {
  color: red;
}
```

### `:first-child`
Targets the first child of a parent.

```css
li:first-child {
  font-weight: bold;
}
```

## Pseudo-elements

### `::before` and `::after`
Inserts content before or after the element content.

```css
p::before {
  content: "Note: ";
  font-weight: bold;
}
```

## Attribute Selectors

### Select by attribute
```css
input[type="text"] {
  border: 1px solid gray;
}
```

### Select if attribute exists
```css
a[target] {
  color: green;
}
```