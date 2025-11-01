# 🖋️ Writing and Running the First C Program

Let’s learn how to **write, compile, and run** your very first program in the **C programming language**.

---

## ✍️ Step 1 — Writing the Program

Open any text editor such as:

- **Notepad** (Windows)  
- **VS Code**  
- **Code::Blocks**  
- **Dev-C++**  
- **Turbo C**  
- Or any other IDE that supports C programming

Now, write the following code:

```c
#include <stdio.h>

int main()
{
    printf("Hello, World!");
    return 0;
}
```
# 🖋️ Writing and Running the First C Program

---

## 💾 Save the File

Save the file as **`hello.c`**

> 📝 The **`.c`** extension indicates that this is a **C source code file**.

---

## ⚙️ Step 2 — Compiling the Program

Before you can run the program, it must be **compiled**.

### Using GCC (on Command Line):
```bash
gcc hello.c -o hello
```
# ▶️ Step 3 — Running the Program

After compilation, run the executable file.

---

## 🪟 On Windows:
```bash
hello
```
## 🐧 On Linux/macOS:
```bash
./hello
```
# 🖥️ Output

When you run the program, the output will be:
Hello, World!

---

🎉 **Congratulations!**  
You’ve successfully written, compiled, and executed your very first **C program!**

