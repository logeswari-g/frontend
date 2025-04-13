# Semantic Elements in HTML

## What are Semantic Elements?

**Semantic HTML elements** clearly describe their meaning in a human- and machine-readable way.  
They add **meaning and structure** to the content, improving accessibility, SEO, and maintainability.

---

## Common Semantic Elements

| Tag            | Description |
|----------------|-------------|
| `<header>`     | Defines a header for a page or section |
| `<nav>`        | Defines navigation links |
| `<main>`       | Specifies the main content |
| `<section>`    | Represents a standalone section |
| `<article>`    | Self-contained content (e.g., blog post, news article) |
| `<aside>`      | Content related to the main content (e.g., sidebar) |
| `<footer>`     | Defines a footer for a page or section |
| `<figure>`     | Used to group media content with caption |
| `<figcaption>` | Caption for the `<figure>` content |
| `<mark>`       | Highlights or marks important text |
| `<time>`       | Represents date/time information |

---

## 📦 Example: Blog Layout Using Semantic Elements

```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Semantic Example</title>
</head>
<body>

  <header>
    <h1>My Blog</h1>
    <nav>
      <a href="#">Home</a> |
      <a href="#">About</a>
    </nav>
  </header>

  <main>
    <article>
      <header>
        <h2>Post Title</h2>
        <p>Published on <time datetime="2025-04-10">April 10, 2025</time></p>
      </header>
      <section>
        <p>This is the main content of the article.</p>
        <figure>
          <img src="image.jpg" alt="Example Image">
          <figcaption>Figure 1: An example image</figcaption>
        </figure>
      </section>
    </article>

    <aside>
      <h3>Related Links</h3>
      <ul>
        <li><a href="#">Another article</a></li>
        <li><a href="#">Resource link</a></li>
      </ul>
    </aside>
  </main>

  <footer>
    <p>Copyright © 2025</p>
  </footer>

</body>
</html>
```

---
