# Java Calculator

A simple console calculator created as a Day 3 exercise for a QA Automation Bootcamp. The program accepts two numbers and lets the user choose addition, subtraction, multiplication, or division.

## Features

- Accepts whole numbers and decimal numbers using `Scanner`.
- Displays a numbered menu of four arithmetic operations.
- Prints the result of the selected operation.
- Prevents division by zero and displays an error message.
- Displays `Invalid Choice` when the selected number is outside the menu.

## Java Concepts Practiced

- Variables and data types: `double` for the two numbers and `int` for the menu choice.
- User input with `Scanner`, `nextDouble()`, and `nextInt()`.
- Arithmetic operators: `+`, `-`, `*`, and `/`.
- Comparison operators: `==` and `!=`.
- Conditional statements: `if`, `else if`, `else`, and a nested `if/else` for division.
- Console output with `System.out.println()`.
- Closing the scanner after collecting input.

## How to Run in Eclipse

You need a Java Development Kit (JDK) configured in Eclipse IDE for Java Developers. No external libraries are required.

1. Open your Java project in Eclipse.
2. Create a package named `day3` under the source folder if it does not already exist.
3. Save the source code in that package as `Calculator.java`. The file must begin with `package day3;`.
4. Right-click `Calculator.java` and select **Run As > Java Application**.
5. Enter the first number and press Enter.
6. Enter the second number and press Enter.
7. Enter the operation number and press Enter.

| Choice | Operation |
| --- | --- |
| 1 | Addition |
| 2 | Subtraction |
| 3 | Multiplication |
| 4 | Division |

## Example

Enter `10` as the first number, `4` as the second number, and `1` for addition. The result is:

```text
Result: 14.0
```

The program also prints each entered number and the selected menu choice before displaying the result.

## Suggested Manual Checks

These are expected results to check when running the program.

| First number | Second number | Choice | Expected output |
| --- | --- | --- | --- |
| 10 | 4 | 1 | `Result: 14.0` |
| 10 | 4 | 2 | `Result: 6.0` |
| 10 | 4 | 3 | `Result: 40.0` |
| 10 | 4 | 4 | `Result: 2.5` |
| 10 | 0 | 4 | `Error:Division by zero is not allowed` |
| 10 | 4 | 5 | `Invalid Choice` |
| 2.5 | 1.5 | 1 | `Result: 4.0` |

## Current Limitations

- Performs one calculation per run. Run the program again for another calculation.
- Expects numeric input. Text input or a decimal menu choice causes an input mismatch exception.
- Uses `double` values, so some decimal calculations can display small rounding differences.
