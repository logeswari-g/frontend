## CSS Colors

### Named Colors
**Use predefined color names like `red`, `blue`, etc.**
```css
p {
  color: blue;
}
```

### HEX (Hexadecimal)
**Use hex codes starting with `#` to define colors.**
```css
h1 {
  color: #ff5733;
}
```

### RGB (Red, Green, Blue)
**Define colors using Red, Green, and Blue values (0–255).**
```css
div {
  color: rgb(255, 0, 0);
}
```

### RGBA (RGB + Alpha)
**Adds transparency with the alpha channel (0 to 1).**
```css
div {
  background-color: rgba(0, 0, 255, 0.5);
}
```

### HSL (Hue, Saturation, Lightness)
**Colors based on hue (0–360), saturation, and lightness.**
```css
h2 {
  color: hsl(120, 100%, 50%);
}
```

### HSLA (HSL + Alpha)
**HSL with transparency using an alpha value.**
```css
h2 {
  color: hsla(240, 100%, 50%, 0.5);
}
```

---

## CSS Text & Fonts

### `font-family`
**Defines the font used for text.**
```css
p {
  font-family: Arial, sans-serif;
}
```

### `font-size`
**Sets the size of the font.**
```css
p {
  font-size: 16px;
}
```

### `font-style`
**Makes text normal, italic, or oblique.**
```css
p {
  font-style: italic;
}
```

### `font-weight`
**Sets how thick or bold the text appears.**
```css
p {
  font-weight: bold;
}
```

### `text-align`
**Aligns text horizontally (`left`, `right`, `center`).**
```css
h1 {
  text-align: center;
}
```

### `text-decoration`
**Adds decoration like underline, overline, line-through.**
```css
h1 {
  text-decoration: underline;
}
```

### `text-transform`
**Controls capitalization (`uppercase`, `lowercase`, `capitalize`).**
```css
h1 {
  text-transform: uppercase;
}
```

### `line-height`
**Sets space between lines of text.**
```css
p {
  line-height: 1.6;
}
```

### `letter-spacing`
**Controls space between letters.**
```css
p {
  letter-spacing: 1px;
}
```

---

## CSS Backgrounds

### `background-color`
**Sets the background color of an element.**
```css
body {
  background-color: #f0f0f0;
}
```

### `background-image`
**Adds an image as the background.**
```css
body {
  background-image: url('bg.jpg');
}
```

### `background-repeat`
**Controls if and how a background image repeats.**
```css
body {
  background-repeat: no-repeat;
}
```

### `background-size`
**Specifies the size of the background image (`cover`, `contain`).**
```css
body {
  background-size: cover;
}
```

### `background-position`
**Sets the starting position of a background image.**
```css
body {
  background-position: center;
}
```

---

## CSS Borders

### Border styles, widths, and colors
**Defines border appearance using style, width, and color.**
```css
div {
  border: 2px solid black;
}
```

### `border-radius`
**Rounds the corners of an element.**
```css
button {
  border-radius: 10px;
}
```

---

## CSS Display and Visibility

### `display: block | inline | inline-block | none`
**Controls how elements are displayed in the layout.**
```css
span {
  display: inline;
}
div {
  display: block;
}
img {
  display: inline-block;
}
.hidden {
  display: none;
}
```

### `visibility: visible | hidden`
**Shows or hides the element but keeps its space.**
```css
p {
  visibility: hidden;
}
```

### `overflow: hidden | scroll | auto`
**Manages content that overflows the element's box.**
```css
.container {
  overflow: auto;
}
```
