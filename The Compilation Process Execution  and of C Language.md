<img width="1400" height="788" alt="image" src="https://github.com/user-attachments/assets/6bc4232b-53ac-4760-bfc6-28c8258f3340" />


# ⚙️ What is Compilation?

**Compilation** is the process the computer takes to transform a program written in a **high-level language** from **source code** into **machine code** that the computer can understand.

---

## 🧾 Source Code

**Source code** appears in a **human-readable text format** and includes instructions that guide the program’s execution.

### Example: Printing “Hello World”
```c
#include<stdio.h>
int main()
{
  printf("Hello World");
  return 0;
}
```


# 4 Stages of Compilation in C Language

The process of compiling a C program involves **four main stages**.  
<img width="865" height="237" alt="image" src="https://github.com/user-attachments/assets/78b041ac-fa56-4323-8089-5405770c53c3" />

Each stage transforms the source code into a different intermediate form, ultimately resulting in an executable file.

---

## 🧩 Stage 1 — Preprocessing

The **preprocessor** is a program that is used to process source code **before it is compiled**.  
It performs several important tasks, including:

- Removing comments  
- Expanding macros  
- Including files  
- Converting source code to expanded code  

**Output file:** `hello.i`

---

## 🧠 Stage 2 — Compiling

The **C compiler** checks for **valid syntax** in the C language.  
If any syntax error is found, the compiler reports it.  

After the expanded code has been syntactically verified, the compiler converts it into **assembly code**.

**Output file:** `hello.s`

---

## ⚙️ Stage 3 — Assembling

In this stage, the **assembler** converts **assembly code** into **pure binary code** or **machine code**, which is known as the **object code**.

**Output file:** `hello.o`

---

## 🔗 Stage 4 — Linking

The **linker** merges all the **object code** from multiple modules and libraries into a single file and produces the **final executable file**.

**Output file:** `hello.exe`

---

<img width="900" height="800" alt="image" src="https://github.com/user-attachments/assets/70e5106d-dcb9-45ec-b9cc-163ba99a690d" />

# 🚀 Execution Process

This is the phase where the **compiled program** is actually **run by the computer**.

---

## 🧩 Steps Involved

1. The **operating system** loads the **executable file** into memory.  
2. The **CPU** begins executing instructions from the **binary file**.  
3. **Output** is generated based on the logic written in the program.

---

## 🎯 Purpose

To **perform the tasks** defined in your code.

---

## 🖥️ Output

The **results of the program**, such as:

- Printed text  
- Calculations  
- Any other specified operation

---

> ✅ The execution process is where your program comes to life — transforming written code into real actions performed by the computer.
<img width="1024" height="1024" alt="image" src="https://github.com/user-attachments/assets/b473bfdb-199a-4665-9b8c-f3d91c46cdd7" />

