# PR-C-Circlet
# C Programming Patterns README

## Program Collection

This repository contains C programs demonstrating various patterns using nested loops. Below are the programs included:

### 1. Incrementing Number Triangle
```c
#include <stdio.h>

int main()
{
    for (int i = 1; i <= 5; i++)
    {
        for (int j = 1; j <= i; j++)
        {
            printf("%d ", 40 + j);
        }
        printf("\n");
    }
    return 0;
}
```

![image](https://github.com/user-attachments/assets/ea6a1431-97d7-48e6-ba39-f3d52c7725df)


---

### 2. Sequential Number Pyramid  
```c
#include <stdio.h>

int main()
{
    int num = 11;
    for (int i = 1; i <= 4; i++)
    {
        for (int j = 1; j <= i; j++)
        {
            printf("%d ", num);
            num++;
        }
        printf("\n");
    }
    return 0;
}
```

![image](https://github.com/user-attachments/assets/6c79c96e-f8de-4a70-bac8-8791f8958a0d)


---

### 3. Right-Aligned Number Pattern
```c
#include <stdio.h>

int main()
{
    for (int i = 1; i <= 5; i++)
    {
        for (int s = 1; s <= 6 - i; s++)
        {
            printf("  ");
        }
        for (int j = 6 - i; j <= 5; j++)
        {
            printf("%d ", j);
        }
        printf("\n");
    }
    return 0;
}
```

![image](https://github.com/user-attachments/assets/13007f5d-52ca-4843-87e4-b9166c94168b)



---

### 4. Binary Number Triangle
```c
#include <stdio.h>

int main()
{
    for (int i = 1; i <= 5; i++)
    {
        for (int j = i; j <= 5; j++)
        {
            printf("%d ", j % 2);
        }
        printf("\n");
    }
    return 0;
}
```

![image](https://github.com/user-attachments/assets/ab87a534-6b02-4fed-bbca-7235b02129f5)


---

### 5. Diamond Number Pattern
```c
#include <stdio.h>

int main()
{
    for (int i = 1; i <= 5; i++)
    {
        for (int s = 1; s <= 5 - i; s++)
        {
            printf("  ");
        }
        for (int j = 6 - i; j <= 5; j++)
        {
            printf("%d ", j);
        }
        for (int j = 4; j > 5 - i; j--)
        {
            printf("%d ", j);
        }
        printf("\n");
    }
    return 0;
}
```

![image](https://github.com/user-attachments/assets/38891157-3147-4bc0-8892-9f2130291034)


---

### 6. Symmetric Number Pattern
```c
#include <stdio.h>

int main()
{
    for (int i = 1; i <= 5; i++)
    {
        for (int j = 1; j <= i; j++)
        {
            printf("%d ", j);
        }
        for (int s = 1; s <= 2*(5 - i); s++)
        {
            printf("  ");
        }
        for (int j = i; j >= 1; j--)
        {
            printf("%d ", j);
        }
        printf("\n");
    }
    return 0;
}
```

![image](https://github.com/user-attachments/assets/81a1d91c-cfce-4123-a122-276246e347cd)


---

### 7. Special Star Pattern
```c
#include <stdio.h>

int main()
{
    for (int i = 1; i <= 5; i++)
    {
        for (int j = 1; j <= 5; j++)
        {
            if (i == 1 || j == 1 || i == 3 || j == 5 && !(j == 5 && i == 4) && !(j == 5 && i == 5))
            {
                printf("* ");
            }
            else
            {
                printf("  ");
            }
        }
        printf("\n");
    }
    return 0;
}
```

![image](https://github.com/user-attachments/assets/e9c5d46d-f2b9-4a8c-a270-ba0287814077)


---

## How to Use
1. Compile each program with GCC:
   ```bash
   gcc filename.c -o output
   ```
2. Run the executable:
   ```bash
   ./output
   ```

## License
MIT Licensed - free to use and modify
