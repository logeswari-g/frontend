## Objects

In JavaScript, an object is a collection of key-value pairs. Each key (also called a property) is a string, and its value can be any data type — a number, string, function, array, or even another object..

### Object Creation

Objects store key–value pairs.

#### Using `{}` (Object Literal)
```js
let person = {
  name: "Alice",
  age: 25
};
```

#### Using `new Object()`
```js
let person = new Object();
person.name = "Alice";
person.age = 25;
```

---

### Accessing and Modifying Properties

#### Dot Notation
```js
console.log(person.name);
person.age = 30;
```

#### Bracket Notation
```js
console.log(person["age"]);
person["name"] = "Bob";
```

---

### Nested Objects

Objects can contain other objects.

```js
let student = {
  name: "John",
  address: {
    city: "Chennai",
    zip: "600001"
  }
};

console.log(student.address.city);
```

---