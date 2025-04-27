NAME:G Theja sree
REGISTER NUMBER:21224110056
EX-01-Datatypes-Operators
AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

ALGORITHM:
Declare three character variables to store the input characters.
Use the scanf function to read the characters one by one from the user.
Print the characters in reverse order using the printf function.
End the program.
PROGRAM:4
```
#include <stdio.h>
int main()
{
    char ch1, ch2, ch3;
    printf("Enter first character: ");
    scanf(" %c", &ch1);
    printf("Enter second character: ");
    scanf(" %c", &ch2);
    printf("Enter third character: ");
    scanf(" %c", &ch3);
    printf("Characters in reverse order: %c %c %c\n", ch3, ch2, ch1);
    return 0;
}
```

OUTPUT:
![image](https://github.com/user-attachments/assets/f2623ab3-040b-411c-ba9f-685e08b1a7e4)

RESULT:
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.

EX-02- Conditional-Statements
AIM:
Write a C program to read A values and check whether A is positive number or not.

ALGORITHM:
Declare a variable to store the input value A.
Use the scanf function to read the value of A from the user.
Check if the value of A is greater than zero.
If A is greater than zero, print a message indicating that it's a positive number.
Otherwise, print a message indicating that it's not a positive number. 6.End the program.



PROGRAM:
```
#include <stdio.h>
int main() 
{
    int A;
    printf("Enter a value: ");
    scanf("%d", &A);
    if (A > 0)
    {
        printf("%d is a positive number.\n", A);
    }
    else 
    {
        printf("%d is not a positive number.\n", A);
    }
    return 0;
}
```
OUTPUT:
![image](https://github.com/user-attachments/assets/09bb76a4-717b-4cf5-9b15-afbc56f5072e)


RESULT:
Thus the program to read A values and check whether A is positive number or not has been executed successfully.

EX-03- Operators-Expressions
AIM:
Write a program to find minimum between two fraction numbers using conditional operator or ternary operator.

ALGORITHM:
Declare variables to store the two fraction numbers and the result.
Use the printf function to prompt the user to enter the first fraction number (numerator and denominator separately).
Use the scanf function to read the numerator and denominator of the first fraction.
Repeat steps 2 and 3 to get the second fraction from the user.
Calculate the decimal values of both fractions by dividing the numerators by the denominators.
Use the conditional (ternary) operator to compare the decimal values and store the minimum value in the result variable.
Print the minimum value.
PROGRAM:
```
#include <stdio.h>
int main() 
{
    int num1, den1, num2, den2;
    float frac1, frac2, min;
    printf("Enter numerator and denominator of first fraction: ");
    scanf("%d%d", &num1, &den1);
    printf("Enter numerator and denominator of second fraction: ");
    scanf("%d%d", &num2, &den2);
    frac1 = (float)num1 / den1;
    frac2 = (float)num2 / den2;
    min = (frac1 < frac2) ? frac1 : frac2;
    printf("Minimum value between the two fractions is: %.2f\n", min);
    return 0;
}
```
OUTPUT:
![image](https://github.com/user-attachments/assets/c60a6fda-3891-437e-82d5-5db5b2144181)


RESULT:
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.

EX-04- Using Conditional Statements
AIM:
Write a C program to check whether the input value is equal to 1 using simple if statement

ALGORITHM:
Declare a variable to store the input value.
Use the scanf function to read the input value from the user.
Use an if statement to check if the input value is equal to 1.
If the condition in the if statement is true, print a message indicating that the input value is equal to 1.
Otherwise, print a message indicating that it's not equal to 1.
End the program.
PROGRAM:
```
#include <stdio.h>

int main() {
    int value;
    printf("Enter a value: ");
    scanf("%d", &value);
    
    if (value == 1) {
        printf("The input value is equal to 1.\n");
    } else {
        printf("The input value is not equal to 1.\n");
    }
    
    return 0;
}
```

OUTPUT:
![image](https://github.com/user-attachments/assets/eb7f3ac4-d06e-4ee0-96df-67059f894c56)


RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully

EX-05- Calculating Total, Percentage, And Division Using Conditional Statements
AIM:
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determines the division (First, Second, Pass, or Fail) based on the percentage and minimum marks criteria.

ALGORITHM:
Start
Declare integer variables m1, m2, m3 for marks, and float variables tot, per.
Input the marks for three subjects.
Calculate total marks: tot = m1 + m2 + m3
Calculate percentage: per = tot / 3
Display total and percentage.
Check if all marks are greater than or equal to 40:
If yes: a. If percentage >= 60: Print “Division = First” b. Else if percentage >= 48: Print “Division = Second” c. Else if percentage >= 36: Print “Division = Pass”
Else: Print “Division = Fail”
End
PROGRAM:
```
#include <stdio.h>
int main()
{
    int m1, m2, m3;
    float tot, per;
    printf("Enter marks of three subjects: ");
    scanf("%d%d%d", &m1, &m2, &m3);
    tot = m1 + m2 + m3;
    per = tot / 3;
    printf("Total Marks = %.2f\n", tot);
    printf("Percentage = %.2f\n", per);
    if (m1 >= 40 && m2 >= 40 && m3 >= 40)
    {
        if (per >= 60)
	{
            printf("Division = First\n");
        }
	else if (per >= 48)
	{
            printf("Division = Second\n");
        } 
	else if (per >= 36) 
	{
            printf("Division = Pass\n");
        }
    } 
    else
    {
        printf("Division = Fail\n");
    }
    
    return 0;
}
```
OUTPUT:
![image](https://github.com/user-attachments/assets/2f1f3ddd-91d7-4fc9-944b-8befbe50de2e)
![image](https://github.com/user-attachments/assets/f429d77c-cbd2-4414-9be4-c572ace22eb8)


RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.
