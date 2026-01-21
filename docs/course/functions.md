# Functions

Functions are reusable blocks of code that perform a specific task. They help make your code more organized and maintainable.

## Defining Functions

Use the `def` keyword to define a function.

```python
def greet():
    print("Hello, World!")

# Call the function
greet()
```

## Parameters and Arguments

Functions can accept input values.

```python
def greet(name):
    print(f"Hello, {name}!")

greet("Alice")  # Hello, Alice!
greet("Bob")    # Hello, Bob!
```

### Multiple Parameters

```python
def add(a, b):
    result = a + b
    print(f"{a} + {b} = {result}")

add(5, 3)  # 5 + 3 = 8
```

### Default Parameters

```python
def greet(name, greeting="Hello"):
    print(f"{greeting}, {name}!")

greet("Alice")              # Hello, Alice!
greet("Bob", "Hi")          # Hi, Bob!
```

### Keyword Arguments

```python
def describe_pet(animal, name):
    print(f"I have a {animal} named {name}")

describe_pet(animal="dog", name="Max")
describe_pet(name="Whiskers", animal="cat")
```

## Return Values

Functions can return values using the `return` statement.

```python
def add(a, b):
    return a + b

result = add(5, 3)
print(result)  # 8

# Multiple return values
def get_name():
    first = "John"
    last = "Doe"
    return first, last

first_name, last_name = get_name()
print(first_name, last_name)  # John Doe
```

## Variable Scope

### Local Variables

Variables defined inside a function are local to that function.

```python
def my_function():
    x = 10  # Local variable
    print(x)

my_function()
# print(x)  # Error: x is not defined outside the function
```

### Global Variables

Variables defined outside functions are global.

```python
x = 10  # Global variable

def my_function():
    print(x)  # Can access global variable

my_function()
```

### Modifying Global Variables

```python
x = 10

def modify():
    global x
    x = 20

modify()
print(x)  # 20
```

## Args and Kwargs

### *args (Variable Positional Arguments)

Accept any number of positional arguments.

```python
def sum_all(*args):
    total = 0
    for num in args:
        total += num
    return total

print(sum_all(1, 2, 3))        # 6
print(sum_all(1, 2, 3, 4, 5))  # 15
```

### **kwargs (Variable Keyword Arguments)

Accept any number of keyword arguments.

```python
def print_info(**kwargs):
    for key, value in kwargs.items():
        print(f"{key}: {value}")

print_info(name="Alice", age=25, city="New York")
# name: Alice
# age: 25
# city: New York
```

### Combining Parameters

```python
def example(pos1, pos2, *args, kwarg1="default", **kwargs):
    print(f"Positional: {pos1}, {pos2}")
    print(f"Args: {args}")
    print(f"Keyword: {kwarg1}")
    print(f"Kwargs: {kwargs}")

example(1, 2, 3, 4, kwarg1="custom", extra="value")
```

## Lambda Functions

Small anonymous functions defined with the `lambda` keyword.

```python
# Regular function
def square(x):
    return x ** 2

# Lambda function
square = lambda x: x ** 2

print(square(5))  # 25

# Lambda with multiple parameters
add = lambda a, b: a + b
print(add(3, 5))  # 8

# Lambda in sorted()
points = [(1, 5), (3, 2), (2, 8)]
sorted_points = sorted(points, key=lambda point: point[1])
print(sorted_points)  # [(3, 2), (1, 5), (2, 8)]
```

## Recursion

A function can call itself.

```python
def factorial(n):
    if n == 0 or n == 1:
        return 1
    else:
        return n * factorial(n - 1)

print(factorial(5))  # 120

# Fibonacci sequence
def fibonacci(n):
    if n <= 1:
        return n
    return fibonacci(n - 1) + fibonacci(n - 2)

for i in range(10):
    print(fibonacci(i), end=" ")
# 0 1 1 2 3 5 8 13 21 34
```

## Docstrings

Document your functions with docstrings.

```python
def calculate_area(radius):
    """
    Calculate the area of a circle.
    
    Parameters:
        radius (float): The radius of the circle
        
    Returns:
        float: The area of the circle
    """
    import math
    return math.pi * radius ** 2

print(calculate_area.__doc__)  # Prints the docstring
```

## Built-in Functions

Python provides many built-in functions:

```python
# Common built-in functions
print(len([1, 2, 3]))           # 3
print(max([1, 5, 3]))           # 5
print(min([1, 5, 3]))           # 1
print(sum([1, 2, 3]))           # 6
print(abs(-5))                  # 5
print(round(3.14159, 2))        # 3.14
print(type(5))                  # <class 'int'>

# Type conversion functions
int("10")
float("3.14")
str(123)
list("hello")

# Input/output
input("Enter your name: ")
print("Hello, World!")
```

## Practice Exercises

1. **Temperature Converter**: Create functions to convert between Celsius and Fahrenheit

```python
def celsius_to_fahrenheit(celsius):
    return (celsius * 9/5) + 32

def fahrenheit_to_celsius(fahrenheit):
    return (fahrenheit - 32) * 5/9
```

2. **Palindrome Checker**: Write a function that checks if a string is a palindrome

3. **Calculator**: Create a calculator with functions for add, subtract, multiply, and divide

4. **Prime Number Checker**: Write a function that returns True if a number is prime

## Next Steps

Congratulations! You've learned the fundamentals of Python. Continue practicing and explore:

- **File Handling**: Read and write files
- **Object-Oriented Programming**: Classes and objects
- **Modules and Packages**: Organize code into modules
- **Error Handling**: Exception handling
- **Libraries**: NumPy, Pandas, requests, etc.

Check out the [Exercises](../exercises.md) section to practice what you've learned!
