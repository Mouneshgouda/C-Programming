# 🧱 C Language Building Blocks: Keywords, Identifiers, Constants, and Variables

In the C programming language, every program is built upon a few fundamental components known as **building blocks**.  
These are essential for writing meaningful and functional C programs.

---

## 🏷️ 1. Keywords

**Keywords** are **reserved words** in C that have predefined meanings and purposes.  
They are part of the C language syntax and **cannot be used as identifiers (like variable names or function names).**

Examples of keywords in C include:
```c
- auto break case char const
- continue default do double else
- enum extern float for goto
- if int long register return
- short signed sizeof static struct
- switch typedef union unsigned void
- volatile while
```

> 🧠 **Note:** All keywords in C are written in **lowercase**.

---

## 🪪 2. Identifiers

**Identifiers** are the **names** given to various program elements such as **variables, functions, arrays, or structures**.

They are user-defined and must follow certain rules.

### Rules for Identifiers:
- Must **begin with a letter** (A–Z or a–z) or an underscore (`_`).
- Can contain **letters, digits, and underscores**.
- **No spaces** or special characters are allowed.
- **Case-sensitive** (`Age`, `age`, and `AGE` are different).
- **Cannot be a keyword.**

### Example:
```c
int age;
float totalMarks;
char student_name[50];
```
# 🔢 3. Constants

**Constants** are fixed values that do not change during program execution.

They can be of different types such as:

- Integer constants  
- Floating-point constants  
- Character constants  
- String constants  
- Symbolic constants (defined using `#define`)

### 🧩 Example:
```c
#define PI 3.14
const int MAX = 100;
const char GRADE = 'A';
```

# 📦 4. Variables

**Variables** are named memory locations used to store data that can change during program execution.

Each variable must be declared with a **data type** before it is used.

---

## 🧱 Syntax
```c
data_type variable_name = value;

int age = 20;
float salary = 45000.50;
char grade = 'A';

```
# 🧠 Note
The value of a variable can be modified throughout the program, **unlike a constant**.

---

## 📚 Summary

| Building Block | Description | Example |
|----------------|-------------|----------|
| **Keyword** | Reserved word with predefined meaning | `int`, `return` |
| **Identifier** | User-defined name for a variable or function | `totalMarks` |
| **Constant** | Fixed value that doesn’t change | `#define PI 3.14` |
| **Variable** | Named memory location that can store and change data | `int age = 20;` |

---

✅ **Understanding these building blocks is the first step toward mastering the C programming language!**


