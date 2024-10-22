# Factorial-of-a-Number

#include <stdio.h>

// Function to calculate factorial using recursion
int factorial(int n) {
    if (n == 0) {
        return 1;  // Base case: factorial of 0 is 1
    }
    return n * factorial(n - 1);  // Recursive case
}

int main() {
    int num;

    // Input from the user
    printf("Enter a positive integer: ");
    scanf("%d", &num);

    // Input validation
    if (num < 0) {
        printf("Factorial of a negative number is not possible.\n");
    } else {
        printf("Factorial of %d is %d\n", num, factorial(num));
    }

    return 0;
}
