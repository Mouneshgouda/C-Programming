# 🧠 Identifiers and Variables in C

🗝️ Note: Identifiers are names only — they don’t store data by themselves.

## 🔹 What is an Identifier?

An **identifier** is a **name** used to identify elements in a C program such as:
- Variables  
- Functions  
- Arrays  
- Structures  
- Constants  

It’s simply a *symbolic name* that refers to some entity in the code.

### ✅ Example:
```c
int total;           // 'total' → identifier (variable name)
float averageScore;  // 'averageScore' → identifier
void display();      // 'display' → identifier (function name)
```
---

## 🔹 What is a Variable?

A variable is a named memory location that can store a value of a specific data type.

✅ Example:
```c
int age = 20;

Here:

age → Identifier (name)  
age → Variable (it holds value 20)  
int → Data type (defines type of value stored)

---

## 🔸 Difference Between Identifier and Variable

| Concept | Description | Example | Notes |
|----------|--------------|----------|--------|
| Identifier | A name used to identify variables, functions, arrays, etc. | age, sum, main | It’s just a name |
| Variable | A named memory location that stores a value | int age = 20; | Has both name and data |

---

## ⚙️ Rules for Identifiers in C

- Can contain letters, digits, and underscores (_)
- Must start with a letter or underscore
- Case-sensitive (Age ≠ age)
- Cannot be a C keyword
- No spaces or special symbols allowed

