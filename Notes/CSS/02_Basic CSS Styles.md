## CSS Colors

### Named Colors
```css
p {
  color: blue;
}
```

### HEX (Hexadecimal)
```css
h1 {
  color: #ff5733;
}
```

### RGB (Red, Green, Blue)
```css
div {
  color: rgb(255, 0, 0); /* red */
}
```

### RGBA (RGB + Alpha)
```css
div {
  background-color: rgba(0, 0, 255, 0.5); /* semi-transparent blue */
}
```

### HSL (Hue, Saturation, Lightness)
```css
h2 {
  color: hsl(120, 100%, 50%); /* bright green */
}
```

### HSLA (HSL + Alpha)
```css
h2 {
  color: hsla(240, 100%, 50%, 0.5); /* semi-transparent blue */
}
```

---

## CSS Text & Fonts

### `font-family`, `font-size`, `font-style`, `font-weight`
```css
p {
  font-family: Arial, sans-serif;
  font-size: 16px;
  font-style: italic;
  font-weight: bold;
}
```

### `text-align`, `text-decoration`, `text-transform`
```css
h1 {
  text-align: center;
  text-decoration: underline;
  text-transform: uppercase;
}
```

### Line height and letter spacing
```css
p {
  line-height: 1.6;
  letter-spacing: 1px;
}
```

---

## CSS Backgrounds

### `background-color`, `background-image`
```css
body {
  background-color: #f0f0f0;
  background-image: url('bg.jpg');
}
```

### `background-repeat`, `background-size`, `background-position`
```css
body {
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
}
```

---

## CSS Borders

### Border styles, widths, and colors
```css
div {
  border: 2px solid black;
}
```

### Rounded corners (`border-radius`)
```css
button {
  border: 1px solid gray;
  border-radius: 10px;
}
```

---

## CSS Display and Visibility

### `display`: `block`, `inline`, `inline-block`, `none`
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

### `visibility`: `visible`, `hidden`
```css
p {
  visibility: hidden;
}
```

### `overflow`: `hidden`, `scroll`, `auto`
```css
.container {
  width: 200px;
  height: 100px;
  overflow: auto;
}
```
```

---