# Simple Calculator Program

This is a simple calculator program written in C, utilizing switch-case statements to perform basic arithmetic operations.

## Features

- Supports addition, subtraction, multiplication, and division.
- Handles incorrect operator input by displaying an error message.
- Uses `double` data type for operands to support decimal numbers.

## Usage

1. Compile the program using a C compiler (e.g., `gcc calculator.c -o calculator`).
2. Run the program (e.g., `./calculator` on Linux/macOS or `calculator.exe` on Windows).
3. Enter an operator (+, -, \*, /) when prompted.
4. Enter two operands when prompted.
5. The program will display the result of the operation.

// Read the operator
printf("Enter an operator (+, -, *, /): ");
scanf("%c", &op);

// Read the two numbers
printf("Enter two operands: ");
scanf("%lf %lf", &a, &b);

// Define all four operations in the corresponding
// switch-case
switch (op) {
case '+':
    res = a + b;
    break;
case '-':
    res = a - b;
    break;
case '*':
     res = a * b;
    break;
case '/':
    res = a / b;
    break;
default:
    printf("Error! Incorrect Operator Value\n");
    res = -DBL_MAX;
}
if(res!=-DBL_MAX)
  printf("%.2lf", res);

return 0;
