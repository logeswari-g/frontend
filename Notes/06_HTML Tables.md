# HTML Tables

HTML tables are used to **display data in rows and columns**, much like a spreadsheet. They're built using specific table-related tags.

---

## Basic Table Structure

```html
<table>
  <tr>
    <th>Heading 1</th>
    <th>Heading 2</th>
  </tr>
  <tr>
    <td>Data 1</td>
    <td>Data 2</td>
  </tr>
</table>
```

---

## Table Tags & Their Meaning

| Tag       | Description                                  |
|-----------|----------------------------------------------|
| `<table>` | The container for all table content          |
| `<tr>`    | Table row                                    |
| `<th>`    | Table header cell (bold + centered by default) |
| `<td>`    | Table data cell (regular data)               |
| `<caption>` | Table title (optional, appears above the table) |

---

## Example with Caption

```html
<table border="1">
  <caption>Monthly Sales</caption>
  <tr>
    <th>Month</th>
    <th>Sales</th>
  </tr>
  <tr>
    <td>January</td>
    <td>$1000</td>
  </tr>
  <tr>
    <td>February</td>
    <td>$1200</td>
  </tr>
</table>
```

---

## Additional Attributes

| Attribute     | Use/Meaning                                     |
|---------------|-------------------------------------------------|
| `border`      | Adds a border around table and cells            |
| `colspan`     | Makes a cell span multiple columns              |
| `rowspan`     | Makes a cell span multiple rows                 |
| `cellpadding` | Adds spacing inside each cell                   |
| `cellspacing` | Adds space between table cells                  |

---