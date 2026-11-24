// Write a program to check whether a number is positive or negative or zero.
#include <stdio.h>

int main() {
    int num;
    printf("Enter a number: ");
    scanf("%d", &num);
    if (num > 0) {
        printf("Positive number\n");
    } else if (num < 0) {
        printf("Negative number\n");
    } else {
        printf("Zero\n");
    }
    return 0;
}

// Write a program that prints the ASCII values of the characters 'H' and 'f'.
#include <stdio.h>

int main() {
    char ch1 = 'H';
    char ch2 = 'f';
    printf("ASCII value of %c = %d\n", ch1, ch1);
    printf("ASCII value of %c = %d\n", ch2, ch2);
    return 0;
}

// Write a program to add two numbers that accept numbers from the user console.
#include <stdio.h>

int main() {
    int num1, num2, sum;
    printf("Enter two numbers: ");
    scanf("%d %d", &num1, &num2);
    sum = num1 + num2;
    printf("Sum = %d\n", sum);
    return 0;
}

// Write a 

struct Employee {
    int id;
    char name[50];
    float salary;
};

int main() {
    struct Employee emp[5];
    int i;
    for (i = 0; i < 5; i++) {
        printf("Enter ID, Name, and Salary for employee %d: ", i + 1);
        scanf("%d %s %f", &emp[i].id, emp[i].name, &emp[i].salary);
    }
    printf("\nEmployees with salary greater than 50000:\n");
    for (i = 0; i < 5; i++) {
        if (emp[i].salary > 50000) {
            printf("ID: %d, Name: %s, Salary: %.2f\n", emp[i].id, emp[i].name, emp[i].salary);
        }
    }
    return 0;
}

// Write a .
#include <stdio.h>

struct Student {
    char name[50];
    int rollNo;
    float marks;
};

int main() {
    struct Student s;
    printf("Enter student name: ");
    scanf("%s", s.name);
    printf("Enter roll number: ");
    scanf("%d", &s.rollNo);
    printf("Enter marks: ");
    scanf("%f", &s.marks);
    printf("\nStudent Details:\n");
    printf("Name: %s\n", s.name);
    printf("Roll Number: %d\n", s.rollNo);
    printf("Marks: %.2f\n", s.marks);
    return 0;
}

// Write a C program using a function with arguments and a return value to calculate the sum of two numbers.
#include <stdio.h>

int add(int a, int b) {
    return a + b;
}

int main() {
    int num1, num2, result;
    printf("Enter two numbers: ");
    scanf("%d %d", &num1, &num2);
    result = add(num1, num2);
    printf("Sum = %d\n", result);
    return 0;
}// Write a C program using a function with arguments and a return value to calculate the sum of two numbers.
#include <stdio.h>

int add(int a, int b) {
    return a + b;
}

int main() {
    int num1, num2, result;
    printf("Enter two numbers: ");
    scanf("%d %d", &num1, &num2);
    result = add(num1, num2);
    printf("Sum = %d\n", result);
    return 0;
}

// Write a C program to swap two numbers with using third variable.
#include <stdio.h>

int main() {
    int a, b, temp;
    printf("Enter two numbers: ");
    scanf("%d %d", &a, &b);
    temp = a;
    a = b;
    b = temp;
    printf("After swapping: a = %d, b = %d\n", a, b);
    return 0;
}

// Write a.
#include <stdio.h>

int main() {
    int a, b, *p1, *p2, temp;
    printf("Enter two numbers: ");
    scanf("%d %d", &a, &b);
    printf("Before swapping: a = %d, b = %d\n", a, b);
    p1 = &a;
    p2 = &b;
    temp = *p1;
    *p1 = *p2;
    *p2 = temp;
    printf("After swapping: a = %d, b = %d\n", a, b);
    return 0;
}

// Write a C program to print the palindromic number pyramid pattern using nested loops.
#include <stdio.h>

int main() {
    int i, j, space, num;
    for (i = 1; i <= 5; i++) {
        for (space = 1; space <= 5 - i; space++) {
            printf("  ");
        }
        num = i;
        for (j = 1; j <= i; j++) {
            printf("%d ", num++);
        }
        num = num - 2;
        for (j = 1; j < i; j++) {
            printf("%d ", num--);
        }
        printf("\n");
    }
    return 0;
}

// Write a C program to print the number right-angle triangle pattern using nested loops.
#include <stdio.h>

int main() {
    int i, j;
    for (i = 1; i <= 5; i++) {
        for (j = 1; j <= i; j++) {
            printf("%d ", j);
        }
        printf("\n");
    }
    return 0;
}

// Write a C program to print the inverted star pyramid pattern using nested loops.
#include <stdio.h>

int main() {
    int i, j, space;
    for (i = 5; i >= 1; i--) {
        for (space = 0; space < 5 - i; space++) {
            printf("  ");
        }
        for (j = 1; j <= (2 * i - 1); j++) {
            printf("* ");
        }
        printf("\n");
    }
    return 0;
}

// Write a C program to print numbers from 1 to 50 using a loop, but skip the multiples of 5 using the continue statement.
#include <stdio.h>

int main() {
    int i;
    for (i = 1; i <= 50; i++) {
        if (i % 5 == 0) {
            continue;
        }
        printf("%d ", i);
    }
    printf("\n");
    return 0;
}

// Write a C program to print numbers from 1 to 100 and stop the loop when the number reaches 50 using the break statement.
#include <stdio.h>

int main() {
    int i;
    for (i = 1; i <= 100; i++) {
        if (i == 50) {
            break;
        }
        printf("%d ", i);
    }
    printf("\n");
    return 0;
}

// Write a C program to find the size of int, float, double and char.
#include <stdio.h>

int main() {
    printf("Size of int: %zu bytes\n", sizeof(int));
    printf("Size of float: %zu bytes\n", sizeof(float));
    printf("Size of double: %zu bytes\n", sizeof(double));
    printf("Size of char: %zu byte\n", sizeof(char));
    return 0;
}

// Write a C program to find the length of a string and copy one string into another using standard string functions.
#include <stdio.h>
#include <string.h>

int main() {
    char str1[100], str2[100];
    int length;
    printf("Enter a string: ");
    scanf("%s", str1);
    length = strlen(str1);
    strcpy(str2, str1);
    printf("Length of string = %d\n", length);
    printf("Copied string = %s\n", str2);
    return 0;
}

// Write a C program to find the largest number among three numbers.
#include <stdio.h>

int main() {
    int a, b, c;
    printf("Enter three numbers: ");
    scanf("%d %d %d", &a, &b, &c);
    if (a >= b && a >= c) {
        printf("Largest = %d\n", a);
    } else if (b >= a && b >= c) {
        printf("Largest = %d\n", b);
    } else {
        printf("Largest = %d\n", c);
    }
    return 0;
}

// Write a C program to find the largest and smallest elements in a one-dimensional array.
#include <stdio.h>

int main() {
    int arr[100], n, i, largest, smallest;
    printf("Enter number of elements: ");
    scanf("%d", &n);
    printf("Enter %d elements: ", n);
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    largest = arr[0];
    smallest = arr[0];
    for (i = 1; i < n; i++) {
        if (arr[i] > largest) {
            largest = arr[i];
        }
        if (arr[i] < smallest) {
            smallest = arr[i];
        }
    }
    printf("Largest = %d\n", largest);
    printf("Smallest = %d\n", smallest);
    return 0;
}

// Write a  C program to find the factorial of a number using recursion

#include <stdio.h>

unsigned long long factorial(int n) {
    if (n == 0 || n == 1) {
        return 1;
    }
    return n * factorial(n - 1);
}

int main() {
    int num;
    printf("Enter a positive integer: ");
    scanf("%d", &num);
    printf("Factorial = %llu\n", factorial(num));
    return 0;
}

// Write a C program to find the LCM (Least Common Multiple) of two numbers.
#include <stdio.h>

int main() {
    int a, b, max;
    printf("Enter two positive integers: ");
    scanf("%d %d", &a, &b);
    max = (a > b) ? a : b;
    while (1) {
        if (max % a == 0 && max % b == 0) {
            printf("LCM = %d\n", max);
            break;
        }
        max++;
    }
    return 0;
}

// Write a C program to find the GCD (Greatest Common Divisor) of two numbers.
#include <stdio.h>

int main() {
    int a, b, i, gcd;
    printf("Enter two integers: ");
    scanf("%d %d", &a, &b);
    for (i = 1; i <= a && i <= b; i++) {
        if (a % i == 0 && b % i == 0) {
            gcd = i;
        }
    }
    printf("GCD = %d\n", gcd);
    return 0;
}

// Write a C program to find factorial of given number.
#include <stdio.h>

int main() {
    int n, i;
    unsigned long long fact = 1;
    printf("Enter a positive integer: ");
    scanf("%d", &n);
    for (i = 1; i <= n; i++) {
        fact = fact * i;
    }
    printf("Factorial = %llu\n", fact);
    return 0;
}

// Write a C program to display Fibonacci series.

#include <stdio.h>

int main() {
    int n, i, t1 = 0, t2 = 1, nextTerm;
    printf("Enter number of terms: ");
    scanf("%d", &n);
    printf("Fibonacci Series: ");
    for (i = 1; i <= n; i++) {
        printf("%d ", t1);
        nextTerm = t1 + t2;
        t1 = t2;
        t2 = nextTerm;
    }
    printf("\n");
    return 0;
}

// Write a C program to demonstrate the use of the exit() function with a suitable condition.

#include <stdio.h>
#include <stdlib.h>

int main() {
    int age;
    printf("Enter your age: ");
    scanf("%d", &age);
    if (age < 0) {
        printf("Invalid age! Exiting program.\n");
        exit(0);
    }
    printf("Your age is %d\n", age);
    return 0;
}

/ Write a C program to demonstrate the use of a union and display its members.
#include <stdio.h>
#include <string.h>

union Data {
    int i;
    float f;
    char str[20];
};

int main() {
    union Data data;
    data.i = 10;
    printf("data.i : %d\n", data.i);
    data.f = 220.5;
    printf("data.f : %.2f\n", data.f);
    strcpy(data.str, "C Programming");
    printf("data.str : %s\n", data.str);
    return 0;
}

// Write a C program to demonstrate call by value and call by reference by swapping two numbers.
#include <stdio.h>

void swapByValue(int a, int b) {
    int temp = a;
    a = b;
    b = temp;
    printf("Inside swapByValue: a = %d, b = %d\n", a, b);
}

void swapByReference(int *a, int *b) {
    int temp = *a;
    *a = *b;
    *b = temp;
    printf("Inside swapByReference: a = %d, b = %d\n", *a, *b);
}

int main() {
    int x = 10, y = 20;
    printf("Before swapping: x = %d, y = %d\n", x, y);
    swapByValue(x, y);
    printf("After swapByValue in main: x = %d, y = %d\n", x, y);
    swapByReference(&x, &y);
    printf("After swapByReference in main: x = %d, y = %d\n", x, y);
    return 0;
}

// Write a C program to create a simple calculator using switch-case for addition, subtraction, multiplication and division.
#include <stdio.h>

int main() {
    char op;
    float num1, num2;
    printf("Enter an operator (+, -, *, /): ");
    scanf(" %c", &op);
    printf("Enter two numbers: ");
    scanf("%f %f", &num1, &num2);
    switch (op) {
        case '+':
            printf("Result = %.2f\n", num1 + num2);
            break;
        case '-':
            printf("Result = %.2f\n", num1 - num2);
            break;
        case '*':
            printf("Result = %.2f\n", num1 * num2);
            break;
        case '/':
            if (num2 != 0)
                printf("Result = %.2f\n", num1 / num2);
            else
                printf("Cannot divide by zero\n");
            break;
        default:
            printf("Invalid operator\n");
    }
    return 0;
}

// Write a C program to concatenate two strings and compare two strings using standard string library functions.
#include <stdio.h>
#include <string.h>

int main() {
    char str1[100], str2[100];
    printf("Enter first string: ");
    scanf("%s", str1);
    printf("Enter second string: ");
    scanf("%s", str2);
    if (strcmp(str1, str2) == 0) {
        printf("Strings are equal\n");
    } else {
        printf("Strings are not equal\n");
    }
    strcat(str1, str2);
    printf("Concatenated string: %s\n", str1);
    return 0;
}

// Write a C program to compute quotient and remainder.
#include <stdio.h>

int main() {
    int dividend, divisor, quotient, remainder;
    printf("Enter dividend and divisor: ");
    scanf("%d %d", &dividend, &divisor);
    quotient = dividend / divisor;
    remainder = dividend % divisor;
    printf("Quotient = %d\n", quotient);
    printf("Remainder = %d\n", remainder);
    return 0;
}

// Write a C program to check whether a number is even or odd using ternary operator.
#include <stdio.h>

int main() {
    int num;
    printf("Enter a number: ");
    scanf("%d", &num);
    (num % 2 == 0) ? printf("Even\n") : printf("Odd\n");
    return 0;
}

// Write a C program to check whether a number is a palindrome or not.
#include <stdio.h>

int main() {
    int n, reversed = 0, remainder, original;
    printf("Enter an integer: ");
    scanf("%d", &n);
    original = n;
    while (n != 0) {
        remainder = n % 10;
        reversed = reversed * 10 + remainder;
        n = n / 10;
    }
    if (original == reversed) {
        printf("Palindrome number\n");
    } else {
        printf("Not a palindrome number\n");
    }
    return 0;
}

// Write a C program to check whether a given number is prime or not.
#include <stdio.h>

int main() {
    int n, i, isPrime = 1;
    printf("Enter a positive integer: ");
    scanf("%d", &n);
    if (n <= 1) {
        isPrime = 0;
    } else {
        for (i = 2; i <= n / 2; i++) {
            if (n % i == 0) {
                isPrime = 0;
                break;
            }
        }
    }
    if (isPrime == 1) {
        printf("Prime number\n");
    } else {
        printf("Not a prime number\n");
    }
    return 0;
}

// Write a C program to check whether a character is an alphabet or not.
#include <stdio.h>

int main() {
    char ch;
    printf("Enter a character: ");
    scanf(" %c", &ch);
    if ((ch >= 'a' && ch <= 'z') || (ch >= 'A' && ch <= 'Z')) {
        printf("It is an alphabet\n");
    } else {
        printf("It is not an alphabet\n");
    }
    return 0;
}

// Write a C program to check given number is an Armstrong or not.
#include <stdio.h>

int main() {
    int num, original, remainder, result = 0;
    printf("Enter a three-digit integer: ");
    scanf("%d", &num);
    original = num;
    while (original != 0) {
        remainder = original % 10;
        result = result + (remainder * remainder * remainder);
        original = original / 10;
    }
    if (result == num) {
        printf("Armstrong number\n");
    } else {
        printf("Not an Armstrong number\n");
    }
    return 0;
}

// Write a C program to calculate the grade of a student based on marks using if-else-if statements.
#include <stdio.h>

int main() {
    int marks;
    printf("Enter marks (0-100): ");
    scanf("%d", &marks);
    if (marks >= 90) {
        printf("Grade: A\n");
    } else if (marks >= 75) {
        printf("Grade: B\n");
    } else if (marks >= 60) {
        printf("Grade: C\n");
    } else if (marks >= 40) {
        printf("Grade: D\n");
    } else {
        printf("Grade: F (Fail)\n");
    }
    return 0;
}

// Write a C program to calculate sum of natural numbers.
#include <stdio.h>

int main() {
    int n, i, sum = 0;
    printf("Enter a positive integer: ");
    scanf("%d", &n);
    for (i = 1; i <= n; i++) {
        sum = sum + i;
    }
    printf("Sum = %d\n", sum);
    return 0;
}

// Write a C program to calculate area and perimeter of rectangle.
#include <stdio.h>

int main() {
    float length, width, area, perimeter;
    printf("Enter length and width of rectangle: ");
    scanf("%f %f", &length, &width);
    area = length * width;
    perimeter = 2 * (length + width);
    printf("Area = %.2f\n", area);
    printf("Perimeter = %.2f\n", perimeter);
    return 0;
}

// Write a C program to calculate Fahrenheit to Celsius.
#include <stdio.h>

int main() {
    float fahrenheit, celsius;
    printf("Enter temperature in Fahrenheit: ");
    scanf("%f", &fahrenheit);
    celsius = (fahrenheit - 32) * 5.0 / 9.0;
    printf("Temperature in Celsius = %.2f\n", celsius);
    return 0;
}

// Write a C program to add two matrices using two-dimensional arrays.
#include <stdio.h>

int main() {
    int a[10][10], b[10][10], sum[10][10], r, c, i, j;
    printf("Enter rows and columns: ");
    scanf("%d %d", &r, &c);
    printf("Enter elements of first matrix:\n");
    for (i = 0; i < r; i++) {
        for (j = 0; j < c; j++) {
            scanf("%d", &a[i][j]);
        }
    }
    printf("Enter elements of second matrix:\n");
    for (i = 0; i < r; i++) {
        for (j = 0; j < c; j++) {
            scanf("%d", &b[i][j]);
        }
    }
    printf("Sum of matrices:\n");
    for (i = 0; i < r; i++) {
        for (j = 0; j < c; j++) {
            sum[i][j] = a[i][j] + b[i][j];
            printf("%d ", sum[i][j]);
        }
        printf("\n");
    }
    return 0;
}

// Write a C program that accepts the salary and age from the user and displays the same on the screen as output.
#include <stdio.h>

int main() {
    float salary;
    int age;
    printf("Enter your age: ");
    scanf("%d", &age);
    printf("Enter your salary: ");
    scanf("%f", &salary);
    printf("Age: %d\n", age);
    printf("Salary: %.2f\n", salary);
    return 0;
}
