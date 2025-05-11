# EX 33 C program to read a file name from user and create that file using fopen().
## DATE:11/05/2025
## AIM:
To write a C program to read a file name from user and create that file using fopen().

## Algorithm
1.Start the program and declare a character array to store the file name.

2.Read the file name from the user using scanf().

3.Use fopen() in write mode ("w") to create the file.

4.Check if the file is created successfully and display a message.

5.Close the file using fclose().

## Program:
```
/*
C program to read a file name from user and create that file using fopen().
Developed by: Kamalesh S
RegisterNumber:  212223060108
*/
#include <stdio.h>

int main()
{
    char filename[100];
    FILE *fp;

    printf("Enter the file name to create: ");
    scanf("%s", filename);

    fp = fopen(filename, "w");

    if(fp == NULL)
    {
        printf("File creation failed.\n");
        return 1;
    }

    printf("File '%s' created successfully.\n", filename);
    fclose(fp);

    return 0;
}


```

## Output:

![image](https://github.com/user-attachments/assets/bfb2aaec-e2f7-44df-a01a-70769dcfd719)


## Result:
Thus the program was executed and the output was verified successfully.
