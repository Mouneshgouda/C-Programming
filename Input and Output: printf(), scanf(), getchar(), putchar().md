# 🖥️ Input and Output in C

C provides several built-in functions to handle **input** (reading data from the user) and **output** (displaying data on the screen).  
The most commonly used ones are:

- `printf()` – for output  
- `scanf()` – for input  
- `getchar()` – for reading a single character  
- `putchar()` – for displaying a single character  

---

## 🧾 1. printf() – Output Function

**Definition:**  
`printf()` is used to display text or variables on the screen.

**Syntax:**
```c
printf("format string", variable_list);
```
## Example

```c
#include <stdio.h>

int main() {
    int age = 20;
    printf("My age is %d\n", age);
    return 0;
}
```
## output
```c
My age is 20

```

## Common Format Specifiers

| Specifier | Meaning | Example |
|------------|----------|----------|
| %d | Integer | printf("%d", 10); |
| %f | Floating-point number | printf("%f", 3.14); |
| %c | Single character | printf("%c", 'A'); |
| %s | String | printf("%s", "Hello"); |

---

## ⌨️ 2. scanf() – Input Function

**Definition:**  
`scanf()` is used to take input from the user.

**Syntax:**
```c
scanf("format string", &variable_list);
```
## Example

```c
#include <stdio.h>

int main() {
    int age;
    printf("Enter your age: ");
    scanf("%d", &age);
    printf("You entered: %d\n", age);
    return 0;
}
```
## output
```c
Enter your age: 25
You entered: 25
```
# 🔤 3. getchar() – Read a Single Character

**Definition:**  
`getchar()` reads a single character from the standard input (keyboard).

**Example:**
```c
#include <stdio.h>

int main() {
    char ch;
    printf("Enter a character: ");
    ch = getchar();
    printf("You entered: %c\n", ch);
    return 0;
}
```
## Output
```
Enter a character: A
You entered: A
```
# 🔡 4. putchar() – Display a Single Character

**Definition:**  
`putchar()` prints a single character to the screen.

**Example:**
```c
#include <stdio.h>

int main() {
    char ch = 'Z';
    putchar(ch);
    return 0;
}
```
## output
```c
Z
```
# 📚 Summary

| Function | Purpose | Type | Example |
|-----------|----------|------|----------|
| printf() | Displays output on screen | Output | printf("%d", num); |
| scanf() | Takes input from user | Input | scanf("%d", &num); |
| getchar() | Reads a single character | Input | ch = getchar(); |
| putchar() | Prints a single character | Output | putchar(ch); |

