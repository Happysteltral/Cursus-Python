# Data Types

Python has several built-in data types. Understanding these is crucial for writing effective programs.

## Numeric Types

### Integers (int)

Whole numbers without decimals.

```python
x = 5
y = -10
z = 0
```

### Floating Point (float)

Numbers with decimals.

```python
pi = 3.14159
temperature = -5.5
```

### Complex Numbers

Numbers with real and imaginary parts.

```python
z = 3 + 4j
```

## Text Type

### Strings (str)

Text data enclosed in quotes.

```python
name = "Alice"
message = 'Hello, World!'
multiline = """This is a
multi-line string"""
```

#### String Operations

```python
# Concatenation
greeting = "Hello" + " " + "World"

# Repetition
laugh = "ha" * 3  # "hahaha"

# Indexing
text = "Python"
first_char = text[0]    # "P"
last_char = text[-1]    # "n"

# Slicing
substring = text[0:3]   # "Pyt"
substring = text[:3]    # "Pyt" (same as above)
substring = text[3:]    # "hon"

# Common methods
print(text.upper())     # "PYTHON"
print(text.lower())     # "python"
print(text.replace("P", "J"))  # "Jython"
print(len(text))        # 6
```

## Boolean Type

True or False values.

```python
is_active = True
is_closed = False

# Boolean operations
print(5 > 3)           # True
print(10 == 5)         # False
print(bool(0))         # False (0 is falsy)
print(bool(1))         # True (non-zero is truthy)
```

## Sequence Types

### Lists

Ordered, mutable collections.

```python
fruits = ["apple", "banana", "cherry"]
numbers = [1, 2, 3, 4, 5]
mixed = [1, "hello", 3.14, True]

# Accessing elements
print(fruits[0])       # "apple"
print(fruits[-1])      # "cherry"

# Modifying lists
fruits.append("orange")      # Add to end
fruits.insert(1, "mango")    # Insert at position
fruits.remove("banana")      # Remove by value
fruits.pop()                 # Remove last item
fruits[0] = "grape"          # Change value

# List operations
print(len(fruits))           # Length
print("apple" in fruits)     # Check membership
```

### Tuples

Ordered, immutable collections.

```python
coordinates = (10, 20)
rgb = (255, 0, 0)

# Accessing elements
x = coordinates[0]     # 10
y = coordinates[1]     # 20

# Tuples cannot be modified after creation
# coordinates[0] = 15  # This would cause an error!
```

## Mapping Type

### Dictionaries (dict)

Key-value pairs.

```python
person = {
    "name": "Alice",
    "age": 25,
    "city": "New York"
}

# Accessing values
print(person["name"])        # "Alice"
print(person.get("age"))     # 25

# Modifying dictionaries
person["age"] = 26           # Update value
person["email"] = "alice@example.com"  # Add new key
del person["city"]           # Remove key

# Dictionary operations
print(person.keys())         # All keys
print(person.values())       # All values
print(person.items())        # All key-value pairs
```

## Set Types

### Sets

Unordered collections of unique elements.

```python
numbers = {1, 2, 3, 4, 5}
fruits = {"apple", "banana", "cherry"}

# Set operations
numbers.add(6)               # Add element
numbers.remove(3)            # Remove element
numbers.discard(10)          # Remove if exists (no error)

# Set mathematics
set1 = {1, 2, 3}
set2 = {3, 4, 5}
print(set1 | set2)           # Union: {1, 2, 3, 4, 5}
print(set1 & set2)           # Intersection: {3}
print(set1 - set2)           # Difference: {1, 2}
```

## Type Conversion

Convert between different data types:

```python
# To integer
x = int("10")          # 10
y = int(3.14)          # 3

# To float
a = float("3.14")      # 3.14
b = float(5)           # 5.0

# To string
s = str(123)           # "123"
t = str(3.14)          # "3.14"

# To list
lst = list("hello")    # ['h', 'e', 'l', 'l', 'o']

# To tuple
tup = tuple([1, 2, 3]) # (1, 2, 3)
```

## Checking Types

Use the `type()` function to check data types:

```python
x = 5
print(type(x))         # <class 'int'>

y = "Hello"
print(type(y))         # <class 'str'>

z = [1, 2, 3]
print(type(z))         # <class 'list'>
```

## Practice Exercises

1. Create a list of your favorite movies
2. Create a dictionary with information about yourself
3. Convert a string number to an integer and perform arithmetic
4. Create a set of unique numbers and add/remove elements

## Next Steps

Continue to [Control Flow](control-flow.md) to learn about conditionals and loops.
