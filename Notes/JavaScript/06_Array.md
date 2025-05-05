## Arrays

### Creating Arrays
Arrays store multiple values in a single variable.

```js
let fruits = ["apple", "banana", "orange"];
```

---

### Accessing and Modifying Elements
Access elements using index (starting from 0). Modify by assigning new values.

```js
let fruits = ["apple", "banana", "orange"];
console.log(fruits[1]);

fruits[1] = "grape";
console.log(fruits);
```

---

### Common Array Methods

#### `push()` – Adds item to the end
```js
fruits.push("mango");
```

#### `pop()` – Removes item from the end
```js
fruits.pop();
```

#### `shift()` – Removes first item
```js
fruits.shift();
```

#### `unshift()` – Adds item to the start
```js
fruits.unshift("kiwi");
```

#### `length` – Returns array size
```js
console.log(fruits.length);
```

#### `slice(start, end)` – Returns part of the array without changing the original
```js
let newFruits = fruits.slice(1, 3);
console.log(newFruits);
```

#### `splice(start, deleteCount, item1, ...)` – Modifies array by removing/adding elements
```js
fruits.splice(1, 1, "pear");
```

---

### Looping Through Arrays

#### Using `for` loop:
```js
let numbers = [1, 2, 3, 4];

for (let i = 0; i < numbers.length; i++) {
  console.log(numbers[i]);
}
```

#### Using `for...of` loop:
```js
for (let num of numbers) {
  console.log(num);
}
```

---