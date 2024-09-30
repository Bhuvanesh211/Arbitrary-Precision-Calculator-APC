# Arbitrary-Precision Arithmetic Calculator

## Introduction
Arbitrary-precision arithmetic, also called big-num arithmetic, multiple precision arithmetic, or sometimes infinite-precision arithmetic, indicates that calculations are performed on numbers whose digits of precision are limited only by the available memory of the host system. This contrasts with the faster fixed-precision arithmetic found in most arithmetic logic unit (ALU) hardware, which typically offers between 8 and 64 bits of precision. Explore the world of arbitrary-precision arithmetic with our calculator project in C.

### Example Applications
- **Public-Key Cryptography**: Algorithms commonly employ arithmetic with integers having hundreds of digits.
- **Mathematical Constants**: Compute fundamental mathematical constants such as π to millions or more digits.

## Project Goals
The goal of this project is to implement various mathematical operations on two big numbers by storing them in an Abstract Data Type (ADT) like a linked list.

### Supported Operations
- Addition (+)
- Subtraction (-)
- Multiplication (*)
- Division (/)
- Modulus (%)
- Power (^)

## Implementation Details
Given two big numbers, they are sliced and stored across different nodes of the linked list. Depending on the type of operation performed, a result linked list is created to store the output. It should also print the output from the newly created output list. Appropriate handling of specific scenarios (e.g., carry forward) needs to be implemented. All operations should work for both integer numbers and numbers with a decimal point. The numbers should be sliced according to `sizeof(int)` to ensure portability across different machines.

### Handling Special Cases
Special care is taken for handling zero inputs and other corner cases to optimize the program:
- If Num1 = 0 and Num2 = x, print Num2.
- If Num1 = x and Num2 = 0, print Num1.
- If Num1 = 0 and Num2 = 0, print 0.

## Requirements
1. The user will enter two big numbers along with an operator in the terminal, e.g., `x+y`, where `x` and `y` are very large numbers and `+` is the operation to be performed.
2. The application will perform the operation based on the user input and display the result.

## User Interface
1. **Run the Application**
   ```sh
   ./apc
