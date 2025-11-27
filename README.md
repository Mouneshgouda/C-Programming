# 📘 C Program Solutions

1. Fibonacci Series  
2. Count digits in a number  
3. Search an element in an array  
4. Count vowels and consonants  
5. Find the middle value of an array  
6. Reverse a string
7. Your task is to write a program that takes the temperature in Celsius as input, converts it to Fahrenheit
8. Write a program to calculate and display the total electricity bill amount
9. sort them by using bubble sort new sequence.
10. Implement a function to copy a string
11. the system must dynamically manage storage for uneven rows of data—much like a ragged 2D array.
12. *Precision Code** or a **Regular Code*

---

## ✨ 1. Fibonacci Series

```c
#include <stdio.h>

int main() {
    int n = 10, a = 0, b = 1, c;

    printf("%d %d ", a, b);

    for(int i = 2; i < n; i++) {
        c = a + b;
        printf("%d ", c);
        a = b;
        b = c;
    }
```

## 2.Count digits in a number

```c
#include <stdio.h>

int main() {
    int num = 123456;
    int count = 0;

    while (num != 0) {
        count++;
        num /= 10;
    }

    printf("Number of digits: %d", count);

    return 0;
}
```

##  3.Search an element in an array

```c

#include <stdio.h>

int main() {
    int arr[] = {10, 20, 30, 40, 50};
    int target = 30, found = 0;

    for(int i = 0; i < 5; i++) {
        if(arr[i] == target) {
            found = 1;
            break;
        }
    }

    if(found)
        printf("Element found");
    else
        printf("Element not found");

    return 0;
}
```

## 4.Count vowels and consonants  

```c
#include <stdio.h>
#include <ctype.h>

int main() {
    char str[] = "Hello World";
    int vowels = 0, consonants = 0;

    for(int i = 0; str[i] != '\0'; i++) {
        char c = tolower(str[i]);
        if(c >= 'a' && c <= 'z') {
            if(c=='a' || c=='e' || c=='i' || c=='o' || c=='u')
                vowels++;
            else
                consonants++;
        }
    }

    printf("Vowels: %d\n", vowels);
    printf("Consonants: %d\n", consonants);

    return 0;
}
```
## 5. Find the middle value of an array

```c
#include <stdio.h>

int main() {
    int arr[] = {5, 10, 15, 20, 25};
    int midIndex = sizeof(arr)/sizeof(arr[0]) / 2;

    printf("Middle value: %d", arr[midIndex]);

    return 0;
}

```
## 6.Reverse a string 

```c
#include <stdio.h>
#include <string.h>

int main() {
    char str[] = "Hello";
    int len = strlen(str);

    printf("Reversed string: ");
    for(int i = len - 1; i >= 0; i--) {
        putchar(str[i]);
    }

    return 0;
}
```

