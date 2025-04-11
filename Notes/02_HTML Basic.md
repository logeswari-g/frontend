# HTML Basics

## 1. Basic HTML Attributes

Attributes provide additional information about HTML elements. They are always specified in the start tag and usually come in pairs like `key="value"`.

### Common Attributes:

### 📌 `id`: Uniquely identifies an element.

  ```html
  <div id="header"></div>
  ```
### 📌`class`: Specifies one or more class names for styling with CSS.

  ```html
  <p class="highlight"></p>
  ```
### 📌 `style`: Adds inline CSS to an element.

  ```html
  <h1 style="color: blue;">Hello</h1>
  ```
### 📌 `title`: Provides additional information, shown as a tooltip.

  ```html
  <abbr title="World Health Organization">WHO</abbr>
  ```
### 📌 `href`: Specifies the URL for links.

  ```html
  <a href="https://example.com">Visit</a>
  ```
### 📌 `src`: Specifies the path to images or external media.

  ```html
  <img src="image.jpg" alt="Sample Image">
  ```
### 📌 `alt` – Provides alternative text for images.

```html
<img src="logo.png" alt="Company Logo">
```

### 📌 `target` – Specifies where to open a linked document.

    1. `_blank`: Opens in a new tab.
    2. `_self`: Opens in the same window (default).

```html
<a href="https://www.google.com" target="_blank">Open Google in new tab</a>
```

### 📌 `disabled` – Disables form elements.

```html
<input type="text" value="Can't edit this" disabled>
```

### 📌 `readonly` – Makes input read-only (user cannot edit the value, but it is still submitted with the form).

```html
<input type="text" value="Read-only value" readonly>
```

### 📌 `checked` – Pre-selects radio/checkbox options(Automatically selects the input when the page loads)

```html
<input type="checkbox" name="subscribe" checked> Subscribe to newsletter
<br>
<input type="radio" name="gender" value="male" checked> Male
<input type="radio" name="gender" value="female"> Female
```

## 2. Basic HTML Tags

HTML tags are used to create HTML elements. They define the structure and content of web pages.

### Structural Tags:
- `<html>`: Root of the HTML document.
- `<head>`: Contains metadata, links, scripts.
- `<body>`: Contains the content visible to users.

### Content Tags:
- `<h1>` to `<h6>`: Headings from most important (`<h1>`) to least (`<h6>`).

```html
<h1>Main Heading (h1)</h1>
<h2>Subheading (h2)</h2>
<h3>Section Title (h3)</h3>
<h4>Subsection (h4)</h4>
<h5>Note (h5)</h5>
<h6>Smallest Heading (h6)</h6>
```

- `<p>`: Paragraphs.

```html
<p>This is a paragraph of text that contains some information.</p>
```

- `<a>`: Anchors (hyperlinks).

```html
<a href="https://www.openai.com" target="_blank">Visit</a>
```

- `<img>`: Images.

```html
<img src="logo.png" alt="Company Logo" width="150" height="100">
```

- `<ul>`, `<ol>`, `<li>`, `<dl>`: Unordered/Ordered lists and list items.

#### Unordered List:

```html
<ul>
  <li>Apple</li>
  <li>Banana</li>
  <li>Cherry</li>
</ul>
```

#### Ordered List:

```html
<ol>
  <li>Wake up</li>
  <li>Brush teeth</li>
  <li>Have breakfast</li>
</ol>
```

#### Description List:
  ```html
  <dl>
    <dt>HTML</dt>
    <dd>HyperText Markup Language</dd>
    <dt>CSS</dt>
    <dd>Cascading Style Sheets</dd>
  </dl>
  ```

- `<div>`: Used as a block-level container.

```html
<div style="background-color: #f0f0f0; padding: 10px;">
  <h2>This is a section</h2>
  <p>Grouped content inside a div.</p>
</div>
```

- `<span>`: Inline container, Used to style part of a line of text.

```html
<p>This is a <span style="color: red;">red word</span> in a sentence.</p>
```

- `<!-- Comments -->`: You can add comments to your HTML source.

```html
<!-- This is a comment -->
```

- `<link>`: Used to **link external resources** to the HTML document.

```html
<link rel="stylesheet" href="styles.css">
<link rel="icon" href="logo.png">
```

- `<iframe>`: An HTML iframe is used to display a web page within a web page.

```html
<iframe src="demo_iframe.html" height="200" width="300" title="Iframe Example"></iframe>
```

---
