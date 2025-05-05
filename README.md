
# EX-01-Datatypes-Operators
## AIM:
Write a C program to read 3 characters one by one and print the characters in a reverse order.

## ALGORITHM:
1.	Declare three character variables to store the input characters.
2.	Use the scanf function to read the characters one by one from the user.
3.	Print the characters in reverse order using the printf function.
4.	End the program.

## PROGRAM:
#include <stdio.h>

int main() {
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



## OUTPUT:
Enter first character: A
Enter second character: B
Enter third character: C
Characters in reverse order: C B A


















## RESULT:
Thus the program to read 3 characters one by one and print the characters in a reverse order has been executed successfully.


# EX-02- Conditional-Statements
## AIM:
Write a C program to read A values and check whether A is positive number or not.

# ALGORITHM:
1.	Declare a variable to store the input value A.
2.	Use the scanf function to read the value of A from the user.
3.	Check if the value of A is greater than zero.
4.	If A is greater than zero, print a message indicating that it's a positive number. 
5.	Otherwise, print a message indicating that it's not a positive number.
6.End the program.

# PROGRAM:
#include <stdio.h>
int main()
{
    int A;
    printf("Enter a number (A): ");
    scanf("%d", &A);
    if (A > 0) {
        printf("A is a positive number.\n");
    } else {
        printf("A is not a positive number.\n");
    }
    return 0;
}


# OUTPUT:
User Input:
Enter a number (A): 15
Program Output:
A is a positive number.

yser input:
Enter a number (A): -7
program output:
A is not a positive number.

# RESULT:
Thus the program to read A values and check whether A is positive number or not has been executed successfully.
 
 
 


# EX-03- Operators-Expressions
## AIM:
Write a program to find minimum between two fraction numbers using conditional operator or ternary operator.

## ALGORITHM:
1.	Declare variables to store the two fraction numbers and the result.
2.	Use the printf function to prompt the user to enter the first fraction number (numerator and denominator separately).
3.	Use the scanf function to read the numerator and denominator of the first fraction.
4.	Repeat steps 2 and 3 to get the second fraction from the user.
5.	Calculate the decimal values of both fractions by dividing the numerators by the denominators.
6.	Use the conditional (ternary) operator to compare the decimal values and store the minimum value in the result variable.
7.	Print the minimum value.

## PROGRAM:
#include <stdio.h>

int main() {
    float num1, num2, min
    printf("Enter first number: ");
    scanf("%f", &num1);
    printf("Enter second number: ");
    scanf("%f", &num2);
    min = (num1 < num2) ? num1 : num2;
    printf("Minimum number is: %.2f\n", min);
    return 0;
}


## OUTPUT:
Input:
Enter first number: 5.25
Enter second number: 3.14
Output:
Minimum number is: 3.14










## RESULT:
Thus the program to find minimum between two fraction numbers using conditional operator or ternary operator has been executed successfully.




# EX-04- Using Conditional Statements

## AIM:
Write a C program to check whether the input value is equal to 1 using simple if statement

## ALGORITHM:
1.	Declare a variable to store the input value.
2.	Use the scanf function to read the input value from the user.
3.	Use an if statement to check if the input value is equal to 1.
4.	If the condition in the if statement is true, print a message indicating that the input value is equal to 1.
5.	Otherwise, print a message indicating that it's not equal to 1.
6.	End the program.

## PROGRAM:
#include <stdio.h>

int main() {
    int value;
    printf("Enter a number: ");
    scanf("%d", &value);
    if (value == 1) {
        printf("The value is equal to 1.\n");
    }
    return 0;
}

## OUTPUT:

Input:
Enter a number: 1
Output:
The value is equal to 1.










	

## RESULT:
Thus the program to check whether the input value is equal to 1 using simple if statement has been executed successfully



# EX-05- Calculating Total, Percentage, And Division Using Conditional Statements 
## AIM:
To write a C program that reads marks of three subjects, calculates the total and percentage, and then determines the division (First, Second, Pass, or Fail) based on the percentage and minimum marks criteria.
## ALGORITHM:
1.	Start
2.	Declare integer variables m1, m2, m3 for marks, and float variables tot, per.
3.	Input the marks for three subjects.
4.	Calculate total marks: tot = m1 + m2 + m3
5.	Calculate percentage: per = tot / 3
6.	Display total and percentage.
7.	Check if all marks are greater than or equal to 40:
8.	If yes:
a.	If percentage >= 60: Print “Division = First”
b.	Else if percentage >= 48: Print “Division = Second”
c.	Else if percentage >= 36: Print “Division = Pass”
9.	Else: Print “Division = Fail”
10.	End
## PROGRAM:

#include <stdio.h>

int main() {
    int m1, m2, m3;
    int total;
    float percentage;
    printf("Enter marks for subject 1: ");
    scanf("%d", &m1);
    printf("Enter marks for subject 2: ");
    scanf("%d", &m2);
    printf("Enter marks for subject 3: ");
    scanf("%d", &m3);
    total = m1 + m2 + m3;
    percentage = total / 3.0;
    printf("Total Marks = %d\n", total);
    printf("Percentage = %.2f%%\n", percentage);
    if (m1 < 33 || m2 < 33 || m3 < 33) {
        printf("Result: Fail (One or more subjects below passing marks)\n");
    } else if (percentage >= 60) {
        printf("Result: First Division\n");
    } else if (percentage >= 45) {
        printf("Result: Second Division\n");
    } else if (percentage >= 33) {
        printf("Result: Pass (Third Division)\n");
    } else {
        printf("Result: Fail\n");
    }
    return 0;
}


## OUTPUT:
Input:
Enter marks for subject 1: 70
Enter marks for subject 2: 55
Enter marks for subject 3: 60
Output:m
Total Marks = 185
Percentage = 61.67%
Result: First Division


## RESULT:
The program successfully takes three subject marks, calculates the total and percentage, and correctly determines the division based on predefined grading logic.

