# Exercises

Practice makes perfect! Here are exercises to reinforce what you've learned.

## Basic Exercises

### Exercise 1: Variables and Print

Create a program that:
1. Stores your name in a variable
2. Stores your age in a variable
3. Prints a message like "My name is [name] and I am [age] years old"

<details>
<summary>Solution</summary>

```python
name = "Alice"
age = 25
print(f"My name is {name} and I am {age} years old")
```
</details>

### Exercise 2: Simple Calculator

Create a program that asks the user for two numbers and displays their sum, difference, product, and quotient.

<details>
<summary>Solution</summary>

```python
num1 = float(input("Enter first number: "))
num2 = float(input("Enter second number: "))

print(f"Sum: {num1 + num2}")
print(f"Difference: {num1 - num2}")
print(f"Product: {num1 * num2}")
print(f"Quotient: {num1 / num2}")
```
</details>

## Intermediate Exercises

### Exercise 3: List Operations

Create a program that:
1. Creates a list of 5 numbers
2. Prints the list
3. Adds a new number to the end
4. Removes the first number
5. Prints the final list

<details>
<summary>Solution</summary>

```python
numbers = [10, 20, 30, 40, 50]
print("Original list:", numbers)

numbers.append(60)
print("After adding 60:", numbers)

numbers.pop(0)
print("After removing first:", numbers)
```
</details>

### Exercise 4: Dictionary Practice

Create a program that stores information about a book in a dictionary (title, author, year, pages) and prints it in a formatted way.

<details>
<summary>Solution</summary>

```python
book = {
    "title": "Python Programming",
    "author": "John Smith",
    "year": 2023,
    "pages": 350
}

print(f"Title: {book['title']}")
print(f"Author: {book['author']}")
print(f"Year: {book['year']}")
print(f"Pages: {book['pages']}")
```
</details>

## Control Flow Exercises

### Exercise 5: Even or Odd

Write a program that asks for a number and prints whether it's even or odd.

<details>
<summary>Solution</summary>

```python
number = int(input("Enter a number: "))

if number % 2 == 0:
    print("Even")
else:
    print("Odd")
```
</details>

### Exercise 6: Grade Calculator

Write a program that converts a numeric score (0-100) to a letter grade (A, B, C, D, F).

<details>
<summary>Solution</summary>

```python
score = int(input("Enter your score: "))

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
</details>

### Exercise 7: FizzBuzz

Write a program that prints numbers from 1 to 100:
- For multiples of 3, print "Fizz"
- For multiples of 5, print "Buzz"
- For multiples of both 3 and 5, print "FizzBuzz"
- Otherwise, print the number

<details>
<summary>Solution</summary>

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
</details>

### Exercise 8: Multiplication Table

Write a program that prints the multiplication table for a given number (1-10).

<details>
<summary>Solution</summary>

```python
number = int(input("Enter a number: "))

for i in range(1, 11):
    print(f"{number} x {i} = {number * i}")
```
</details>

## Function Exercises

### Exercise 9: Temperature Converter

Write two functions:
- `celsius_to_fahrenheit(celsius)` - converts Celsius to Fahrenheit
- `fahrenheit_to_celsius(fahrenheit)` - converts Fahrenheit to Celsius

<details>
<summary>Solution</summary>

```python
def celsius_to_fahrenheit(celsius):
    return (celsius * 9/5) + 32

def fahrenheit_to_celsius(fahrenheit):
    return (fahrenheit - 32) * 5/9

# Test
print(celsius_to_fahrenheit(0))    # 32.0
print(celsius_to_fahrenheit(100))  # 212.0
print(fahrenheit_to_celsius(32))   # 0.0
print(fahrenheit_to_celsius(212))  # 100.0
```
</details>

### Exercise 10: Palindrome Checker

Write a function that checks if a string is a palindrome (reads the same forwards and backwards).

<details>
<summary>Solution</summary>

```python
def is_palindrome(text):
    # Remove spaces and convert to lowercase
    text = text.replace(" ", "").lower()
    return text == text[::-1]

# Test
print(is_palindrome("racecar"))      # True
print(is_palindrome("hello"))        # False
print(is_palindrome("A man a plan a canal Panama"))  # True
```
</details>

### Exercise 11: Prime Number Checker

Write a function that returns True if a number is prime, False otherwise.

<details>
<summary>Solution</summary>

```python
def is_prime(n):
    if n < 2:
        return False
    for i in range(2, int(n ** 0.5) + 1):
        if n % i == 0:
            return False
    return True

# Test
print(is_prime(7))   # True
print(is_prime(10))  # False
print(is_prime(13))  # True
```
</details>

### Exercise 12: List Statistics

Write a function that takes a list of numbers and returns a dictionary with:
- `min`: minimum value
- `max`: maximum value
- `mean`: average value
- `sum`: sum of all values

<details>
<summary>Solution</summary>

```python
def list_stats(numbers):
    return {
        'min': min(numbers),
        'max': max(numbers),
        'mean': sum(numbers) / len(numbers),
        'sum': sum(numbers)
    }

# Test
numbers = [1, 2, 3, 4, 5]
print(list_stats(numbers))
# {'min': 1, 'max': 5, 'mean': 3.0, 'sum': 15}
```
</details>

## Challenge Exercises

### Exercise 13: Number Guessing Game

Create a number guessing game where:
1. The computer picks a random number between 1 and 100
2. The user has to guess the number
3. The program tells if the guess is too high or too low
4. Count how many guesses it takes

<details>
<summary>Solution</summary>

```python
import random

def guessing_game():
    number = random.randint(1, 100)
    guesses = 0
    
    print("I'm thinking of a number between 1 and 100")
    
    while True:
        guess = int(input("Your guess: "))
        guesses += 1
        
        if guess < number:
            print("Too low!")
        elif guess > number:
            print("Too high!")
        else:
            print(f"Correct! It took you {guesses} guesses.")
            break

guessing_game()
```
</details>

### Exercise 14: Word Counter

Write a function that counts the frequency of each word in a string.

<details>
<summary>Solution</summary>

```python
def word_count(text):
    words = text.lower().split()
    word_freq = {}
    
    for word in words:
        # Remove punctuation
        word = word.strip('.,!?;:')
        if word in word_freq:
            word_freq[word] += 1
        else:
            word_freq[word] = 1
    
    return word_freq

# Test
text = "Hello world! Hello Python. Python is great."
print(word_count(text))
# {'hello': 2, 'world': 1, 'python': 2, 'is': 1, 'great': 1}
```
</details>

### Exercise 15: Fibonacci Sequence

Write a function that generates the first n numbers in the Fibonacci sequence.

<details>
<summary>Solution</summary>

```python
def fibonacci(n):
    if n <= 0:
        return []
    elif n == 1:
        return [0]
    elif n == 2:
        return [0, 1]
    
    fib = [0, 1]
    for i in range(2, n):
        fib.append(fib[i-1] + fib[i-2])
    
    return fib

# Test
print(fibonacci(10))
# [0, 1, 1, 2, 3, 5, 8, 13, 21, 34]
```
</details>

## Project Ideas

Once you're comfortable with the basics, try these projects:

1. **To-Do List Manager**: Create a command-line to-do list application
2. **Contact Book**: Store and manage contact information
3. **Simple Quiz Game**: Create a quiz with multiple-choice questions
4. **Text-Based Adventure Game**: Build a simple interactive story game
5. **Password Generator**: Generate random secure passwords
6. **File Organizer**: Sort files in a directory by type/date
7. **Currency Converter**: Convert between different currencies
8. **BMI Calculator**: Calculate Body Mass Index with health recommendations

## Keep Learning!

These exercises are just the beginning. Keep practicing and exploring Python. The more you code, the better you'll get!

Check out the [Resources](resources.md) page for more learning materials and practice platforms.
