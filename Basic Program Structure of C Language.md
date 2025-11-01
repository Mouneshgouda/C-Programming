# 🧩 Basic Program Structure of C Language

From the given image below, you can see the basic program structure of C language:
<img width="958" height="1080" alt="image" src="https://github.com/user-attachments/assets/56a383e6-91ef-4ca0-b6a0-da91255b582e" />

---

## 📘 Basic Program Structure of C Language

The above mentioned program structure contains following parts:

- **Pre-Processor**  
- **Library/Header Files**  
- **Built-in Functions**

Let’s break down whole program structure and understand the meaning of each part.

---

## ⚙️ Pre-Processor

**`#`** is called as **Pre-processor**.

This tells the compiler that first pre-process (executes) the process of importing a library/header file.

### For example:
The **`#include`** directive is a preprocessor directive that tells the compiler to include the content of a specified file.

```c
#include<stdio.h>
#include<conio.h>
```
# 📚 Library / Header Files

A **library** or **header file** is a file containing **declarations and definitions** of functions, variables, macros, and other constructs that can be reused in various programs.

A header file typically has a **.h** extension  
(e.g., `stdio.h`, `conio.h`, `stdlib.h`).

Header files are included in C source code using the **`#include`** preprocessor directive.

---

## 🧾 Two Commonly Used Header Files (with Full Forms)

- **`stdio.h`** stands for **Standard Input Output Header File**  
- **`conio.h`** stands for **Console Input Output Header File**

> **Note:** `conio.h` is **not a part of the standard C language library**. *(Read more here.)*

---

# 🔧 Built-in Functions

The **built-in functions** come from **library or header files** that are included in a C source code.

### For example:

- The **`printf()`** function is coming from the **`stdio.h`** library.  
- The **`clrscr()`** function is coming from the **`conio.h`** library.  
- The **`getch()`** function is coming from the **`conio.h`** library.

---

# 🧠 Note

The **`main()`** function is a **globally available function** in the C environment.
