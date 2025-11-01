# 🧾 Format Specifiers and Escape Sequences in C

Whenever we write a program in C, we have to use **format specifiers** to define the variable type in input and output, and **escape characters** to format the output.

---

## 🧩 Format Specifiers

A **format specifier** in C programming is used to define the type of data we are printing to the output or accepting through the input.  

Through this, we tell the compiler what type of variable we are using for input (while using `scanf()`) or output (while using `printf()`).  

Some examples of format specifiers are `%d`, `%c`, `%f`, etc.

---

### 📋 List of Common Format Specifiers

| Format Specifier | Type |
|------------------|------|
| %c | Used to print a character |
| %d | Used to print the signed integer |
| %f | Used to print the float values |
| %i | Used to print the unsigned integer |
| %l | Used to print the long integer |
| %lf | Used to print the double values |
| %lu | Used to print the unsigned integer or unsigned long integer |
| %s | Used to print the string |
| %u | Used to print the unsigned integer |

---

### 💻 Example

```c
#include <stdio.h>

int main()
{
    char c[100] = "Mounesh";
    printf("Printing a string, %s.", c);
}
```
## output
```c
Printing a string, Mounesh.
```

# 🧠 The %s used in the printf() is a Format Specifier

It tells `printf()` to treat the variable as a **string** and print it accordingly.

---

## 🎯 Escape Sequences

Many programming languages support the concept of **Escape Sequences**.

An **escape sequence** is a series of characters used to control how output appears on the screen.

They are **not displayed directly** when printed — instead, they perform a special function such as adding a new line, inserting a tab, or printing quotes.

**For example:**
- `\t` is used to insert a tab.  
- `\n` is used to add a new line.

---

## 📋 List of Escape Sequences

| Escape Sequence | Description |
|------------------|-------------|
| \t | Inserts a tab space |
| \b | Inserts a backspace |
| \n | Inserts a new line |
| \r | Inserts a carriage return |
| \f | Inserts a form feed |
| \' | Inserts a single quote character |
| \" | Inserts a double quote character |
| \\ | Inserts a backslash character |

---

## 💻 Example

```c
#include <stdio.h>

int main()
{
    printf("Printing inside a double quotation, \"Code With Mounesh\"");
}
```
## Output
```c
Printing inside a double quotation, "Code With Mounesh".
```
## ✅ Summary

- **Format Specifiers** define the **type of data** being read or printed.  
- **Escape Sequences** control **how text is displayed** (formatting the output).  

Together, they make your C programs **clearer, formatted, and more professional!**
