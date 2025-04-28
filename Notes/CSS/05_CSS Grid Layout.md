# CSS Grid Layout
CSS Grid Layout is a two-dimensional layout system, meaning it can handle both columns and rows. It makes complex layouts easy to build.

## 2. Creating a Grid

Turns an element into a grid container.

```css
.container {
  display: grid;
}
```

---

## 3. Defining Rows and Columns

Defines the number and size of columns in the grid.

```css
.container {
  display: grid;
  grid-template-columns: 200px 200px;
  grid-template-rows: 100px 100px;
}
```

- Use `fr` unit for flexible layouts:

```css
grid-template-columns: 1fr 2fr; /* First column: 1 part, second: 2 parts */
```

- Auto-fit/auto-fill with repeat:

```css
grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
```

---

## 4. Gap (Spacing)

```css
grid-gap: 10px;
```

---

## 5. Placing Grid Items

### a. Line-based placement

```css
.item {
  grid-column: 1 / 3;  /* Starts at column line 1 and ends before 3 */
  grid-row: 2 / 4;
}
```

### b. Grid Area (shorthand)

```css
.item {
  grid-area: 2 / 1 / 4 / 3; /* row-start / col-start / row-end / col-end */
}
```

---

## 6. Named Grid Areas

```css
.container {
  display: grid;
  grid-template-areas:
    "header header"
    "sidebar main"
    "footer footer";
  grid-template-columns: 1fr 3fr;
  grid-template-rows: auto 1fr auto;
}

.header { grid-area: header; }
.sidebar { grid-area: sidebar; }
.main { grid-area: main; }
.footer { grid-area: footer; }
```

---