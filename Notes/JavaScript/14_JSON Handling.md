#  What is JSON?

**JSON** (JavaScript Object Notation) is a lightweight data format used for storing and exchanging data. It is easy for humans to read and write and easy for machines to parse and generate.

### JSON Format Example

```json
{
  "name": "Alice",
  "age": 25,
  "isStudent": false,
  "skills": ["HTML", "CSS", "JavaScript"]
}
````

---

## Working with JSON in JavaScript

JavaScript provides two main methods for handling JSON:

| Method             | Purpose                                 |
| ------------------ | --------------------------------------- |
| `JSON.stringify()` | Convert JavaScript object → JSON        |
| `JSON.parse()`     | Convert JSON string → JavaScript object |

---

## 1. JSON.stringify()

Converts a JavaScript object to a **JSON string**.

```js
const user = {
  name: "Bob",
  age: 30,
  isAdmin: true
};

const jsonString = JSON.stringify(user);
console.log(jsonString);
```

**Output:**

```
{"name":"Bob","age":30,"isAdmin":true}
```

---

## 2. JSON.parse()

Converts a **JSON string** back to a JavaScript object.

```js
const jsonString = '{"name":"Bob","age":30,"isAdmin":true}';

const userObj = JSON.parse(jsonString);
console.log(userObj.name);  // Bob
console.log(userObj.age);   // 30
```

---

## JSON Rules to Remember

* Keys and string values **must be in double quotes** (`"`)
* JSON **cannot contain functions**, `undefined`, or `Date` objects
* JSON must be a valid JavaScript **object or array structure**

---

## Real-Time Example

### JSON from an API:

```js
const jsonData = '{"title":"Learn JS","completed":false}';

try {
  const data = JSON.parse(jsonData);
  console.log("Title:", data.title);
} catch (err) {
  console.error("Invalid JSON:", err.message);
}
```

---

## Summary

| Task                 | Method             | Example               |
| -------------------- | ------------------ | --------------------- |
| Object → JSON string | `JSON.stringify()` | `JSON.stringify(obj)` |
| JSON string → Object | `JSON.parse()`     | `JSON.parse(jsonStr)` |

---
