# Python Basics

## Variables

Variables are containers for storing data values. In Python, you don't need to declare the type of a variable.

```python
# Creating variables
name = "Alice"
age = 25
height = 1.75
is_student = True
```

### Variable Naming Rules

- Must start with a letter or underscore
- Can contain letters, numbers, and underscores
- Case-sensitive (`name` and `Name` are different)
- Cannot use Python keywords (like `if`, `for`, `while`, etc.)

```python
# Good variable names
user_name = "Bob"
total_count = 100
_private_var = "secret"

# Bad variable names (will cause errors)
# 2nd_name = "Invalid"  # starts with a number
# my-name = "Invalid"   # contains hyphen
# for = "Invalid"       # Python keyword
```

## Comments

Comments help explain your code and are ignored by Python.

```python
# This is a single-line comment

"""
This is a multi-line comment.
It can span multiple lines.
"""

x = 5  # This is an inline comment
```

## Print Function

The `print()` function displays output to the console.

```python
print("Hello, World!")
print("My name is", name)
print(f"I am {age} years old")  # f-string (formatted string)
```

## Input Function

The `input()` function gets user input from the console.

```python
name = input("What is your name? ")
print(f"Hello, {name}!")

# Convert input to numbers
age = int(input("How old are you? "))
height = float(input("What is your height in meters? "))
```

## Basic Operators

### Arithmetic Operators

```python
a = 10
b = 3

print(a + b)   # Addition: 13
print(a - b)   # Subtraction: 7
print(a * b)   # Multiplication: 30
print(a / b)   # Division: 3.333...
print(a // b)  # Floor division: 3
print(a % b)   # Modulus (remainder): 1
print(a ** b)  # Exponentiation: 1000
```

### Comparison Operators

```python
x = 5
y = 10

print(x == y)  # Equal to: False
print(x != y)  # Not equal to: True
print(x < y)   # Less than: True
print(x > y)   # Greater than: False
print(x <= y)  # Less than or equal to: True
print(x >= y)  # Greater than or equal to: False
```

### Logical Operators

```python
a = True
b = False

print(a and b)  # AND: False
print(a or b)   # OR: True
print(not a)    # NOT: False
```

## Practice Exercise

Try creating a simple calculator program:

```python
# Simple calculator
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))

print(f"Sum: {num1 + num2}")
print(f"Difference: {num1 - num2}")
print(f"Product: {num1 * num2}")
print(f"Quotient: {num1 / num2}")
```

## Next Steps

Continue to [Data Types](data-types.md) to learn about different types of data in Python.
