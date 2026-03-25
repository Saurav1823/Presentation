
# JavaScript Core Concepts

## Regular Function
A regular function is a function declared using the `function` keyword.  
It has its own `this`, can be used as a constructor, and is hoisted.

## Arrow Function
An arrow function is a function declared using `=>`.  
It does not have its own `this`, cannot be used as a constructor, and is not hoisted.

---

## Difference Between Regular and Arrow Functions

| Feature           | Regular Function          | Arrow Function           |
|------------------|-------------------------|-------------------------|
| Syntax           | `function name(){}`      | `const name = () => {}` |
| `this`           | Has its own `this`       | Inherits `this` from parent |
| Constructor      | Can be used with `new`   | Cannot be used with `new` |
| Hoisting         | Hoisted                  | Not hoisted             |

---

## Code Examples

### Hoisting Example
```javascript
// Regular function is hoisted
greet();
function greet() {
    console.log("Hello from regular function");
}

// Arrow function is not hoisted
sayHi(); // Error
const sayHi = () => {
    console.log("Hello from arrow function");
};
````

---

### `this` Example

```javascript id="bifi91"
const obj = {
    name: "John",
    regular: function() {
        console.log(this.name);
    },
    arrow: () => {
        console.log(this.name);
    }
};

obj.regular(); // John
obj.arrow();   // undefined
```

---

### Constructor Example

```javascript id="9m1md7"
// Regular function as constructor
function Person(name, age) {
    this.name = name;
    this.age = age;
}

const user1 = new Person("John", 25);
console.log(user1.name); // John
console.log(user1.age);  // 25

// Arrow function cannot be used as constructor
const PersonArrow = (name, age) => {
    this.name = name;
    this.age = age;
};

const user2 = new PersonArrow("John", 25); // Error
```

---

## Difference Between `==` and `===`

| Operator | Meaning                                    |
| -------- | ------------------------------------------ |
| `==`     | Checks value only, converts type if needed |
| `===`    | Checks value and type, no conversion       |

```javascript id="dhrcqi"
console.log(5 == "5");   // true
console.log(5 === "5");  // false
```

---

## Difference Between `null` and `undefined`

| Feature | null                | undefined                |
| ------- | ------------------- | ------------------------ |
| Meaning | Intentionally empty | Not assigned             |
| Type    | object              | undefined                |
| Set by  | Developer           | JavaScript automatically |

```javascript id="q8xsfx"
let a;
console.log(a); // undefined

let b = null;
console.log(b); // null
```

---

## Why `value === undefined` is Better than `!value`

* `!value` checks for all falsy values (`0`, `""`, `false`, `null`, `undefined`)
* `value === undefined` only checks if the variable is undefined

```javascript id="sza0o1"
let value = 0;

if (!value) {
    console.log("Falsy value"); // Runs because 0 is falsy
}

if (value === undefined) {
    console.log("Undefined value"); // Does not run
}
```

```
```
