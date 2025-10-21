# EX-04 Program to Count the Total Number of Words in a String.

## AIM:
To write a C program that counts and displays the total number of words in a given string.

## ALGORITHM:

1. Start
2. Declare a character array ch[100] to store the input string.
3. Read the entire line of input (including spaces) using:

    a. scanf("%[^\n]%*c", ch);
5. Find the length of the string using strlen(ch) and store it in len.
6. Initialize a variable count = 0.
7. Use a for loop from i = 0 to i < len:

   a. If ch[i] == ' ', increment count by 1.
9. After the loop, print count + 1 (since the number of words = spaces + 1).
10. Stop

## PROGRAM:
```
#include <stdio.h>
#include <string.h>

int main()
{
    char ch[100];
    printf("Enter an string: ");
    scanf("%[^\n]%*c",ch);
    int len = strlen(ch);
    int count = 0;
    for(int i = 0; i < len; i++)
    {
        if(ch[i] == ' ')
        {
            count++;
        }
    }
    printf("Total number of words: %d",count + 1);
}
```

## OUTPUT:
<img width="666" height="131" alt="image" src="https://github.com/user-attachments/assets/6af69dde-294d-4be2-bc39-39eb48921d2c" />

## RESULT:
The program successfully counts and displays the total number of words in a given string using a do-while loop.
