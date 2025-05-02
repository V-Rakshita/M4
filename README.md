# EX-16-LEFT-SHIFT-OPERATION
## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 44 and 3.
3.	Use left shift operator (<<) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```c
#include <stdio.h>
int main() 
{
    int a=44,b=3,shifted;
    shifted = a<<b;
    printf("After shifting 'a' is: %d",shifted);
    return 0;
}
```

## OUTPUT

![Screenshot_2-5-2025_83036_www programiz com](https://github.com/user-attachments/assets/8629d7c0-07a1-4845-845c-49efdffa43d9)

## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT


## AIM

Write a C Program to check whether the two numbers are equal or not using simple if statement.

## ALGORITHM

1.	Start the program.
2.	Read two numbers.
3.	If first number is equal to second number, display both are equal.
4.	Otherwise display both are not equal.
5.	Stop the program.

## PROGRAM
```c
#include <stdio.h>
int main() 
{
    int a,b;
    scanf("%d%d",&a,&b);
    if (a==b)
        printf("The numbers are equal");
    else
        printf("The numbers are not equal");
    return 0;
}
```


## OUTPUT

![Screenshot_2-5-2025_83249_www programiz com](https://github.com/user-attachments/assets/cd27cf19-23f9-48d5-a735-4b7182769541)
  
## RESULT

Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```c
#include <stdio.h>
#include <ctype.h>
int main() 
{
    char str[5];
    int i;
    scanf("%s",&str);
    printf("Lowercase is:\n");
    for (i=0;str[i]!='\0';i++)
        printf("%c",tolower(str[i]));
    return 0;
}
```


## OUTPUT

![Screenshot_2-5-2025_84426_www programiz com](https://github.com/user-attachments/assets/13bb7664-3b94-438e-bec9-625ad56efd76)

## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
## AIM
Write a C Program to count the total number of words in a given string using do While loop.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM
```c
#include <stdio.h>
int main() 
{
    char str[15];
    scanf("%[^\n]s",&str);
    int count=0,i;
    for (i=0;str[i]!='\0';i++)
    {
        if (str[i] == ' ')
            count++;           
    }
    printf("The total number of words are: %d",count+1);
}
```

## OUTPUT

![Screenshot_2-5-2025_85756_www programiz com](https://github.com/user-attachments/assets/780f8c35-ee77-4118-950c-62590c17165d)

## RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS
## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM
Step 1: Start the program.
Step 2: Declare two character arrays c1 and c2 of size 100 to store the strings. Also, declare an integer variable
             flag and initialize it to 0, and i for indexing.      
Step 3: Read the first string c1 using scanf("%[^\n]", c1); — this reads input until a newline is encountered 
            (i.e., can include spaces).
Step 4: Read the second string c2 using scanf("%s", c2); — this reads input until a space or newline (i.e., no 
            spaces in the second string).
Step 5: Start comparing characters of both strings from index i = 0.
Step 6: Repeat the following while neither c1[i] nor c2[i] is '\0' (i.e., end of string):
•	If c1[i] is not equal to c2[i], set flag = 1.
•	Increment i by 1.
Step 7: After the loop, check the value of flag:
•	If flag == 0, print "strings are same".
•	Otherwise, print "strings are not same".
Step 8: End the program.

## PROGRAM
```c
#include <stdio.h>
int main() 
{
    char c1[100],c2[100];
    int flag = 0,i;
    printf("Enter the first string:\n");
    scanf(" %[^\n]s",c1);
    printf("Enter the second string:\n");
    scanf(" %s",c2);
    for (i=0;c1[i]!='\0' || c2[i]!='\0';i++)
    {
        if (c1[i] != c2[i])
            flag = 1;
    }
    if (flag == 0)
        printf("The strings are the same");
    else
        printf("The strings are not the same");
}
```


## OUTPUT
 
![Screenshot_2-5-2025_92056_www programiz com](https://github.com/user-attachments/assets/efd3e9ca-7078-4612-9f7f-3df075713b0f)

## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

