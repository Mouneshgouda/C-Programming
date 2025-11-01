# 🌍 Scope and Lifetime of Variables in C

In C programming, every variable has a **scope** (where it can be accessed)  
and a **lifetime** (how long it exists in memory).

Understanding these two concepts helps manage memory efficiently and avoid unexpected behavior.

---

## 🔹 1. Scope of Variables

**Scope** defines the part of the program where a variable is accessible.

### Types of Scope:

| Type | Description | Example |
|------|--------------|----------|
| **Local Scope** | Variable declared inside a function or block; accessible only within that block. | `int x` inside a function |
| **Global Scope** | Variable declared outside all functions; accessible throughout the program. | `int x` declared before `main()` |
| **Block Scope** | Variable declared within curly braces `{}` (inside loops, if statements, etc.). | Variable inside `{}` |
| **Function Scope** | Function name is visible only within its declaration context. | Declared function names |

---

### 🧩 Example: Scope

```c
#include <stdio.h>

int globalVar = 10; // Global variable

int main() {
    int localVar = 20; // Local variable

    {
        int blockVar = 30; // Block variable
        printf("Inside block: %d\n", blockVar);
    }

    printf("Global: %d\n", globalVar);
    printf("Local: %d\n", localVar);
    // printf("%d", blockVar); // ❌ Error: blockVar not accessible here
```
# ⏳ 2. Lifetime of Variables

**Lifetime** determines how long a variable exists in memory during program execution.

---

## 🧮 Types of Lifetime

| Storage Class | Lifetime | Memory Location | Keyword |
|----------------|-----------|------------------|----------|
| **Automatic** | Created when function is called; destroyed when function ends | Stack | `auto` *(default)* |
| **Static** | Exists throughout program execution | Data Segment | `static` |
| **Register** | Stored in CPU registers for faster access | CPU Register | `register` |
| **External** | Exists for entire program; can be shared across files | Data Segment | `extern` |

---

## 🧩 Example: Lifetime

```c
#include <stdio.h>

void demo() {
    static int count = 0; // Static variable
    int temp = 0;         // Automatic variable

    count++;
    temp++;

    printf("Static: %d, Auto: %d\n", count, temp);
}

int main() {
    for (int i = 0; i < 3; i++) {
        demo();
    }
    return 0;
}
```
## Output
```c
Static: 1, Auto: 1
Static: 2, Auto: 1
Static: 3, Auto: 1
```
# 🧠 Explanation

- The **static variable** retains its value between function calls.  
- The **automatic variable** is re-created each time the function runs.

---

## ✅ Summary

- **Automatic variables:** Temporary, created and destroyed within function calls.  
- **Static variables:** Persistent, maintain value for the program’s entire runtime.  
- **Register variables:** Fast access, stored in CPU registers.  
- **External variables:** Global, shared across files.

    return 0;
}
