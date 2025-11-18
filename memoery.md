## malloc
```c
#include <stdio.h>
#include <stdlib.h>

int main() {
    int *ptr;
    ptr = (int*) malloc(sizeof(int)); // allocate memory for 1 integer

    if (ptr == NULL) {
        printf("Memory not allocated!\n");
        return 1;
    }

    *ptr = 10;
    printf("Value: %d\n", *ptr);

    free(ptr); // free memory
    return 0;
}
```

## calloc
```c
#include <stdio.h>
#include <stdlib.h>

int main() {
    int *arr;
    arr = (int*) calloc(5, sizeof(int)); // allocate array of 5 integers

    for (int i = 0; i < 5; i++) {
        printf("%d ", arr[i]);  // will print 0 0 0 0 0
    }

    free(arr);
    return 0;
}
```

## reallocat

```c
#include <stdio.h>
#include <stdlib.h>

int main() {
    int *ptr = (int*) malloc(2 * sizeof(int));

    ptr[0] = 10;
    ptr[1] = 20;

    // Increase memory for 4 integers
    ptr = (int*) realloc(ptr, 4 * sizeof(int));

    ptr[2] = 30;
    ptr[3] = 40;

    for (int i = 0; i < 4; i++) {
        printf("%d ", ptr[i]);
    }

    free(ptr);
    return 0;
}
```

## array
```c
#include <stdio.h>
#include <stdlib.h>

int main() {
    int *arr;
    int n = 5;

    arr = (int*) malloc(n * sizeof(int));   // allocate array of 5 integers

    for (int i = 0; i < n; i++) {
        arr[i] = i + 1;
    }

    printf("Array using malloc: ");
    for (int i = 0; i < n; i++) {
        printf("%d ", arr[i]);
    }

    free(arr);
    return 0;
}
```
