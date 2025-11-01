# ⚙️ Basic Data Types in C

In the C programming language, **data types** specify the type of data that a variable can hold.  
Each data type requires a different amount of memory and has a specific range of values.

---

## 🧩 Primary Data Types

| Data Type | Description | Memory (in bytes)* | Range / Example |
|------------|--------------|--------------------|-----------------|
| **int** | Used to store integer (whole number) values | 2 or 4 | `int age = 25;` |
| **float** | Used to store single-precision decimal (floating-point) values | 4 | `float price = 99.99;` |
| **char** | Used to store a single character | 1 | `char grade = 'A';` |
| **double** | Used to store double-precision decimal values (more accurate than float) | 8 | `double distance = 12345.6789;` |

> 🧠 **Note:**  
> The size of data types can vary depending on the **compiler** and **system architecture** (16-bit, 32-bit, or 64-bit).

---

## 🧮 Example Program

```c
#include <stdio.h>

int main() {
    int age = 25;
    float price = 99.99;
    char grade = 'A';
    double distance = 12345.6789;

    printf("Age: %d\n", age);
    printf("Price: %.2f\n", price);
    printf("Grade: %c\n", grade);
    printf("Distance: %.4lf\n", distance);

    return 0;
}
```
## Output
```c
Age: 25
Price: 99.99
Grade: A
Distance: 12345.6789
```
