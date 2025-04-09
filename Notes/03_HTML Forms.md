## 🧾 HTML Form Elements

These tags are used to collect user input on web pages.

---

### 📋 `<form>` – Form Container

Wraps all input fields and defines how form data is submitted.

```html
<form action="/submit-form" method="post">
  <!-- form fields go here -->
</form>
```

- `action`: URL where the form data is sent.
- `method`: HTTP method (`get` or `post`).

---

### 🧾 `<input>` – Input Field

Used for various types of user input.

```html
<input type="text" name="username" placeholder="Enter your name">
<input type="email" name="email" placeholder="Enter your email">
<input type="password" name="password" placeholder="Enter password">
<input type="checkbox" name="subscribe" checked> Subscribe
<input type="radio" name="gender" value="male"> Male
<input type="radio" name="gender" value="female"> Female
<input type="number" name="age" placeholder="e.g., 25">
<input type="date" name="dob">
```

- `type`: Defines the input type (`text`, `email`, `password`, `checkbox`, `radio`, etc.).
- `name`: Used to identify the data when submitted.
- `placeholder`: Hints at the expected input.

---

### 📝 `<textarea>` – Multi-line Text Input

Allows users to enter longer text.

```html
<textarea name="message" rows="4" cols="30" placeholder="Enter your message here..."></textarea>
```

---

### 🔘 `<button>` – Clickable Button

Triggers form submission or other actions.

```html
<button type="submit">Submit</button>
<button type="reset">Reset</button>
<button type="button" onclick="alert('Clicked!')">Click Me</button>
```

---

### ⬇️ `<select>` and `<option>` – Dropdown Menu

Creates a list of options for the user to choose from.

```html
<select name="country">
  <option value="in">India</option>
  <option value="us">United States</option>
  <option value="uk">United Kingdom</option>
</select>
```

- `<option>` defines each choice in the dropdown.
- `value`: The value that gets submitted when the option is selected.

---

### ✅ Complete Example

```html
<form action="/submit" method="post">
  <label>Name:</label>
  <input type="text" name="name" required><br><br>

  <label>Message:</label><br>
  <textarea name="message" rows="4" cols="40"></textarea><br><br>

  <label>Country:</label>
  <select name="country">
    <option value="in">India</option>
    <option value="ca">Canada</option>
    <option value="au">Australia</option>
  </select><br><br>

  <input type="checkbox" name="agree" required> I agree to the terms <br><br>

  <button type="submit">Send</button>
</form>
```

---
