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

Need to use minmax() while using autofit or auto-fill

| Feature      | auto-fill                                  | auto-fit                                |
|--------------|---------------------------------------------|------------------------------------------|
| Empty slots  | Reserves space for invisible columns        | Collapses empty columns                  |
| Behavior     | Keeps the grid size even if items are missing | Makes columns stretch to fill space   |
| Use case     | You want the layout to keep the structure   | You want items to grow and fill the row  |

```css
.grid {
  display: grid;
  gap: 10px;
  padding: 10px;
}

.auto-fill {
  grid-template-columns: repeat(auto-fill, minmax(150px, 1fr));
}

.auto-fit {
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
}

.grid-item {
  background: #4caf50;
  color: white;
  padding: 20px;
  text-align: center;
  font-weight: bold;
}
```
```html
<h2>auto-fill</h2>
<div class="grid auto-fill">
  <div class="grid-item">1</div>
  <div class="grid-item">2</div>
  <div class="grid-item">3</div>
</div>

<h2>auto-fit</h2>
<div class="grid auto-fit">
  <div class="grid-item">1</div>
  <div class="grid-item">2</div>
  <div class="grid-item">3</div>
</div>

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

Named Grid Areas in CSS Grid allow you to assign semantic names to different parts of your layout using grid-template-areas, which makes grid layouts more readable, maintainable, and easier to manage.

In the Grid Container:

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
```

In the Grid Items:

```css
.header { grid-area: header; }
.sidebar { grid-area: sidebar; }
.main { grid-area: main; }
.footer { grid-area: footer; }
```

## How It Works

Each row in grid-template-areas is a string.
Each string consists of area names (identifiers like "header", "main").
The same name can be repeated to span columns or rows.
You can use a . (dot) to define an empty cell.

---
