## HTML Entities

Some characters in HTML have special meanings (like `<`, `>`, `&`).  
To display them on a webpage, we use **HTML entities**.

### Common HTML Entities:

| Character | Entity Name | Entity Number |
|-----------|-------------|---------------|
| `<`       | `&lt;`      | `&#60;`        |
| `>`       | `&gt;`      | `&#62;`        |
| `&`       | `&amp;`     | `&#38;`        |
| `"`       | `&quot;`    | `&#34;`        |
| `'`       | `&apos;`    | `&#39;`        |
| `©`       | `&copy;`    | `&#169;`       |
| `®`       | `&reg;`     | `&#174;`       |
| `₹`       | `&#8377;`   | (No named entity) |

### Example:

```html
<p>5 &lt; 10 and 10 &gt; 5</p>
```

## HTML Symbols

HTML allows you to display special symbols like currency, math operators, and arrows using entities.

### Examples:

```html
<p>&copy; 2025 Company Name</p>
<p>Price: &#8377;1000</p>
<p>Math: a &ne; b and a &le; b</p>
<p>Arrow: &larr; &uarr; &rarr; &darr;</p>
```

## Using Emojis in HTML

You can directly copy and paste emojis into your HTML, or use their Unicode values.

### Example 1: Direct Emoji

```html
<p>Welcome 🎉</p>
```

### Example 2: Unicode Emoji

```html
<p>Smile: &#128512;</p>
```

Some popular emojis:

| Emoji | Unicode | Description       |
|-------|---------|-------------------|
| 😀    | `&#128512;` | Grinning face      |
| ❤️    | `&#10084;`  | Red heart          |
| 🔥    | `&#128293;` | Fire               |
| ✅    | `&#9989;`   | Check mark         |
| 🕒    | `&#128338;` | Clock face 3:00    |
```
