# Unexpected Type Coercion in JavaScript Arithmetic

This code demonstrates a common JavaScript pitfall: the unexpected type coercion that occurs when performing arithmetic operations with mixed data types.

## The Bug

The `foo` function attempts to add two numbers. However, when a string is passed as an argument, JavaScript implicitly converts the number to a string and performs string concatenation instead of addition.  This can lead to incorrect calculations and unexpected program behavior.

## The Solution

To avoid this issue, explicitly convert the operands to numbers before performing the addition.  The updated `foo` function utilizes the `Number()` function to ensure that both arguments are treated as numbers before adding them.