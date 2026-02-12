# 🐍 Python Data Types and Control Flow

---

# 📚 Table of Contents

- Data Types
  - Numeric Types
  - Boolean Type
  - String
  - List
  - Tuple
  - Set
  - Dictionary
- Control Flow
  - Conditional Statements
  - Loops
  - Loop Control Statements
  - Nested Structures
  - Match Case

---

# 🧩 Python Data Types

Data types define the type of value that can be stored in a variable.  
Python automatically determines the data type when a value is assigned.

---

## 🔢 1. Numeric Types

Python supports three main numeric types:

| Type     | Description              | Example   |
|----------|--------------------------|------------|
| `int`    | Whole numbers            | `10`, `-5` |
| `float`  | Decimal numbers          | `3.14`     |
| `complex`| Numbers in form `a + bj` | `2+3j`     |

```python
a = 10
b = 3.14
c = 2 + 3j
```

Integers store whole numbers, floats store decimal values, and complex numbers are written in the form `a + bj`.

---

## ✅ 2. Boolean Type

Boolean data type has only two values:

- `True`
- `False`

```python
is_student = True
```

Boolean values are mainly used in decision-making and conditional statements.

---

## 🔤 3. String (`str`)

A string is a sequence of characters enclosed in single or double quotes.  
Strings are ordered and immutable, which means their content cannot be changed after creation.

```python
name = "Python"
print(name[0])
```

Strings are commonly used to store text such as names, messages, or sentences.

---

## 📋 4. List

A list is used to store multiple values in a single variable.

- Ordered  
- Mutable  
- Allows duplicate values  

```python
numbers = [1, 2, 3, 4]
```

### Common List Methods

```python
numbers.append(5)     # Adds element at the end
numbers.remove(2)     # Removes first occurrence of value
```

Lists are widely used because they allow modification after creation.

---

## 📌 5. Tuple

A tuple is similar to a list but is immutable.

- Ordered  
- Cannot be modified after creation  

```python
coordinates = (10, 20)
```

Tuples are used when data should remain constant.

---

## 🎯 6. Set

A set is an unordered collection of unique elements.

- Unordered  
- No duplicates  
- Mutable  

```python
unique_numbers = {1, 2, 3, 3}
```

### Common Set Methods

```python
unique_numbers.add(4)      # Adds element
unique_numbers.remove(1)   # Removes element
```

Sets automatically remove duplicate values.

---

## 📖 7. Dictionary

A dictionary stores data in key-value pairs.

- Mutable  
- Keys must be unique  

```python
student = {
    "name": "Saurav",
    "age": 21
}
```

### Common Dictionary Methods

```python
student.keys()       # Returns all keys
student.get("age")   # Safely accesses value
```

Dictionaries are useful for storing related data like student information, product details, etc.

---

# 🔁 Control Flow in Python

Control flow determines the order in which statements are executed in a program.  
It allows programs to make decisions and repeat actions.

---

## 🔀 1. Conditional Statements

Conditional statements are used for decision-making.

### if Statement

```python
if age >= 18:
    print("Eligible")
```

The `if` statement executes a block of code only if the condition is true.

---

### if-else Statement

```python
if number % 2 == 0:
    print("Even")
else:
    print("Odd")
```

`if-else` is used when there are two possible outcomes.

---

### if-elif-else Statement

```python
if marks >= 90:
    print("Grade A")
elif marks >= 75:
    print("Grade B")
else:
    print("Grade C")
```

Used when multiple conditions need to be checked.

---

## 🔄 2. Loops

Loops are used to repeat a block of code multiple times.

---

### for Loop

```python
for i in range(5):
    print(i)
```

The `for` loop is generally used when the number of iterations is known.

---

### while Loop

```python
while count <= 5:
    print(count)
```

The `while` loop runs as long as the condition remains true.

---

## ⛔ 3. Loop Control Statements

### break

```python
break
```

Stops the loop completely.

---

### continue

```python
continue
```

Skips the current iteration and moves to the next one.

---

### pass

```python
pass
```

Acts as a placeholder and does nothing.

---

## 🔂 4. Nested Structures

Nesting means placing one control structure inside another.

```python
for i in range(3):
    for j in range(2):
        print(i, j)
```

Nested structures are useful for solving complex problems.

---


---


