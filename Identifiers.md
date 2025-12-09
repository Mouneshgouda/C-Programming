https://colab.research.google.com/drive/1HESsVCu6sIAmaakHmepT1d0XFx7e8iuN#scrollTo=X0qyVPh3gXGj


https://colab.research.google.com/drive/1_xU0RCQfChSvx_LH8HUejc9ZBC8Go14Y#scrollTo=yikxKvG_1tsM


https://colab.research.google.com/drive/19K4UKIi2-ikKdEWqkssbeBW8iNj7D9VJ#scrollTo=fsbNm3GqxQSz


https://colab.research.google.com/drive/1oEHSwg9-GPtMOwYjWAG5EW8r7a5s1Vxq?usp=sharing

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

