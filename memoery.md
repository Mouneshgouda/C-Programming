## malloc
```c
#include <stdio.h>
#include <string.h>

struct Contact {
    char name[32];
    char phone[16];
};

int main() {
    int n, i;
    scanf("%d", &n);

    struct Contact c[n];

    for (i = 0; i < n; i++)
        scanf("%s %s", c[i].name, c[i].phone);

    char q[32];
    scanf("%s", q);

    for (i = 0; i < n; i++)
        if (strcmp(c[i].name, q) == 0) {
            printf("%s\n", c[i].phone);
            return 0;
        }

    printf("Not Found\n");
    return 0;
}
```


























