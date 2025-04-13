# HTML Computer Code Elements

HTML provides special elements to display **computer code**, **keyboard input**, and other **technical content** in a way that’s easy to read and understand.

---

## 1. `<code>` – Code Snippets

Used to wrap inline or block-level programming code.

```html
<p>Use the <code>print()</code> function to display output in Python.</p>
```

---

## 2. `<pre>` – Preformatted Text

Used when you want to preserve exact spacing, indentation, and line breaks.

```html
<pre>
def greet():
    print("Hello, World!")
</pre>
```
You can also combine `<pre>` with `<code>` for displaying formatted code blocks.

```html
<pre><code>
function sum(a, b) {
  return a + b;
}
</code></pre>
```

---

## 3. `<kbd>` – Keyboard Input

Used to indicate what the user should type on the keyboard.

```html
<p>Press <kbd>Ctrl</kbd> + <kbd>C</kbd> to copy.</p>
```

---

## 4. `<samp>` – Sample Output

Displays output from a computer program or command-line interface.

```html
<p>Program Output: <samp>Hello, user!</samp></p>
```

---

## 5. `<var>` – Variables

Defines a variable name in code, math, or text. Often italicized by default.

```html
<p>The formula is <var>a</var> + <var>b</var> = <var>c</var>.</p>
```

---
