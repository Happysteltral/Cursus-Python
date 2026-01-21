# Control Flow

Control flow determines the order in which your code executes. Python provides several control flow statements.

## Conditional Statements

### if Statement

Execute code only if a condition is true.

```python
age = 18

if age >= 18:
    print("You are an adult")
```

### if-else Statement

Execute one block if the condition is true, another if it's false.

```python
temperature = 25

if temperature > 30:
    print("It's hot outside")
else:
    print("It's not too hot")
```

### if-elif-else Statement

Check multiple conditions.

```python
score = 85

if score >= 90:
    print("Grade: A")
elif score >= 80:
    print("Grade: B")
elif score >= 70:
    print("Grade: C")
elif score >= 60:
    print("Grade: D")
else:
    print("Grade: F")
```

### Nested Conditions

```python
age = 20
has_license = True

if age >= 18:
    if has_license:
        print("You can drive")
    else:
        print("You need a license")
else:
    print("You're too young to drive")
```

## Loops

### for Loop

Iterate over a sequence (list, tuple, string, etc.).

```python
# Loop through a list
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)

# Loop through a string
for char in "Python":
    print(char)

# Loop with range
for i in range(5):  # 0, 1, 2, 3, 4
    print(i)

# Range with start and end
for i in range(2, 6):  # 2, 3, 4, 5
    print(i)

# Range with step
for i in range(0, 10, 2):  # 0, 2, 4, 6, 8
    print(i)
```

### while Loop

Execute code while a condition is true.

```python
count = 0
while count < 5:
    print(count)
    count += 1

# Input validation example
password = ""
while password != "secret":
    password = input("Enter password: ")
print("Access granted!")
```

### Loop Control Statements

#### break

Exit the loop prematurely.

```python
for i in range(10):
    if i == 5:
        break
    print(i)  # Prints 0, 1, 2, 3, 4
```

#### continue

Skip the rest of the current iteration.

```python
for i in range(5):
    if i == 2:
        continue
    print(i)  # Prints 0, 1, 3, 4 (skips 2)
```

#### pass

Do nothing (placeholder).

```python
for i in range(5):
    if i == 2:
        pass  # TODO: Add logic later
    print(i)  # Prints all numbers
```

### else with Loops

The `else` clause executes when the loop completes normally (not via `break`).

```python
for i in range(5):
    print(i)
else:
    print("Loop completed")

# With break
for i in range(5):
    if i == 3:
        break
    print(i)
else:
    print("This won't print")  # Because of break
```

## Nested Loops

```python
# Multiplication table
for i in range(1, 4):
    for j in range(1, 4):
        print(f"{i} x {j} = {i * j}")
    print()  # Empty line between tables
```

## Comprehensions

### List Comprehensions

Create lists in a concise way.

```python
# Traditional way
squares = []
for i in range(10):
    squares.append(i ** 2)

# List comprehension
squares = [i ** 2 for i in range(10)]

# With condition
even_squares = [i ** 2 for i in range(10) if i % 2 == 0]
```

### Dictionary Comprehensions

```python
# Create a dictionary
squares_dict = {i: i ** 2 for i in range(5)}
# {0: 0, 1: 1, 2: 4, 3: 9, 4: 16}
```

### Set Comprehensions

```python
# Create a set
unique_squares = {i ** 2 for i in range(-5, 6)}
```

## Practice Exercises

1. **FizzBuzz**: Print numbers 1-100, but for multiples of 3 print "Fizz", for multiples of 5 print "Buzz", and for multiples of both print "FizzBuzz"

2. **Number Guessing Game**: Create a program where the computer picks a random number and the user has to guess it

3. **Prime Number Checker**: Write a program that checks if a number is prime

4. **Factorial Calculator**: Calculate the factorial of a number using a loop

## Example Solutions

### FizzBuzz

```python
for i in range(1, 101):
    if i % 15 == 0:
        print("FizzBuzz")
    elif i % 3 == 0:
        print("Fizz")
    elif i % 5 == 0:
        print("Buzz")
    else:
        print(i)
```

### Sum of Numbers

```python
total = 0
number = 1

while number <= 100:
    total += number
    number += 1

print(f"Sum of 1 to 100: {total}")
```

## Next Steps

Continue to [Functions](functions.md) to learn how to organize your code into reusable blocks.
