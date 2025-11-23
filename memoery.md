```c
#include <stdio.h>

int main() {
    FILE *fn;
    fn=fopen("Hi.txt","w");
    printf("creat");

}
```
```c
#include <stdio.h>

int main() {
    FILE *fn;
    fn=fopen("Hi.txt","r");
    char line[1000];

    while(fgets(line,sizeof(line),fn)){
        printf("%s\n",line);
    }
    fclose(fn);

}
```

```
#include <stdio.h>

int main() {
    FILE *fn;
    fn=fopen("Hi.txt","w");
    fprintf(fn,"Hi this meee");
    fclose(fn);

}
```

```
#include <stdio.h>

int main() {
    FILE *fn;
    fn=fopen("Hi.txt","a");
    fputs("Hi this meee thsjk",fn);
    fclose(fn);

}
```

```c
#include <stdio.h>
int main(){
    FILE *fn=fopen("Mounesh.txt","r");
    char line[1000];

    while(fgets(line,sizeof(line),fn)){
        printf("%s\n",line);

        fseek(fn,0,SEEK_END);
        long size=ftell(fn);
        printf("%ld",size);
    }
    
}
```

## binary

```c
#include <stdio.h>

int main(){
    FILE *fn;
    int arr[5]={1,2,3,4,5};
    fn=fopen("hii.bin","wb");
    fwrite(arr,sizeof(int),5,fn);
    fclose(fn);

    printf("done");
    
}
```

```c
#include <stdio.h>

int main(){
    FILE *fn;
    int arr[5],i;
    fn=fopen("hii.bin","rb");
    fread(arr,sizeof(int),5,fn);
    fclose(fn);
    for(i=0;i<5;i++){
        printf("%d",arr[i]);
    }
    printf("done");
    
}
```



```
#include <stdio.h>

int main() {
    if (remove("Hi.txt") == 0) {
        printf("File deleted successfully!\n");
    } 
    return 0;
}
```

##
```
#include <stdio.h>

int main() {
    // Rename Hi.txt to newname.txt
    if (rename("hii.bin", "newname.txt") == 0) {
        printf("File renamed successfully!\n");
    }

    return 0;
}
```
```
#include <stdio.h>
#define DEBUG

int main() {
#ifdef DEBUG
    printf("Debug mode is ON\n");
#endif
    return 0;
}
```

