# 🐍 Python Data Types and Control Flow

---

# 📚 Table of Contents

- Data Types
  - Numeric Types
  - Boolean Type
  - Sequence Types
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

Data types define the type of value a variable can store.

---

## 🔢 1. Numeric Types

| Type     | Description        | Example   |
|----------|-------------------|------------|
| `int`    | Integer numbers   | `10`, `-5` |
| `float`  | Decimal numbers   | `3.14`     |
| `complex`| Complex numbers   | `2+3j`     |

```python
a = 10
b = 3.14
c = 2 + 3j
```

---

## ✅ 2. Boolean Type

Boolean has only two values:

- `True`
- `False`

```python
is_student = True
```

---

## 📦 3. Sequence Types

---

### 🔤 String (`str`)

A **string** is a sequence of characters enclosed in quotes (`""` or `''`).  
Strings are **ordered** and **immutable** (cannot be changed after creation).

```python
name = "Python"
print(name[0])     # P
```

---

### 📋 List

- Ordered
- Mutable
- Allows duplicates

```python
numbers = [1, 2, 3, 4]
```

### Common List Methods

```python
numbers.append(5)      # Adds element at end
numbers.remove(2)      # Removes first occurrence
print(numbers)
```

---

### 📌 Tuple

- Ordered
- Immutable

```python
coordinates = (10, 20)
```

---

## 🎯 4. Set

- Unordered
- No duplicates
- Mutable

```python
unique_numbers = {1, 2, 3, 3}
print(unique_numbers)
```

### Common Set Methods

```python
unique_numbers.add(4)       # Adds element
unique_numbers.remove(1)    # Removes element
```

---

## 📖 5. Dictionary

- Key–Value pairs
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
student.keys()      # Returns all keys
student.get("age")  # Safely gets value
```

---

# 🔁 Control Flow in Python

Control flow determines how the program executes statements.

---

## 🔀 1. Conditional Statements

### ▶️ if Statement

```python
age = 18

if age >= 18:
    print("Eligible to vote")
```

---

### ▶️ if-else Statement

```python
number = 5

if number % 2 == 0:
    print("Even")
else:
    print("Odd")
```

---

### ▶️ if-elif-else Statement

```python
marks = 85

if marks >= 90:
    print("Grade A")
elif marks >= 75:
    print("Grade B")
else:
    print("Grade C")
```

---

## 🔄 2. Loops

### 🔁 for Loop

```python
for i in range(5):
    print(i)
```

Looping through list:

```python
fruits = ["apple", "banana", "mango"]

for fruit in fruits:
    print(fruit)
```

---

### 🔁 while Loop

```python
count = 1

while count <= 5:
    print(count)
    count += 1
```

---

## ⛔ 3. Loop Control Statements

### 🔴 break

Stops the loop.

```python
for i in range(10):
    if i == 5:
        break
```

---

### 🟡 continue

Skips current iteration.

```python
for i in range(5):
    if i == 2:
        continue
```

---

### ⚪ pass

Placeholder statement.

```python
for i in range(5):
    pass
```

---

## 🔂 4. Nested Structures

### Nested if

```python
age = 20
citizen = True

if age >= 18:
    if citizen:
        print("Eligible to vote")
```

---

### Nested Loop

```python
for i in range(3):
    for j in range(2):
        print(i, j)
```

---

## 🆕 5. Match Case (Python 3.10+)

```python
day = 2

match day:
    case 1:
        print("Monday")
    case 2:
        print("Tuesday")
    case _:
        print("Invalid")
```

---

