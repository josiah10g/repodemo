# Project1 - Python Basics

This folder contains basic Python files and examples.

## Basic Python File Structure

### Hello World Example
Create a file named `hello.py`:
```python
# hello.py
print("Hello, World!")
```

Run it with:
```bash
python hello.py
```

### Basic Python Concepts

#### Variables and Data Types
```python
# variables.py
name = "John"              # String
age = 25                   # Integer
height = 5.9               # Float
is_student = True          # Boolean
```

#### Functions
```python
# functions.py
def greet(name):
    """A simple function that greets someone"""
    return f"Hello, {name}!"

# Call the function
message = greet("Alice")
print(message)
```

#### Lists and Loops
```python
# lists.py
fruits = ["apple", "banana", "cherry"]

# Loop through list
for fruit in fruits:
    print(fruit)
```

#### Conditional Statements
```python
# conditionals.py
age = 18

if age >= 18:
    print("You are an adult")
else:
    print("You are a minor")
```

## Running Python Files

1. Make sure Python is installed: `python --version`
2. Navigate to this directory: `cd Project1`
3. Run any Python file: `python filename.py`

## Common Python File Extensions
- `.py` - Python source files
- `.pyc` - Python compiled files
- `.pyw` - Python GUI scripts (Windows)
- `.pyx` - Cython source files

## Getting Started with Python

1. **Install Python**: Download from [python.org](https://www.python.org/)
2. **Choose an IDE**: VS Code, PyCharm, or IDLE
3. **Learn the basics**: Variables, functions, loops, and conditionals
4. **Practice**: Write small programs to solidify your understanding
