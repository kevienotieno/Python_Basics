# Python Basics

Python is a high-level, interpreted programming language known for its simplicity and readability. Key features include:

- **Easy-to-learn syntax:** Makes it accessible for beginners.
- **Rich standard library:** Provides modules and packages for various functionalities.
- **Dynamically typed:** Allows flexibility in variable types.
- **Versatility:** Used in web development, scientific computing, automation, etc.

## Installing Python

### Windows:

1. Download the installer from [python.org](https://www.python.org).
2. Run the installer and select "Add Python to PATH".
3. Click "Install Now" and follow the prompts.

### macOS:

- Install via Homebrew (`brew install python`).
- Alternatively, download the macOS installer from [python.org](https://www.python.org) and follow the steps.

### Linux:

- Use the package manager (`sudo apt-get install python3` for Ubuntu).
- Or download from [python.org](https://www.python.org) and follow installation instructions.

### Verify Installation:

Open a terminal or command prompt and type `python --version` or `python3 --version`.

## Set Up Virtual Environment:

1. Install `virtualenv` using `pip install virtualenv`.
2. Create a virtual environment: `virtualenv myenv`.
3. Activate the virtual environment:
   - Windows: `myenv\Scripts\activate`
   - macOS/Linux: `source myenv/bin/activate`

## Python Syntax and Semantics

```python
# Simple Hello World program
print("Hello, World!")
```

## Variables and Data Types in Python

In Python, variables can hold various types of data. Here are some basic data types and examples:

- **int**: Integer numbers (e.g., `5`, `-10`, `1000`).
- **float**: Floating-point numbers (e.g., `3.14`, `2.718`).
- **str**: String of characters (e.g., `"hello"`, `'world'`).
- **bool**: Boolean values (`True`, `False`).

### Example Usage

```python
# Define variables
my_int = 10
my_float = 3.14
my_str = "Python"
my_bool = True

# Print variables
print("Integer:", my_int)
print("Float:", my_float)
print("String:", my_str)
print("Boolean:", my_bool)
```

## Control Structures: Conditional Statements and Loops

## If-else Statement

```python
# If-else statement example
x = 10
if x > 5:
    print("x is greater than 5")
else:
    print("x is less than or equal to 5")

# For loop example
for i in range(5):
    print(i)
```

## Functions in Python
Functions in Python are reusable blocks of code that perform a specific task.

```python
# Function to add two numbers
def add_numbers(a, b):
    return a + b

# Calling the function
result = add_numbers(5, 3)
print("Sum:", result)  # Output: Sum: 8
```


## Lists and Dictionaries
Lists and dictionaries are fundamental data structures in Python.
```python
# Lists and dictionaries
numbers = [1, 2, 3, 4, 5]
my_dict = {'a': 1, 'b': 2, 'c': 3}

# Accessing elements
print(numbers[0])     # Output: 1
print(my_dict['b'])   # Output: 2

# Adding elements
numbers.append(6)
my_dict['d'] = 4
```
## Exception Handling
Exception handling in Python manages errors gracefully.

```python
# Exception handling
try:
    result = 10 / 0
except ZeroDivisionError:
    print("Error: division by zero")
finally:
    print("Execution completed")
```
## Modules and Packages
Modules are Python files containing functions and variables, while packages are directories of modules.

```python
# Importing and using modules
import math

# Using math module
print(math.sqrt(16))  # Output: 4.0
```
## File I/O
File I/O involves reading from and writing to files.

### Reading from a file:
```python
# Reading from a file
with open('file.txt', 'r') as f:
    content = f.read()
    print(content)
```
### Writing to a file:
```python
# Writing to a file
data = ["Hello", "world", "Python"]
with open('output.txt', 'w') as f:
    for line in data:
        f.write(line + '\n')
```
