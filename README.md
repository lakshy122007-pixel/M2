# EX-06 - Looping

## AIM:

Write a C program to print even numbers ranging from M to N (including M and N values).

## ALGORITHM:
1. Start the program.
2. Declare two integer variables M and N.
3. Read values of M and N from the user.
4. Use a loop from M to N.
5. For each number, check if it is even (num % 2 == 0).
6. If even, print the number.
7. Stop the program.
## PROGRAM:

```
#include <stdio.h>

int main() {
    int M, N, i;

    printf("Enter the values of M and N: ");
    scanf("%d %d", &M, &N);

    printf("Even numbers from %d to %d are: ", M, N);

    for (i = M; i <= N; i++) {
        if (i % 2 == 0) {
            printf("%d ", i);
        }
    }

    return 0;
}

```

## OUTPUT:
```
Enter the values of M and N: 1 10
Even numbers from 1 to 10 are: 2 4 6 8 10

```
## RESULT:

Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully

# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1. Start the program.
2. Declare an integer variable n for number of rows.
3. Read the value of n from the user.
4. Use an outer loop from i = 1 to n (for rows).
5. For each row, use an inner loop from j = 1 to i.
6. Print * in the inner loop.
7. After each row, move to the next line.
8. Stop the program.

## PROGRAM:

```
#include <stdio.h>

int main() {
    int n, i, j;

    printf("Enter number of rows: ");
    scanf("%d", &n);

    for (i = 1; i <= n; i++) {
        for (j = 1; j <= i; j++) {
            printf("* ");
        }
        printf("\n");
    }

    return 0;
}

```

## OUTPUT:

```
Enter number of rows: 5
* 
* * 
* * * 
* * * * 
* * * * *
```
## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully

# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:
1. Start the program.
2. Declare two integer variables a and b.
3. Declare two functions:
4. add(int, int) for addition
5. sub(int, int) for subtraction
6. Read values of a and b from the user.
7. Call add(a, b) to perform addition and display result.
8. Call sub(a, b) to perform subtraction and display result.
9. Stop the program.

## PROGRAM:

```
#include <stdio.h>

// Function for addition (with argument, no return)
void add(int x, int y) {
    int sum = x + y;
    printf("Addition = %d\n", sum);
}

// Function for subtraction (with argument, no return)
void sub(int x, int y) {
    int diff = x - y;
    printf("Subtraction = %d\n", diff);
}

int main() {
    int a, b;

    printf("Enter two numbers: ");
    scanf("%d %d", &a, &b);

    add(a, b);
    sub(a, b);

    return 0;
}

```

## OUTPUT:
```
Enter two numbers: 10 5
Addition = 15
Subtraction = 5
```
## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully

# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:
1. Start the program.
2. Declare variables num, digit, and sum = 0.
3. Read the number from the user.
4. Use a for loop to extract digits:
5. Get last digit using digit = num % 10.
6. Check if the digit is odd (digit % 2 != 0).
7. If odd, add it to sum.
8. Remove last digit using num = num / 10.
9. Repeat until num > 0.
10. Print the sum of odd digits.
11. Stop the program.

## PROGRAM:

```
#include <stdio.h>

int main() {
    int num, digit, sum = 0;

    printf("Enter a number: ");
    scanf("%d", &num);

    for (; num > 0; num = num / 10) {
        digit = num % 10;

        if (digit % 2 != 0) {
            sum = sum + digit;
        }
    }

    printf("Sum of odd digits = %d", sum);

    return 0;
}

```

## OUTPUT:
```
Enter a number: 12345
Sum of odd digits = 9
```
## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.

# EX – 10 - Factorial of a Number Using a Function

## AIM:

To write a C program that calculates the factorial of a given number using a user-defined function.

## ALGORITHM:
1. Start the program.
2. Declare an integer variable n.
3. Declare a user-defined function factorial(int n).
4. Read the value of n from the user.
5. Call the function factorial(n).
6. Inside the function:
7. Initialize fact = 1.
8. Use a loop from 1 to n.
9. Multiply fact = fact * i.
10. Return the factorial value.
11. Display the result.
12. Stop the program.
## PROGRAM:

```
#include <stdio.h>

// Function to calculate factorial
int factorial(int n) {
    int i, fact = 1;

    for (i = 1; i <= n; i++) {
        fact = fact * i;
    }

    return fact;
}

int main() {
    int n, result;

    printf("Enter a number: ");
    scanf("%d", &n);

    result = factorial(n);

    printf("Factorial of %d = %d", n, result);

    return 0;
}

```

## OUTPUT:

```
Enter a number: 5
Factorial of 5 = 120
```
## RESULT:

The program correctly computes the factorial of a given number using a separate function and displays the result.
