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
```
#include <stdio.h>

int main() {
    int a = 44, b = 3;
    int result;
    result = a << b;
    printf("Result of %d << %d = %d\n", a, b, result);

    return 0;
}

```

## OUTPUT

<img width="486" height="186" alt="{82AE8CBB-BF7E-4470-B12A-D1073072AA69}" src="https://github.com/user-attachments/assets/1a9e6991-94bc-43b9-8edf-ea436f017a78" />








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
```
#include <stdio.h>

int main() {
    int num1, num2;
    printf("Enter first number: ");
    scanf("%d", &num1);

    printf("Enter second number: ");
    scanf("%d", &num2);
    if (num1 == num2) {
        printf("Both are equal\n");
    } else {
        printf("Both are not equal\n");
    }

    return 0;
}
```

## OUTPUT
       <img width="535" height="253" alt="{EE7A9CC9-CA5B-450E-932C-BA27FFE22A8D}" src="https://github.com/user-attachments/assets/70302868-adab-43c9-ba6b-a3711ddd1264" />
    
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
```
#include <stdio.h>
#include <ctype.h>  
int main() {
    char str[100];
    int i = 0;
    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin); 
    while(str[i]) {
        str[i] = tolower(str[i]);
        i++;
    }
    printf("Lowercase string: %s", str);

    return 0;
}

```
## OUTPUT

<img width="457" height="188" alt="{A5B8B83D-D260-4EDD-849A-D076D2A6B675}" src="https://github.com/user-attachments/assets/56c9ee4c-d155-47ad-b588-73d4ad0d4875" />



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
```
#include <stdio.h>

int main() {
    char str[100];
    int i, count = 0;
    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin); 
    for(i = 0; str[i] != '\0'; i++) {
        if(str[i] == ' ') {
            count++;
        }
    }
    printf("Number of spaces in the string: %d\n", count);

    return 0;
}
```
## OUTPUT

<img width="515" height="204" alt="{3BDDC9E7-C553-44ED-9E2D-B8842F434ADE}" src="https://github.com/user-attachments/assets/632fcb42-4e0b-49df-bdcb-4af8e2b4a57b" />




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
```
#include <stdio.h>

int main() {
    char c1[100], c2[100];
    int flag = 0, i = 0;
    printf("Enter first string: ");
    scanf("%[^\n]", c1);
    getchar();
    printf("Enter second string: ");
    scanf("%s", c2);
    while(c1[i] != '\0' && c2[i] != '\0') {
        if(c1[i] != c2[i]) {
            flag = 1;
            break; 
        }
        i++;
    }
    if(c1[i] != '\0' || c2[i] != '\0') {
        flag = 1;
    }
    if(flag == 0) {
        printf("Strings are same\n");
    } else {
        printf("Strings are not same\n");
    }

    return 0;
}

```


## OUTPUT
 <img width="463" height="217" alt="{C74CA43D-5EA4-445E-8E5C-A01E2920D435}" src="https://github.com/user-attachments/assets/3f60c6ac-6c17-4240-b096-41ebf6f0dd26" />


## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

